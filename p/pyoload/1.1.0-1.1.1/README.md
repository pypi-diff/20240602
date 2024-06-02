# Comparing `tmp/pyoload-1.1.0.tar.gz` & `tmp/pyoload-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoload-1.1.0.tar", last modified: Tue May 28 14:42:39 2024, max compression
+gzip compressed data, was "pyoload-1.1.1.tar", last modified: Sun Jun  2 08:22:38 2024, max compression
```

## Comparing `pyoload-1.1.0.tar` & `pyoload-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.721882 pyoload-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 14:42:37.000000 pyoload-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-28 14:42:39.721882 pyoload-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-05-28 14:42:37.000000 pyoload-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.717882 pyoload-1.1.0/pyoload/
--rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-05-28 14:42:32.000000 pyoload-1.1.0/pyoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.721882 pyoload-1.1.0/pyoload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:42:39.721882 pyoload-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-28 14:42:32.000000 pyoload-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.721882 pyoload-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 14:42:32.000000 pyoload-1.1.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:22:38.410623 pyoload-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-06-02 08:22:36.000000 pyoload-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-06-02 08:22:38.410623 pyoload-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-06-02 08:22:36.000000 pyoload-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:22:38.406623 pyoload-1.1.1/pyoload/
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-06-02 08:22:33.000000 pyoload-1.1.1/pyoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:22:38.406623 pyoload-1.1.1/pyoload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-06-02 08:22:38.000000 pyoload-1.1.1/pyoload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-02 08:22:38.000000 pyoload-1.1.1/pyoload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 08:22:38.000000 pyoload-1.1.1/pyoload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-02 08:22:38.000000 pyoload-1.1.1/pyoload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 08:22:38.000000 pyoload-1.1.1/pyoload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 08:22:38.410623 pyoload-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-06-02 08:22:33.000000 pyoload-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:22:38.406623 pyoload-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 08:22:33.000000 pyoload-1.1.1/tests/test_cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-02 08:22:33.000000 pyoload-1.1.1/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-02 08:22:33.000000 pyoload-1.1.1/tests/test_overload.py
```

### Comparing `pyoload-1.1.0/LICENSE` & `pyoload-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoload-1.1.0/pyoload/__init__.py` & `pyoload-1.1.1/pyoload/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,158 @@
-from typing import Any, GenericAlias
+"""pyoload
+
+pyoload is a little python script to incorporate some features of
+annotation and typechecking in python.
+
+"""
+from typing import Any, GenericAlias, Callable
 from types import UnionType
 from functools import wraps, partial
 from inspect import isclass
 
 import sys
 
 
 class AnnotationError(ValueError):
-    pass
+    """class AnnotationError(ValueError)
+    base exception for most pyoload errors
+    """
 
 
 class AnnotationErrors(AnnotationError):
-    pass
+    """class AnnotationErrors(AnnotationError)
+    Hosts a list of AnnotationError
+    """
 
 
 class InternalAnnotationError(Exception):
-    pass
+    """class InternalAnnotationError(Exception)
+    **internam**
+    raised by overloads on type mismatch
+    """
 
 
 class CastingError(TypeError):
-    pass
+    """class CastingError(TypeError)
+    Error during casting
+    """
 
 
 class OverloadError(TypeError):
-    pass
+    """class OverloadError(TypeError)
+    Error in or during overload
+    """
 
 
 class AnnotationResolutionError(AnnotationError):
+    """class AnnotationResolutionError(AnnotationError)
+    Annotations could not be resolved or evaluated.
+    """
     _raise = False
 
 
-class Values(tuple):
-    """wrapper class in case of several value"""
+class PyoloadAnnotation:
+    """class PyoloadAnnotation
+    A parent class for pyoload extra annotations
+    """
+
+
+class Values(PyoloadAnnotation, tuple):
+    """class Values(PyoloadAnnotation, tuple)
+    A tuple subclass which holds several values as possible annotations
+    """
 
-    def __call__(self, val):
+    def __call__(self: 'Values', val: Any) -> bool:
+        """def __call__(self, val)
+        :param self: the `Values` object
+        :param val: the value to be checked
+
+        :returns: if the value `val` is contained in `self`
+        """
         return val in self
 
     def __str__(self):
         return 'Values(' + ', '.join(map(repr, self)) + ')'
 
     __repr__ = __str__
 
 
-Vs = Values
-
-
-def get_name(funcOrCls):
+def get_name(funcOrCls: Any):
+    """def get_name(funcOrCls: Any)
+    Gives a class or function name, possibly unique gotten from
+    it's module name and qualifier name
+    """
     return funcOrCls.__module__ + '.' + funcOrCls.__qualname__
 
 
 class Check:
