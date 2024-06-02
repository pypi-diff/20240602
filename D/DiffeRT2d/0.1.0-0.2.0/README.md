# Comparing `tmp/differt2d-0.1.0.tar.gz` & `tmp/differt2d-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "differt2d-0.1.0.tar", max compression
+gzip compressed data, was "differt2d-0.2.0.tar", max compression
```

## Comparing `differt2d-0.1.0.tar` & `differt2d-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-10-02 09:15:30.712563 differt2d-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     3925 2023-10-02 09:15:30.712563 differt2d-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/__init__.py
--rw-r--r--   0        0        0       22 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/__version__.py
--rw-r--r--   0        0        0     7132 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/abc.py
--rw-r--r--   0        0        0      502 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/defaults.py
--rw-r--r--   0        0        0    29640 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/geometry.py
--rw-r--r--   0        0        0    16291 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/logic.py
--rw-r--r--   0        0        0     6251 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/optimize.py
--rw-r--r--   0        0        0    36820 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/scene.py
--rw-r--r--   0        0        0     2903 2023-10-02 09:15:30.716563 differt2d-0.1.0/differt2d/utils.py
--rw-r--r--   0        0        0     2183 2023-10-02 09:15:30.720564 differt2d-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5007 1970-01-01 00:00:00.000000 differt2d-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-29 13:58:13.878998 differt2d-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4356 2024-04-29 13:58:13.878998 differt2d-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/__version__.py
+-rw-r--r--   0        0        0     7132 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/abc.py
+-rw-r--r--   0        0        0      551 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/defaults.py
+-rw-r--r--   0        0        0    30109 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/geometry.py
+-rw-r--r--   0        0        0    17247 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/logic.py
+-rw-r--r--   0        0        0     6329 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/optimize.py
+-rw-r--r--   0        0        0    38780 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/scene.py
+-rw-r--r--   0        0        0     2775 2024-04-29 13:58:13.878998 differt2d-0.2.0/differt2d/utils.py
+-rw-r--r--   0        0        0     2288 2024-04-29 13:58:13.882999 differt2d-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 differt2d-0.2.0/PKG-INFO
```

### Comparing `differt2d-0.1.0/LICENSE.md` & `differt2d-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `differt2d-0.1.0/README.md` & `differt2d-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 <img alt="DiffeRT2d Logo" align="right" width="512px" src="https://raw.githubusercontent.com/jeertmans/DiffeRT2d/main/static/logo_light_transparent.png">
 
 # DiffeRT2d
 
+[![Latest Release][pypi-version-badge]][pypi-version-url]
+[![Python version][pypi-python-version-badge]][pypi-version-url]
 [![Documentation][documentation-badge]][documentation-url]
 [![codecov][codecov-badge]][codecov-url]
 
 Differentiable Ray Tracing (RT) Python framework for Telecommunications-oriented
 applications.
 
-> **NOTE**: the present work offers a simple Python module to create basic 2D scenarios,
-> and should be used for experimental purposes only.
+> [!IMPORTANT]
+> The present work offers a simple Python module to create basic 2D scenarios,
+> and should be used for experimental purposes only. For practical 3D applications,
+> checkout [DiffeRT](https://github.com/jeertmans/DiffeRT).
 
 - [Installation](#installation)
   * [Dependencies](#dependencies)
   * [Pip install](#pip-install)
   * [Install From Repository](#install-from-repository)
 - [Usage](#usage)
 - [Contributing](#contributing)
@@ -119,11 +123,14 @@
 
 Finally, if you do not have any GitHub account,
 or just wish to contact the author of DiffeRT2d,
 you can do so at: [jeertmans@icloud.com](mailto:jeertmans@icloud.com).
 
 <!-- end contact -->
 
+[pypi-version-badge]: https://img.shields.io/pypi/v/DiffeRT2d?label=DiffeRT2d
+[pypi-version-url]: https://pypi.org/project/DiffeRT2d/
+[pypi-python-version-badge]: https://img.shields.io/pypi/pyversions/DiffeRT2d
 [documentation-badge]: https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=documentation&up_color=green&up_message=online&url=https%3A%2F%2Feertmans.be%2FDiffeRT2d%2F
 [documentation-url]: https://eertmans.be/DiffeRT2d/
 [codecov-badge]: https://codecov.io/gh/jeertmans/DiffeRT2d/branch/main/graph/badge.svg?token=1dJ1AKWMR5
 [codecov-url]: https://codecov.io/gh/jeertmans/DiffeRT2d
```

### Comparing `differt2d-0.1.0/differt2d/abc.py` & `differt2d-0.2.0/differt2d/abc.py`

 * *Files identical despite different names*

### Comparing `differt2d-0.1.0/differt2d/geometry.py` & `differt2d-0.2.0/differt2d/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from jax import Array
     from matplotlib.artist import Artist
     from matplotlib.axes import Axes
 else:
     from chex import dataclass
 
 
