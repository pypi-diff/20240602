# Comparing `tmp/plum_dispatch-2.3.6.tar.gz` & `tmp/plum_dispatch-2.4.tar.gz`

## Comparing `plum_dispatch-2.3.6.tar` & `plum_dispatch-2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/_version.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/alias.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/autoreload.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/dispatcher.py
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/function.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/method.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/overload.py
--rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/parametric.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/promotion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/py.typed
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/repr.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/resolver.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/signature.py
--rw-r--r--   0        0        0     9721 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/type.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/typing.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/util.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/LICENCE.txt
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/README.md
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/pyproject.toml
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/PKG-INFO
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/_version.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/alias.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/autoreload.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/dispatcher.py
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/function.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/method.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/overload.py
+-rw-r--r--   0        0        0    23379 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/parametric.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/promotion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/py.typed
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/repr.py
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/resolver.py
+-rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/signature.py
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/type.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/typing.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 plum_dispatch-2.4/plum/util.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.4/LICENCE.txt
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 plum_dispatch-2.4/README.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 plum_dispatch-2.4/pyproject.toml
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 plum_dispatch-2.4/PKG-INFO
```

### Comparing `plum_dispatch-2.3.6/plum/__init__.py` & `plum_dispatch-2.4/plum/__init__.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/plum/alias.py` & `plum_dispatch-2.4/plum/alias.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,20 +84,20 @@
     for union in found_unions:
         found_args |= union
 
     # Insert the aliases right before the first found argument. When we insert an
     # element, the positions of following insertions need to be appropriately
     # incremented.
     args = list(args)
-    delta = 0
     # Sort by insertion position to ensure that all following insertions are at higher
     # indices. This makes the bookkeeping simple.
-    for i, alias in sorted(zip(found_positions, found_aliases), key=lambda x: x[0]):
+    for delta, (i, alias) in enumerate(
+        sorted(zip(found_positions, found_aliases), key=lambda x: x[0])
+    ):
         args.insert(i + delta, alias)
-        delta += 1
 
     # Filter all elements of unions that are aliased.
     new_args = ()
     for arg in args:
         if arg not in found_args:
             new_args += (arg,)
     args = new_args
@@ -148,18 +148,15 @@
     Args:
         union (type or type hint): A union.
         alias (str): How to print `union`.
 
     Returns:
         type or type hint: `union`.
     """
-    if not isinstance(union, _union_type):
-        args = (union,)
-    else:
-        args = get_args(union)
+    args = get_args(union) if isinstance(union, _union_type) else (union,)
     for existing_union, existing_alias in _aliased_unions:
         if set(existing_union) == set(args) and alias != existing_alias:
             if isinstance(union, _union_type):
                 union_str = _original_str(union)
             else:
                 union_str = repr(union)
             raise RuntimeError(f"`{union_str}` already has alias `{existing_alias}`.")
```

### Comparing `plum_dispatch-2.3.6/plum/autoreload.py` & `plum_dispatch-2.4/plum/autoreload.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,13 +65,13 @@
 if _autoload in ("y", "yes", "t", "true", "on", "1"):  # pragma: no cover
     try:
         # Try to load iPython and get the iPython session, but don't crash if
         # this does not work (for example IPython not installed, or python shell)
         from IPython import get_ipython  # type: ignore
 
         ip = get_ipython()
-        if ip is not None:
-            if "IPython.extensions.storemagic" in ip.extension_manager.loaded:
-                activate_autoreload()
+        ext_loaded = "IPython.extensions.storemagic" in ip.extension_manager.loaded
+        if (ip is not None) and ext_loaded:
+            activate_autoreload()
 
     except ImportError:
         pass
```

### Comparing `plum_dispatch-2.3.6/plum/dispatcher.py` & `plum_dispatch-2.4/plum/dispatcher.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/plum/function.py` & `plum_dispatch-2.4/plum/function.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/plum/method.py` & `plum_dispatch-2.4/plum/method.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/plum/parametric.py` & `plum_dispatch-2.4/plum/parametric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 from typing import Type, TypeVar, Union
 
 import beartype.door
 from beartype.roar import BeartypeDoorNonpepException
 
 from .dispatcher import Dispatcher
 from .function import _owner_transfer
@@ -52,18 +53,17 @@
         Args:
             *args: Positional arguments passed to the `__init__` method.
             **kw_args: Keyword arguments passed to the `__init__` method.
 
         Returns:
             type: A concrete class.
         """