+    """class Check
+    A class basicly abstract which holds registerred checks in pyoload
+    """
     checks_list = {}
 
-    def __init_subclass__(cls, subclass):
+    def __init_subclass__(cls: Any, subclass: Any):
+        """def __init_subclass__(cls, subclass)
+        register's subclasses as chexks
+        """
         cls.register(cls.name, cls.__call__)
 
     @classmethod
-    def register(cls, name):
+    def register(cls: Any, name: str) -> Any:
+        """def register(cls, name)
+        returns a callable which registers a new checker mathod
+        :param cls: the Check class
+        :param name: the name to be registerred as
+        """
         if name in cls.checks_list:
             raise Check.CheckNameAlreadyExistsError(name)
 
-        def inner(func):
+        def inner(func: Callable) -> Callable:
+            """def inner(func: Callable)
+            :param func: The callable to register
+
+            :returns: func
+            """
             cls.checks_list[name] = func
+            return func
         return inner
 
     @classmethod
-    def check(cls, name, params, val):
-        print(cls, name, params, val)
+    def check(cls: Any, name: str, params: Any, val: Any) -> None:
+        """def check(cls: Any, name: str, params: Any, val: Any)
+        Performs the specified check with the specified params on
+        the specified value
+        :param cls: pyoload.Check class
+        :param name: The registerred name of the check
+        :param params: The parameters to pass to the check
+        :param val: The value to check
+        """
         check = cls.checks_list.get(name)
         if check is None:
             raise Check.CheckDoesNotExistError(name)
         check(params, val)
 
     class CheckNameAlreadyExistsError(ValueError):
-        pass
+        """class CheckNameAlreadyExistsError(ValueError)
+        The check name to be registerred already exists
+        """
 
     class CheckDoesNotExistError(ValueError):
-        pass
+        """class CheckDoesNotExistError(ValueError)
+        The specified check does not exist
+        """
 
     class CheckError(Exception):
-        pass
+        """class CheckError(Exception)
+        Error occurring during check call.
+        """
 
 
 @Check.register('len')
 def len_check(params, val):
-    print(params, val)
     if isinstance(params, int):
         if not len(val) == params:
             raise Check.CheckError(f'length of {val!r} not eq {params!r}')
     elif isinstance(params, tuple) and len(params) > 0:
         mi = ma = None
         mi, ma = params
         if mi is not None:
@@ -98,77 +162,139 @@
             if not len(val) < ma:
                 raise Check.CheckError(f'length of {val!r} not lt {mi!r}')
 
 
 @Check.register('lt')
 def lt_check(param, val):
     if not val < param:
-        raise Check.CheckError()
+        raise Check.CheckError(f'{val!r} not lt {param!r}')
 
 
 @Check.register('le')
 def le_check(param, val):
     if not val <= param:
-        raise Check.CheckError()
+        raise Check.CheckError(f'{val!r} not gt {param!r}')
 
 
 @Check.register('ge')
 def ge_check(param, val):
     if not val >= param:
-        raise Check.CheckError()
+        raise Check.CheckError(f'{val!r} not ge {param!r}')
 
 
 @Check.register('gt')
 def gt_check(param, val):
     if not val > param:
-        raise Check.CheckError()
+        raise Check.CheckError(f'{val!r} not gt {param!r}')
+
+
+@Check.register('eq')
+def eq_check(param, val):
+    if not val == param:
+        raise Check.CheckError(f'{val!r} not eq {param!r}')
 
 
 @Check.register('func')
 def func_check(param, val):
     if not param(val):
-        raise Check.CheckError()
+        raise Check.CheckError(f'{param!r} call returned false on {val!r}')
 
 
-@Check.register('match_')
+@Check.register('type')
 def matches_check(param, val):
     if not typeMatch(val, param):
-        raise Check.CheckError()
+        raise Check.CheckError(f'{val!r} foes not match type {param!r}')
+
+
+@Check.register('isinstance')
+def instance_check(param, val):
+    if not isinstance(val, param):
+        raise Check.CheckError(f'{val!r} not instance of {param!r}')
+
+
+class Checks(PyoloadAnnotation):
+    """class Checks(Annotation)
+    Pyoload annotation holding several checks
+    """
 
+    def __init__(self: PyoloadAnnotation, **checks):
+        """def __init__(self: PyoloadAnnotation, **checks)
+        crates the check object,e.g
 
-class Checks:
-    def __init__(self, **checks):
+        class foo:
+            bar = pyoload.Checks(gt=4)
+        """
         self.checks = checks
-        print(f'{checks=}')
 
-    def __call__(self, val):
-        print(self.checks, val)
+    def __call__(self: PyoloadAnnotation, val: Any) -> None:
+        """def __call__(self: PyoloadAnnotation, val: Any) -> None
+        Performs the several checks contained in `self.checks`
+        """
         for name, params in self.checks.items():
             Check.check(name, params, val)
 