-@partial(jax.jit, inline=True, static_argnames=["approx", "function"])
+@partial(jax.jit, static_argnames=["approx", "function"])
 def segments_intersect(
     P1: Array,
     P2: Array,
     P3: Array,
     P4: Array,
     tol: float = 0.005,
     approx: Optional[bool] = None,
@@ -108,15 +108,15 @@
     A = P2 - P1
     B = P3 - P4
     C = P1 - P3
     a = B[1] * C[0] - B[0] * C[1]  # alpha numerator
     b = A[0] * C[1] - A[1] * C[0]  # beta numerator
     d = A[1] * B[0] - A[0] * B[1]  # both denominator
 
-    @jax.jit
+    @partial(jax.jit, inline=True)
     def test(num, den):
         den_is_zero = den == 0.0
         den = jnp.where(den_is_zero, 1.0, den)
         t = jnp.where(den_is_zero, jnp.inf, num / den)
         return logical_and(
             greater_equal(t, -tol, approx=approx, **kwargs),
             less_equal(t, 1.0 + tol, approx=approx, **kwargs),
@@ -295,14 +295,15 @@
     """Cartesian coordinates."""
 
     def plot(
         self,
         ax: Axes,
         *args: Any,
         annotate: Optional[str] = None,
+        annotate_offset: Array = jnp.array([0.0, 0.0]),
         annotate_kwargs: Mapping[str, Any] = {},
         **kwargs: Any,
     ) -> List[Artist]:
         """
         :param annotate: Text to put next the the point.
         :param annotate_kwargs:
             Keyword arguments to be passed to
@@ -317,16 +318,17 @@
             [x],
             [y],
             *args,
             **kwargs,
         )
 
         if annotate:
+            xytext = self.point + jnp.asarray(annotate_offset, dtype=float)
             artists.append(
-                ax.annotate(annotate, xy=(x, y), xytext=(x, y), **annotate_kwargs)
+                ax.annotate(annotate, xy=(x, y), xytext=xytext, **annotate_kwargs)
             )
 
         return artists
 
     def bounding_box(self) -> Array:
         return jnp.vstack([self.point, self.point])
 
@@ -345,15 +347,15 @@
 
         ax = plt.gca()
         wall = Wall(points=jnp.array([[0., 0.], [1., 0.]]))
         _ = wall.plot(ax)
         plt.show()
     """
 
-    @jax.jit
+    @partial(jax.jit, inline=True)
     def normal(self) -> Array:
         """
         Returns the normal to the current wall, expressed in cartesian coordinates and
         normalized.
 
         :return: The normal, (2,)
         """
@@ -509,15 +511,15 @@
         """
         Returns a path from TX to RX, traversing each object in the list in the provided
         order.
 
         The present implementation will sample a point at :python:`t = 0.5`
         on each object.
 
-        :param tx: The emitting node, (2,).
+        :param tx: The transmitting node, (2,).
         :param objects:
             The list of objects to interact with (order is important).
         :param rx: The receiving node, (2,).
         :return: The resulting path.
 
         :Examples:
 
@@ -529,23 +531,23 @@
             from differt2d.geometry import Path
             from differt2d.scene import Scene
 
             ax = plt.gca()
             scene = Scene.square_scene()
             _ = scene.plot(ax)
             path = Path.from_tx_objects_rx(
-                scene.emitters["tx"].point,
+                scene.transmitters["tx"].point,
                 scene.objects,
                 scene.receivers["rx"].point
             )
             _ = path.plot(ax)
             plt.show()
         """
         points = [obj.parametric_to_cartesian(0.5) for obj in objects]
-        points = jnp.vstack([tx, points, rx])
+        points = jnp.vstack([tx, *points, rx])
         return cls(points=points)
 
     @jax.jit
     def length(self) -> Array:
         """
         Returns the length of this path.
 
@@ -587,15 +589,15 @@
 
         return contains
 
     @partial(jax.jit, inline=True, static_argnames=["approx", "function"])
     def intersects_with_objects(
         self,
         objects: List[Interactable],
-        path_candidate: List[int],
+        path_candidate: Array,
         patch: float = DEFAULT_PATCH,
         approx: Optional[bool] = None,
         **kwargs: Any,
     ) -> Array:
         """
         Returns whether the path intersects with any of the objects.
 
@@ -607,15 +609,15 @@
         :param patch: The patch value for intersection check,
             see :meth:`Interactable.intersects_cartesian<differt2d.abc.Interactable.intersects_cartesian>`.
         :param approx: Whether approximation is enabled or not.
         :param kwargs: Keyword arguments to be passed to
             :func:`activation<differt2d.logic.activation>`.
         :return: Whether this path intersects any of the objects, ().
         """
-        interacting_object_indices = [-1] + [i - 1 for i in path_candidate[1:-1]] + [-1]
+        interacting_object_indices = [-1] + [i for i in path_candidate] + [-1]
         intersects = false_value(approx=approx)
 
         for i in range(self.points.shape[0] - 1):
             ray_path = self.points[i : i + 2, :]
             for obj_index, obj in enumerate(objects):
                 ignore = jnp.logical_or(
                     obj_index == interacting_object_indices[i + 0],
@@ -634,18 +636,19 @@
                         ),
                         approx=approx,
                     ),
                 )
 
         return intersects
 
+    @partial(jax.jit, inline=True, static_argnames=["approx", "function"])
     def is_valid(
         self,
         objects: List[Interactable],
-        path_candidate: List[int],
+        path_candidate: Array,
         interacting_objects: List[Interactable],
         tol: float = 1e-2,
         patch: float = DEFAULT_PATCH,
         approx: Optional[bool] = None,
         **kwargs: Any,
     ) -> Array:
         """
@@ -655,15 +658,15 @@
         1. the path loss is below some tolerance;
         2. the coordinate points are correctly placed inside the corresponding
            interacting objects;
         3. and the path does not intersect with any of the objects in the scene
            (except those concerned by 2.).
 
         :param objects: The objects in the scene.
-        :param path_candidate: The list of indices of interacting objects,
+        :param path_candidate: The array of indices of interacting objects,
             usually generated with
             :meth:`Scene.all_path_candidates<differt2d.scene.Scene.all_path_candidates>`
         :param interacting_objects: The list of interacting objects,
             usually obtained by calling
             :meth:`Scene.get_interacting_objects<differt2d.scene.Scene.get_interacting_objects>`.
         :param tol: The maximum allowed value for the path loss before it is considered
             invalid. I.e., a path loss greater than ``tol`` will make this path invalid.
@@ -735,15 +738,15 @@
         objects: List[Wall],
         rx: Array,
         **kwargs: Any,
     ) -> "ImagePath":
         """
         Returns a path with minimal length.
 
-        :param tx: The emitting node, (2,).
+        :param tx: The transmitting node, (2,).
         :param objects:
             The list of walls to interact with (order is important).
         :param rx: The receiving node, (2,).
         :return: The resulting path of the Image method.
 
         :Examples:
 
@@ -755,15 +758,15 @@
             from differt2d.geometry import ImagePath
             from differt2d.scene import Scene
 
             ax = plt.gca()
             scene = Scene.square_scene()
             _ = scene.plot(ax)
             path = ImagePath.from_tx_objects_rx(
-                scene.emitters["tx"].point,
+                scene.transmitters["tx"].point,
                 scene.objects,
                 scene.receivers["rx"].point
             )
             _ = path.plot(ax)
             plt.show()
         """
         n = len(objects)
@@ -798,47 +801,48 @@
             inc = jnp.where(un == 0.0, 0.0, vn * u / un)
             point = point + inc
             return point, point
 
         _, images = jax.lax.scan(forward, init=tx, xs=walls)
         _, points = jax.lax.scan(backward, init=rx, xs=(walls, images), reverse=True)
 
-        points = jnp.vstack([tx, points, rx])
+        points = jnp.vstack([tx, *points, rx])
 
         return cls(points=points, loss=path_loss(points))
 
 
 @dataclass
 class FermatPath(Path):
     """A path object that was obtained with the Fermat's Principle Tracing method."""
 
     @classmethod
-    @partial(jax.jit, static_argnames=("cls", "steps", "optimizer"))
+    @partial(jax.jit, static_argnames=["cls", "steps", "optimizer"])
     def from_tx_objects_rx(
         cls,
         tx: Array,
         objects: List[Interactable],
         rx: Array,
         key: Optional[Array] = None,
         seed: int = 1234,
         **kwargs: Any,
     ) -> "FermatPath":
         """
         Returns a path with minimal length.
 
-        :param tx: The emitting node, (2,).
+        :param tx: The transmitting node, (2,).
         :param objects:
             The list of objects to interact with (order is important).
         :param rx: The receiving node, (2,).
         :param key: The random key to generate the initial guess.
         :param seed: The random seed used to generate the start iteration,
             only used if :python:`key is None`.
         :param kwargs:
             Keyword arguments to be passed to
             :func:`minimize_many_random_uniform<differt2d.optimize.minimize_many_random_uniform>`.
+            Note that the ``many`` parameter defaults to ``1`` here.
         :return: The resulting path of the FPT method.
 
         :Examples:
 
         .. plot::
             :include-source: true
 
@@ -847,15 +851,15 @@
             from differt2d.geometry import FermatPath
             from differt2d.scene import Scene
 
             ax = plt.gca()
             scene = Scene.square_scene()
             _ = scene.plot(ax)
             path = FermatPath.from_tx_objects_rx(
-                scene.emitters["tx"].point,
+                scene.transmitters["tx"].point,
                 scene.objects,
                 scene.receivers["rx"].point
             )
             _ = path.plot(ax)
             plt.show()
         """
         n = len(objects)
@@ -879,14 +883,16 @@
                 _loss += obj.evaluate_cartesian(cartesian_coords[i : i + 3, :])
 
             return _loss
 
         if key is None:
             key = jax.random.PRNGKey(seed)
 
+        kwargs.setdefault("many", 1)
+
         theta, _ = minimize_many_random_uniform(
             fun=loss_fun, n=n_unknowns, key=key, **kwargs
         )
 
         points = parametric_to_cartesian(objects, theta, n, tx, rx)
 
         return cls(points=points, loss=path_loss(points))
@@ -906,24 +912,25 @@
         key: Optional[Array] = None,
         seed: int = 1234,
         **kwargs: Any,
     ) -> "MinPath":
         """
         Returns a path that minimizes the sum of interactions.
 
-        :param tx: The emitting node, (2,).
+        :param tx: The transmitting node, (2,).
         :param objects:
             The list of objects to interact with (order is important).
         :param rx: The receiving node, (2,).
         :param key: The random key to generate the initial guess.
         :param seed: The random seed used to generate the start iteration,
             only used if :python:`key is None`.
         :param kwargs:
             Keyword arguments to be passed to
             :func:`minimize_many_random_uniform<differt2d.optimize.minimize_many_random_uniform>`.
+            Note that the ``many`` parameter defaults to ``1`` here.
         :return: The resulting path of the MPT method.
 
         :Examples:
 
         .. plot::
             :include-source: true
 
@@ -932,15 +939,15 @@
             from differt2d.geometry import MinPath
             from differt2d.scene import Scene
 
             ax = plt.gca()
             scene = Scene.square_scene()
             _ = scene.plot(ax)
             path = MinPath.from_tx_objects_rx(
-                scene.emitters["tx"].point,
+                scene.transmitters["tx"].point,
                 scene.objects,
                 scene.receivers["rx"].point
             )
             _ = path.plot(ax)
             plt.show()
         """
         n = len(objects)
@@ -960,14 +967,16 @@
                 _loss += obj.evaluate_cartesian(cartesian_coords[i : i + 3, :])
 
             return _loss
 
         if key is None:
             key = jax.random.PRNGKey(seed)
 
+        kwargs.setdefault("many", 1)
+
         theta, loss = minimize_many_random_uniform(
             fun=loss_fun, n=n_unknowns, key=key, **kwargs
         )
 
         points = parametric_to_cartesian(objects, theta, n, tx, rx)
 
         return cls(points=points, loss=loss)
```

### Comparing `differt2d-0.1.0/differt2d/logic.py` & `differt2d-0.2.0/differt2d/logic.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,75 +9,101 @@
 when :code:`approx` is set to :python:`False`.
 
 .. note::
 
     Whenever a function takes an argument named ``approx``, it can take
     three different values:
 
-    1. :python:`None`: defaults to :py:attr:`jax.config.jax_enable_approx`,
+    1. :python:`None`: defaults to :py:data:`differt2d.logic.ENABLE_APPROX`,
        see :py:func:`enable_approx` for comments on that;
     2. :python:`True`: forces to enable approximation;
     3. or :python:`False`: forces to disable approximation.
 """
 
 from __future__ import annotations
 
 __all__ = [
+    "ENABLE_APPROX",
     "activation",
+    "set_approx",
     "disable_approx",
     "enable_approx",
     "greater",
     "greater_equal",
+    "hard_sigmoid",
     "is_false",
     "is_true",
     "less",
     "less_equal",
     "logical_all",
     "logical_and",
     "logical_any",
     "logical_not",
     "logical_or",
+    "sigmoid",
 ]
 
+import os
 from contextlib import contextmanager
 from functools import partial
-from typing import TYPE_CHECKING, Any, Literal, Optional, Tuple, Union
+from threading import Lock
+from typing import Any, Callable, Optional, Tuple, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
+from jax import Array
 
-from .defaults import DEFAULT_ALPHA, DEFAULT_FUNCTION
+from .defaults import DEFAULT_ALPHA
 
-if TYPE_CHECKING:  # pragma: no cover
-    from jax import Array
+ENABLE_APPROX: bool = "ENABLE_APPROX" not in os.environ
+"""Enable approximation using some activation function."""
 
-_enable_approx = jax.config.define_bool_state(
-    name="jax_enable_approx",
-    default=True,
-    help=("Enable approximation using some activation function."),
-)
+_LOCK = Lock()
+"""Lock to prevent mutating ``ENABLE_APPROX`` in multiple threads."""
 
-jit_approx = partial(jax.jit, inline=True, static_argnames=["approx", "function"])
+
+def set_approx(enable: bool):
+    """
+    Enable or disable the approximation in future function calls.
+
+    Note that JIT-compiled version will not be affected if they
+    were compiled before this function was called.
+
+    :param enable: Whether to enable or not approximation.
+
+    :Examples:
+
+    >>> from differt2d.logic import greater, set_approx
+    >>>
+    >>> # doc: hide
+    >>> greater.clear_cache()
+    >>> # doc: hide
+    >>> set_approx(False)
+    >>> print(greater(20.0, 5.0))
+    True
+    """
+    global ENABLE_APPROX
+
+    ENABLE_APPROX = enable
 
 
 @contextmanager
 def enable_approx(enable: bool = True):
     """
     Context manager for enabling or disabling approximation of true/false values with
     continuous numbers from 0 (false) to 1 (true).
 
     By default, approximation is enabled.
 
     To disable approximation, you have multiple options:
 
     1. use this context manager to disable it (see example below);