-        if getattr(cls, "parametric", False):
-            if not cls.concrete:
-                type_parameter = cls.__infer_type_parameter__(*args, **kw_args)
-                cls = cls[type_parameter]
+        if getattr(cls, "parametric", False) and not cls.concrete:
+            type_parameter = cls.__infer_type_parameter__(*args, **kw_args)
+            cls = cls[type_parameter]
         return cls
 
     def __init_type_parameter__(cls, *ps):
         """Function called to initialise the type parameters.
 
         The default behaviour is to just return `ps`.
 
@@ -132,23 +132,26 @@
         return p_left == p_right
 
 
 class CovariantMeta(ParametricTypeMeta):
     """A metaclass that implements *covariance* of parametric types."""
 
     def __subclasscheck__(cls, subclass):
-        if is_concrete(cls) and is_concrete(subclass):
-            # Check that they are instances of the same parametric type.
-            if all(issubclass(b, cls.__bases__) for b in subclass.__bases__):
-                p_sub = subclass.type_parameter
-                p_cls = cls.type_parameter
-                # Ensure that both are in tuple form.
-                p_sub = p_sub if isinstance(p_sub, tuple) else (p_sub,)
-                p_cls = p_cls if isinstance(p_cls, tuple) else (p_cls,)
-                return cls.__le_type_parameter__(p_sub, p_cls)
+        # Check that they are instances of the same parametric type.
+        if (
+            is_concrete(cls)
+            and is_concrete(subclass)
+            and all(issubclass(b, cls.__bases__) for b in subclass.__bases__)
+        ):
+            p_sub = subclass.type_parameter
+            p_cls = cls.type_parameter
+            # Ensure that both are in tuple form.
+            p_sub = p_sub if isinstance(p_sub, tuple) else (p_sub,)
+            p_cls = p_cls if isinstance(p_cls, tuple) else (p_cls,)
+            return cls.__le_type_parameter__(p_sub, p_cls)
 
         # Default behaviour to `type`s subclass check.
         return type.__subclasscheck__(cls, subclass)
 
     def __instancecheck__(cls, instance):
         # If `A` is a parametric type, then `A[T1]` and `A[T2]` are subclasses of
         # `A`. With the implementation of `__subclasscheck__` above, we have that
@@ -253,18 +256,16 @@
             )
             subclass._parametric = True
             subclass._concrete = True
             subclass._type_parameter = ps[0] if len(ps) == 1 else ps
             subclass.__module__ = original_class.__module__
 
             # Attempt to correct docstring.
-            try:
+            with contextlib.suppress(AttributeError):
                 subclass.__doc__ = original_class.__doc__
-            except AttributeError:  # pragma: no cover
-                pass
 
             subclasses[ps] = subclass
         return subclasses[ps]
 
     def __init_subclass__(cls, **kw_args):
         cls._parametric = False
         # If the subclass has the same `__new__` as `ParametricClass`, then we should
@@ -403,18 +404,16 @@
     # will happen is that `original_class` will be the next in the MRO, which means
     # that, whenever a `NotFoundLookupError` happens, the method will try itself again,
     # resulting in an infinite loop. To prevent this from happening, we must adjust the
     # owner.
     _owner_transfer[parametric_class] = original_class
 
     # Attempt to correct docstring.
-    try:
+    with contextlib.suppress(AttributeError):
         parametric_class.__doc__ = original_class.__doc__
-    except AttributeError:  # pragma: no cover
-        pass
 
     return parametric_class
 
 
 def is_concrete(t):
     """Check if a type `t` is a concrete instance of a parametric type.
 