-    def __str__(self):
+    def __str__(self: Any) -> str:
         ret = '<Checks('
         for k, v in self.checks.items():
             ret += f'{k}={v!r}, '
         ret = ret[:-2] + ')>'
         return ret
 
     __repr__ = __str__
 
 
-class Cast:
+class CheckedAttr(Checks):
+    """class CheckedAttr(Checks)
+    A descriptor class providing attributes which are checked on assignment
+    """
+
+    name: str
+    value: Any
+
+    def __set_name__(self: Any, obj: Any, name: str, typo: Any = None):
+        """def __set_name__(self: Any, obj: Any, name: str, typo: Any = None)
+        setd the name of the attribute
+        """
+        self.name = name
+        self.value = None
+
+    def __get__(self: Any, obj: Any, type: Any):
+        """def __get__(self: Any, obj: Any, type: Any)
+        returns the value in `self.value`
+        """
+        return self.value
+
+    def __set__(self: Any, obj: Any, value: Any):
+        """def __set__(self: Any, obj: Any, value: Any)
+        Performs checks then assigns the new value
+        """
+        self(value)
+        self.value = value
+
+
+class Cast(PyoloadAnnotation):
+    """class Cast(PyoloadAnnotation)
+    Holds a cast object which describes the casts to be performed
+    """
     @staticmethod
-    def cast(val, totype):
+    def cast(val: Any, totype: Any) -> Any:
+        """def cast(val: Any, totype: Any) -> Any
+        The gratest deal.
+        Recursively casts the given value to the specified structure or type
+        e.g
+        Cast.cast({ 1: 2}, dict[str, float])
+
+        returns: {'1': 2.0}
+        """
         if isinstance(totype, GenericAlias):
             if totype.__origin__ == dict:
                 if len(totype.__args__) == 2:
                     kt, vt = totype.__args__
                 elif len(totype.__args__) == 1:
                     kt, vt = Any, totype.__args__[1]