-    2. set the environ variable ``JAX_ENABLE_APPROX`` to ``0``
-       (or any falsy value);
+    2. set the environ variable ``DISABLE_APPROX`` (any value);
     3. update the config with
-       :python:`jax.config.update("jax_enable_approx", False)`;
+       :py:func:`set_approx(False)`;
     4. or set, for specific logic functions only, the keyword argument
        ``approx`` to :python:`False`.
 
     :param enable: Whether to enable or not approximation.
 
     :Examples:
 
@@ -106,26 +132,27 @@
     >>> # doc: hide
     >>> with enable_approx():
     ...     print(greater(20.0, 5.0))
     1.0
 
     .. warning::
 
-        Calling already-jitted functions after mutating ``jax_enable_approx``
+        Calling already-jitted functions after mutating ``ENABLE_APPROX``
         will not produce any visible change. This is because
-        ``jax.config.jax_enable_approx`` is evaluated once, at compilation.
+        ``differt2d.logic.ENABLE_APPROX`` is evaluated once, at compilation.
 
         For example:
 
         >>> import jax
+        >>> import differt2d.logic
         >>> from differt2d.logic import enable_approx
         >>>
         >>> @jax.jit
         ... def f():
-        ...     if jax.config.jax_enable_approx:
+        ...     if differt2d.logic.ENABLE_APPROX:
         ...         return 1.0
         ...     else:
         ...         return 0.0
         >>>
         >>> with enable_approx(True):
         ...     print(f())
         1.0
@@ -138,29 +165,35 @@
         :py:func:`jax.disable_jit` or use the ``approx`` parameter
         when available.
 
         >>> from jax import disable_jit
         >>>
         >>> @jax.jit
         ... def f():
-        ...     if jax.config.jax_enable_approx:
+        ...     if differt2d.logic.ENABLE_APPROX:
         ...         return 1.0
         ...     else:
         ...         return 0.0
         >>>
         >>> with enable_approx(True), disable_jit():
         ...     print(f())
         1.0
         >>>
         >>> with enable_approx(False), disable_jit():
         ...     print(f())
         0.0
     """
-    with _enable_approx(enable):
-        yield
+    global ENABLE_APPROX
+    state = ENABLE_APPROX
+    with _LOCK:
+        try:
+            ENABLE_APPROX = enable
+            yield
+        finally:
+            ENABLE_APPROX = state
 
 
 @contextmanager
 def disable_approx(disable: bool = True):  # pragma: no cover
     """
     Context manager for disable or enabling approximation of true/false values with
     continuous numbers from 0 (false) to 1 (true).
@@ -171,83 +204,112 @@
     :param disable: Whether to disable or not approximation.
 
     .. note::
 
         Contrary to :py:func:`enable_approx`, there is no ``JAX_DISABLE_APPROX``
         environ variable, nor ``jax.config.jax_disable_approx`` config variable.
     """
-    with _enable_approx(not disable):
+    with enable_approx(not disable):
         yield
 
 
+X = TypeVar("X", bound=Array)
+Y = TypeVar("Y", bound=Array)
+
+
+@partial(jax.jit, inline=True)
+def sigmoid(x: Array, alpha: float) -> Array:
+    r"""
+    Element-wise sigmoid, parametrized with ``alpha``.
+
+    .. math::
+        \text{sigmoid}(x;\alpha) = \frac{1}{1 + e^{-\alpha x}},
+
+    where :math:`\alpha` (``alpha``) is a slope parameter.
+
+    See :func:`jax.nn.sigmoid` for more details.
+
+    :param x: The input array.
+    :param alpha: The slope parameter.
+    :return: The corresponding values.
+    """
+    return jax.nn.sigmoid(alpha * x)
+
+
+@partial(jax.jit, inline=True)
+def hard_sigmoid(x: Array, alpha: float) -> Array:
+    r"""
+    Element-wise sigmoid, parametrized with ``alpha``.
+
+    .. math::
+        \text{hard_sigmoid}(x;\alpha) = \frac{\text{relu6}(\alpha x + 3)}{6},
+
+    where :math:`\alpha` (``alpha``) is a slope parameter.
+
+    See :func:`jax.nn.hard_sigmoid` and :func:`jax.nn.relu6` for more details.
+
+    :param x: The input array.
+    :param alpha: The slope parameter.
+    :return: The corresponding values.
+    """
+    return jax.nn.hard_sigmoid(alpha * x)
+
+
 @partial(jax.jit, inline=True, static_argnames=["function"])
 def activation(
     x: Array,
     alpha: float = DEFAULT_ALPHA,
-    function: Literal["sigmoid", "hard_sigmoid"] = DEFAULT_FUNCTION,
+    function: Callable[[X, float], Y] = hard_sigmoid,
 ) -> Array:
     r"""
     Element-wise function for approximating a discrete transition between 0 and 1, with
     a smoothed transition centered at :python:`x = 0.0`.
 
     Depending on the ``function`` argument, the activation function has the
-    following definition:
-
-    .. math::
-        \text{sigmoid}(x;\alpha) = \frac{1}{1 + e^{-\alpha x}},
-
-    or
-
-    .. math::
-        \text{hard_sigmoid}(x;\alpha) = \frac{\text{relu6}(\alpha x+3)}{6},
-
-    where :math:`\alpha` (:code:`alpha`) is a slope parameter.
+    different definition.
 
-    See :func:`jax.nn.sigmoid` or :func:`jax.nn.hard_sigmoid` for more details.
+    Two basic activation functions are provided: :func:`sigmoid` and :func:`hard_sigmoid`.
+    If needed, you can implement your own activation function and pass it as an argument,
+    granted that it satisfies the properties defined in the related paper.
 
     :param x: The input array.
     :param alpha: The slope parameter.
     :return: The corresponding values.
 
     :EXAMPLES:
 
     .. plot::
         :include-source: true
 
         import matplotlib.pyplot as plt
         import numpy as np
-        from differt2d.logic import activation
+        from differt2d.logic import activation, hard_sigmoid, sigmoid
         from jax import grad, vmap
 
         x = np.linspace(-5, +5, 200)
 
         _, (ax1, ax2) = plt.subplots(2, 1, sharex=True, figsize=[6.4, 8])
 
-        for function in ["sigmoid", "hard_sigmoid"]:
+        for name, function in [("sigmoid", sigmoid), ("hard_sigmoid", hard_sigmoid)]:
             def f(x):
-                return activation(x, alpha=1.0, function=function)
+                return activation(x, alpha=1.5, function=function)
 
             y = f(x)
             dydx = vmap(grad(f))(x)
-            _ = ax1.plot(x, y, "--", label=f"{function}")
-            _ = ax2.plot(x, dydx, "-", label=f"{function}")
+            _ = ax1.plot(x, y, "--", label=f"{name}")
+            _ = ax2.plot(x, dydx, "-", label=f"{name}")
 
         ax2.set_xlabel("$x$")
         ax1.set_ylabel("$f(x)$")
         ax2.set_ylabel(r"$\frac{\partial f(x)}{\partial x}$")
         plt.legend()
         plt.tight_layout()
         plt.show()
     """
-    if function == "sigmoid":
-        return jax.nn.sigmoid(alpha * x)
-    elif function == "hard_sigmoid":
-        return jax.nn.hard_sigmoid(alpha * x)
-    else:
-        raise ValueError(f"Unknown function '{function}'")
+    return function(x, alpha)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def logical_or(x: Array, y: Array, approx: Optional[bool] = None) -> Array:
     """
     Element-wise logical :python:`x or y`.
 
@@ -256,15 +318,15 @@
 
     :param x: The first input array.
     :param y: The second input array.
     :param approx: Whether approximation is enabled or not.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.maximum(x, y) if approx else jnp.logical_or(x, y)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def logical_and(x: Array, y: Array, approx: Optional[bool] = None) -> Array:
     """
     Element-wise logical :python:`x and y`.
@@ -274,15 +336,15 @@
 
     :param x: The first input array.
     :param y: The second input array.
     :param approx: Whether approximation is enabled or not.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.minimum(x, y) if approx else jnp.logical_and(x, y)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def logical_not(x: Array, approx: Optional[bool] = None) -> Array:
     """
     Element-wise logical :python:`not x`.