@@ -453,18 +452,15 @@
 
     Args:
         x (object): Concrete parametric type or instance thereof.
 
     Returns:
         object: Type parameter.
     """
-    if is_type(x):
-        t = x
-    else:
-        t = type(x)
+    t = x if is_type(x) else type(x)
     if hasattr(t, "parametric"):
         return t.type_parameter
     raise ValueError(
         f"`{x}` is not a concrete parametric type or an instance of a"
         f" concrete parametric type."
     )
```

### Comparing `plum_dispatch-2.3.6/plum/promotion.py` & `plum_dispatch-2.4/plum/promotion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-from beartype.door import TypeHint
-
-import plum.function
-
-from . import _is_bearable
-from .dispatcher import Dispatcher
-from .repr import repr_short
-from .type import resolve_type_hint
+"""Promotion and conversion functions."""
 
 __all__ = [
     "convert",
     "add_conversion_method",
     "conversion_method",
     "add_promotion_rule",
     "promote",
 ]
 
+from typing import Callable, Protocol, Type, TypeVar
+
+from beartype.door import TypeHint
+
+import plum.function
+from . import _is_bearable
+from .dispatcher import Dispatcher
+from .repr import repr_short
+from .type import resolve_type_hint
+
+T = TypeVar("T")
+R = TypeVar("R")
+
 _dispatch = Dispatcher()
 
 
 @_dispatch
 def convert(obj, type_to):
     """Convert an object to a particular type.
 
@@ -36,45 +42,54 @@
 
 # Deliver `convert`.
 plum.function._promised_convert = convert
 
 
 @_dispatch
 def _convert(obj, type_to):
-    if _is_bearable(obj, resolve_type_hint(type_to)):
-        return obj
-    else:
+    if not _is_bearable(obj, resolve_type_hint(type_to)):
         raise TypeError(f"Cannot convert `{obj}` to `{repr_short(type_to)}`.")
+    return obj
+
+
+class _ConversionCallable(Protocol[T, R]):
+    def __call__(self, obj: T) -> R: ...
 
 
-def add_conversion_method(type_from, type_to, f):
+def add_conversion_method(
+    type_from: Type[T],
+    type_to: Type[R],
+    f: _ConversionCallable[T, R],
+) -> None:
     """Add a conversion method to convert an object from one type to another.
 
     Args:
         type_from (type): Type to convert from.
         type_to (type): Type to convert to.
         f (function): Function that converts an object of type `type_from` to
             type `type_to`.
     """
 
     @_convert.dispatch
     def perform_conversion(obj: type_from, _: type_to):
         return f(obj)
 
 
-def conversion_method(type_from, type_to):
+def conversion_method(
+    type_from: Type[T], type_to: Type[R]
+) -> Callable[[_ConversionCallable[T, R]], _ConversionCallable[T, R]]:
     """Decorator to add a conversion method to convert an object from one
     type to another.
 
     Args:
         type_from (type): Type to convert from.
         type_to (type): Type to convert to.
     """
 
-    def add_method(f):
+    def add_method(f: _ConversionCallable[T, R]) -> _ConversionCallable[T, R]:
         add_conversion_method(type_from, type_to, f)
         return f
 
     return add_method
 
 
 # Add some common conversion methods.
```

### Comparing `plum_dispatch-2.3.6/plum/repr.py` & `plum_dispatch-2.4/plum/repr.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/plum/resolver.py` & `plum_dispatch-2.4/plum/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 import sys
 from functools import wraps
 from typing import Callable, Optional, Tuple, Union
 
 from rich.padding import Padding
 from rich.text import Text
 