-                print(f'{totype=} {kt=} {vt=}')
                 return {
                     Cast.cast(k, kt): Cast.cast(v, vt) for k, v in val.items()
                 }
             else:
                 sub = totype.__args__[0]
                 return totype.__origin__([
                     Cast.cast(v, sub) for v in val
@@ -181,50 +307,83 @@
                 except Exception as e:
                     errors.append(e)
             else:
                 raise errors
         else:
             return totype(val) if not isinstance(val, totype) else val
 
-    def __init__(self, type):
+    def __init__(self: PyoloadAnnotation, type: Any):
         """
         creates a casting object for the specified type
         """
         self.type = type
 
-    def __call__(self: 'Cast', val: Any):
+    def __call__(self: PyoloadAnnotation, val: Any):
         """
         Calls to the type specified in the object `.type` attribute
         :param self: The cast onject
         :param val: the value to be casted
 
         :return: The casted value
         """
         try:
             return Cast.cast(val, self.type)
         except Exception as e:
             raise CastingError(
                 f'Exception({e}) while casting: {val!r} to {self.type}',
             ) from e
 
+    def __str__(self):
+        return f'pyoload.Cast({self.type!s})'
+
+
+class CastedAttr(Cast):
+    """class CastedAttr(Cast)
+    A descriptor class providing attributes which are checked on assignment
+    """
+
+    name: str
+    value: Any
+
+    def __set_name__(self: Any, obj: Any, name: str, typo: Any = None):
+        """def __set_name__(self: Any, obj: Any, name: str, typo: Any = None)
+        setd the name of the attribute
+        """
+        self.name = name
+        self.value = None
+
+    def __get__(self: Any, obj: Any, type: Any):
+        """def __get__(self: Any, obj: Any, type: Any)
+        returns the value in `self.value`
+        """
+        return self.value
+
+    def __set__(self: Any, obj: Any, value: Any):
+        """def __set__(self: Any, obj: Any, value: Any)
+        Performs checks then assigns the new value
+        """
+        self.value = self(value)
+
 
 def typeMatch(val: Any, spec: type) -> bool:
     """
     recursively checks if type matches
     :param val: The value to typecheck
     :param spec: The type specifier
 
     :return: A boolean
     """
+    if spec == any:
+        raise TypeError('May be have you confused `Any` and `any`')
+
     if spec == Any or spec is None or val is None:
         return True
     if isinstance(spec, Values):
         return spec(val)
     elif isinstance(spec, Checks):
-        print(val)
         try:
             spec(val)
         except Check.CheckError:
             return False
         else:
             return True
     elif isinstance(spec, GenericAlias):
@@ -293,17 +452,19 @@
                     obj.__annotations__[k] = eval(v, obj.__globals__)
                 except Exception as e:
                     raise AnnotationResolutionError(
                         f'Exception: {k!s} while resolving'
                         f' annotation {v!r} of function {obj!r}',
                         f'globals: {obj.__globals__}',
                     ) from e
+    else:
+        raise AnnotationError(f'unknown resolution method for {obj}')
 
 
-def annotate(func: callable, oload: bool = False) -> callable:
+def annotate(func: Callable, oload: bool = False) -> Callable:
     """
     returns a wrapper over the passed function
     which typechecks arguments on each call
     :param func: the function to annotate
     :param oload: internal
 
     :returns: the wrapper function
@@ -367,15 +528,15 @@
                     f'{ann} of function {get_name(func)}',
                 )
         return ret
     wrapper.__pyod_annotate__ = func
     return wrapper
 
 
-__overloads__ = {}
+__overloads__: dict[str, list[Callable]] = {}
 
 
 def overload(func: callable, name: str | None = None):
     """
     returns a wrapper over the passed function
     which typechecks arguments on each call
     and finds the function instance with same name which does not raise
@@ -401,20 +562,21 @@
             except InternalAnnotationError:
                 continue
             else:
                 break
         else:
             raise OverloadError(
                 f'No overload of function: {get_name(func)}'
-                ' matches types of arguments',
+                f' matches types of arguments: {args}, {kw}',
             )
         return val
 
-    wrapper.__pyo_overloads__ = __overloads__[name]
-    wrapper.__pyo_overloads_name__ = name
+    wrapper.__pyod_overloads__ = __overloads__[name]
+    wrapper.__pyod_overloads_name__ = name
+    wrapper.overload = partial(overload, name=name)
 
     return wrapper
 
 
 def annotateClass(cls):
     """
     Annotates a class object, wrapping and replacing over it's __setattr__
@@ -437,26 +599,32 @@
                         getattr(
                             cls,
                             x,
                         ),
                     ),
                 )
 
-    def new_setter(self, name, value):
+    @wraps(cls.__setattr__)
+    def new_setter(self: Any, name: str, value: Any) -> Any:
+        """def new_setter(self: Any, name: str, value: Any) -> Any
+        """
         if any(isinstance(x, str) for x in self.__annotations__.values()):
             resolveAnnotations(self)
 
         if name not in self.__annotations__:
             if value is not None:
                 self.__annotations__[name] = type(value)
+        elif isinstance(self.__annotations__[name], Cast):
+            return setter(self, name, self.__annotations__[name](value))
         elif not typeMatch(value, self.__annotations__[name]):
             raise AnnotationError(
                 f'value {value!r} does not match annotation'
                 f'of attribute: {name!r}:{self.__annotations__[name]!r}'
                 f' of object of class {get_name(cls)}',
             )
         return setter(self, name, value)
     cls.__setattr__ = new_setter
     return cls
 
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
+__author__ = 'ken-morel'
```

### Comparing `pyoload-1.1.0/setup.py` & `pyoload-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from setuptools import setup, find_packages
 
 from pyoload import __version__
 
 project_dir = Path(__file__).parent
 
 try:
-    long_description = (project_dir / 'README.rst').read_text()
+    long_description = (project_dir / 'README.md').read_text()
 except FileNotFoundError:
     try:
-        long_description = Path('README.rst').read_text()
+        long_description = Path('README.md').read_text()
     except FileNotFoundError:
-        long_description = Path('/src/README.rst').read_text()
+        long_description = Path('/src/README.md').read_text()
 
 deps = ()
 
 extra_flake8 = (
     'flake8',
     'flake8-commas',
     'flake8-quotes',
@@ -39,26 +39,32 @@
     'coveralls',
 )
 
 setup(
     name='pyoload',
     version=__version__,
     packages=find_packages(exclude=['tests', 'tests.*']),
+    project_urls={
+        'Documentation': 'https://pyoload.readthedocs.io/',
+        'Funding': 'https://ko-fi.com/kenmorel',
+        'Source': 'https://github.com/ken-morel/pyoload/',
+        'Tracker': 'https://github.com/ken-morel/pyoload/issues',
+    },
     url='https://github.com/ken-morel/pyoload',
     license='MIT',
     author='ken-morel',
     author_email='engonken8@gmail.com',
     maintainer='ken-morel',
     maintainer_email='engonken8@gmail.com',
     description=(
         'Python package for function argument overload,'
         ' typechecking and casting'
     ),
     long_description=long_description,
-    long_description_content_type='text/x-rst',
+    long_description_content_type='text/markdown',
 
     install_requires=deps,
     extras_require={
         'dev': extra_dev,
         'ci': extra_ci,
     },
```

