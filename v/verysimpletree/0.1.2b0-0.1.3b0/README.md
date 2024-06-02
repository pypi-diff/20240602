# Comparing `tmp/verysimpletree-0.1.2b0.tar.gz` & `tmp/verysimpletree-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimpletree-0.1.2b0.tar", last modified: Sun May 19 10:39:06 2024, max compression
+gzip compressed data, was "verysimpletree-0.1.3b0.tar", last modified: Sun Jun  2 10:36:44 2024, max compression
```

## Comparing `verysimpletree-0.1.2b0.tar` & `verysimpletree-0.1.3b0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-19 10:39:06.833341 verysimpletree-0.1.2b0/
--rw-r--r--   0 aligorji   (501) staff       (20)      479 2024-05-19 10:39:06.832893 verysimpletree-0.1.2b0/PKG-INFO
--rw-r--r--   0 aligorji   (501) staff       (20)      101 2024-05-12 13:01:46.000000 verysimpletree-0.1.2b0/README.rst
--rw-r--r--   0 aligorji   (501) staff       (20)       38 2024-05-19 10:39:06.833438 verysimpletree-0.1.2b0/setup.cfg
--rw-r--r--   0 aligorji   (501) staff       (20)      694 2024-05-19 10:38:14.000000 verysimpletree-0.1.2b0/setup.py
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-19 10:39:06.829878 verysimpletree-0.1.2b0/verysimpletree/
--rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-12 13:01:46.000000 verysimpletree-0.1.2b0/verysimpletree/__init__.py
--rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-15 21:30:24.000000 verysimpletree-0.1.2b0/verysimpletree/py.typed
--rw-r--r--   0 aligorji   (501) staff       (20)     6824 2024-05-19 10:38:04.000000 verysimpletree-0.1.2b0/verysimpletree/test_tree.py
--rw-r--r--   0 aligorji   (501) staff       (20)    19002 2024-05-19 10:38:04.000000 verysimpletree-0.1.2b0/verysimpletree/tree.py
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-19 10:39:06.832272 verysimpletree-0.1.2b0/verysimpletree.egg-info/
--rw-r--r--   0 aligorji   (501) staff       (20)      479 2024-05-19 10:39:06.000000 verysimpletree-0.1.2b0/verysimpletree.egg-info/PKG-INFO
--rw-r--r--   0 aligorji   (501) staff       (20)      273 2024-05-19 10:39:06.000000 verysimpletree-0.1.2b0/verysimpletree.egg-info/SOURCES.txt
--rw-r--r--   0 aligorji   (501) staff       (20)        1 2024-05-19 10:39:06.000000 verysimpletree-0.1.2b0/verysimpletree.egg-info/dependency_links.txt
--rw-r--r--   0 aligorji   (501) staff       (20)       15 2024-05-19 10:39:06.000000 verysimpletree-0.1.2b0/verysimpletree.egg-info/top_level.txt
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-06-02 10:36:44.743553 verysimpletree-0.1.3b0/
+-rw-r--r--   0 aligorji   (501) staff       (20)      443 2024-06-02 10:36:44.742964 verysimpletree-0.1.3b0/PKG-INFO
+-rw-r--r--   0 aligorji   (501) staff       (20)       65 2024-06-02 10:34:17.000000 verysimpletree-0.1.3b0/README.rst
+-rw-r--r--   0 aligorji   (501) staff       (20)       38 2024-06-02 10:36:44.743680 verysimpletree-0.1.3b0/setup.cfg
+-rw-r--r--   0 aligorji   (501) staff       (20)      694 2024-06-02 10:33:40.000000 verysimpletree-0.1.3b0/setup.py
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-06-02 10:36:44.740423 verysimpletree-0.1.3b0/verysimpletree/
+-rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-12 13:01:46.000000 verysimpletree-0.1.3b0/verysimpletree/__init__.py
+-rw-r--r--   0 aligorji   (501) staff       (20)     1973 2024-06-01 14:13:24.000000 verysimpletree-0.1.3b0/verysimpletree/bla.py
+-rw-r--r--   0 aligorji   (501) staff       (20)     1564 2024-06-01 14:13:32.000000 verysimpletree-0.1.3b0/verysimpletree/gla.py
+-rw-r--r--   0 aligorji   (501) staff       (20)        0 2024-05-15 21:30:24.000000 verysimpletree-0.1.3b0/verysimpletree/py.typed
+-rw-r--r--   0 aligorji   (501) staff       (20)     9780 2024-06-02 10:31:24.000000 verysimpletree-0.1.3b0/verysimpletree/test_tree.py
+-rw-r--r--   0 aligorji   (501) staff       (20)    19474 2024-06-02 10:32:40.000000 verysimpletree-0.1.3b0/verysimpletree/tree.py
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-06-02 10:36:44.742454 verysimpletree-0.1.3b0/verysimpletree.egg-info/
+-rw-r--r--   0 aligorji   (501) staff       (20)      443 2024-06-02 10:36:44.000000 verysimpletree-0.1.3b0/verysimpletree.egg-info/PKG-INFO
+-rw-r--r--   0 aligorji   (501) staff       (20)      317 2024-06-02 10:36:44.000000 verysimpletree-0.1.3b0/verysimpletree.egg-info/SOURCES.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)        1 2024-06-02 10:36:44.000000 verysimpletree-0.1.3b0/verysimpletree.egg-info/dependency_links.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)       15 2024-06-02 10:36:44.000000 verysimpletree-0.1.3b0/verysimpletree.egg-info/top_level.txt
```

### Comparing `verysimpletree-0.1.2b0/setup.py` & `verysimpletree-0.1.3b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.rst").read_text()
 setuptools.setup(
     name="verysimpletree",
-    version="0.1.2beta",
+    version="0.1.3beta",
     author="Alex Gorji",
     author_email="aligorji@hotmail.com",
     description="lightweight tree data structure for musicxml and musicscore",
     url="https://github.com/alexgorji/verysimpletree.git",
     packages=setuptools.find_packages(),
     install_requires=[],
     classifiers=[
```

### Comparing `verysimpletree-0.1.2b0/verysimpletree/test_tree.py` & `verysimpletree-0.1.3b0/verysimpletree/test_tree.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,65 @@
+from typing import Any
 from unittest import TestCase
 
-from verysimpletree.tree import Tree, ChildNotFoundError, grandchild1
+from verysimpletree.tree import Tree, ChildNotFoundError, grandchild1, TreeReferenceError
 
 
-class A(Tree):
+class AContent:
+    def __init__(self, value):
+        self.value = value
+
+
+class BContent:
+    def __init__(self, value):
+        self.value = value
+
+
+class A(Tree[Any]):
     def __init__(self, name, parent=None, *args, **keyword):
         super().__init__(*args, **keyword)
         self._children = []
         self._parent = parent
         self.name = name
+        self.content = AContent(value=10)
 
     def _check_child_to_be_added(self, child):
-        if not isinstance(child, self.__class__):
+        if not isinstance(child, Tree):
             raise TypeError
 
-    def add_child(self, name):
-        child = type(self)(parent=self, name=name)
+    def add_child_by_name(self, name):
+        child = self.__class__(parent=self, name=name)
         return super().add_child(child)
 
     def __str__(self):
         return self.name
 
-    def __repr__(self):
-        return self.__str__()
+
+class B(Tree[Any]):
+    def __init__(self, name, *args, **keyword):
+        super().__init__(*args, **keyword)
+        self.name = name
+        self.content = BContent(value=10)
+
+    def _check_child_to_be_added(self, child):
+        if not isinstance(child, Tree):
+            raise TypeError
 
 
 class TestTree(TestCase):
     def setUp(self) -> None:
         self.root = A(name='root')
-        self.child1 = self.root.add_child('child1')
-        self.child2 = self.root.add_child('child2')
-        self.child3 = self.root.add_child('child3')
-        self.child4 = self.root.add_child('child4')
-        self.grandchild1 = self.child2.add_child('grandchild1')
-        self.grandchild2 = self.child2.add_child('grandchild2')
-        self.grandchild3 = self.child4.add_child('grandchild3')
-        self.greatgrandchild1 = self.grandchild2.add_child('greatgrandchild1')
+        self.child1 = self.root.add_child_by_name('child1')
+        self.child2 = self.root.add_child_by_name('child2')
+        self.child3 = self.root.add_child_by_name('child3')
+        self.child4 = self.root.add_child_by_name('child4')
+        self.grandchild1 = self.child2.add_child_by_name('grandchild1')
+        self.grandchild2 = self.child2.add_child_by_name('grandchild2')
+        self.grandchild3 = self.child4.add_child_by_name('grandchild3')
+        self.greatgrandchild1 = self.grandchild2.add_child_by_name('greatgrandchild1')
 
     def test_is_last_child(self):
         t = self.root
         for node in t.traverse():
             if node.name in ['root', 'child4', 'grandchild2', 'grandchild3', 'greatgrandchild1']:
                 assert node.is_last_child
             else:
@@ -87,16 +107,16 @@
         assert self.greatgrandchild1.get_position_in_tree() == '2.2.1'
         assert self.child2.get_position_in_tree() == '2'
         assert self.root.get_position_in_tree() == '0'
 
     def test_replace_child(self):
         self.child2.replace_child(self.grandchild1, A(name='new_grand_child'))
         assert [ch.name for ch in self.child2.get_children()] == ['new_grand_child', 'grandchild2']
-        self.child1.add_child('grandchild')
-        self.child1.add_child('grandchild')
+        self.child1.add_child_by_name('grandchild')
+        self.child1.add_child_by_name('grandchild')
         new = A(name='other_new_grand_child')
         self.child1.replace_child(lambda x: x.name == 'grandchild', new, 1)
         assert new.get_parent() == self.child1
         assert [ch.name for ch in self.child1.get_children()] == ['grandchild', 'other_new_grand_child']
         with self.assertRaises(ValueError):
             self.child2.replace_child(None, None)
         with self.assertRaises(TypeError):
@@ -135,14 +155,52 @@
         assert [n for n in self.root.traverse() if n.get_level() == 2] == [self.grandchild1, self.grandchild2,
                                                                            self.grandchild3]
         for n in self.root.traverse():
             if n.get_level() == 2:
                 print(n)
                 break
 
+    def test_content(self):
+        self.child1.content.value = 20
+        assert [ch.content.value for ch in self.root.get_children()] == [20, 10, 10, 10]
+
+    def test_get_wrong_distance(self):
+        with self.assertRaises(TreeReferenceError):
+            assert self.greatgrandchild1.get_distance(self.child1) == 'bla'
+
+    def test_get_farthest_leave_of_root_without_children(self):
+        root = A('root')
+        assert root.get_farthest_leaf() == root
+
+    def test_get_leaves_of_root_without_children(self):
+        root = A('root')
+        assert root.get_leaves() == [root]
+        assert root.get_leaves(key=lambda node: node.name) == ['root']
+
+    def test_get_number_of_layers_of_root_without_children(self):
+        root = A('root')
+        assert root.get_number_of_layers() == 0
+
+    def test_get_layer_with_key(self):
+        assert self.root.get_layer(1, lambda node: node.name) == ['child1', 'child2', 'child3', 'child4']
+        assert self.root.get_layer(2, lambda node: node.name) == ['child1', 'grandchild1', 'grandchild2', 'child3',
+                                                                  'grandchild3']
+        assert self.root.get_layer(3, lambda node: node.name) == ['child1', 'grandchild1', 'greatgrandchild1', 'child3',
+                                                                  'grandchild3']
+
+    def test_remove_children(self):
+        self.root.remove_children()
+        assert self.root.get_children() == []
+        assert self.child1.name == 'child1'
+
+    def test_tree_representation_wrong_space(self):
+        with self.assertRaises(TypeError):
+            self.root.get_tree_representation(space=None)
+        with self.assertRaises(ValueError):
+            self.root.get_tree_representation(space=0)
 
 class TestNodeReturnValue(TestCase):
 
     def test_with_string(self):
         assert grandchild1.get_self_with_key(key='name') == 'grandchild1'
         with self.assertRaises(AttributeError):
             grandchild1.get_self_with_key(key='wrong')
@@ -154,7 +212,21 @@
 
     def test_with_node(self):
         assert grandchild1.get_self_with_key() == grandchild1.get_self_with_key(key=None) == grandchild1
 
     def test_wrong_type(self):
         with self.assertRaises(TypeError):
             grandchild1.get_self_with_key(key=1)
+
+
+class TestTwoTypesOfChildren(TestCase):
+    def setUp(self) -> None:
+        self.root = A(name='root_a')
+        self.ach1 = self.root.add_child(A(name='b_child_1'))
+        self.bch1 = self.root.add_child(B(name='a_child_1'))
+        self.ach2 = self.root.add_child(A(name='b_child_2'))
+        self.bch2 = self.root.add_child(B(name='a_child_2'))
+
+    def test_get_children_of_type(self):
+        assert self.root.get_children() == [self.ach1, self.bch1, self.ach2, self.bch2]
+        assert self.root.get_children_of_type(A) == [self.ach1, self.ach2]
+        assert self.root.get_children_of_type(B) == [self.bch1, self.bch2]
```

### Comparing `verysimpletree-0.1.2b0/verysimpletree/tree.py` & `verysimpletree-0.1.3b0/verysimpletree/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,92 @@
 from abc import ABC, abstractmethod
-from typing import Optional, Callable, List, Iterator, Union, TypeVar, Any, Generic, cast
+from typing import Optional, Callable, Iterator, TypeVar, Any, Generic, cast, Union
 
 
 class TreeException(Exception):
     pass
 
 
+class TreeReferenceError(TreeException, AttributeError):
+    pass
+
+
 class ChildNotFoundError(TreeException):
     pass
 
 
-_TREE_TYPE = TypeVar('_TREE_TYPE', bound='Tree')
+T = TypeVar('T', bound='Tree[Any]')
 
 
-class Tree(ABC, Generic[_TREE_TYPE]):
+class Tree(ABC, Generic[T]):
     """
     An abstract lightweight tree class for managing tree structures in MusicXML and musicscore packages.
     """
     _TREE_ATTRIBUTES = {'compact_repr', 'is_leaf', 'is_last_child', 'is_root', '_parent', '_children',
                         'up'}
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, content: Any = None, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
-        self._parent: Optional['_TREE_TYPE'] = None
-        self._children: List['_TREE_TYPE'] = []
-        self._traversed: Optional[List['_TREE_TYPE']] = None
-        self._iterated_leaves: Optional[List['_TREE_TYPE']] = None
-        self._reversed_path_to_root: Optional[List['_TREE_TYPE']] = None
+        self._content: Any
+        self.content = content
+        self._parent: Optional[T] = None
+        self._children: list[T] = []
+        self._traversed: Optional[list[T]] = None
+        self._iterated_leaves: Optional[list[T]] = None
+        self._reversed_path_to_root: Optional[list[T]] = None
         self._is_leaf: bool = True
 
     @abstractmethod
-    def _check_child_to_be_added(self, child):
-        pass
+    def _check_child_to_be_added(self, child: T) -> bool:
+        """each child must be checked before being added to the Tree"""
 
-    def _raw_traverse(self):
+    def _raw_traverse(self: T) -> Iterator[T]:
         yield self
         for child in self.get_children():
             for node in child._raw_traverse():
                 yield node
 
-    def _raw_reversed_path_to_root(self):
+    def _raw_reversed_path_to_root(self: T) -> Iterator[T]:
         yield self
-        if self.get_parent():
-            for node in self.get_parent().get_reversed_path_to_root():
+        parent = self.get_parent()
+        if parent is not None:
+            for node in parent.get_reversed_path_to_root():
                 yield node
 
-    def _reset_iterators(self):
+    def _reset_iterators(self) -> None:
         """
         This method is used to reset both parent's and this class's iterators for :obj:'~traverse', obj:'~iterate_leaves' and obj:'~get_reversed_path_to_root'
         """
         if self.up:
             self.up._reset_iterators()
         self._traversed = None
         self._iterated_leaves = None
         self._reversed_path_to_root = None
 
     @property
-    def is_last_child(self):
+    def content(self) -> Any:
+        return self._content
+
+    @content.setter
+    def content(self, value: Any) -> None:
+        self._content = value
+
+    @property
+    def is_last_child(self) -> bool:
         """
         >>> t = TestTree('root')
         >>> for node in t.traverse():
         ...    if node.name in ['root', 'child4', 'grandchild2', 'grandchild3', 'greatgrandchild1']:
         ...        assert node.is_last_child
         ...    else:
         ...        assert not node.is_last_child
         """
         if self.is_root:
             return True
-        if self.up.get_children()[-1] == self:
+        if cast(T, self.up).get_children()[-1] == self:
             return True
         return False
 
     @property
     def is_leaf(self) -> bool:
         """
         :obj:`~tree.tree.Tree` property
@@ -87,73 +102,51 @@
         :obj:`~tree.tree.Tree` property
 
         :return: ``True`` if self has no parent, else ``False``.
         :rtype: bool
         """
         return True if self.get_parent() is None else False
 
-    def get_level(self) -> int:
-        """
-        :obj:`~tree.tree.Tree`
-
-        :return: ``0`` for ``root``, ``1, 2 etc.`` for each layer of children
-        :rtype: nonnegative int
-
-        >>> root.get_level()
-        0
-        >>> child1.get_level()
-        1
-        >>> grandchild1.get_level()
-        2
-        >>> greatgrandchild1.get_level()
-        3
-        """
-        parent = self.get_parent()
-        if parent is None:
-            return 0
-        else:
-            return parent.get_level() + 1
-
     @property
-    def next(self: '_TREE_TYPE') -> Optional['_TREE_TYPE']:
+    def next(self) -> Optional[T]:
         """
         :obj:`~tree.tree.Tree` property
 
         :return: next sibling. ``None`` if this is the last current child of the parent.
         :rtype: :obj:`~tree.tree.Tree`
         """
         if self.up and self != self.up.get_children()[-1]:
-            return self.up.get_children()[self.up.get_children().index(self) + 1]
+            return cast(T, self.up.get_children()[self.up.get_children().index(self) + 1])
         else:
             return None
 
     @property
-    def previous(self: '_TREE_TYPE') -> Optional['_TREE_TYPE']:
+    def previous(self) -> Optional[T]:
         """
         :obj:`~tree.tree.Tree` property
 
         :return: previous sibling. ``None`` if this is the first child of the parent.
         :rtype: :obj:`~tree.tree.Tree`
         """
         if self.up and self != self.up.get_children()[0]:
-            return self.up.get_children()[self.up.get_children().index(self) - 1]
+            return cast(T, self.up.get_children()[self.up.get_children().index(self) - 1])
         else:
             return None
 
     @property
-    def up(self: '_TREE_TYPE') -> Optional[_TREE_TYPE]:
+    def up(self) -> Optional[T]:
         """
         :obj:`~tree.tree.Tree` property
 
         :return: :obj:`get_parent()`
         :rtype: :obj:`~tree.tree.Tree`
         """
         return self.get_parent()
 
-    def add_child(self, child: '_TREE_TYPE') -> '_TREE_TYPE':
+    def add_child(self, child: T) -> T:
         """
         :obj:`~tree.tree.Tree` method
 
         Check and add child to list of children. Child's parent is set to self.
 
         :param child:
         :return: child
@@ -163,148 +156,194 @@
         child._parent = self
         self._children.append(child)
         self._reset_iterators()
         if self._is_leaf is True:
             self._is_leaf = False
         return child
 
-    def get_children(self) -> List['_TREE_TYPE']:
+    def get_children(self: T) -> list[T]:
         """
         :obj:`~tree.tree.Tree` method
 
         :return: list of added children.
         """
         return self._children
 
-    def get_children_of_type(self, type_: type) -> List['_TREE_TYPE']:
+    def get_children_of_type(self, type_: type) -> list[T]:
         """
         :obj:`~tree.tree.Tree` method
 
         :return: list of added children of type.d
-        :rtype: List[:obj:`~tree.tree.Tree`]
+        :rtype: list[:obj:`~tree.tree.Tree`]
         """
-        return [cast(_TREE_TYPE, ch) for ch in self.get_children() if isinstance(ch, type_)]
+        return [cast(T, ch) for ch in self.get_children() if isinstance(ch, type_)]
 
-    def get_position_in_tree(self) -> str:
-        """
-        :obj:`~tree.tree.Tree` method
-
-        :return: 0 for ``root``. 1, 2, ... for layer 1. Other layers: x.y.z.... Example: 3.2.2 => third child of secod child of second child
-                 of the root.
-        :rtype: str
-
-        >>> print(root.get_tree_representation(key=lambda node: node.get_position_in_tree()))
-        └── 0
-            ├── 1
-            ├── 2
-            │   ├── 2.1
-            │   │   ├── 2.1.1
-            │   │   └── 2.1.2
-            │   └── 2.2
-            ├── 3
-            └── 4
-                └── 4.1
-        <BLANKLINE>
-        """
-        parent = self.get_parent()
-        if parent is None:
-            return '0'
-        elif self.get_level() == 1:
-            return str(parent.get_children().index(self) + 1)
-        else:
-            return f"{parent.get_position_in_tree()}.{parent.get_children().index(self) + 1}"
-
-    def get_distance(self, reference: Optional['_TREE_TYPE'] = None) -> Optional[int]:
+    def get_distance(self, reference: Optional[T] = None) -> int:
         """
         >>> root.get_distance()
         0
         >>> greatgrandchild1.get_distance()
         3
         >>> greatgrandchild1.get_distance(child2)
         2
-        >>> print(greatgrandchild1.get_distance(child1))
-        None
         """
 
         if self.is_root:
             return 0
 
         if reference is None:
             reference = self.get_root()
 
         parent = self.up
         count = 1
-        while parent is not reference:
-            parent = parent.up  # type: ignore
+        while parent is not None and parent is not reference:
+            parent = parent.up
             count += 1
-            if parent.is_root and parent is not reference:  # type: ignore
-                return None
+            if parent is not None and parent.is_root and parent is not reference:
+                raise TreeReferenceError(f"Wrong reference {reference} not in path to root.")
         return count
 
-    def get_farthest_leaf(self: '_TREE_TYPE') -> '_TREE_TYPE':
+    def get_farthest_leaf(self: T) -> T:
         """
         >>> root.get_farthest_leaf()
         greatgrandchild1
         """
-        leaves: List[_TREE_TYPE] = list(self.iterate_leaves())
-        if not leaves:
-            leaves = [self]
-        return max(leaves, key=lambda leaf: leaf.get_distance())  # type: ignore
+        leaves: list[T] = list(self.iterate_leaves())
+        return max(leaves, key=lambda leaf: leaf.get_distance())
 
-    def filter_nodes(self, key: Callable[['_TREE_TYPE'], Any], return_value: Any) -> List['_TREE_TYPE']:
+    def get_layer(self, level: int, key: Optional[Callable[['Tree[Any]'], Any]] = None) -> list[T]:
         """
         :obj:`~tree.tree.Tree` method
 
-        >>> root.filter_nodes(lambda node: node.get_level(), 2)
-        [grandchild1, grandchild2, grandchild3]
+        :param level: layer number where 0 is the ``root``.
+        :param key: An optional callable for each node in the layer.
+        :return: All nodes on this level. The leaves of branches which are shorter than the given level will be repeated on this and all
+                 following layers.
+        :rtype: list
         """
-        output = []
-
-        for node in self.traverse():
-            if key(node) == return_value:
-                output.append(node)
-        return output
+        output: list[T]
 
-    def get_parent(self: '_TREE_TYPE') -> Optional[_TREE_TYPE]:
-        """
-        :obj:`~tree.tree.Tree` method
+        if level == 0:
+            output = [cast(T, self)]
+        elif level == 1:
+            output = self.get_children()
+        else:
+            output = []
+            for child in self.get_layer(level - 1):
+                if child.is_leaf:
+                    output.append(child)
+                else:
+                    output.extend(child.get_children())
 
-        :return: parent. ``None`` for ``root``.
-        :rtype: :obj:`~tree.tree.Tree`
-        """
-        return self._parent
+        if key is None:
+            return output
+        else:
+            return [key(child) for child in output]
 
-    def get_leaves(self, key: Optional[Callable[['_TREE_TYPE'], Any]] = None) -> List[List[Any]]:
+    def get_leaves(self, key: Optional[Callable[['Tree[Any]'], Any]] = None) -> list[Union[Any, list[Any]]]:
         """
         Tree method
 
         :param key: An optional callable to be called on each leaf.
         :return: nested list of leaves or values of key(leaf) for each leaf
 
         >>> root.get_leaves()
         [child1, [[greatgrandchild1, greatgrandchild2], grandchild2], child3, [grandchild3]]
         """
-        output: List[List[Any]] = []
-        child: '_TREE_TYPE'
+        output: list[Union[Any, list[Any]]] = []
+        child: T
         for child in self.get_children():
             if not child.is_leaf:
                 output.append(child.get_leaves(key=key))
             else:
                 if key is not None:
                     output.append(key(child))
                 else:
                     output.append(child)
         if not output:
             if key is not None:
                 return [key(self)]
             else:
-                return [cast('_TREE_TYPE', self)]
+                return [cast(list[Any], self)]
         return output
 
-    def get_root(self: _TREE_TYPE) -> '_TREE_TYPE':
+    def get_level(self) -> int:
+        """
+        :obj:`~tree.tree.Tree`
+
+        :return: ``0`` for ``root``, ``1, 2 etc.`` for each layer of children
+        :rtype: nonnegative int
+
+        >>> root.get_level()
+        0
+        >>> child1.get_level()
+        1
+        >>> grandchild1.get_level()
+        2
+        >>> greatgrandchild1.get_level()
+        3
+        """
+        parent = self.get_parent()
+        if parent is None:
+            return 0
+        else:
+            return parent.get_level() + 1
+
+    def get_parent(self: T) -> Optional[T]:
+        """
+        :obj:`~tree.tree.Tree` method
+
+        :return: parent. ``None`` for ``root``.
+        :rtype: :obj:`~tree.tree.Tree`
+        """
+        return self._parent
+
+    def get_position_in_tree(self) -> str:
+        """
+        :obj:`~tree.tree.Tree` method
+
+        :return: 0 for ``root``. 1, 2, ... for layer 1. Other layers: x.y.z.... Example: 3.2.2 => third child of secod child of second child
+                 of the root.
+        :rtype: str
+
+        >>> print(root.get_tree_representation(key=lambda node: node.get_position_in_tree()))
+        └── 0
+            ├── 1
+            ├── 2
+            │   ├── 2.1
+            │   │   ├── 2.1.1
+            │   │   └── 2.1.2
+            │   └── 2.2
+            ├── 3
+            └── 4
+                └── 4.1
+        <BLANKLINE>
+        """
+        parent = self.get_parent()
+        if parent is None:
+            return '0'
+        elif self.get_level() == 1:
+            return str(parent.get_children().index(self) + 1)
+        else:
+            return f"{parent.get_position_in_tree()}.{parent.get_children().index(self) + 1}"
+
+    def get_reversed_path_to_root(self) -> list[T]:
+        """
+        :obj:`~tree.tree.Tree` method
+
+        :return: path from self upwards through all ancestors up to the ``root``.
+
+        >>> greatgrandchild1.get_reversed_path_to_root()
+        [greatgrandchild1, grandchild1, child2, root]
+        """
+        if self._reversed_path_to_root is None:
+            self._reversed_path_to_root = list(self._raw_reversed_path_to_root())
+        return self._reversed_path_to_root
+
+    def get_root(self: T) -> T:
         """
         :obj:`~tree.tree.Tree` method
 
         :return: ``root`` (upmost node of a tree which has no parent)
         :rtype: :obj:`~tree.tree.Tree`
 
         >>> greatgrandchild1.get_root() == root
@@ -317,77 +356,88 @@
         node = self
         parent = node.get_parent()
         while parent is not None:
             node = parent
             parent = node.get_parent()
         return node
 
-    def get_self_with_key(self, key=None):
+    def get_self_with_key(self, key: Optional[Callable[['Tree[Any]'], Any]] = None) -> Any:
         if key is None:
             return self
         elif isinstance(key, str):
             return getattr(self, key)
         elif callable(key):
             return key(self)
         else:
             raise TypeError(f'{self.__class__}: key: {key} must be None, string or a callable object')
 
-    def get_layer(self, level: int, key: Optional[Callable[['_TREE_TYPE'], Any]] = None) -> List['_TREE_TYPE']:
+    def get_tree_representation(self, key: Optional[Callable[['Tree[Any]'], Any]] = None, space: int = 3) -> str:
         """
         :obj:`~tree.tree.Tree` method
 
-        :param level: layer number where 0 is the ``root``.
-        :param key: An optional callable for each node in the layer.
-        :return: All nodes on this level. The leaves of branches which are shorter than the given level will be repeated on this and all
-                 following layers.
-        :rtype: list
-        """
-        output: List['_TREE_TYPE']
+        :param key: An optional callable if ``None`` :obj:`~compact_repr` property of each node is called.
+        :return: a representation of all nodes as string in tree form.
 
-        if level == 0:
-            output = [cast(_TREE_TYPE, self)]
-        elif level == 1:
-            output = self.get_children()
-        else:
-            output = []
-            for child in self.get_layer(level - 1):
-                if child.is_leaf:
-                    output.append(child)
-                else:
-                    output.extend(child.get_children())
+        >>> print(root.get_tree_representation())
+        └── root
+            ├── child1
+            ├── child2
+            │   ├── grandchild1
+            │   │   ├── greatgrandchild1
+            │   │   └── greatgrandchild2
+            │   └── grandchild2
+            ├── child3
+            └── child4
+                └── grandchild3
+        <BLANKLINE>
+        """
 
-        if key is None:
-            return output
-        else:
-            return [key(child) for child in output]
+        tree_representation = TreeRepresentation(tree=self, space=space)
+        if key:
+            tree_representation.key = key
+        return tree_representation.get_representation()
 
     def get_number_of_layers(self) -> int:
         """
         >>> root.get_number_of_layers()
         3
         """
         distance = self.get_farthest_leaf().get_distance(self)
 
         if not distance:
             return 0
         else:
             return distance
 
-    def iterate_leaves(self) -> Iterator[_TREE_TYPE]:
+    def filter_nodes(self, key: Callable[['Tree[Any]'], Any], return_value: Any) -> list[T]:
+        """
+        :obj:`~tree.tree.Tree` method
+
+        >>> root.filter_nodes(lambda node: node.get_level(), 2)
+        [grandchild1, grandchild2, grandchild3]
+        """
+        output = []
+
+        for node in self.traverse():
+            if key(node) == return_value:
+                output.append(node)
+        return output
+
+    def iterate_leaves(self) -> Iterator[T]:
         """
         :obj:`~tree.tree.Tree` method
 
         :return: A generator iterating over all leaves.
         """
         if self._iterated_leaves is None:  # Ensure self._iterated_leaves is not None
             self._iterated_leaves = [n for n in self.traverse() if n.is_leaf]
 
         return iter(self._iterated_leaves)
 
-    def remove(self, child: '_TREE_TYPE') -> None:
+    def remove(self, child: T) -> None:
         """
         :obj:`~tree.tree.Tree` method
 
         Child's parent will be set to ``None`` and child will be removed from list of children.
 
         :param child:
         :return: None
@@ -407,15 +457,15 @@
         :return: None
         """
         for child in self.get_children()[:]:
             parent = child.get_parent()
             if parent is not None:
                 parent.remove(child)
 
-    def replace_child(self, old, new, index: int = 0) -> None:
+    def replace_child(self, old: T, new: T, index: int = 0) -> None:
         """
         :obj:`~tree.tree.Tree` method
 
         :param old: child or function
         :param new: child
         :param index: index of old child in the list of its appearances
         :return: None
@@ -431,88 +481,50 @@
         old_child = self.get_children()[old_index]
         self.get_children().remove(old_child)
         self.get_children().insert(old_index, new)
         old_child._parent = None
         self._reset_iterators()
         new._parent = self
 
-    def get_reversed_path_to_root(self) -> List['_TREE_TYPE']:
-        """
-        :obj:`~tree.tree.Tree` method
-
-        :return: path from self upwards through all ancestors up to the ``root``.
-
-        >>> greatgrandchild1.get_reversed_path_to_root()
-        [greatgrandchild1, grandchild1, child2, root]
-        """
-        if self._reversed_path_to_root is None:
-            self._reversed_path_to_root = list(self._raw_reversed_path_to_root())
-        return self._reversed_path_to_root
-
-    def traverse(self) -> Iterator['_TREE_TYPE']:
+    def traverse(self) -> Iterator[T]:
         """
         :obj:`~tree.tree.Tree` method
 
         Traverse all tree nodes.
 
         :return: generator
         """
         if self._traversed is None:
             self._traversed = list(self._raw_traverse())
         return iter(self._traversed)
 
-    def get_tree_representation(self, key: Optional[Callable] = None, space=None) -> str:
-        """
-        :obj:`~tree.tree.Tree` method
-
-        :param key: An optional callable if ``None`` :obj:`~compact_repr` property of each node is called.
-        :return: a representation of all nodes as string in tree form.
-
-        >>> print(root.get_tree_representation())
-        └── root
-            ├── child1
-            ├── child2
-            │   ├── grandchild1
-            │   │   ├── greatgrandchild1
-            │   │   └── greatgrandchild2
-            │   └── grandchild2
-            ├── child3
-            └── child4
-                └── grandchild3
-        <BLANKLINE>
-        """
-
-        tree_representation = TreeRepresentation(tree=self)
-        if key:
-            tree_representation.key = key
-        if space:
-            tree_representation.space = space
-        return tree_representation.get_representation()
-
 
 class TreeRepresentation:
-    def __init__(self, tree: _TREE_TYPE, key: Callable[['_TREE_TYPE'], Any] = lambda x: str(x), space: int = 3):
-        self._tree: _TREE_TYPE = tree
-        self._key: Callable[['_TREE_TYPE'], Any] = key
-        self._space: int = space
+    def __init__(self, tree: Tree[Any], key: Callable[[Tree[Any]], Any] = lambda x: str(x), space: int = 3):
+        self._tree: Tree[Any]
+        self._key: Callable[[Tree[Any]], Any]
+        self._space: int
+        self.tree = tree
+        self.key = key
+        self.space = space
 
     @property
-    def tree(self):
+    def tree(self) -> Tree[Any]:
         return self._tree
 
     @tree.setter
-    def tree(self, val: _TREE_TYPE) -> None:
+    def tree(self, val: Tree[Any]) -> None:
         self._tree = val
 
     @property
-    def key(self) -> Callable[['_TREE_TYPE'], Any]:
+    def key(self) -> Callable[[Tree[Any]], Any]:
         return self._key
 
     @key.setter
-    def key(self, val: Callable[['_TREE_TYPE'], Any]) -> None:
+    def key(self, val: Callable[[Tree[Any]], Any]) -> None:
         self._key = val
 
     @property
     def space(self) -> int:
         return self._space
 
     @space.setter
@@ -550,28 +562,28 @@
           ├ 3
           └ 4
             └ 4.1
         <BLANKLINE>
 
         """
 
-        last_hook = '└'
-        continue_hook = '├'
-        no_hook = '│'
-        horizontal = '─'
+        last_hook: str = '└'
+        continue_hook: str = '├'
+        no_hook: str = '│'
+        horizontal: str = '─'
 
-        def get_vertical():
+        def get_vertical() -> str:
             if node.is_last_child:
                 return last_hook
             return continue_hook
 
-        def get_horizontal():
+        def get_horizontal() -> str:
             return (horizontal * (self.space - 1)) + ' '
 
-        def get_path():
+        def get_path() -> str:
             path = ''
             for i, n in enumerate(node.get_reversed_path_to_root()):
                 if i == 0:
                     pass
                 else:
                     if n.is_last_child:
                         path = (self.space + 1) * ' ' + path
@@ -582,38 +594,40 @@
         output = ''
         for node in self.tree.traverse():
             output += get_path()
             output += get_vertical() + get_horizontal() + str(self.key(node)) + '\n'
         return output
 
 
-class TestTree(Tree):
-    def __init__(self, name=None, *args, **kwargs):
+# Example usage
+class TestTree(Tree[Any]):  # pragma: no cover
+
+    def __init__(self, name: str = '', *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.name = name
 
-    def _check_child_to_be_added(self, child):
-        if not isinstance(child, self.__class__):
+    def _check_child_to_be_added(self, child: T) -> bool:
+        if not isinstance(child, Tree):
             raise TypeError
+        return True
 
-    def add_child(self, name):
-        child = type(self)(name=name)
-        return super().add_child(child)
+    def add_string_child(self, name: str) -> 'TestTree':
+        child: 'TestTree' = self.__class__(name=name)
+        return cast(TestTree, self.add_child(child))
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.__str__()
 
 
-# Example usage
 root = TestTree('root')
-child1 = root.add_child('child1')
-child2 = root.add_child('child2')
-child3 = root.add_child('child3')
-child4 = root.add_child('child4')
-grandchild1 = child2.add_child('grandchild1')
-grandchild2 = child2.add_child('grandchild2')
-grandchild3 = child4.add_child('grandchild3')
-greatgrandchild1 = grandchild1.add_child('greatgrandchild1')
-greatgrandchild2 = grandchild1.add_child('greatgrandchild2')
+child1: TestTree = root.add_string_child('child1')
+child2: TestTree = root.add_string_child('child2')
+child3: TestTree = root.add_string_child('child3')
+child4: TestTree = root.add_string_child('child4')
+grandchild1: TestTree = child2.add_string_child('grandchild1')
+grandchild2: TestTree = child2.add_string_child('grandchild2')
+grandchild3: TestTree = child4.add_string_child('grandchild3')
+greatgrandchild1: TestTree = grandchild1.add_string_child('greatgrandchild1')
+greatgrandchild2: TestTree = grandchild1.add_string_child('greatgrandchild2')
```