+from .util import argsort
 from plum.method import Method, MethodList
 from plum.repr import rich_repr
 from plum.signature import Signature
 
-from .util import argsort
-
 __all__ = ["AmbiguousLookupError", "NotFoundLookupError"]
 
 
 def _render_function_call(f: str, target: Union[Tuple, Signature]) -> str:
     """Render a function call.
 
     Args:
```

### Comparing `plum_dispatch-2.3.6/plum/signature.py` & `plum_dispatch-2.4/plum/signature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
 import operator
 import typing
 from copy import copy
 from typing import Callable, List, Set, Tuple, Union
 
+from rich.segment import Segment
+
 import beartype.door
 from beartype.peps import resolve_pep563 as beartype_resolve_pep563
-from rich.segment import Segment
 
 from . import _is_bearable
 from .repr import repr_short, rich_repr
 from .type import is_faithful, resolve_type_hint
 from .typing import get_type_hints
 from .util import Comparable, Missing, TypeHint, multihash, wrap_lambda
 
@@ -144,50 +145,90 @@
         if self.has_varargs:
             expansion_size = max(n - len(self.types), 0)
             return self.types + (self.varargs,) * expansion_size
         else:
             return self.types
 
     def __le__(self, other) -> bool:
-        # If this signature has variable arguments, but the other does not, then this
-        # signature cannot be possibly smaller.
-        if self.has_varargs and not other.has_varargs:
-            return False
-
-        # If this signature and the other signature both have variable arguments, then
-        # the variable type of this signature must be less than the variable type of the
-        # other signature.
-        if (
-            self.has_varargs
-            and other.has_varargs
-            and not (
-                beartype.door.TypeHint(self.varargs)
-                <= beartype.door.TypeHint(other.varargs)
-            )
-        ):
-            return False
-
         # If the number of types of the signatures are unequal, then the signature
         # with the fewer number of types must be expanded using variable arguments.
         if not (
             len(self.types) == len(other.types)
             or (len(self.types) > len(other.types) and other.has_varargs)
             or (len(self.types) < len(other.types) and self.has_varargs)
         ):
             return False
 
-        # Finally, expand the types and compare.
+        # Expand the types and compare. We implement the subset relationship, but, very
+        # importantly, deviate from the subset relationship in exactly one place.
         self_types = self.expand_varargs(len(other.types))
         other_types = other.expand_varargs(len(self.types))
-        return all(
+        if all(
+            [
+                beartype.door.TypeHint(x) == beartype.door.TypeHint(y)
+                for x, y in zip(self_types, other_types)
+            ]
+        ):
+            if self.has_varargs and other.has_varargs:
+                self_varargs = beartype.door.TypeHint(self.varargs)
+                other_varargs = beartype.door.TypeHint(other.varargs)
+                return self_varargs <= other_varargs
+
+            # Having variable arguments makes you slightly larger.
+            elif self.has_varargs:
+                return False
+            elif other.has_varargs:
+                return True
+
+            else:
+                return True
+
+        elif all(
             [
                 beartype.door.TypeHint(x) <= beartype.door.TypeHint(y)
                 for x, y in zip(self_types, other_types)
             ]
-        )
+        ):
+            # In this case, we have that `other >= self` is `False`, so returning `True`
+            # gives that `other < self` and returning `False` gives that `other` cannot
+            # be compared to `self`. Regardless of the return value, `other != self`.
+
+            if self.has_varargs and other.has_varargs:
+                # TODO: This implements the subset relationship. However, if the
+                #       variable arguments are not used, then this may unnecessarily
+                #       return `False`. For example, `(int, *A)` would not be
+                #       comparable to `(Number, *B)`. However, if the argument given
+                #       is `1.0`, then reasonably the variable arguments should be
+                #       ignored and `(int, *A)` should be considered more specific
+                #       than `(Number, *B)`.
+                self_varargs = beartype.door.TypeHint(self.varargs)
+                other_varargs = beartype.door.TypeHint(other.varargs)
+                return self_varargs <= other_varargs
+
+            elif self.has_varargs:
+                # Previously, this returned `False`, which would implement the subset
+                # relationship. We now deviate from the subset relationship! The
+                # rationale for this is as follows.
+                #
+                # A non-variable-arguments signature is compared to a variable-arguments
+                # signature only to determine which is more specific. At this point, the
+                # non-variable-arguments signature has number of types equal to the
+                # number of arguments given to the function, so any additional variable
+                # arguments are not necessary. Hence, we ignore the additional
+                # variable arguments in the comparison and return correctly `True`. For
+                # example, `(int, *int)` would be more specific than `(Number)`.
+                return True
+            elif other.has_varargs:
+                return True
+
+            else:
+                return True
+
+        else:
+            return False
 
     def match(self, values) -> bool:
         """Check whether values match the signature.
 
         Args:
             values (tuple): Values.
 