@@ -292,15 +354,15 @@
     :func:`jax.numpy.logical_or` otherwise.
 
     :param x: The input array.
     :param approx: Whether approximation is enabled or not.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.subtract(1.0, x) if approx else jnp.logical_not(x)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx", "function"])
 def greater(
     x: Array,
     y: Array,
@@ -318,15 +380,15 @@
     :param y: The second input array.
     :param approx: Whether approximation is enabled or not.
     :param kwargs:
         Keyword arguments to be passed to :func:`activation`.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return activation(jnp.subtract(x, y), **kwargs) if approx else jnp.greater(x, y)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx", "function"])
 def greater_equal(
     x: Array, y: Array, approx: Optional[bool] = None, **kwargs: Any
 ) -> Array:
@@ -341,15 +403,15 @@
     :param y: The second input array.
     :param approx: Whether approximation is enabled or not.
     :param kwargs:
         Keyword arguments to be passed to :func:`activation`.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return (
         activation(jnp.subtract(x, y), **kwargs) if approx else jnp.greater_equal(x, y)
     )
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx", "function"])
 def less(x: Array, y: Array, approx: Optional[bool] = None, **kwargs: Any) -> Array:
@@ -364,15 +426,15 @@
     :param y: The second input array.
     :param approx: Whether approximation is enabled or not.
     :param kwargs:
         Keyword arguments to be passed to :func:`activation`.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return activation(jnp.subtract(y, x), **kwargs) if approx else jnp.less(x, y)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx", "function"])
 def less_equal(
     x: Array,
     y: Array,
@@ -390,15 +452,15 @@
     :param y: The second input array.
     :param approx: Whether approximation is enabled or not.
     :param kwargs:
         Keyword arguments to be passed to :func:`activation`.
     :return: Output array, with element-wise comparison.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return activation(jnp.subtract(y, x), **kwargs) if approx else jnp.less_equal(x, y)
 
 
 @partial(jax.jit, inline=True, static_argnames=["axis", "approx"])
 def logical_all(
     *x: Array,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
@@ -413,15 +475,15 @@
     :param x: The input array, or array-like.
     :param axis: Axis or axes along which to operate.
         By default, flattened input is used.
     :param approx: Whether approximation is enabled or not.
     :return: Output array.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     arr = jnp.asarray(x)
     return jnp.min(arr, axis=axis) if approx else jnp.all(arr, axis=axis)
 
 
 @partial(jax.jit, inline=True, static_argnames=["axis", "approx"])
 def logical_any(
     *x: Array,
@@ -437,15 +499,15 @@
     :param x: The input array, or array-like.
     :param axis: Axis or axes along which to operate.
         By default, flattened input is used.
     :param approx: Whether approximation is enabled or not.
     :return: Output array.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     arr = jnp.asarray(x)
     return jnp.max(arr, axis=axis) if approx else jnp.any(arr, axis=axis)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def is_true(x: Array, tol: float = 0.5, approx: Optional[bool] = None) -> Array:
     """
@@ -457,15 +519,15 @@
     :param x: The input array.
     :param tol: The tolerance on how close it should be to 1.
         Only used if :code:`approx` is set to :python:`True`.
     :param approx: Whether approximation is enabled or not.
     :return: True array if the value is considered to be true.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.greater(x, 1.0 - tol) if approx else jnp.asarray(x)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def is_false(x: Array, tol: float = 0.5, approx: Optional[bool] = None) -> Array:
     """
     Element-wise check if a given truth value can be considered to be false.
@@ -476,39 +538,39 @@
     :param x: The input array.
     :param tol: The tolerance on how close it should be to 0.
         Only used if :code:`approx` is set to :python:`True`.
     :param approx: Whether approximation is enabled or not.
     :return: True if the value is considered to be false.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.less(x, tol) if approx else jnp.logical_not(x)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def true_value(approx: Optional[bool] = None) -> Array:
     """
     Returns a scalar true value.
 
     When using approximation, this function returns 1.
 
     :param approx: Whether approximation is enabled or not.
     :return: A value that evaluates to true.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.array(1.0) if approx else jnp.array(True)
 
 
 @partial(jax.jit, inline=True, static_argnames=["approx"])
 def false_value(approx: Optional[bool] = None) -> Array:
     """
     Returns a scalar false value.
 
     When using approximation, this function returns 0.
 
     :param approx: Whether approximation is enabled or not.
     :return: A value that evaluates to false.
     """
     if approx is None:
-        approx = jax.config.jax_enable_approx  # type: ignore[attr-defined]
+        approx = ENABLE_APPROX
     return jnp.array(0.0) if approx else jnp.array(False)
```

### Comparing `differt2d-0.1.0/differt2d/optimize.py` & `differt2d-0.2.0/differt2d/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,17 +191,19 @@
     ...     x = x - 1.0
     ...     return jnp.dot(x, x)
     >>>
     >>> x, y = minimize_many_random_uniform(f, jax.random.PRNGKey(1234), 10)
     >>> chex.assert_trees_all_close(x, jnp.ones(10), rtol=1e-2)
     >>> chex.assert_trees_all_close(y, 0.0, atol=1e-4)
     """
+    if many == 1:
+        return minimize_random_uniform(fun=fun, key=key, n=n, **kwargs)
+
     keys = jax.random.split(key, num=many)
 
-    @jax.jit
     def _minimize(key):
         return minimize_random_uniform(fun=fun, key=key, n=n, **kwargs)
 
     xs, losses = vmap(_minimize, in_axes=0)(keys)
 
     i_min = jnp.argmin(losses)
```

### Comparing `differt2d-0.1.0/differt2d/scene.py` & `differt2d-0.2.0/differt2d/scene.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Scenes for tracing rays between emitters and receivers."""
+"""Scenes for tracing rays between transmitters and receivers."""
 
 from __future__ import annotations
 
 __all__ = ["Scene", "SceneName"]
 
 import json
-from functools import singledispatchmethod
+from functools import partial, singledispatchmethod
 from itertools import groupby, product
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
@@ -20,18 +20,17 @@
     Sequence,
     Tuple,
     Type,
     Union,
     runtime_checkable,
 )
 
+import differt_core
 import jax
 import jax.numpy as jnp
-import numpy as np
-import rustworkx as rx
 
 from .abc import Interactable, Loc, Object, Plottable
 from .geometry import ImagePath, Path, Point, Wall, closest_point
 from .logic import is_true
 
 if TYPE_CHECKING:  # pragma: no cover
     from dataclasses import dataclass
@@ -53,24 +52,24 @@
 ]
 """Literal type for all valid scene names."""
 
 
 @runtime_checkable
 class Readable(Protocol):
     def read(self) -> S:
-        pass
+        pass  # pragma: no cover
 
 
 @dataclass
 class Scene(Plottable):
-    """2D Scene made of objects, one or more emitting node(s), and one or more receiving
-    node(s)."""
+    """2D Scene made of objects, one or more transmitting node(s), and one or more
+    receiving node(s)."""
 
-    emitters: Dict[str, Point]
-    """The emitting nodes."""
+    transmitters: Dict[str, Point]
+    """The transmitting nodes."""
     receivers: Dict[str, Point]
     """The receiving nodes."""
     objects: List[Object]
     """The list of objects in the scene."""
 
     @singledispatchmethod
     @classmethod
@@ -284,30 +283,30 @@
             if geometry := feature.get("geometry", None):
                 _type = geometry["type"]
                 coordinates = geometry["coordinates"][0]
                 n = len(coordinates)
 
                 if _type == "Polygon":
                     for i in range(n):
-                        points = jnp.vstack(
+                        points = jnp.array(
                             [coordinates[i - 1], coordinates[i]], dtype=float
                         )
                         wall = Wall(points=points)
                         walls.append(wall)
 
         if len(walls) > 0:
             tx = Point(point=walls[0].origin())
             rx = Point(point=walls[0].dest())
 
-        else:
+        else:  # pragma: no cover
             tx = Point(point=jnp.array([0.0, 0.0]))
             rx = Point(point=jnp.array([1.0, 1.0]))
 
-        scene = cls(emitters=dict(tx=tx), receivers=dict(rx=rx), objects=walls)  # type: ignore[arg-type]
-        scene.emitters["tx"] = Point(point=scene.get_location(tx_loc))
+        scene = cls(transmitters=dict(tx=tx), receivers=dict(rx=rx), objects=walls)  # type: ignore[arg-type]
+        scene.transmitters["tx"] = Point(point=scene.get_location(tx_loc))
         scene.receivers["rx"] = Point(point=scene.get_location(rx_loc))
         return scene
 
     @from_geojson.register(Readable)
     @classmethod
     def _(cls, fp: Readable, *args: Any, **kwargs: Any) -> "Scene":
         return cls.from_geojson(fp.read(), *args, **kwargs)
@@ -331,23 +330,23 @@
         return getattr(cls, scene_name)(*args, **kwargs)
 
     @classmethod
     def random_uniform_scene(
         cls,
         key: Array,
         *,
-        n_emitters: int = 1,
+        n_transmitters: int = 1,
         n_walls: int = 1,
         n_receivers: int = 1,
     ) -> "Scene":
         """
         Generates a random scene, drawing coordinates from a random distribution.
 
         :param key: The random key to be used.
-        :param n_emitters: The number of emitters.
+        :param n_transmitters: The number of transmitters.
         :param n_walls: The number of walls.
         :param n_receivers: The number of receivers.
         :return: The scene.
 
         :Examples:
 
         .. code-block::
@@ -358,52 +357,56 @@
 
             ax = plt.gca()
             key = jax.random.PRNGKey(1234)
             scene = Scene.random_uniform_scene(key, n_walls=5)
             _ = scene.plot(ax)
             plt.show()
         """
-        points = jax.random.uniform(key, (n_emitters + 2 * n_walls + n_receivers, 2))
-        emitters = {f"tx_{i}": Point(point=points[i, :]) for i in range(n_emitters)}
+        points = jax.random.uniform(
+            key, (n_transmitters + 2 * n_walls + n_receivers, 2)
+        )
+        transmitters = {
+            f"tx_{i}": Point(point=points[i, :]) for i in range(n_transmitters)
+        }
         receivers = {
             f"rx_{i}": Point(point=points[-(i + 1), :]) for i in range(n_receivers)
         }
 
         walls: List[Object] = [
-            Wall(points=points[2 * i + n_emitters : 2 * i + 2 + n_emitters, :])
+            Wall(points=points[2 * i + n_transmitters : 2 * i + 2 + n_transmitters, :])
             for i in range(n_walls)
         ]
-        return cls(emitters=emitters, receivers=receivers, objects=walls)
+        return cls(transmitters=transmitters, receivers=receivers, objects=walls)
 
     @classmethod
     def basic_scene(
         cls,
         *,
         tx_coords: Array = jnp.array([0.1, 0.1]),
         rx_coords: Array = jnp.array([0.302, 0.2147]),
     ) -> "Scene":
         """
         Instantiates a basic scene with a main room, and a second inner room in the
         lower left corner, with a small entrance.
 
-        :param tx_coords: The emitter's coordinates, array-like, (2,).
+        :param tx_coords: The transmitter's coordinates, array-like, (2,).
         :param rx_coords: The receiver's coordinates, array-like, (2,).
         :return: The scene.
 
         :Examples:
 
         >>> from differt2d.scene import Scene
         >>>
         >>> scene = Scene.basic_scene()
         >>> scene.bounding_box()
         Array([[0., 0.],
                [1., 1.]], dtype=float32)
         >>> len(scene.objects)
         7
-        >>> scene.emitters["tx"]
+        >>> scene.transmitters["tx"]
         Point(point=Array([0.1, 0.1], dtype=float32))
 
         .. plot::
 
             import matplotlib.pyplot as plt
             from differt2d.scene import Scene
 
@@ -423,41 +426,41 @@
             Wall(points=jnp.array([[0.0, 1.0], [0.0, 0.0]])),
             # Small room
             Wall(points=jnp.array([[0.4, 0.0], [0.4, 0.4]])),
             Wall(points=jnp.array([[0.4, 0.4], [0.3, 0.4]])),
             Wall(points=jnp.array([[0.1, 0.4], [0.0, 0.4]])),
         ]
 
-        return cls(emitters=dict(tx=tx), receivers=dict(rx=rx), objects=walls)
+        return cls(transmitters=dict(tx=tx), receivers=dict(rx=rx), objects=walls)
 
     @classmethod
     def square_scene(
         cls,
         *,
         tx_coords: Array = jnp.array([0.2, 0.2]),
         rx_coords: Array = jnp.array([0.5, 0.6]),
     ) -> "Scene":
         """
         Instantiates a square scene with one main room.
 
-        :param tx_coords: The emitter's coordinates, array-like, (2,).
+        :param tx_coords: The transmitter's coordinates, array-like, (2,).
         :param rx_coords: The receiver's coordinates, array-like, (2,).
         :return: The scene.
 
         :Examples:
 
         >>> from differt2d.scene import Scene
         >>>
         >>> scene = Scene.square_scene()
         >>> scene.bounding_box()
         Array([[0., 0.],
                [1., 1.]], dtype=float32)
         >>> len(scene.objects)
         4
-        >>> scene.emitters["tx"]
+        >>> scene.transmitters["tx"]
         Point(point=Array([0.2, 0.2], dtype=float32))
 
         .. plot::
 
             import matplotlib.pyplot as plt
             from differt2d.scene import Scene
 
@@ -472,44 +475,44 @@
         walls: List[Object] = [
             Wall(points=jnp.array([[0.0, 0.0], [1.0, 0.0]])),
             Wall(points=jnp.array([[1.0, 0.0], [1.0, 1.0]])),
             Wall(points=jnp.array([[1.0, 1.0], [0.0, 1.0]])),
             Wall(points=jnp.array([[0.0, 1.0], [0.0, 0.0]])),
         ]
 
-        return Scene(emitters=dict(tx=tx), receivers=dict(rx=rx), objects=walls)
+        return Scene(transmitters=dict(tx=tx), receivers=dict(rx=rx), objects=walls)
 
     @classmethod
     def square_scene_with_wall(
         cls,
         ratio: float = 0.1,
         *,
         tx_coords: Array = jnp.array([0.2, 0.5]),
         rx_coords: Array = jnp.array([0.8, 0.5]),
     ) -> "Scene":
         """
         Instantiates a square scene with one main room, and vertical wall in the middle.
 
         :param ratio: The ratio of the obstacle's side length to
             the room's side length.
-        :param tx_coords: The emitter's coordinates, array-like, (2,).
+        :param tx_coords: The transmitter's coordinates, array-like, (2,).
         :param rx_coords: The receiver's coordinates, array-like, (2,).
         :return: The scene.
 
         :Examples:
 
         >>> from differt2d.scene import Scene
         >>>
         >>> scene = Scene.square_scene_with_wall()
         >>> scene.bounding_box()
         Array([[0., 0.],
                [1., 1.]], dtype=float32)
         >>> len(scene.objects)
         5
-        >>> scene.emitters["tx"]
+        >>> scene.transmitters["tx"]
         Point(point=Array([0.2, 0.5], dtype=float32))
 
         .. plot::
 
             import matplotlib.pyplot as plt
             from differt2d.scene import Scene
 
@@ -544,15 +547,15 @@
         >>>
         >>> scene = Scene.square_scene_with_obstacle()
         >>> scene.bounding_box()
         Array([[0., 0.],
                [1., 1.]], dtype=float32)
         >>> len(scene.objects)
         8
-        >>> scene.emitters["tx"]
+        >>> scene.transmitters["tx"]
         Point(point=Array([0.2, 0.2], dtype=float32))
 
         .. plot::
 
             import matplotlib.pyplot as plt
             from differt2d.scene import Scene
 
@@ -579,374 +582,376 @@
 
         return scene
 
     def plot(
         self,
         ax,
         *args: Any,
-        emitters_args: Sequence = (),
-        emitters_kwargs: Dict[str, Any] = {},
+        transmitters: bool = True,
+        transmitters_args: Sequence = (),
+        transmitters_kwargs: Dict[str, Any] = {},
+        objects: bool = True,
         objects_args: Sequence = (),
         objects_kwargs: Dict[str, Any] = {},
+        receivers: bool = True,
         receivers_args: Sequence = (),
         receivers_kwargs: Dict[str, Any] = {},
         annotate: bool = True,
         **kwargs: Any,
     ) -> List[Artist]:
         """
-        :param emitters_args:
-            Arguments to be passed to each emitter's plot function.
-        :param tx_kwargs:
-            Keyword arguments to be passed to each emitter's plot function.
+        :param transmitters:
+            If set, includes transmitters in the plot.
+        :param transmitters_args:
+            Arguments to be passed to each transmitter's plot function.
+        :param transmitters_kwargs:
+            Keyword arguments to be passed to each transmitter's plot function.
+        :param objects:
+            If set, includes objects in the plot.
         :param objects_args:
             Arguments to be passed to the each object' plot function.
         :param objects_kwargs:
             Keyword arguments to be passed to each object' plot function.
-        :param receiver_args:
+        :param receivers:
+            If set, includes receivers in the plot.
+        :param receivers_args:
             Arguments to be passed to each receiver's plot function.
-        :param receiver_kwargs:
+        :param receivers_kwargs:
             Keyword arguments to be passed to each receiver's plot function.
         :param annotate:
-            If set, will annotate all emitters and receivers with their name,
+            If set, will annotate all transmitters and receivers with their name,
             and append the corresponding artists
             to the returned list.
         """
-        emitters_kwargs.setdefault("color", "blue")
+        transmitters_kwargs.setdefault("color", "blue")
         receivers_kwargs.setdefault("color", "green")
 
         artists = []
 
-        for e_key, emitter in self.emitters.items():
-            artists.extend(
-                emitter.plot(
-                    ax,
-                    *emitters_args,
-                    *args,
-                    annotate=e_key if annotate else None,
-                    **emitters_kwargs,
-                    **kwargs,
+        if transmitters:
+            for tx_key, transmitter in self.transmitters.items():
+                artists.extend(
+                    transmitter.plot(
+                        ax,
+                        *transmitters_args,
+                        *args,
+                        annotate=tx_key if annotate else None,
+                        **transmitters_kwargs,
+                        **kwargs,
+                    )
                 )
-            )
 
-        for r_key, receiver in self.receivers.items():
-            artists.extend(
-                receiver.plot(
-                    ax,
-                    *receivers_args,
-                    *args,
-                    annotate=r_key if annotate else None,
-                    **receivers_kwargs,
-                    **kwargs,
+        if objects:
+            for obj in self.objects:
+                artists.extend(
+                    obj.plot(ax, *objects_args, *args, **objects_kwargs, **kwargs)  # type: ignore[union-attr]
                 )
-            )
 
-        for obj in self.objects:
-            artists.extend(
-                obj.plot(ax, *objects_args, *args, **objects_kwargs, **kwargs)  # type: ignore[union-attr]
-            )
+        if receivers:
+            for rx_key, receiver in self.receivers.items():
+                artists.extend(
+                    receiver.plot(
+                        ax,
+                        *receivers_args,
+                        *args,
+                        annotate=rx_key if annotate else None,
+                        **receivers_kwargs,
+                        **kwargs,
+                    )
+                )
 
         return artists
 
     def bounding_box(self) -> Array:
         bounding_boxes_list = (
-            [emitter.bounding_box() for emitter in self.emitters.values()]
+            [transmitter.bounding_box() for transmitter in self.transmitters.values()]
             + [receiver.bounding_box() for receiver in self.receivers.values()]
             + [obj.bounding_box() for obj in self.objects]  # type: ignore[union-attr]
         )
         bounding_boxes = jnp.dstack(bounding_boxes_list)
 
         return jnp.vstack(
             [
                 jnp.min(bounding_boxes[0, :, :], axis=1),
                 jnp.max(bounding_boxes[1, :, :], axis=1),
             ]
         )
 
-    def get_closest_emitter(self, coords: Array) -> Tuple[Point, Array]:
+    def get_closest_transmitter(self, coords: Array) -> Tuple[Point, Array]:
         """
-        Returns the closest emitter to the given coordinates.
+        Returns the closest transmitter to the given coordinates.
 
         :param coords: The x-y coordinates, (2,).
-        :return: The closet emitter and its distance to the coordinates.
+        :return: The closet transmitter and its distance to the coordinates.
         """
-        emitters = list(self.emitters.values())
-        points = jnp.vstack([tx.point for tx in emitters])
+        transmitters = list(self.transmitters.values())
+        points = jnp.vstack([tx.point for tx in transmitters])
         i_min, distance = closest_point(points, coords)
-        return emitters[i_min], distance
+        return transmitters[i_min], distance
 
     def get_closest_receiver(self, coords: Array) -> Tuple[Point, Array]:
         """
         Returns the closest receivers to the given coordinates.
 
         :param coords: The x-y coordinates, (2,).
         :return: The closet receiver and its distance to the coordinates.
         """
         receivers = list(self.receivers.values())
         points = jnp.vstack([rx.point for rx in receivers])
         i_min, distance = closest_point(points, coords)
         return receivers[i_min], distance
 
-    def all_emitter_receiver_pairs(
+    def all_transmitter_receiver_pairs(
         self,
     ) -> Iterator[Tuple[Tuple[str, Point], Tuple[str, Point]]]:
         """
-        Returns all possible pairs of (emitter, receiver) in the scene.
+        Returns all possible pairs of (transmitter, receiver) in the scene.
 
         Each pair ``P := ((KE, E), (KR, R))`` is made of the following:
 
-        + ``KE`` the name of the emitter (key);
-        + ``E`` the actual emitter :class:`Point<differt2d.geometry.Point>` (value);
+        + ``KE`` the name of the transmitter (key);
+        + ``E`` the actual transmitter :class:`Point<differt2d.geometry.Point>` (value);
         + ``KR`` the name of the receiver (key);
         + ``R`` the actual receiver :class:`Point<differt2d.geometry.Point>` (value).
 
         :return: A generator of all possible pairs.
         """
-        return product(self.emitters.items(), self.receivers.items())
-
-    def get_visibility_matrix(self) -> np.array:
-        """
-        Returns the visibility matrix between all objects in the scene, plus one
-        arbitrary emitter and one arbitrary receiver.
-
-        Arbitrary because, for scenes with multiple emitters
-        or receivers, the same matrix will be used, so it should
-        not be computed for a specific (emitter, receiver) pair.
-
-        The first row / column is for :attr:`emitters`,
-        and the last row / column for :attr:`receivers`.
-
-        If :python:`V` is the visibility matrix, then
-        :python:`V[i, j]` indicates whether object ``i``
-        can see object ``j``. In general, :python:`V` is
-        expected to be symmetric (but this is not a requirement),
-        and visibility is indicated by a :python:`1` value, whereas
-        obstruction is indicated by a :python:`0` value.
-
-        :Examples:
-
-        >>> from differt2d.scene import Scene
-        >>> scene = Scene.square_scene()
-        >>> scene.get_visibility_matrix()
-        array([[0., 1., 1., 1., 1., 1.],
-               [1., 0., 1., 1., 1., 1.],
-               [1., 1., 0., 1., 1., 1.],
-               [1., 1., 1., 0., 1., 1.],
-               [1., 1., 1., 1., 0., 1.],
-               [1., 1., 1., 1., 1., 0.]])
-
-        :return: The visibility matrix,
-            (:python:`len(self.objects) + 2`, :python:`len(self.objects) + 2`).
-        """
-        n = len(self.objects)
-        return np.ones((n + 2, n + 2)) - np.eye(n + 2, n + 2)
+        return product(self.transmitters.items(), self.receivers.items())
 
+    @partial(jax.jit, static_argnames=["min_order", "max_order"])
     def all_path_candidates(
         self, min_order: int = 0, max_order: int = 1
-    ) -> List[List[int]]:
+    ) -> List[Array]:
         """
-        Returns all path candidates, from any of the :attr:`emitters` to any of the
-        :attr:`receivers`, as a list of list of indices.
+        Returns all path candidates, from any of the :attr:`transmitters` to any of the
+        :attr:`receivers`, as a list of array of indices.
 
-        Note that index 0 is for :attr:`emitters`,
-        and last index is for :attr:`receivers`.
+        Note that it only inclides indices for objects.
 
-        :param min_order:
-            The minimum order of the path, i.e., the number of interactions.
-        :param max_order:
-            The maximum order of the path, i.e., the number of interactions.
+        :param min_order: The minimum order of the path, i.e., the number of
+            interactions.
+        :param max_order: The maximum order of the path, i.e., the number of
+            interactions.
         :return: The list of list of indices.
         """
-        n = len(self.objects)
+        num_primitives = len(self.objects)
 
-        graph = rx.PyGraph.from_adjacency_matrix(self.get_visibility_matrix())
-
-        return rx.all_simple_paths(
-            graph, 0, n + 1, min_depth=min_order + 2, cutoff=max_order + 2
-        )
+        return [
+            path_candidate
+            for order in range(min_order, max_order + 1)
+            for path_candidate in jnp.asarray(
+                differt_core.generate_path_candidates(num_primitives, order),
+                dtype=jnp.uint32,
+            ).T
+        ]
 
-    def get_interacting_objects(self, path_candidate: List[int]) -> List[Interactable]:
+    def get_interacting_objects(self, path_candidate: Array) -> List[Interactable]:
         """
         Returns the list of interacting objects from a path candidate.
 
         An `interacting` object is simply an object on which the
         path should pass.
 
         :param path_candidates: A path candidate,
             as returned by :meth:`all_path_candidates`.
         :return: The list of interacting objects.
         """
-        return [self.objects[i - 1] for i in path_candidate[1:-1]]
+        return [self.objects[i] for i in path_candidate]
 
     def all_paths(
         self,
         path_cls: Type[Path] = ImagePath,
         min_order: int = 0,
         max_order: int = 1,
         **kwargs: Any,
     ) -> Iterator[Tuple[str, str, Array, Path, List[int]]]:
         """
-        Returns all paths from any of the :attr:`emitters` to any of the
+        Returns all paths from any of the :attr:`transmitters` to any of the
         :attr:`receivers`, using the given method, see,
         :class:`differt2d.geometry.ImagePath` :class:`differt2d.geometry.FermatPath` and
         :class:`differt2d.geometry.MinPath`.
 
         :param path_cls: Method to be used to find the path coordinates.
         :param min_order:
             The minimum order of the path, i.e., the number of interactions.
         :param max_order:
             The maximum order of the path, i.e., the number of interaction
         :param kwargs:
             Keyword arguments to be passed to
             :meth:`Path.is_valid<differt2d.geometry.Path.is_valid>`.
         :return: The generator of paths, as
-            (emitter name, receiver name, valid, path, path_candidate) tuples,
+            (transmitter name, receiver name, valid, path, path_candidate) tuples,
             where validity path validity can be later evaluated using
             :python:`is_true(valid)`.
         """
         path_candidates = self.all_path_candidates(
             min_order=min_order, max_order=max_order
         )
 
-        for (e_key, emitter), (r_key, receiver) in self.all_emitter_receiver_pairs():
+        for (tx_key, transmitter), (
+            rx_key,
+            receiver,
+        ) in self.all_transmitter_receiver_pairs():
             for path_candidate in path_candidates:
                 interacting_objects = self.get_interacting_objects(path_candidate)
                 path = path_cls.from_tx_objects_rx(
-                    emitter.point, interacting_objects, receiver.point
+                    transmitter.point, interacting_objects, receiver.point
                 )
                 valid = path.is_valid(
                     self.objects,  # type: ignore[arg-type]
                     path_candidate,
                     interacting_objects,  # type: ignore[arg-type]
                     **kwargs,
                 )
 
-                yield (e_key, r_key, valid, path, path_candidate)
+                yield (tx_key, rx_key, valid, path, path_candidate)
 
     def all_valid_paths(
         self,
         approx=None,
         **kwargs: Any,
     ) -> Iterator[Tuple[str, str, Path, List[int]]]:
         """
         Returns only valid paths as returned by :meth:`all_paths`, by filtering out
         paths using :func:`is_true<differt2d.logic.is_true>`.
 
         :param kwargs:
             Keyword arguments to be passed to :meth:`all_paths`.
         :return: The generator of valid paths, as
-            (emitter name, receiver name, path, path_candidate) tuples.
+            (transmitter name, receiver name, path, path_candidate) tuples.
         """
-        for e_key, r_key, valid, path, path_candidate in self.all_paths(
+        for tx_key, rx_key, valid, path, path_candidate in self.all_paths(
             approx=approx, **kwargs
         ):
             if is_true(valid, approx=approx):
-                yield (e_key, r_key, path, path_candidate)
+                yield (tx_key, rx_key, path, path_candidate)
 
     def accumulate_over_paths(
         self,
         fun: PathFun,
         fun_args: Tuple = (),
         fun_kwargs: Mapping = {},
+        reduce_all: bool = False,
         **kwargs: Any,
     ) -> Iterator[Tuple[str, str, Array]]:
         """
-        Repeatedly calls ``fun`` on all paths between each pair of (emitter, receiver)
-        in the scene, and accumulates the results.
+        Repeatedly calls ``fun`` on all paths between each pair of (transmitter,
+        receiver) in the scene, and accumulates the results.
 
-        Produces an iterator with each (emitter, receiver) pair.
+        Produces an iterator with each (transmitter, receiver) pair.
 
         :param fun: The function to evaluate on each path.
         :param fun_args:
             Positional arguments to be passed to ``fun``.
         :param fun_kwargs:
             Keyword arguments to be passed to ``fun``.
+        :param reduce_all: Whether to reduce the output by summing
+            all accumulated results. This is especially useful
+            if you only care about the total accumulated results.
         :param kwargs:
             Keyword arguments to be passed to
             :meth:`all_paths`.
         :return:
-            An iterator of emitter name, receiver name
-            and the corresponding accumulated result.
-        """
-        acc = 0.0
-        for (e_key, r_key), paths_group in groupby(
-            self.all_paths(**kwargs), lambda key: key[:2]
-        ):
-            acc = 0.0
-            emitter = self.emitters[e_key]
-            receiver = self.receivers[r_key]
+            An iterator of transmitter name, receiver name
+            and the corresponding accumulated result, or the
+            sum of accumulated results if :python:`reduce_all=True`.
+        """
+
+        def results() -> Iterator[Tuple[str, str, Array]]:
+            for (tx_key, rx_key), paths_group in groupby(
+                self.all_paths(**kwargs), lambda key: key[:2]
+            ):
+                acc = 0.0
+                transmitter = self.transmitters[tx_key]
+                receiver = self.receivers[rx_key]
+
+                for _, _, valid, path, path_candidate in paths_group:
+                    interacting_objects = self.get_interacting_objects(path_candidate)
+                    acc = acc + valid * fun(
+                        transmitter,
+                        receiver,
+                        path,
+                        interacting_objects,  # type: ignore[arg-type]
+                        *fun_args,
+                        **fun_kwargs,
+                    )
 
-            for _, _, valid, path, path_candidate in paths_group:
-                interacting_objects = self.get_interacting_objects(path_candidate)
-                acc = acc + valid * fun(
-                    emitter,
-                    receiver,
-                    path,
-                    interacting_objects,  # type: ignore[arg-type]
-                    *fun_args,
-                    **fun_kwargs,
-                )
+                yield tx_key, rx_key, acc
 
-            yield e_key, r_key, acc
+        if reduce_all:
+            return sum(p for _, _, p in results())
+        else:
+            return results()
 
-    def accumulate_on_emitters_grid_over_paths(
+    def accumulate_on_transmitters_grid_over_paths(
         self,
         X: Array,
         Y: Array,
         fun: PathFun,
         fun_args: Tuple = (),
         fun_kwargs: Mapping = {},
-        reduce: bool = False,
+        reduce_all: bool = False,
+        grad: bool = False,
+        value_and_grad: bool = False,
         path_cls: Type[Path] = ImagePath,
-        emitter_cls: Type[Point] = Point,
+        transmitter_cls: Type[Point] = Point,
         min_order: int = 0,
         max_order: int = 1,
         **kwargs,
-    ) -> Union[Iterator[Tuple[str, Array]], Array]:
+    ) -> Union[
+        Iterator[Tuple[str, Union[Array, Tuple[Array, Array]]]],
+        Union[Array, Tuple[Array, Array]],
+    ]:
         """
         Repeatedly calls ``fun`` on all paths between the receivers in the scene and
-        every emitter coordinate in :python:`(X, Y)`, and accumulates the results over
-        one array that has the same shape a ``X`` and ``Y``.
+        every transmitter coordinate in :python:`(X, Y)`, and accumulates the results
+        over one array that has the same shape a ``X`` and ``Y``.
 
         Produces an iterator with one element for each receiver location.
 
         :param X: The grid of x-coordinates, (m, n).
         :param Y: The grid of y-coordinates, (m, n).
         :param fun: The function to evaluate on each path.
         :param fun_args:
             Positional arguments to be passed to ``fun``.
         :param fun_kwargs:
             Keyword arguments to be passed to ``fun``.
-        :param reduce: Whether to reduce the output by summing
+        :param reduce_all: Whether to reduce the output by summing
             all accumulated results. This is especially useful
             if you only care about the total accumulated results.
+        :param grad: If set, returns the gradient of ``fun`` with respect
+            to the transmitter's position. The output array(s) will then have
+            an additional axis of size two.
+        :param value_and_grad: If set, returns both the ``fun`` and its
+            gradient. Takes precedence over setting :python:`grad=True`.
         :param path_cls: Method to be used to find the path coordinates.
-        :param emitter_cls: A point constructor called on every emitter,
+        :param transmitter_cls: A point constructor called on every transmitter,
             should inherit from :class:`Point<differt2d.geometry.Point>`.
         :param min_order:
             The minimum order of the path, i.e., the number of interactions.
         :param max_order:
             The maximum order of the path, i.e., the number of interactions.
         :param kwargs:
             Keyword arguments to be passed to
             :meth:`Path.is_valid<differt2d.geometry.Path.is_valid>`.
         :return:
             An iterator of receiver name and the corresponding
-            accumulated result, or the sum of accumulated
-            if :python:`reduce=True`.
+            accumulated result, or the sum of accumulated results
+            if :python:`reduce_all=True`.
         """
-        emitters = self.emitters
-        self.emitters = {"tx": Point(point=jnp.array([0.0, 0.0]))}
+        transmitters = self.transmitters
+        self.transmitters = {"tx": Point(point=jnp.array([0.0, 0.0]))}
 
         path_candidates = self.all_path_candidates(
             min_order=min_order,
             max_order=max_order,
         )
 
-        pairs = list(self.all_emitter_receiver_pairs())
-        self.emitters = emitters
+        pairs = list(self.all_transmitter_receiver_pairs())
+        self.transmitters = transmitters
 
         def facc(tx_coords: Array, receiver: Point) -> Array:
             acc = 0.0
             for path_candidate in path_candidates:
                 interacting_objects = self.get_interacting_objects(path_candidate)
                 path = path_cls.from_tx_objects_rx(
                     tx_coords, interacting_objects, receiver.point
@@ -954,127 +959,167 @@
                 valid = path.is_valid(
                     self.objects,  # type: ignore[arg-type]
                     path_candidate,
                     interacting_objects,  # type: ignore[arg-type]
                     **kwargs,
                 )
                 acc = acc + valid * fun(
-                    emitter_cls(point=tx_coords),
+                    transmitter_cls(point=tx_coords),
                     receiver,
                     path,
                     interacting_objects,
                     *fun_args,
                     **fun_kwargs,
                 )
 
             return acc
 
+        if value_and_grad:
+            facc = jax.value_and_grad(facc, argnums=0)
+        elif grad:
+            facc = jax.grad(facc, argnums=0)
+
         vfacc = jax.vmap(
             jax.vmap(facc, in_axes=(0, None)),
             in_axes=(0, None),
         )
 
         grid = jnp.dstack((X, Y))
 
         def results() -> Iterator[Array]:
-            return ((r_key, vfacc(grid, receiver)) for _, (r_key, receiver) in pairs)
+            return ((rx_key, vfacc(grid, receiver)) for _, (rx_key, receiver) in pairs)
 
-        if reduce:
-            return sum(p for _, p in results())
+        if reduce_all:
+            if value_and_grad:
+                Z = 0.0
+                dZ = 0.0
+                for _, (p, dp) in results():
+                    Z = Z + p
+                    dZ = dZ + dp
+
+                return Z, dZ
+            else:
+                return sum(p for _, p in results())
         else:
             return results()
 
     def accumulate_on_receivers_grid_over_paths(
         self,
         X: Array,
         Y: Array,
         fun: PathFun,
         fun_args: Tuple = (),
         fun_kwargs: Mapping = {},
-        reduce: bool = False,
+        reduce_all: bool = False,
+        grad: bool = False,
+        value_and_grad: bool = False,
         path_cls: Type[Path] = ImagePath,
         receiver_cls: Type[Point] = Point,
         min_order: int = 0,
         max_order: int = 1,
         **kwargs,
-    ) -> Union[Iterator[Tuple[str, Array]], Array]:
+    ) -> Union[
+        Iterator[Tuple[str, Union[Array, Tuple[Array, Array]]]],
+        Union[Array, Tuple[Array, Array]],
+    ]:
         """
-        Repeatedly calls ``fun`` on all paths between the emitters in the scene and
+        Repeatedly calls ``fun`` on all paths between the transmitters in the scene and
         every receiver coordinate in :python:`(X, Y)`, and accumulates the results over
         one array that has the same shape a ``X`` and ``Y``.
 
-        Produces an iterator with one element for each emitter location.
+        Produces an iterator with one element for each transmitter location.
 
         :param X: The grid of x-coordinates, (m, n).
         :param Y: The grid of y-coordinates, (m, n).
         :param fun: The function to evaluate on each path.
         :param fun_args:
             Positional arguments to be passed to ``fun``.
         :param fun_kwargs:
             Keyword arguments to be passed to ``fun``.
-        :param reduce: Whether to reduce the output by summing
+        :param reduce_all: Whether to reduce the output by summing
             all accumulated results. This is especially useful
             if you only care about the total accumulated results.
+        :param grad: If set, returns the gradient of ``fun`` with respect
+            to the receiver's position. The output array(s) will then have
+            an additional axis of size two.
+        :param value_and_grad: If set, returns both the ``fun`` and its
+            gradient. Takes precedence over setting :python:`grad=True`.
         :param path_cls: Method to be used to find the path coordinates.
         :param receiver_cls: A point constructor called on every receiver,
             should inherit from :class:`Point<differt2d.geometry.Point>`.
         :param min_order:
             The minimum order of the path, i.e., the number of interactions.
         :param max_order:
             The maximum order of the path, i.e., the number of interactions.
         :param kwargs:
             Keyword arguments to be passed to
             :meth:`Path.is_valid<differt2d.geometry.Path.is_valid>`.
         :return:
-            An iterator of emitter name and the corresponding
-            accumulated result, or the sum of accumulated
-            if :python:`reduce=True`.
+            An iterator of transmitter name and the corresponding
+            accumulated result, or the sum of accumulated results
+            if :python:`reduce_all=True`.
         """
         receivers = self.receivers
         self.receivers = {"rx": Point(point=jnp.array([0.0, 0.0]))}
 
         path_candidates = self.all_path_candidates(
             min_order=min_order,
             max_order=max_order,
         )
 
-        pairs = list(self.all_emitter_receiver_pairs())
+        pairs = list(self.all_transmitter_receiver_pairs())
         self.receivers = receivers
 
-        def facc(emitter: Point, rx_coords: Array) -> Array:
+        def facc(transmitter: Point, rx_coords: Array) -> Array:
             acc = 0.0
             for path_candidate in path_candidates:
                 interacting_objects = self.get_interacting_objects(path_candidate)
                 path = path_cls.from_tx_objects_rx(
-                    emitter.point, interacting_objects, rx_coords
+                    transmitter.point, interacting_objects, rx_coords
                 )
                 valid = path.is_valid(
                     self.objects,  # type: ignore[arg-type]
                     path_candidate,
                     interacting_objects,  # type: ignore[arg-type]
                     **kwargs,
                 )
                 acc = acc + valid * fun(
-                    emitter,
+                    transmitter,
                     receiver_cls(point=rx_coords),
                     path,
                     interacting_objects,
                     *fun_args,
                     **fun_kwargs,
                 )
 
             return acc
 
+        if value_and_grad:
+            facc = jax.value_and_grad(facc, argnums=1)
+        elif grad:
+            facc = jax.grad(facc, argnums=1)
+
         vfacc = jax.vmap(
             jax.vmap(facc, in_axes=(None, 0)),
             in_axes=(None, 0),
         )
 
         grid = jnp.dstack((X, Y))
 
         def results() -> Iterator[Array]:
-            return ((e_key, vfacc(emitter, grid)) for (e_key, emitter), _ in pairs)
+            return (
+                (tx_key, vfacc(transmitter, grid)) for (tx_key, transmitter), _ in pairs
+            )
 
-        if reduce:
-            return sum(p for _, p in results())
+        if reduce_all:
+            if value_and_grad:
+                Z = 0.0
+                dZ = 0.0
+                for _, (p, dp) in results():
+                    Z = Z + p
+                    dZ = dZ + dp
+
+                return Z, dZ
+            else:
+                return sum(p for _, p in results())
         else:
             return results()
```

### Comparing `differt2d-0.1.0/differt2d/utils.py` & `differt2d-0.2.0/differt2d/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,30 @@
     TypeVar,
     Union,
 )
 
 import jax
 import jax.numpy as jnp
 
+from .defaults import DEFAULT_HEIGHT, DEFAULT_R_COEF
+
+P0: float = 100.0
+"""Received power at zero distance from transmitter when using default parameter values,
+see :func:`received_power`."""
+
+
 if TYPE_CHECKING:  # pragma: no cover
     from jax import Array
 
     from .abc import Interactable
     from .geometry import Path, Point
 
 Pytree = Union[list, tuple, dict]
 T = TypeVar("T")
 
-DEFAULT_R_COEF: float = 0.5
-"""Default value for real reflection coefficient."""
-
-DEFAULT_HEIGHT: float = 0.1
-"""Default TX antenna height, used to avoid division by zero when computing
-:func:`received_power`."""
-
-P0 = 1 / (DEFAULT_HEIGHT * DEFAULT_HEIGHT)
-"""Default received power at zero distance from emitter, see :func:`received_power`."""
-
 
 def stack_leaves(
     pytrees: Pytree, axis: int = 0, is_leaf: Optional[Callable[..., Any]] = None
 ) -> Pytree:
     """
     Stacks the leaves of one or more Pytrees along a new axis.
 
@@ -65,32 +62,33 @@
     """
     leaves, treedef = jax.tree_util.tree_flatten(pytrees)
     return [treedef.unflatten(leaf) for leaf in zip(*leaves)]
 
 
 @jax.jit
 def received_power(
-    emitter: Point,
+    transmitter: Point,
     receiver: Point,
     path: Path,
     interacting_objects: Sequence[Interactable],
     r_coef: float = DEFAULT_R_COEF,
     height: float = DEFAULT_HEIGHT,
 ) -> Array:
     """
-    Returns the received power for a given path between some emitter and some receiver.
+    Returns the received power for a given path between some transmitter and some
+    receiver.
 
     Here, the power decreases with the square of the path length, and each interaction
     introduces some reflection coefficient.
 
-    :param emitter: The emitting node, ignored.
+    :param transmitter: The transmitting node, ignored.
     :param receiver: The receiving node, ignored.
     :param path: The ray path.
     :param interacting_objects: The sequence of interacting objects, ignored.
     :param r_coef: The reflection coefficient, with :python:`0 <= r_coef <= 1`.
-    :param height: The TX antenna height to avoid division by zero when emitter and
+    :param height: The TX antenna height to avoid division by zero when transmitter and
         receiver are located at the same coordinates.
     :return: The received power.
     """
     r = path.length()
     n = path.points.shape[0] - 2  # Number of interactions
     return (r_coef**n) / (height * height + r * r)
```

### Comparing `differt2d-0.1.0/pyproject.toml` & `differt2d-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 profile = "black"
 py_version = 39
 
 [tool.poetry]
 authors = ["Jérome Eertmans <jeertmans@icloud.com>"]
 classifiers = [
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering"
 ]
 description = "2D Toolbox for Differentiable Ray Tracing"
 documentation = "https://eertmans.be/DiffeRT2d"
 exclude = ["docs/", "static/"]
@@ -33,39 +33,38 @@
 license = "MIT"
 name = "DiffeRT2d"
 packages = [
   {include = "differt2d"}
 ]
 readme = "README.md"
 repository = "https://github.com/jeertmans/DiffeRT2d"
-version = "0.1.0"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
-chex = "^0.1.7"
+chex = ">=0.1.7"
+differt-core = "0.0.5"
 jax = "^0.4.7"
-matplotlib = "^3.7.1"
-numpy = "^1.24"
-optax = "^0.1.5"
-python = "<3.12,>=3.9"
-rustworkx = "^0.12.1"
+matplotlib = ">=3.7.1"
+optax = ">=0.1.5"
+python = "<3.13,>=3.9"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
 pre-commit = "^3.0.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.5.20"
 myst-parser = ">=2"
-pyside6 = "^6.5.2"
+pyside6 = {version = "^6.5.2", python = "<3.12"}
 qtgallery = "^0.0.2"
 qtpy = "^2.4.0"
 sphinx = "^7.2.6"
 sphinx-autodoc-typehints = "^1.23.2"
 sphinx-click = "^4.4.0"
 sphinx-copybutton = "^0.5.1"
 sphinx-gallery = "^0.14.0"
@@ -83,19 +82,24 @@
 [tool.poetry.group.test.dependencies]
 byexample = "^10.5.6"
 pyperf = "^2.6.1"
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-env = "^0.8.1"
 pytest-xdist = "^3.3.1"
+rtoml = "^0.9.0"
 
 [tool.pytest.ini_options]
 env = [
   "JAX_DEBUG_NANS=True",
   "JAX_PLATFORM_NAME=cpu"
 ]
+filterwarnings = [
+  "error"
+]
 
 [tool.ruff]
 ignore = [
   "E501"
 ]
+select = ["F", "E4", "E7", "E9", "F"]
 target-version = "py38"
```

### Comparing `differt2d-0.1.0/PKG-INFO` & `differt2d-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: DiffeRT2d
-Version: 0.1.0
+Version: 0.2.0
 Summary: 2D Toolbox for Differentiable Ray Tracing
 Home-page: https://github.com/jeertmans/DiffeRT2d
 License: MIT
 Keywords: ray tracing,differentiable
 Author: Jérome Eertmans
 Author-email: jeertmans@icloud.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: chex (>=0.1.7,<0.2.0)
+Requires-Dist: chex (>=0.1.7)
+Requires-Dist: differt-core (==0.0.5)
 Requires-Dist: jax (>=0.4.7,<0.5.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24,<2.0)
-Requires-Dist: optax (>=0.1.5,<0.2.0)
-Requires-Dist: rustworkx (>=0.12.1,<0.13.0)
+Requires-Dist: matplotlib (>=3.7.1)
+Requires-Dist: optax (>=0.1.5)
 Project-URL: Documentation, https://eertmans.be/DiffeRT2d
 Project-URL: Repository, https://github.com/jeertmans/DiffeRT2d
 Description-Content-Type: text/markdown
 
 <img alt="DiffeRT2d Logo" align="right" width="512px" src="https://raw.githubusercontent.com/jeertmans/DiffeRT2d/main/static/logo_light_transparent.png">
 
 # DiffeRT2d
 
+[![Latest Release][pypi-version-badge]][pypi-version-url]
+[![Python version][pypi-python-version-badge]][pypi-version-url]
 [![Documentation][documentation-badge]][documentation-url]
 [![codecov][codecov-badge]][codecov-url]
 
 Differentiable Ray Tracing (RT) Python framework for Telecommunications-oriented
 applications.
 
-> **NOTE**: the present work offers a simple Python module to create basic 2D scenarios,
-> and should be used for experimental purposes only.
+> [!IMPORTANT]
+> The present work offers a simple Python module to create basic 2D scenarios,
+> and should be used for experimental purposes only. For practical 3D applications,
+> checkout [DiffeRT](https://github.com/jeertmans/DiffeRT).
 
 - [Installation](#installation)
   * [Dependencies](#dependencies)
   * [Pip install](#pip-install)
   * [Install From Repository](#install-from-repository)
 - [Usage](#usage)
 - [Contributing](#contributing)
@@ -147,12 +150,15 @@
 
 Finally, if you do not have any GitHub account,
 or just wish to contact the author of DiffeRT2d,
 you can do so at: [jeertmans@icloud.com](mailto:jeertmans@icloud.com).
 
 <!-- end contact -->
 
+[pypi-version-badge]: https://img.shields.io/pypi/v/DiffeRT2d?label=DiffeRT2d
+[pypi-version-url]: https://pypi.org/project/DiffeRT2d/
+[pypi-python-version-badge]: https://img.shields.io/pypi/pyversions/DiffeRT2d
 [documentation-badge]: https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=documentation&up_color=green&up_message=online&url=https%3A%2F%2Feertmans.be%2FDiffeRT2d%2F
 [documentation-url]: https://eertmans.be/DiffeRT2d/
 [codecov-badge]: https://codecov.io/gh/jeertmans/DiffeRT2d/branch/main/graph/badge.svg?token=1dJ1AKWMR5
 [codecov-url]: https://codecov.io/gh/jeertmans/DiffeRT2d
```