@@ -263,17 +304,15 @@
 
     Args:
         f (object): Function-like object.
 
     Returns:
         object: Signature.
     """
-    if isinstance(f, operator.itemgetter):
-        f = wrap_lambda(f)
-    elif isinstance(f, operator.attrgetter):
+    if isinstance(f, (operator.itemgetter, operator.attrgetter)):
         f = wrap_lambda(f)
     return inspect.signature(f)
 
 
 def resolve_pep563(f: Callable):
     """Utility function to resolve PEP563-style annotations and make editable.
 
@@ -325,20 +364,20 @@
             # Parameter indicates variable arguments.
             varargs = annotation
         else:
             # Parameter is a regular positional parameter.
             types.append(annotation)
 
         # If there is a default parameter, make sure that it is of the annotated type.
-        if p.default is not inspect.Parameter.empty:
-            if not _is_bearable(p.default, annotation):
-                raise TypeError(
-                    f"Default value `{p.default}` is not an instance "
-                    f"of the annotated type `{repr_short(annotation)}`."
-                )
+        default_is_empty = p.default is inspect.Parameter.empty
+        if not default_is_empty and not _is_bearable(p.default, annotation):
+            raise TypeError(
+                f"Default value `{p.default}` is not an instance "
+                f"of the annotated type `{repr_short(annotation)}`."
+            )
 
     return types, varargs
 
 
 def append_default_args(signature: Signature, f: Callable) -> List[Signature]:
     """Returns a list of signatures of function `f`, where those signatures are derived
     from the input arguments of `f` by treating every non-keyword-only argument with a
```

### Comparing `plum_dispatch-2.3.6/plum/type.py` & `plum_dispatch-2.4/plum/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,23 @@
 
     def retrieve(self):
         """Attempt to retrieve the type from the reference module.
 
         Returns:
             bool: Whether the retrieval succeeded.
         """
-        if self._type is None:
-            if self._module in sys.modules:
-                type = sys.modules[self._module]
-                for name in self._name.split("."):
-                    # If `type` does not contain `name` and `self._allow_fail` is
-                    # set, then silently fail.
-                    if not hasattr(type, name) and self._allow_fail:
-                        return False
-                    type = getattr(type, name)
-                self.deliver(type)
+        if self._type is None and self._module in sys.modules:
+            type = sys.modules[self._module]
+            for name in self._name.split("."):
+                # If `type` does not contain `name` and `self._allow_fail` is
+                # set, then silently fail.
+                if not hasattr(type, name) and self._allow_fail:
+                    return False
+                type = getattr(type, name)
+            self.deliver(type)
         return self._type is not None
 
 
 def _is_hint(x):
     """Check if an object is a type hint.
 
     Args:
@@ -205,31 +204,28 @@
                     # seems to have worked fine.
                     if sys.version_info.minor <= 8:
                         return getattr(typing, origin.__name__.capitalize())[args]
                     else:  # pragma: no cover
                         # This branch can never be reached.
                         raise e
 
-    elif x is None:
-        return x
-    elif x is Ellipsis:
+    elif x is None or x is Ellipsis:
         return x
 
     elif isinstance(x, tuple):
         return tuple(resolve_type_hint(arg) for arg in x)
     elif isinstance(x, list):
         return list(resolve_type_hint(arg) for arg in x)
     elif isinstance(x, type):
         if isinstance(x, ResolvableType):
-            if isinstance(x, ModuleType):
-                if not x.retrieve():
-                    # If the type could not be retrieved, then just return the
-                    # wrapper. Namely, `x.resolve()` will then return `x`, which means
-                    # that the below call will result in an infinite recursion.
-                    return x
+            if isinstance(x, ModuleType) and not x.retrieve():
+                # If the type could not be retrieved, then just return the
+                # wrapper. Namely, `x.resolve()` will then return `x`, which means
+                # that the below call will result in an infinite recursion.
+                return x
             return resolve_type_hint(x.resolve())
         else:
             return x
 
     # For example, `Is[lambda x: x > 0]` is an example of a `BeartypeValidator`. We
     # shouldn't resolve those.
     elif isinstance(x, BeartypeValidator):
@@ -280,17 +276,15 @@
             return True
         else:
             if origin in {typing.Union, typing.Optional}:
                 return all(is_faithful(arg) for arg in args)
             else:
                 return False
 
-    elif x is None:
-        return True
-    elif x == Ellipsis:
+    elif x is None or x == Ellipsis:
         return True
 
     elif isinstance(x, (tuple, list)):
         return all(is_faithful(arg) for arg in x)
     elif isinstance(x, type):
         if hasattr(x, "__faithful__"):
             return x.__faithful__
```

### Comparing `plum_dispatch-2.3.6/plum/typing.py` & `plum_dispatch-2.4/plum/typing.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/plum/util.py` & `plum_dispatch-2.4/plum/util.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/LICENCE.txt` & `plum_dispatch-2.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/README.md` & `plum_dispatch-2.4/README.md`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.6/pyproject.toml` & `plum_dispatch-2.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -62,42 +62,34 @@
 command_line = "-m pytest --verbose test"
 source = ["plum"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests/", "plum", "docs"]
 addopts = [
     "-ra",
-    "-p no:doctest",
+    "-p",
+    "no:doctest",
 ]
 minversion = "6.0"
 
-# Formatting tools
-[tool.black]
-line-length = 88
-target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
-
-[tool.isort]
-profile = "black"
-src_paths = ["plum", "tests"]
-
 
 [tool.ruff]
+src = ["plum"]
 target-version = "py38"
-select = ["B", "E", "F", "W", "D410"]
-fixable = ["B", "E", "F", "W", "D"]
-ignore = ["F811", "B018"]
 line-length = 88
+
+[tool.ruff.lint]
+select = [
+    "B",  # flake8-bugbear
+    "D410",
+    "E",  # pycodestyle
+    "F",  # Pyflakes
+    "I",  # isort
+    "SIM",  # flake8-simplify
+    "UP",  # pyupgrade
+    "W",
+]
+ignore = ["F811", "B018"]
+
+[tool.ruff.lint.isort]
+known-first-party = ["beartype"]
+known-local-folder = ["plum"]
```

### Comparing `plum_dispatch-2.3.6/PKG-INFO` & `plum_dispatch-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: plum-dispatch
-Version: 2.3.6
+Version: 2.4
 Summary: Multiple dispatch in Python
 Project-URL: repository, https://github.com/beartype/plum
 Author-email: Wessel Bruinsma <wessel.p.bruinsma@gmail.com>
 License: MIT
 License-File: LICENCE.txt
 Keywords: multiple dispatch
 Classifier: Development Status :: 5 - Production/Stable
```

