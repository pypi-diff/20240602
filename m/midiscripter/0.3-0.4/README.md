# Comparing `tmp/midiscripter-0.3.tar.gz` & `tmp/midiscripter-0.4.tar.gz`

## Comparing `midiscripter-0.3.tar` & `midiscripter-0.4.tar`

### file list

```diff
@@ -1,48 +1,52 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/__init__.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/msg_base.py
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/port_base.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/shared.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/cli/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/cli/starters.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/file_event/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/file_event/file_event_msg.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/file_event/file_event_port.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/app.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/log_widget.py
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/main_window.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/menu_bar.py
--rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/ports_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/__init__.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/button.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/gui_msg.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/gui_widget_base.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/layout.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/list.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/mixins.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/text.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/keyboard/__init__.py
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/keyboard/keyboard_msg.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/keyboard/keyboard_port.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/__init__.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/console_sink.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/html_sink.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/log.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/metronome/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/metronome/metronome_port.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/__init__.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_msg.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_note_data.py
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_port.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_ports_update.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/osc_msg.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/osc_port.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/osc_query_maker.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/resources/icon.ico
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/resources/icon.svg
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.3/LICENSE
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 midiscripter-0.3/README.md
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 midiscripter-0.3/pyproject.toml
--rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 midiscripter-0.3/PKG-INFO
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/base/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/base/msg_base.py
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/base/port_base.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/cli/__init__.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/cli/starters.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/file_event/__init__.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/file_event/file_event_msg.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/file_event/file_event_port.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/__init__.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/app.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/log_widget.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/main_window.py
+-rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/menu_bar.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/ports_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/__init__.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/button.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/gui_msg.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/gui_widget_base.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/layout.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/list.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/mixins.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/gui/gui_widgets/text.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/keyboard/__init__.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/keyboard/keyboard_msg.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/keyboard/keyboard_port.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/logger/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/logger/console_sink.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/logger/html_sink.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/logger/log.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/metronome/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/metronome/metronome_port.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/midi/__init__.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/midi/midi_msg.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/midi/midi_note_data.py
+-rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/midi/midi_port.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/midi/midi_ports_update.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/mouse/__init__.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/mouse/mouse_msg.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/mouse/mouse_port.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/osc/__init__.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/osc/osc_msg.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/osc/osc_port.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/osc/osc_query_maker.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/resources/icon.ico
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/resources/icon.svg
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/shared/__init__.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 midiscripter-0.4/midiscripter/shared/autostart.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.4/LICENSE
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 midiscripter-0.4/README.md
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 midiscripter-0.4/pyproject.toml
+-rw-r--r--   0        0        0    14668 2020-02-02 00:00:00.000000 midiscripter-0.4/PKG-INFO
```

### Comparing `midiscripter-0.3/midiscripter/base/msg_base.py` & `midiscripter-0.4/midiscripter/base/msg_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,114 @@
 import enum
+from typing import Any
 from collections.abc import Container
 
-import midiscripter.base.shared
+import midiscripter.shared
 from midiscripter.base.port_base import Input
 
 
+class Not:
+    def __init__(self, value: Container | Any):
+        self.value = value
+
+
 class AttrEnum(enum.StrEnum):
     def __repr__(self):
         return f'{self.__class__.__name__}({self.value.__repr__()})'
 
 
 class Msg:
-    """The data object generated by input port that is sent as an argument to it's registered calls
-    and can be sent with an output port."""
+    """The data object generated by input port that is sent as an argument to its subscribed calls
+    and can be sent with an output port"""
 
     type: str
     """Message type description for filtering and representation"""
 
     ctime: float
-    """Message creation time in epoch format"""
+    """Message creation time in ["Unix time"](https://wikipedia.org/wiki/Unix_time) format"""
 
     source: Input
-    """Input port instance that generated the message."""
+    """Input port instance that generated the message"""
 
     __match_args__: tuple[str] = ('type',)
 
     def __init__(self, type: str, source: Input | None = None):
         """
         Args:
             source: Input port instance that generated the message
         """
         self.type = type
         self.source = source
-        self.ctime = midiscripter.base.shared.precise_epoch_time()
+        self.ctime = midiscripter.shared.precise_epoch_time()
 
         self.ctime: float  # workaround for mkdocstrings issue #607
-        """Message creation time in epoch format"""
+        """Message creation time in ["Unix time"](https://wikipedia.org/wiki/Unix_time) format"""
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({", ".join(str(value) for value in self.__as_tuple())})'
+        return f'{self.__class__.__name__}({", ".join(repr(value) for value in self.__as_tuple())})'
 
     def __str__(self):
         return ' | '.join(str(value) for value in self.__as_tuple() if value is not None)
 
     def __eq__(self, other_msg: 'Msg'):
         return type(self) is type(other_msg) and self.__as_tuple() == other_msg.__as_tuple()
 
-    def matches(self, *args_conditions, **kwargs_conditions) -> bool:
+    def matches(self, *conditions_args, **conditions_kwargs) -> bool:
         """Checks if message's attributes match all provided attribute conditions:
-        1. If condition is `None` or omitted it matches anything.
-        2. If condition equals attribute it matches the attribute.
-        3. If condition is a container and contains the message attribute it matches the attribute.
+
+        1. If condition is `None` or omitted, it matches anything.
+
+        2. If condition equals attribute, it matches the attribute.
+
+        3. If condition is a container and contains the attribute, it matches the attribute.
+
+        Use `Not(condition)` to invert condition matching.
 
         Returns:
-            True if all attribute match, False if any are not
+            `True` if all attributes match, `False` if any does not match
         """
-        attr_conditions = dict(zip(self.__match_args__, args_conditions, strict=False))
-        attr_conditions.update(kwargs_conditions)
+        attr_conditions = dict(zip(self.__match_args__, conditions_args, strict=False))
+        attr_conditions.update(conditions_kwargs)
 
-        for parameter, condition in attr_conditions.items():
+        for parameter_name, condition in attr_conditions.items():
             if condition is None:
                 continue
 
             try:
-                attr = getattr(self, parameter)
+                attr = getattr(self, parameter_name)
             except AttributeError:
-                continue
+                if isinstance(condition, Not):
+                    continue
+                else:
+                    return False
 
             if attr == condition:
-                continue
+                if isinstance(condition, Not):
+                    return False
+                else:
+                    continue
 
-            if (
-                isinstance(condition, Container)
-                and not isinstance(condition, str)
-                and attr in condition
-            ):
-                continue
+            try:
+                if attr in condition and not isinstance(condition, str):
+                    if isinstance(condition, Not):
+                        return False
+                    else:
+                        continue
+            except TypeError:  # condition is not a container
+                pass
 
             return False
         return True
 
     @property
     def _age_ms(self) -> float:
-        """Time passed since message creation in milliseconds."""
-        return round((midiscripter.base.shared.precise_epoch_time() - self.ctime) * 1000, 3)
+        """Time passed since message creation in milliseconds"""
+        # Using faster rounding
+        return int((midiscripter.shared.precise_epoch_time() - self.ctime) * 1000000) / 1000
 
     def __as_tuple(self) -> tuple:
         """Converts message to a tuple based on message's __match_args__ class attribute
 
         Returns:
-            Tuple with values of attributes specified in __match_args__ class attribute.
+            Tuple with values of attributes specified in __match_args__ class attribute
         """
         return tuple(getattr(self, attr_name) for attr_name in self.__match_args__)
```

### Comparing `midiscripter-0.3/midiscripter/base/port_base.py` & `midiscripter-0.4/midiscripter/base/port_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import collections
 import contextlib
 import copy
+import inspect
 import traceback
-from collections.abc import Callable, Hashable
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING, TypeVar, ClassVar, Any
 
-import midiscripter.base.shared
+import midiscripter.shared
 from midiscripter.logger import log
 
 if TYPE_CHECKING:
+    from collections.abc import Callable, Hashable, Container
     from midiscripter.base.msg_base import Msg
 
 
 @contextlib.contextmanager
 def _all_opened() -> None:
     for port in _PortRegistryMeta.instance_registry.values():
         port._open()
 
-    for call in midiscripter.base.shared.run_after_ports_open_subscribed_calls:
+    for call in midiscripter.shared.run_after_ports_open_subscribed_calls:
 
         def __call_runner() -> None:
             try:
                 log('Running {call}', call=call)  # noqa: B023
                 call()  # noqa: B023
             except Exception as exc:
                 log.red(''.join(traceback.format_exception(exc)))
 
-        midiscripter.base.shared.thread_executor.submit(__call_runner)
+        midiscripter.shared.thread_executor.submit(__call_runner)
 
     yield
 
     for port in _PortRegistryMeta.instance_registry.values():
         port._close()
 
     log._flush()
     log._sink = None
-    midiscripter.base.shared.thread_executor.shutdown(wait=True)
+    midiscripter.shared.thread_executor.shutdown(wait=False)
 
 
 class _PortRegistryMeta(type):
-    """Metaclass that enforces one uid - one port instance (singleton) rule"""
+    """Metaclass that enforces one declaration - one port instance (singleton) rule"""
 
     __singleton_instance_type = TypeVar('__singleton_instance_type', bound='Port')
     """Type for correct IDE recognition and code completion for returned port subclasses"""
 
-    instance_registry: dict[tuple[str, Hashable], __singleton_instance_type] = {}
+    instance_registry: dict[tuple[str, 'Hashable'], __singleton_instance_type] = {}
     """Declared ports register as port class name and port uid to port instance map"""
 
     def __call__(
         cls: type[__singleton_instance_type], *args, **kwargs
     ) -> __singleton_instance_type:
         """
         Args:
@@ -56,44 +57,56 @@
                    the metaclass uses the first argument as uid
             **kwargs: -
 
         Returns:
             The singleton class instance that has requested uid
         """
         uid = cls._force_uid or args[0]
+        registry_key = (cls.__name__, uid)
+        init_args = inspect.signature(cls.__init__).bind(cls, *args, **kwargs).arguments
+        init_args.pop('self')
 
         try:
-            return cls.instance_registry[(cls.__name__, uid)]
+            instance = cls.instance_registry[registry_key]
+            if instance._inited_with_args == init_args:
+                return instance
+            else:
+                raise ValueError(
+                    f'Init arguments for consecutive declarations '
+                    f'for {cls.__name__} "{uid}" must match: {instance._inited_with_args}'
+                )
         except KeyError:
             instance = super().__call__(*args, **kwargs)
-            cls.instance_registry[(cls.__name__, uid)] = instance
+            cls.instance_registry[registry_key] = instance
+            instance._inited_with_args = init_args
             return instance
 
 
 class Port(metaclass=_PortRegistryMeta):
     """Port base class
 
     Notes:
-        Port declaration with `uid` of an already existing port
-        will return the existing port (singleton)
+        Port declarations with the same arguments will return the same instance port (singleton)
+    """
+
+    _force_uid: ClassVar[None | str] = None
+    """UID override for classes that have can have only one instance per whole class,
+       like keyboard port classes. Object for these classes are declared without arguments.
     """
 
     is_enabled: bool
     """`True` if port is listening messages / ready to send messages"""
 
-    _force_uid = None
-    """UID override for classes that have can have only one instance per whole class,
-       like keyboard port class which can have only one instance for the system.
-       Object for these classe are declared without arguments.
-    """
+    _inited_with_args: dict
+    """Arguments the port singleton was initialized with. Used by `_PortRegistryMeta`."""
 
-    def __init__(self, uid: Hashable):
+    def __init__(self, uid: 'Hashable'):
         """
         Args:
-            uid: Port's unique ID that will always lead to the same port instance
+            uid: Port's unique ID
         """
         self._uid = uid
         self.is_enabled = False
 
         self.is_enabled: bool  # workaround for mkdocstrings issue #607
         """`True` if port is listening messages / ready to send messages"""
 
@@ -131,92 +144,133 @@
         self.is_enabled = False
 
 
 class Input(Port):
     """Input port base class"""
 
     is_enabled: bool
-    """`True` if port is listening and generating messages."""
-
-    subscribed_calls: list[Callable]
-    """Callables that will be called with incoming messages. Can be modified."""
+    """`True` if port is listening and generating messages"""
 
-    _call_statistics: dict[Callable, collections.deque[float]] = {}
-    """Statistics for each call's execution time in milliseconds for the last 20 runs."""
+    calls: list[None | tuple[tuple, dict], list['Callable']]
+    """Message match arguments and callables that will be called with matching incoming messages.
+    `None` conditions matches any message."""
 
-    def __init__(self, uid: Hashable):
+    def __init__(self, uid: 'Hashable'):
         super().__init__(uid)
-        self.subscribed_calls: list[Callable] = []
+        self.calls: 'list[None | tuple[tuple, dict], list[Callable]]' = []
 
-        self.subscribed_calls: list[Callable]  # workaround for mkdocstrings issue #607
-        """Callables that will be called with incoming messages. Can be modified."""
+        # workarounds for mkdocstrings issue #607
+        self.calls: 'list[None | tuple[tuple, dict], list[Callable]]'
+        """Message match arguments and callables that will be called with matching incoming messages.
+           `None` conditions matches any message."""
 
-    # A Decorator
-    def subscribe(self, function: Callable[['Msg'], None]) -> Callable:
-        """Decorator to subscribe a callable to the input's messages
+    def subscribe(
+        self,
+        *msg_matches_args: 'tuple[None | Container[Any] | Any]',
+        **msg_matches_kwargs: 'dict[str, None | Container[Any] | Any]',
+    ) -> 'Callable':
+        """Decorator to subscribe a callable to the input's messages.
 
-        ??? Example
+        Decorator without arguments subscribes a callable to all the input's messages.
+
+        Decorator with arguments subscribes a callable to the input's messages
+        that match conditions set by arguments.
+        It works the same way as message's [`matches`][midiscripter.base.msg_base.Msg.matches] method:
+
+        1. If condition is `None` or omitted it matches anything.
+
+        2. If condition equals attribute it matches the attribute.
+
+        3. If condition is a container and contains the attribute it matches the attribute.
+
+        ??? Examples
+            1. Calls function for all MIDI port's messages:
+            ``` python
+            @midi_input_instance.subscribe
+            def function(msg: MidiMsg) -> None:
+                pass
+            ```
+            2. Calls function for OSC messages from specific address:
             ``` python
-            @input_instance.subscribe
-            def function(msg: Msg) -> None:
+            @osc_input_instance.subscribe(address='/live/song/get/track_data')
+            def function(msg: OscMsg) -> None:
                 pass
             ```
+            3. Call object instance method for MIDI port's "note on" and "note off" messages:
             ``` python
-            input_instance.subscribe(object.method)
+            midi_input_instance.subscribe((MidiType.NOTE_ON, MidiType.NOTE_OFF))(object.method)
             ```
 
-        Args:
-            function: A callable that takes the input port's message as the only argument.
-
         Returns:
             Subscribed callable.
         """
-        if function not in self.subscribed_calls:
-            self._call_statistics[function] = collections.deque(maxlen=20)
-            self.subscribed_calls.append(function)
-            log('{input} subscribed {call}', input=self, call=function)
-        return function
+
+        def wrapped_subscribe(call: 'Callable[[Msg], None]') -> 'Callable':
+            if msg_matches_args[0] is call or not msg_matches_args and not msg_matches_kwargs:  # noqa: SIM108
+                conditions = None
+            else:
+                conditions = (msg_matches_args, msg_matches_kwargs)
+
+            try:
+                call_list_for_conditions = next(
+                    entry[1] for entry in self.calls if entry[0] == conditions
+                )
+                call_list_for_conditions.append(call)
+            except StopIteration:
+                self.calls.append((conditions, [call]))
+
+            call.conditions = conditions
+            call.statistics = collections.deque(maxlen=20)
+
+            return call
+
+        if callable(msg_matches_args[0]):
+            return wrapped_subscribe(msg_matches_args[0])
+
+        return wrapped_subscribe
 
     def _send_input_msg_to_calls(self, msg: 'Msg') -> None:
         """Sends the message received by the input port to subscribed calls.
 
         Notes:
             Not supposed to be overridden in subclasses.
             Supposed to be called from the listener thread started
             by the subclass implementation of `open` method.
 
         Args:
-            msg: A message received by the input port to send to it's registered calls.
+            msg: A message received by the input port to send to its registered calls.
         """
         log('{input} got message {msg}', input=self, msg=msg)
 
-        if self.is_enabled:
-            # pre-copying messages to reduce jitter a little
-            msg_copies = [copy.copy(msg) for _ in range(len(self.subscribed_calls))]
-            midiscripter.base.shared.thread_executor.map(
-                self.__call_worker, self.subscribed_calls, msg_copies
-            )
+        if not self.is_enabled:
+            return
+
+        calls = []
+        for conditions, call_list in self.calls:
+            if conditions is None or msg.matches(*conditions[0], **conditions[1]):
+                calls.extend(call_list)
+
+        msg_copies = [copy.copy(msg) for _ in range(len(calls))]
+        midiscripter.shared.thread_executor.map(self.__call_worker, calls, msg_copies)
 
-    def __call_worker(self, function: Callable, msg: 'Msg') -> None:
+    @staticmethod
+    def __call_worker(call: 'Callable', msg: 'Msg') -> None:
         """Function called in thread for each subscribed call and each received message.
 
         Notes:
             Not supposed to be overridden in subclasses.
             Supposed to be called from `_send_input_msg_to_calls` method.
 
         Args:
-            function: Subscribed callable.
+            call: Subscribed callable.
             msg: Received message to use as callable only argument.
         """
         try:
-            function(msg)
-            self._call_statistics[function].append(msg._age_ms)
-        except TypeError:
-            function()
-            self._call_statistics[function].append(msg._age_ms)
+            call(msg)
+            call.statistics.append(msg._age_ms)
         except Exception as exc:
             log.red(''.join(traceback.format_exception(exc)))
 
 
 class Output(Port):
     """Output port base class"""
```

### Comparing `midiscripter-0.3/midiscripter/cli/starters.py` & `midiscripter-0.4/midiscripter/cli/starters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from typing import NoReturn
 
 import midiscripter.base.port_base
-import midiscripter.base.shared
+import midiscripter.shared
 import midiscripter.logger.console_sink
 import midiscripter.logger.log
 import midiscripter.midi
 from midiscripter.logger import log
 
 
 def start_cli_debug() -> NoReturn:
@@ -28,17 +28,17 @@
     """Starts the script without logging. The fastest way to run the script."""
     log.is_enabled = False
     _run_cli_loop()
 
 
 def _run_cli_loop() -> NoReturn:
     """Opens the ports and loops until broken by user."""
-    if not midiscripter.base.shared.script_path:
+    if not midiscripter.shared.script_path:
         raise RuntimeError('Starter can only be called from a script')
 
-    midiscripter.base.shared._raise_current_process_cpu_priority()
+    midiscripter.shared._raise_current_process_cpu_priority()
     with midiscripter.base.port_base._all_opened():
         while True:
             try:
                 time.sleep(1)
             except (KeyboardInterrupt, SystemExit):
                 break
```

### Comparing `midiscripter-0.3/midiscripter/file_event/file_event_msg.py` & `midiscripter-0.4/midiscripter/file_event/file_event_msg.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,52 +4,54 @@
 import midiscripter.base.msg_base
 
 if TYPE_CHECKING:
     from collections.abc import Container
     from midiscripter.file_event.file_event_port import FileEventIn
 
 
-class FileEventType(midiscripter.base.msg_base.AttrEnum):
+class FileEvent(midiscripter.base.msg_base.AttrEnum):
+    """File event message type enumerator
+    to use as [`FileEventMsg`][midiscripter.FileEventMsg] `type` attribute."""
+
     # Names are hardcoded, equal watchdog's event types
     MOVED = 'MOVED'
     DELETED = 'DELETED'
     CREATED = 'CREATED'
     MODIFIED = 'MODIFIED'
     CLOSED = 'CLOSED'
     OPENED = 'OPENED'
 
 
 class FileEventMsg(midiscripter.base.msg_base.Msg):
     ___match_args__ = ('type', 'path')
 
-    type: FileEventType
+    type: FileEvent
     """File event type"""
 
     path: pathlib.Path
     """File path of event"""
 
     source: 'None | FileEventIn'
 
     def __init__(
         self,
-        type: FileEventType | str,
+        type: FileEvent | str,
         path: pathlib.Path,
         *,
         source: 'None | FileEventIn' = None,
     ):
         """
         Args:
             type: File event type
             path: File path
-            source (FileEventIn): The [`FileEventIn`][midiscripter.FileEventIn]
-                                  instance that generated the message
+            source: The [`FileEventIn`][midiscripter.FileEventIn] instance that generated the message
         """
         super().__init__(type, source)
         self.type = type
         self.path = path
 
     def matches(
         self,
-        type: 'None | Container[FileEventType] | FileEventType | str' = None,
+        type: 'None | Container[FileEvent] | FileEvent | str' = None,
         path: 'None | Container[pathlib.Path] | pathlib.Path' = None,
     ) -> bool:
         return super().matches(type, path)
```

### Comparing `midiscripter-0.3/midiscripter/file_event/file_event_port.py` & `midiscripter-0.4/midiscripter/file_event/file_event_port.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import pathlib
+from typing import TYPE_CHECKING, overload
 
 import watchdog.events
 import watchdog.observers
 
 import midiscripter.base.port_base
 import midiscripter.file_event
 import midiscripter.logger
 
+if TYPE_CHECKING:
+    from collections.abc import Container, Callable
+    from midiscripter.file_event.file_event_msg import FileEvent, FileEventMsg
+
 shared_observer = watchdog.observers.Observer()
 shared_observer.daemon = True
 shared_observer.start()
 
 
 class FileEventIn(midiscripter.base.port_base.Input, watchdog.events.FileSystemEventHandler):
     """File system events input port. Watches file/directory modifications.
@@ -69,7 +74,24 @@
         event_path = pathlib.Path(event.src_path)
 
         if self.__watch_dir_changes or event_path == self.__path:
             msg = midiscripter.file_event.file_event_msg.FileEventMsg(
                 event.event_type.upper(), self.__path, source=self
             )
             self._send_input_msg_to_calls(msg)
+
+    @overload
+    def subscribe(self, call: 'Callable[[FileEventMsg], None]') -> 'Callable': ...
+
+    @overload
+    def subscribe(
+        self,
+        type: 'None | Container[FileEvent] | FileEvent | str' = None,
+        path: 'None | Container[pathlib.Path] | pathlib.Path' = None,
+    ) -> 'Callable': ...
+
+    def subscribe(
+        self,
+        type: 'None | Container[FileEvent] | FileEvent | str' = None,
+        path: 'None | Container[pathlib.Path] | pathlib.Path' = None,
+    ) -> 'Callable':
+        return super().subscribe(type, path)
```

### Comparing `midiscripter-0.3/midiscripter/gui/app.py` & `midiscripter-0.4/midiscripter/gui/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 from typing import NoReturn
 
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import midiscripter.base.port_base
-import midiscripter.base.shared
+import midiscripter.shared
 import midiscripter.file_event.file_event_msg
 import midiscripter.gui.main_window
 import midiscripter.midi.midi_ports_update
 
 
 class ScripterGUI(QApplication):
     request_restart = Signal()
 
     RESTART_DELAY = 2
     widgets_to_add = []
 
     def __init__(self):
         super().__init__()
         self.setOrganizationName('MIDI Scripter')
-        if midiscripter.base.shared.script_path:
-            self.setApplicationName(pathlib.Path(midiscripter.base.shared.script_path).name)
+        if midiscripter.shared.script_path:
+            self.setApplicationName(pathlib.Path(midiscripter.shared.script_path).name)
 
         icon_path = pathlib.Path(midiscripter.__file__).parent / 'resources' / 'icon.ico'
         self.setWindowIcon(QIcon(str(icon_path)))
 
         self.__time_until_restart_sec = self.RESTART_DELAY
         self.request_restart.connect(self, self.restart)
         self.aboutToQuit.connect(self.__cleanup)
@@ -43,30 +43,30 @@
         else:
             self.main_window.close()
 
     def restart_at_file_change(
         self, msg: 'midiscripter.file_event.file_change_msg.FileEventMsg'
     ) -> None:
         if msg.type not in (
-            midiscripter.file_event.file_event_msg.FileEventType.CREATED,
-            midiscripter.file_event.file_event_msg.FileEventType.MODIFIED,
+            midiscripter.file_event.file_event_msg.FileEvent.CREATED,
+            midiscripter.file_event.file_event_msg.FileEvent.MODIFIED,
         ):
             return
 
         self.__time_until_restart_sec = self.RESTART_DELAY
         sleep_step_sec = 0.1
 
         while self.__time_until_restart_sec > 0:
             time.sleep(sleep_step_sec)
             self.__time_until_restart_sec -= sleep_step_sec
 
         self.request_restart.emit()
 
     def restart(self) -> NoReturn:
-        if pathlib.Path(midiscripter.base.shared.script_path).is_file():
+        if pathlib.Path(midiscripter.shared.script_path).is_file():
             # These settings saved only for restart
             self.processEvents()  # update win status to get correct status
             QSettings().setValue('restart win minimized', self.main_window.isMinimized())
             QSettings().setValue('restart closed to tray', not self.main_window.isVisible())
             self.exit(1467)
 
     def __cleanup(self) -> None:
@@ -89,19 +89,19 @@
     try:
         midiscripter.gui.app.ScripterGUI.widgets_to_add.remove(qwidget)
     except ValueError:
         pass
 
 
 def start_gui() -> NoReturn:
-    if not midiscripter.base.shared.script_path:
+    """Starts the script and runs GUI. Logging goes to GUI Log widget."""
+    if not midiscripter.shared.script_path:
         raise RuntimeError('Starter can only be called from a script')
 
-    """Starts the script and runs GUI. Logging goes to GUI Log widget."""
-    midiscripter.base.shared._raise_current_process_cpu_priority()
+    midiscripter.shared._raise_current_process_cpu_priority()
 
     sigint_exit_code = {'Windows': -1073741510, 'Linux': 130, 'Darwin': 2}[platform.system()]
     signal.signal(signal.SIGINT, lambda *_: app_instance.exit(sigint_exit_code))
 
     signal_checker_dummy_timer = QTimer()  # runs python code from Qt to allow the signal to trigger
     signal_checker_dummy_timer.start(1000)
     signal_checker_dummy_timer.timeout.connect(lambda: None)  # dummy python code to run
@@ -109,10 +109,10 @@
     start_minimized_to_tray = '--tray' in sys.argv
 
     with midiscripter.base.port_base._all_opened():
         app_instance.prepare_main_window(start_minimized_to_tray)
         exit_status = app_instance.exec()
 
     if exit_status == 1467:  # exit status for restart request
-        midiscripter.base.shared.restart_script()
+        midiscripter.shared.restart_script()
     else:
         exit(exit_status)
```

### Comparing `midiscripter-0.3/midiscripter/gui/log_widget.py` & `midiscripter-0.4/midiscripter/gui/log_widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,100 +14,130 @@
 
     def __init__(self):
         super().__init__()
         self.setObjectName('Log')
         layout = QGridLayout()
         self.setLayout(layout)
 
-        layout.addWidget(QLabel(self.TOP_LABEL_TEXT), 1, 1, 1, 2)
+        layout.addWidget(QLabel(self.TOP_LABEL_TEXT), 1, 1, 1, 4)
 
         log_view = LogView()
-        layout.addWidget(log_view, 2, 1, 1, 2)
+        layout.addWidget(log_view, 2, 1, 1, 4)
+
+        exclude_line = QLineEdit()
+        exclude_line.setPlaceholderText('Substrings divided by ";"')
+        exclude_line.setClearButtonEnabled(True)
+        exclude_line.textChanged.connect(log_view.set_exclude)
+        exclude_line.setText(QSettings().value('log exclude', ''))
+        layout.addWidget(QLabel('Exclude:'), 3, 1, 1, 1)
+        layout.addWidget(exclude_line, 3, 2, 1, 1)
 
         filter_line = QLineEdit()
+        filter_line.setPlaceholderText('Substrings divided by ";"')
+        filter_line.setClearButtonEnabled(True)
         filter_line.textChanged.connect(log_view.set_filter)
-        layout.addWidget(QLabel('Filter:'), 3, 1, 1, 1)
-        layout.addWidget(filter_line, 3, 2, 1, 1)
+        filter_line.setText(QSettings().value('log filter', ''))
+        layout.addWidget(QLabel('Filter:'), 3, 3, 1, 1)
+        layout.addWidget(filter_line, 3, 4, 1, 1)
 
 
 class LogView(QPlainTextEdit):
     append_html_entry = Signal(list)
+    entry_ctime_part_len = len(log._get_current_precise_time_stamp()) + 2
 
     def __init__(self):
         super().__init__()
         self.__anchor_text: str | None = None
-        self.__filter_words = None
+        self.__filter_text_parts = []
+        self.__exclude_text_parts = []
 
         self.setReadOnly(True)
         self.setUndoRedoEnabled(False)
         self.setWordWrapMode(QTextOption.NoWrap)
         self.setMaximumBlockCount(log.BUFFER_SIZE)
         self.setMouseTracking(True)
 
         self.append_html_entry.connect(self.__add_entry)
         log._sink = midiscripter.logger.html_sink.HtmlSink(self.append_html_entry.emit)
 
     @Slot(str)
     def set_filter(self, filter_text: str) -> None:
-        self.__filter_words = filter_text.split()
+        self.__filter_text_parts = [text.lower().strip() for text in filter_text.split(';') if text]
+        self.__apply_filter()
+        QSettings().setValue('log filter', filter_text)
+
+    @Slot(str)
+    def set_exclude(self, exclude_text: str) -> None:
+        self.__exclude_text_parts = [
+            text.lower().strip() for text in exclude_text.split(';') if text
+        ]
         self.__apply_filter()
+        QSettings().setValue('log exclude', exclude_text)
 
     def __apply_filter(self, to_last_n_blocks: int = 0) -> None:
-        self.__hide_lines_not_matching_filter(to_last_n_blocks)
+        self.__set_lines_visibility(to_last_n_blocks)
         if not to_last_n_blocks:
             self.__clear_highlighting()
         self.__highlight_filter_matches(to_last_n_blocks)
 
-    def __hide_lines_not_matching_filter(self, last_n_blocks: int = 0) -> None:
+    def __set_lines_visibility(self, last_n_blocks: int = 0) -> None:
         document = self.document()
 
-        start_from = 0 if not last_n_blocks else document.blockCount() - last_n_blocks
+        start_from_block_number = 0 if not last_n_blocks else document.blockCount() - last_n_blocks
 
-        for line_n in range(start_from, document.blockCount()):
+        for line_n in range(start_from_block_number, document.blockCount()):
             block = document.findBlockByNumber(line_n)
+            log_entry = block.text()[self.entry_ctime_part_len :]
 
             if (
-                self.__filter_words
-                and block.text()
-                and any(
-                    filter_word.lower() not in block.text().lower()
-                    for filter_word in self.__filter_words
-                )
+                log_entry
+                and self.__text_line_is_excluded(log_entry)
+                or not self.__text_line_matches_filter(log_entry)
             ):
                 block.setVisible(False)
             else:
                 block.setVisible(True)
 
         self.setDocument(document)
 
+    def __text_line_is_excluded(self, text_line: str) -> bool:
+        if not self.__exclude_text_parts:
+            return False
+        return any(text in text_line.lower() for text in self.__exclude_text_parts)
+
+    def __text_line_matches_filter(self, text_line: str) -> bool:
+        if not self.__filter_text_parts:
+            return True
+        return any(text in text_line.lower() for text in self.__filter_text_parts)
+
     def __clear_highlighting(self) -> None:
         text_format = QTextCharFormat()
         text_format.setBackground(QBrush(Qt.NoBrush))
 
         cursor = self.textCursor()
         cursor.select(QTextCursor.SelectionType.Document)
         cursor.mergeCharFormat(text_format)
 
     def __highlight_filter_matches(self, last_n_blocks: int = 0) -> None:
-        if not self.__filter_words:
+        if not self.__filter_text_parts:
             return
 
         cursor = self.textCursor()
 
         text_format = QTextCharFormat()
         text_format.setBackground(QBrush(QColor('yellow')))
 
         if not last_n_blocks:
             start_from = 0
         else:
             document = self.document()
-            block = document.findBlockByNumber(document.blockCount() - last_n_blocks)
-            start_from = block.position()
+            first_new_block = document.findBlockByNumber(document.blockCount() - last_n_blocks)
+            start_from = first_new_block.position()
 
-        for filter_word in self.__filter_words:
+        for filter_word in self.__filter_text_parts:
             regex = QRegularExpression(filter_word, QRegularExpression.CaseInsensitiveOption)
             match_iter = regex.globalMatch(self.toPlainText(), start_from)
 
             while match_iter.hasNext():
                 match = match_iter.next()
                 cursor.setPosition(match.capturedStart())
                 cursor.movePosition(
@@ -118,15 +148,15 @@
                 cursor.mergeCharFormat(text_format)
 
     @Slot(list)
     def __add_entry(self, log_entries: list[str]) -> None:
         [self.appendHtml(f'<div>{entry}</div>') for entry in log_entries]
         self.verticalScrollBar().setValue(self.verticalScrollBar().maximum())
 
-        if self.__filter_words:
+        if self.__filter_text_parts or self.__exclude_text_parts:
             self.__apply_filter(len(log_entries))
 
     def showEvent(self, event: QShowEvent) -> None:
         log.flushing_is_enabled = True
         log._flush()
         super().showEvent(event)
```

### Comparing `midiscripter-0.3/midiscripter/gui/main_window.py` & `midiscripter-0.4/midiscripter/gui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
-import midiscripter.base.shared
+import midiscripter.shared
 import midiscripter.gui.log_widget
 import midiscripter.gui.menu_bar
 import midiscripter.gui.ports_widget
 
 
 class TrayIcon(QSystemTrayIcon):
     def __init__(self, icon: QIcon, parent: 'MainWindow' = None):
```

### Comparing `midiscripter-0.3/midiscripter/gui/menu_bar.py` & `midiscripter-0.4/midiscripter/gui/menu_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from typing import TYPE_CHECKING
 
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
-import midiscripter.base.shared
+import midiscripter.shared
 import midiscripter.file_event
 import midiscripter.gui.main_window
 import midiscripter.midi.midi_ports_update
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from base.msg_base import Msg
@@ -21,36 +21,44 @@
         name: str,
         func_for_state: 'Callable | None' = None,
         *,
         checked_func: 'Callable | None' = None,
         unchecked_func: 'Callable | None' = None,
         default_state: bool = False,
         key_shortcut: 'QKeySequence | None' = None,
+        is_shared_setting: bool = False,
     ):
         super().__init__(name)
         self.__func_for_state = func_for_state
         self.__checked_func = checked_func
         self.__unchecked_func = unchecked_func
         self.__default_state = default_state
         self.__setting_name = f'action {name}'
 
         if key_shortcut:
             self.setShortcut(key_shortcut)
 
+        if is_shared_setting:
+            self.__qsettings_args = (QApplication.instance().organizationName(), 'Shared')
+        else:
+            self.__qsettings_args = (None,)
+
         self.setCheckable(True)
         # replaces force _state_changed that causes widgets toggled by action to pop up
         self.setChecked(default_state)
         self.toggled.connect(self.__state_changed)
         self.setChecked(bool(self))
 
     def __bool__(self):
-        return bool(QSettings().value(self.__setting_name, self.__default_state, type=bool))
+        return QSettings(*self.__qsettings_args).value(
+            self.__setting_name, self.__default_state, type=bool
+        )
 
     def __state_changed(self, state: bool) -> None:
-        QSettings().setValue(self.__setting_name, state)
+        QSettings(*self.__qsettings_args).setValue(self.__setting_name, state)
 
         if self.__func_for_state:
             self.__func_for_state(state)
 
         if state is True and self.__checked_func:
             self.__checked_func()
         if state is False and self.__unchecked_func:
@@ -72,15 +80,15 @@
         script_menu.addAction('Run another', self._run_another_script)
         script_menu.addAction('&Restart', QApplication.instance().restart, QKeySequence('Ctrl+R'))
         script_menu.addAction('&Quit', QApplication.instance().exit, QKeySequence('Ctrl+Q'))
 
         # Options
         options_menu = self.addMenu('Options')
 
-        self.autostart = midiscripter.base.shared.AutostartManager()
+        self.autostart = midiscripter.shared.AutostartManager()
         toggle_autostart = options_menu.addAction('Run at start up')
         toggle_autostart.setCheckable(True)
         toggle_autostart.setChecked(self.autostart._check_if_enabled())
         toggle_autostart.toggled.connect(self.__set_autostart)
 
         self.always_on_top = SavedCheckedStateAction(
             'Window always on top',
@@ -126,23 +134,23 @@
             lambda: QDesktopServices.openUrl(QUrl('https://maboroshy.github.io/midi-scripter')),
         )
 
     def _run_another_script(self) -> None:
         file_path_str = QFileDialog.getOpenFileName(
             self,
             'Select python script',
-            str(pathlib.Path(midiscripter.base.shared.script_path).parent),
+            str(pathlib.Path(midiscripter.shared.script_path).parent),
             'Python script (*.py)',
         )[0]
         if file_path_str:
-            midiscripter.base.shared.script_path = file_path_str
+            midiscripter.shared.script_path = file_path_str
             QApplication.instance().restart()
 
     @Slot(bool)
-    def __set_autostart(self, state: bool) -> None:
+    def __set_autostart(self, new_state: bool) -> None:
         if self.autostart._check_if_other_scripts_present():
             remove_other_dialog = QMessageBox()
             remove_other_dialog.setText(
                 'There are other scripts with enabled autostart. Disable them?'
             )
             remove_other_dialog.setStandardButtons(
                 QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel
@@ -150,31 +158,31 @@
             remove_other_dialog_pressed_button = remove_other_dialog.exec()
 
             if remove_other_dialog_pressed_button == QMessageBox.Cancel:
                 return
             elif remove_other_dialog_pressed_button == QMessageBox.Yes:
                 self.autostart._disable_others()
 
-        if state:
+        if new_state:
             self.autostart._enable()
         else:
             self.autostart._disable()
 
-    def __set_watching_script_file(self, new_status: bool) -> None:
-        if new_status:
+    def __set_watching_script_file(self, new_state: bool) -> None:
+        if new_state:
             self.file_watcher_port = midiscripter.file_event.FileEventIn(
-                midiscripter.base.shared.script_path
+                midiscripter.shared.script_path
             )
             self.file_watcher_port.subscribe(QApplication.instance().restart_at_file_change)
             self.file_watcher_port._open()
         else:
             self.file_watcher_port.is_enabled = False
 
-    def __set_watching_midi_ports(self, new_status: bool) -> None:
-        if new_status:
+    def __set_watching_midi_ports(self, new_state: bool) -> None:
+        if new_state:
             self.midi_port_watcher_port = midiscripter.midi.midi_ports_update.MidiPortsChangedIn()
 
             @self.midi_port_watcher_port.subscribe
             def restart_on_midi_port_change(_: 'Msg') -> None:
                 QApplication.instance().request_restart.emit()
 
             self.midi_port_watcher_port._open()
```

### Comparing `midiscripter-0.3/midiscripter/gui/ports_widget.py` & `midiscripter-0.4/midiscripter/gui/ports_widget.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,293 +5,346 @@
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import midiscripter.logger.html_sink
 from midiscripter.base.port_base import Input, Output
 from midiscripter.logger import log
 from midiscripter.midi import MidiIn, MidiOut
+from midiscripter.keyboard import KeyIn
+from midiscripter.mouse import MouseIn
 
 
-class PortsWidget(QTreeWidget):
-    PORT_CLASS_ROLE = 100
-    PORT_UID_ROLE = 101
-    PORT_REPR_ROLE = 103
-    CALLBACK_FUNCTION_ROLE = 104
-    PASSTHROUGH_OUT_PORT_ROLE = 105
+class PortWidgetItem(QTreeWidgetItem):
+    def request_state_change(self, new_state: bool) -> bool:
+        raise NotImplementedError
+
+
+class PortItemMixin:
+    port_instance: Input | Output
+
+    def set_color_by_port_type(
+        self: 'GeneralPortItem | MidiPortItem', port_type: type[Input | Output]
+    ) -> None:
+        if issubclass(port_type, Input):
+            item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]
+        else:
+            item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]
+        self.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
+
+    def request_state_change(
+        self: 'GeneralPortItem | MidiPortItem | KeyInputPortItem', new_state: bool
+    ) -> bool:
+        if new_state:
+            if not self.port_instance.is_enabled:
+                self.port_instance._open()
+
+                if self.port_instance.is_enabled:
+                    log('Enabled {port}', port=self.port_instance)
+                    return True
+                else:
+                    # Set "broken port" background
+                    self.setData(
+                        0,
+                        Qt.ItemDataRole.BackgroundRole,
+                        QBrush(QColor().fromRgb(255, 0, 0, 20)),
+                    )
+                    log.red("Can't enable {port}", port=self.port_instance)
+                    return False
+            else:
+                # Clear possible "broken port" background
+                self.setData(
+                    0,
+                    Qt.ItemDataRole.BackgroundRole,
+                    QBrush(QColor(Qt.GlobalColor.transparent)),
+                )
+                return True
+        else:
+            self.port_instance.is_enabled = False
+            log('Disabled {port}', port=self.port_instance)
+            return False
+
+    def add_calls(self: 'GeneralPortItem | MidiPortItem') -> None:
+        for _, call_list in self.port_instance.calls:
+            for call in call_list:
+                CallItem(self, self.port_instance, call_list, call)
+
+
+class GeneralPortItem(PortItemMixin, PortWidgetItem):
+    port_instance: Input | Output
+
+    def __init__(self, parent_item: QTreeWidgetItem, port_instance: Input | Output):
+        self.port_instance = port_instance
+        self.repr = self.port_instance.__repr__()
+
+        item_text = self.port_instance._force_uid or str(self.port_instance._uid)
+        super().__init__(parent_item, (item_text,))
+
+        self.set_color_by_port_type(type(self.port_instance))
+        self.setCheckState(0, Qt.CheckState.Checked)
+
+        if issubclass(type(self.port_instance), Input):
+            self.add_calls()
+
+
+class AlwaysPresentInputPortItem(PortItemMixin, PortWidgetItem):
+    port_class: type[KeyIn | MouseIn]
+    port_instance: None | KeyIn | MouseIn
+
+    def __init__(self, parent_item: QTreeWidgetItem, port_class: type[KeyIn | MouseIn]):
+        self.port_class = port_class
+        super().__init__(parent_item, (self.port_class._force_uid,))
+
+        self.repr = f'{port_class.__name__}()'
+
+        item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]
+        self.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
+
+        try:
+            port_index = (port_class.__name__, self.port_class._force_uid)
+            self.port_instance = self.port_class.instance_registry[port_index]
+            self.setCheckState(0, Qt.CheckState.Checked)
+        except KeyError:
+            self.port_instance = None
+            self.setCheckState(0, Qt.CheckState.Unchecked)
+
+    def request_state_change(self, new_state: bool) -> bool:
+        if not self.port_instance:
+            self.port_instance = self.port_class()
+        return PortItemMixin.request_state_change(self, new_state)
+
+
+class AbsentMidiPortItem(QTreeWidgetItem):
+    def __init__(self, parent_item: QTreeWidgetItem, port_name: str):
+        super().__init__(parent_item, (port_name,))
+        self.setDisabled(True)
+        self.setCheckState(0, Qt.CheckState.Unchecked)
 
+
+class MidiPortItem(PortItemMixin, PortWidgetItem):
+    port_instance: MidiIn | MidiOut
+    PORT_CLASS: type[MidiIn | MidiOut]
     VIRTUAL_PORT_PREFIX = '[v]'
 
+    def __init__(self, parent_item: QTreeWidgetItem, port_name: str):
+        self.port_name = port_name
+        port_key = (self.PORT_CLASS.__name__, self.port_name)
+        self.port_instance = self.PORT_CLASS.instance_registry.get(port_key, None)
+        self.repr = f"{self.PORT_CLASS.__name__}('{self.port_name}')"
+
+        if self.port_instance and self.port_instance._is_virtual:
+            item_name = f'{self.VIRTUAL_PORT_PREFIX} {self.port_name}'
+        else:
+            item_name = self.port_name
+
+        super().__init__(parent_item, (item_name,))
+
+        self.set_color_by_port_type(self.PORT_CLASS)
+
+        if not self.port_instance:
+            self.setCheckState(0, Qt.CheckState.Unchecked)
+        elif self.port_instance.is_enabled:
+            self.setCheckState(0, Qt.CheckState.Checked)
+        else:
+            self.setCheckState(0, Qt.CheckState.Unchecked)
+            self.setData(0, Qt.ItemDataRole.BackgroundRole, QBrush(QColor().fromRgb(255, 0, 0, 20)))
+
+    def request_state_change(self, new_state: bool) -> bool:
+        if not self.port_instance:
+            self.port_instance = self.PORT_CLASS(self.port_name)
+        return PortItemMixin.request_state_change(self, new_state)
+
+
+class InputMidiPortItem(MidiPortItem):
+    PORT_CLASS = MidiIn
+
+    def __init__(self, parent_item: QTreeWidgetItem, port_name: str):
+        super().__init__(parent_item, port_name)
+
+        if self.port_instance:
+            for passthrough_out_port in self.port_instance.attached_passthrough_outs:
+                PassthroughOutputMidiPortItem(self, passthrough_out_port._uid)
+
+            self.add_calls()
+
+
+class OutputMidiPortItem(MidiPortItem):
+    PORT_CLASS = MidiOut
+
+
+class PassthroughOutputMidiPortItem(OutputMidiPortItem):
+    def request_state_change(self, new_state: bool) -> bool:
+        parent_port = self.parent().port_instance
+        if new_state:
+            parent_port.attached_passthrough_outs.append(self.port_instance)
+        else:
+            parent_port.attached_passthrough_outs.remove(self.port_instance)
+        return new_state
+
+
+class CallItem(PortWidgetItem):
+    MATCH_CALL_PREFIX = '[m]'
+
+    def __init__(
+        self,
+        parent_item: QTreeWidgetItem,
+        port_instance: Input,
+        origin_call_list: list['Callable'],
+        call: 'Callable',
+    ):
+        if call.conditions:
+            item_name = f'{self.MATCH_CALL_PREFIX} {call.__name__}'
+        else:
+            item_name = call.__name__
+
+        super().__init__(parent_item, (item_name,))
+        self.port_instance = port_instance
+        self.origin_call_list = origin_call_list
+        self.call = call
+
+        item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Callable]
+        self.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
+        self.setCheckState(0, Qt.CheckState.Checked)
+
+    def request_state_change(self, new_state: bool) -> bool:
+        if new_state:
+            self.origin_call_list.append(self.call)
+        else:
+            self.origin_call_list.remove(self.call)
+        return new_state
+
+
+class PortsWidget(QTreeWidget):
     def __init__(self):
         super().__init__()
         self.setObjectName('Ports')
         self.setHeaderHidden(True)
         self.setMinimumWidth(200)
         self.setMinimumHeight(200)
         self.setMouseTracking(True)
         self.itemEntered.connect(self.__update_item_tooltip)
         self.__populate()
 
-    def __add_top_level_item(self, item_text: str) -> None:
-        bold_font = self.font()
-        bold_font.setBold(True)
-
-        top_item = QTreeWidgetItem(self, (item_text,))
-        top_item.setData(0, Qt.ItemDataRole.FontRole, bold_font)
-        top_item.setExpanded(True)
-
-        return top_item
-
     def __populate(self) -> None:
         """Populates the widget with items"""
         self.clear()
-        self.__add_midi_port_class(
-            'MIDI Inputs', MidiIn, midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input], True
-        )
-        self.__add_midi_port_class(
-            'MIDI Outputs', MidiOut, midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output], False
-        )
-        self.__add_ports_if_declared('OSC Inputs', midiscripter.OscIn)
-        self.__add_ports_if_declared('OSC Outputs', midiscripter.OscOut)
-        self.__add_keyboard_in()
-        self.__add_ports_if_declared('Keyboard Output', midiscripter.KeyOut)
-        self.__add_ports_if_declared('Metronome', midiscripter.MetronomeIn)
-        self.__add_ports_if_declared('File Event Watcher', midiscripter.FileEventIn)
-        self.__add_ports_if_declared('MIDI Port Changes Watcher', midiscripter.MidiPortsChangedIn)
 
-        self.itemChanged.connect(self.__item_state_changed)
-        self.itemSelectionChanged.connect(self.__item_selected)
+        self.__add_midi_ports()
 
-    def __add_midi_port_class(
-        self,
-        title: str,
-        port_class: type[MidiIn | MidiOut],
-        item_color: QColor,
-        add_attached: bool,
-    ) -> None:
-        if not port_class._available_names:
-            return
+        self.__add_declared_ports('OSC Inputs', midiscripter.OscIn)
+        self.__add_declared_ports('OSC Outputs', midiscripter.OscOut)
 
-        top_item = self.__add_top_level_item(title)
+        AlwaysPresentInputPortItem(self.__add_top_level_item('Keyboard Input'), KeyIn)
+        self.__add_declared_ports('Keyboard Output', midiscripter.KeyOut)
 
-        virtual_port_names = [
-            port._uid
-            for port in port_class.instance_registry.values()
-            if isinstance(port, port_class) and port._is_virtual
-        ]
-
-        for port_name in itertools.chain(port_class._available_names, virtual_port_names):
-            port_key = (port_class.__name__, port_name)
-            port_instance = port_class.instance_registry.get(port_key, None)
-
-            port_item_name = (
-                f'{self.VIRTUAL_PORT_PREFIX} {port_name}'
-                if port_instance and port_instance._is_virtual
-                else port_name
-            )
-            port_item = QTreeWidgetItem(top_item, (port_item_name,))
+        AlwaysPresentInputPortItem(self.__add_top_level_item('Mouse Input'), MouseIn)
+        self.__add_declared_ports('Mouse Output', midiscripter.MouseOut)
 
-            if not port_instance:
-                port_item.setCheckState(0, Qt.CheckState.Unchecked)
-            elif port_instance.is_enabled:
-                port_item.setCheckState(0, Qt.CheckState.Checked)
-            else:
-                port_item.setCheckState(0, Qt.CheckState.Unchecked)
-                port_item.setData(
-                    0, Qt.ItemDataRole.BackgroundRole, QBrush(QColor().fromRgb(255, 0, 0, 20))
-                )
+        self.__add_declared_ports('Metronome', midiscripter.MetronomeIn)
+        self.__add_declared_ports('File Event Watcher', midiscripter.FileEventIn)
+        self.__add_declared_ports('MIDI Port Changes Watcher', midiscripter.MidiPortsChangedIn)
 
-            port_item.setData(0, self.PORT_CLASS_ROLE, port_class)
-            port_item.setData(0, self.PORT_UID_ROLE, port_name)
+        self.itemSelectionChanged.connect(self.__item_selected)
+        # with set blocks on data change itemChanged is emitted only on check state change
+        self.itemChanged.connect(self.__item_state_changed)
 
-            port_repr = f"{port_class.__name__}('{port_name}')"
-            port_item.setData(0, self.PORT_REPR_ROLE, port_repr)
-            port_item.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
-
-            if add_attached and port_instance:
-                for passthrough_out_port in port_instance.attached_passthrough_outs:
-                    sub_item = QTreeWidgetItem(port_item, (passthrough_out_port._uid,))
-                    sub_item.setCheckState(0, Qt.CheckState.Checked)
+    def __add_top_level_item(self, item_text: str) -> QTreeWidgetItem:
+        bold_font = self.font()
+        bold_font.setBold(True)
 
-                    sub_item.setData(
-                        0,
-                        Qt.ItemDataRole.ForegroundRole,
-                        QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]),
-                    )
-                    sub_item.setData(0, self.PORT_CLASS_ROLE, MidiIn)
-                    sub_item.setData(0, self.PORT_UID_ROLE, port_name)
-                    sub_item.setData(0, self.PASSTHROUGH_OUT_PORT_ROLE, passthrough_out_port)
-                    sub_item.setData(0, self.PORT_REPR_ROLE, passthrough_out_port.__repr__())
-
-                self.__add_inputs_subscribed_calls(port_item)
-
-        for port_instance in port_class.instance_registry.values():
-            if (
-                isinstance(port_instance, port_class)
-                and not port_instance._is_available
-                and port_instance._uid not in virtual_port_names
-            ):
-                absent_input_item = QTreeWidgetItem(top_item, (str(port_instance),))
-                absent_input_item.setCheckState(0, Qt.CheckState.Unchecked)
-                absent_input_item.setDisabled(True)
-
-    def __add_inputs_subscribed_calls(self, input_item: QTreeWidgetItem) -> None:
-        port_class = input_item.data(0, self.PORT_CLASS_ROLE)
-        port_name = input_item.data(0, self.PORT_UID_ROLE)
-
-        port_instance = port_class(port_name) if port_name else port_class()
-
-        for callback_function in port_instance.subscribed_calls:
-            sub_item = QTreeWidgetItem(input_item, (callback_function.__name__,))
-            sub_item.setCheckState(0, Qt.CheckState.Checked)
-
-            sub_item.setData(
-                0,
-                Qt.ItemDataRole.ForegroundRole,
-                QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Callable]),
-            )
-            sub_item.setData(0, self.PORT_CLASS_ROLE, MidiIn)
-            sub_item.setData(0, self.PORT_UID_ROLE, port_name)
-            sub_item.setData(0, self.CALLBACK_FUNCTION_ROLE, callback_function)
+        top_item = QTreeWidgetItem(self, (item_text,))
+        top_item.setData(0, Qt.ItemDataRole.FontRole, bold_font)
+        top_item.setExpanded(True)
+
+        return top_item
 
-    def __add_ports_if_declared(self, title: str, port_type: type[Input | Output]) -> None:
+    def __add_midi_ports(self) -> None:
+        for title, _item_class in [
+            ('MIDI Inputs', InputMidiPortItem),
+            ('MIDI Outputs', OutputMidiPortItem),
+        ]:
+            top_item = self.__add_top_level_item(title)
+            port_class = _item_class.PORT_CLASS
+
+            port_instance_list = [
+                port
+                for port in port_class.instance_registry.values()
+                if isinstance(port, port_class)
+            ]
+            virtual_port_names = [port._uid for port in port_instance_list if port._is_virtual]
+
+            for port_name in itertools.chain(port_class._available_names, virtual_port_names):
+                _item_class(top_item, port_name)
+
+            for port_instance in port_instance_list:
+                if not port_instance._is_available and port_instance._uid not in virtual_port_names:
+                    AbsentMidiPortItem(top_item, port_instance._uid)
+
+    def __add_declared_ports(self, title: str, port_type: type[Input | Output]) -> None:
         port_instances_to_add = []
         for port_key, port_instance in port_type.instance_registry.items():
             if port_key[0] is port_type.__name__:
                 port_instances_to_add.append(port_instance)
 
         if not port_instances_to_add:
             return
 
         port_top = self.__add_top_level_item(title)
 
         for port in port_instances_to_add:
-            port_item = QTreeWidgetItem(port_top, (str(port._uid),))
-            port_item.setCheckState(0, Qt.CheckState.Checked)
-
-            port_item.setData(0, self.PORT_CLASS_ROLE, port_type)
-            port_item.setData(0, self.PORT_REPR_ROLE, port.__repr__())
-
-            if port._force_uid:
-                port_item.setData(0, self.PORT_UID_ROLE, None)
-            else:
-                port_item.setData(0, self.PORT_UID_ROLE, port._uid)
-
-            if issubclass(port_type, Input):
-                item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]
-                self.__add_inputs_subscribed_calls(port_item)
-            else:
-                item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]
-
-            port_item.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
-
-    def __add_keyboard_in(self) -> None:
-        port_top = self.__add_top_level_item('Keyboard Input')
-        port_item = QTreeWidgetItem(port_top, ('Keyboard Input',))
-        if (
-            midiscripter.KeyIn.__name__,
-            midiscripter.KeyIn._force_uid,
-        ) in midiscripter.KeyIn.instance_registry:
-            port_item.setCheckState(0, Qt.CheckState.Checked)
-        else:
-            port_item.setCheckState(0, Qt.CheckState.Unchecked)
-
-        port_item.setData(0, self.PORT_CLASS_ROLE, midiscripter.KeyIn)
-        port_item.setData(0, self.PORT_UID_ROLE, None)
-        port_item.setData(0, self.PORT_REPR_ROLE, f'{midiscripter.KeyIn.__name__}()')
-        port_item.setData(
-            0,
-            Qt.ItemDataRole.ForegroundRole,
-            QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]),
-        )
+            GeneralPortItem(port_top, port)
 
     def __item_selected(self) -> None:
         """Sends selected item text to the clipboard and shows a "copied" tooltip"""
         if not self.selectedItems():
             return
 
-        selected_item: QTreeWidgetItem = self.selectedItems()[0]
-        port_repr = selected_item.data(0, self.PORT_REPR_ROLE)
-        if port_repr:
+        selected_item: MidiPortItem | GeneralPortItem | CallItem = self.selectedItems()[0]
+
+        try:
+            port_repr = selected_item.repr
             QGuiApplication.clipboard().setText(port_repr)
             QTimer.singleShot(
                 200,
                 lambda: QToolTip().showText(
                     self.cursor().pos(), f'Copied {port_repr}', self, msecShowTime=2000
                 ),
             )  # Don't hide on mouse button release
+        except AttributeError:
+            pass
+
         selected_item.setSelected(False)
 
-    def __item_state_changed(self, item: QTreeWidgetItem, _: int) -> None:
+    def __item_state_changed(self, item: PortWidgetItem, _: int) -> None:
         """Enabled or disables the MIDI port / passthrough out / call according to the checked
         state change"""
-        new_checked_state = item.checkState(0) == Qt.CheckState.Checked
-
-        port_class = item.data(0, self.PORT_CLASS_ROLE)
-        port_name = item.data(0, self.PORT_UID_ROLE)
-
-        callback_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
-        passthrough_out_port: MidiOut = item.data(0, self.PASSTHROUGH_OUT_PORT_ROLE)
-
-        port_instance = port_class(port_name) if port_name else port_class()
+        self.blockSignals(True)
+        target_state: bool = item.checkState(0) == Qt.CheckState.Checked
+        new_item_state = item.request_state_change(target_state)
+        item.setCheckState(0, (Qt.CheckState.Unchecked, Qt.CheckState.Checked)[new_item_state])
+        self.blockSignals(False)
 
-        if callback_function:
-            if new_checked_state:
-                port_instance.subscribed_calls.append(callback_function)
-            else:
-                port_instance.subscribed_calls.remove(callback_function)
+    def __update_item_tooltip(self, item: QTreeWidgetItem) -> None:
+        """Updates items tooltip on hover"""
+        if not isinstance(item, CallItem):
+            return
 
-        elif passthrough_out_port:
-            if new_checked_state:
-                port_instance.attached_passthrough_outs.append(passthrough_out_port)
-            else:
-                port_instance.attached_passthrough_outs.remove(passthrough_out_port)
+        call_statistics = list(item.call.statistics)
 
+        if not call_statistics:
+            tooltip_text = 'No calls made yet'
         else:
-            if new_checked_state:
-                if not port_instance.is_enabled:
-                    port_instance._open()
-
-                    if port_instance.is_enabled:
-                        log('Enabled {port}', port=port_instance)
-                    else:
-                        item.setData(
-                            0,
-                            Qt.ItemDataRole.BackgroundRole,
-                            QBrush(QColor().fromRgb(255, 0, 0, 20)),
-                        )
-                        log.red("Can't enable {port}", port=port_instance)
-                else:
-                    item.setData(
-                        0,
-                        Qt.ItemDataRole.BackgroundRole,
-                        QBrush(QColor(Qt.GlobalColor.transparent)),
-                    )
-
-            else:
-                port_instance.is_enabled = False
-                log('Disabled {port}', port=port_instance)
-
-            self.blockSignals(True)
-            item.setCheckState(
-                0, (Qt.CheckState.Unchecked, Qt.CheckState.Checked)[port_instance.is_enabled]
+            call_statistics.sort()
+            tooltip_text = (
+                f'Execution time for last {len(call_statistics)} calls:\n'
+                f'Min: {call_statistics[0]} ms; '
+                f'Med: {call_statistics[int(len(call_statistics) / 2)]} ms; '
+                f'Max: {call_statistics[-1]} ms'
             )
-            self.blockSignals(False)
-
-    def __update_item_tooltip(self, item: QTreeWidgetItem) -> None:
-        """Updates items tooltip on hover"""
-        call_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
-        if call_function:
-            port_class = item.data(0, self.PORT_CLASS_ROLE)
-            call_statistics = list(port_class._call_statistics[call_function])
 
-            if not call_statistics:
-                tooltip_text = 'No calls made yet'
-            else:
-                call_statistics.sort()
-                tooltip_text = (
-                    'Execution time for last 20 calls:\n'
-                    f'Min: {call_statistics[0]} ms; '
-                    f'Med: {call_statistics[int(len(call_statistics) / 2)]} ms; '
-                    f'Max: {call_statistics[-1]} ms'
-                )
+        if item.call.conditions:
+            tooltip_text = (
+                f'Conditions: {item.call.conditions[0]} {item.call.conditions[1]}\n{tooltip_text}'
+            )
 
-            item.setData(0, Qt.ItemDataRole.ToolTipRole, tooltip_text)
+        self.blockSignals(True)
+        item.setData(0, Qt.ItemDataRole.ToolTipRole, tooltip_text)
+        self.blockSignals(False)
```

### Comparing `midiscripter-0.3/midiscripter/gui/gui_widgets/gui_msg.py` & `midiscripter-0.4/midiscripter/gui/gui_widgets/gui_msg.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import midiscripter.base.msg_base
 
 if TYPE_CHECKING:
     from collections.abc import Sequence, Container
     from midiscripter.gui.gui_widgets.gui_widget_base import GuiWidget
 
 
-class GuiEventType(midiscripter.base.msg_base.AttrEnum):
-    """GUI event type enumerator to use as [`GuiEventMsg`][midiscripter.GuiEventMsg] `type` attribute."""
+class GuiEvent(midiscripter.base.msg_base.AttrEnum):
+    """GUI event type enumerator
+    to use as [`GuiEventMsg`][midiscripter.GuiEventMsg] `type` attribute."""
 
     TRIGGERED = 'TRIGGERED'
     CONTENT_SET = 'CONTENT_SET'
     COLOR_SET = 'COLOR_SET'
     TOGGLED = 'TOGGLED'
     SELECTED = 'SELECTED'
     VALUE_CHANGED = 'VALUE_CHANGED'
 
 
 class GuiEventMsg(midiscripter.base.msg_base.Msg):
     """GUI interaction message produced by GUI widget port."""
 
-    type: GuiEventType
+    type: GuiEvent
     """GUI event type."""
 
     data: 'str | int | bool | Sequence | None'
     """New value set by event.
     
     Data meaning for event types:  
     TRIGGERED - None.  
@@ -38,23 +39,22 @@
 
     source: 'None | GuiWidget'
 
     __match_args__: tuple[str] = ('type', 'data')
 
     def __init__(
         self,
-        type: GuiEventType,
+        type: GuiEvent,
         data: 'str | int | bool | Sequence | None' = None,
         *,
         source: 'None | GuiWidget' = None,
     ):
         super().__init__(source)
         self.type = type
         self.data = data
 
     def matches(
         self,
-        type: 'None | Container[GuiEventType] | GuiEventType' = None,
-        data: 'None | Container[str | int | bool | Sequence | None] | \
-                       str | int | bool | Sequence | None' = None,
+        type: 'None | Container[GuiEvent] | GuiEvent' = None,
+        data: 'None | Container | str | int | bool | Sequence' = None,
     ) -> bool:
         return super().matches(type, data)
```

### Comparing `midiscripter-0.3/midiscripter/gui/gui_widgets/gui_widget_base.py` & `midiscripter-0.4/midiscripter/gui/gui_widgets/gui_widget_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 import types
-from typing import TYPE_CHECKING
-from collections.abc import Sequence
+from typing import TYPE_CHECKING, overload
 
 from PySide6.QtWidgets import *
 
 import midiscripter.base.msg_base
 import midiscripter.base.port_base
 import midiscripter.gui.app
 
-from .gui_msg import GuiEventMsg, GuiEventType
+from .gui_msg import GuiEventMsg, GuiEvent
 
 if TYPE_CHECKING:
+    from collections.abc import Container, Callable
     from .mixins import WrappedQWidgetMixin
 
 
 class GuiWidget(midiscripter.base.port_base.Input):
     """GUI windows widget which also acts like an input port."""
 
     _qt_widget_class: type[QWidget, 'WrappedQWidgetMixin']
 
     def __init__(
         self,
-        content: str | tuple[str, ...],
-        title: str | None = None,
-        color: str | tuple[int, int, int] | None = None,
+        title_and_content: str | tuple[str, ...],
+        content: str | tuple[str, ...] | None = None,
         *,
+        color: str | tuple[int, int, int] | None = None,
         value: str | None = None,
         select: int | str | None = None,
         toggle_state: bool | None = None,
     ):
         """
         Args:
+            title (str): Widget's title
             content: Widget's text or text for its items
-            title: Widget's title, `None` for same as content
-            color: Preset text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-            value: Preset value
-            select: Preset item text / index to select
-            toggle_state: Preset toggle state
+            color: Content color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
+            value: Initial value
+            select: Preselected item
+            toggle_state: Initial toggle state
         """
+        if isinstance(title_and_content, types.GeneratorType):
+            title_and_content = tuple(title_and_content)
         if isinstance(content, types.GeneratorType):
             content = tuple(content)
 
-        self.title = title or str(content)
+        self.title = str(title_and_content)
         """Widget's title."""
         super().__init__(self.title)
 
         self.qt_widget = self._qt_widget_class()  # workaround for mkdocstrings issue #607
 
         self.qt_widget: QWidget
         """Wrapped `PySide6` `QWidget` that can be altered for extra customization."""
 
         self.qt_widget.setObjectName(self.title)
         midiscripter.gui.app.add_qwidget(self.qt_widget)
 
-        self.content = content
+        self.content = content if content else title_and_content
 
         if value:
             self.value = value
 
         if select:
             self.select(select)
 
@@ -67,34 +69,34 @@
         if color:
             self.color = color
 
         self.__connect_change_signals()
 
     def __connect_change_signals(self) -> None:
         self.qt_widget.triggered_signal.connect(
-            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEventType.TRIGGERED))
+            lambda: self._send_input_msg_to_calls(GuiEventMsg(GuiEvent.TRIGGERED))
         )
         self.qt_widget.content_changed_signal.connect(
             lambda: self._send_input_msg_to_calls(
-                GuiEventMsg(GuiEventType.CONTENT_SET, self.qt_widget.get_content())
+                GuiEventMsg(GuiEvent.CONTENT_SET, self.qt_widget.get_content())
             )
         )
         self.qt_widget.value_changed_signal.connect(
             lambda: self._send_input_msg_to_calls(
-                GuiEventMsg(GuiEventType.VALUE_CHANGED, self.qt_widget.get_value())
+                GuiEventMsg(GuiEvent.VALUE_CHANGED, self.qt_widget.get_value())
             )
         )
         self.qt_widget.selection_changed_signal.connect(
             lambda: self._send_input_msg_to_calls(
-                GuiEventMsg(GuiEventType.SELECTED, self.qt_widget.get_selected_item_text())
+                GuiEventMsg(GuiEvent.SELECTED, self.qt_widget.get_selected_item_text())
             )
         )
         self.qt_widget.toggle_state_changed_signal.connect(
             lambda: self._send_input_msg_to_calls(
-                GuiEventMsg(GuiEventType.TOGGLED, self.qt_widget.get_toggle_state())
+                GuiEventMsg(GuiEvent.TOGGLED, self.qt_widget.get_toggle_state())
             )
         )
 
     @property
     def content(self) -> str | tuple[str, ...]:
         """Widget's text or text for its items."""
         return self.qt_widget.get_content()
@@ -159,15 +161,30 @@
     def color(self) -> str | tuple[int, int, int] | None:
         """Text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple"""
         return self.qt_widget.get_color()
 
     @color.setter
     def color(self, new_color_value: str | tuple[int, int, int]) -> None:
         self.qt_widget.set_color_signal.emit(new_color_value)
-        self._send_input_msg_to_calls(
-            GuiEventMsg(GuiEventType.COLOR_SET, new_color_value, source=self)
-        )
+        self._send_input_msg_to_calls(GuiEventMsg(GuiEvent.COLOR_SET, new_color_value, source=self))
 
     @property
     def is_visible(self) -> bool:
         """Widget is currently visible."""
         return self.qt_widget.isVisible()
+
+    @overload
+    def subscribe(self, call: 'Callable[[GuiEventMsg], None]') -> 'Callable': ...
+
+    @overload
+    def subscribe(
+        self,
+        type: 'None | Container[GuiEvent] | GuiEvent' = None,
+        data: 'None | Container | str | int | bool | Sequence' = None,
+    ) -> 'Callable': ...
+
+    def subscribe(
+        self,
+        type: 'None | Container[GuiEvent] | GuiEvent' = None,
+        data: 'None | Container | str | int | bool | Sequence' = None,
+    ) -> 'Callable':
+        return super().subscribe(type, data)
```

### Comparing `midiscripter-0.3/midiscripter/gui/gui_widgets/list.py` & `midiscripter-0.4/midiscripter/gui/gui_widgets/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Sequence
+from typing import overload
 
 from PySide6.QtWidgets import *
 
 from .gui_widget_base import GuiWidget
 from .mixins import WrappedQWidgetMixin
 
 
@@ -44,23 +44,61 @@
 
 
 class GuiListSelector(GuiWidget):
     """List of text items to select value."""
 
     _qt_widget_class = ListSelectorWidget
 
+    @overload
     def __init__(
         self,
+        title: str,
         content: tuple[str, ...],
-        title: str | None = None,
+        *,
+        color: str | tuple[int, int, int] | None = None,
+        select: int | str | None = None,
+    ): ...
+
+    @overload
+    def __init__(
+        self,
+        content: tuple[str, ...],
+        *,
         color: str | tuple[int, int, int] | None = None,
+        select: int | str | None = None,
+    ): ...
+
+    def __init__(
+        self,
+        title_and_content: str | tuple[str, ...],
+        content: tuple[str, ...] | None = None,
         *,
+        color: str | tuple[int, int, int] | None = None,
         select: int | str | None = None,
     ):
         """
+        **Overloads:**
+            ``` python
+            GuiListSelector(
+                title: str,
+                content: tuple[str, ...],
+                *,
+                color: str | tuple[int, int, int] | None = None,
+                select: int | str | None = None
+            )
+            ```
+            ``` python
+            GuiListSelector(
+                content: tuple[str, ...],
+                *,
+                color: str | tuple[int, int, int] | None = None,
+                select: int | str | None = None
+            )
+            ```
+
         Args:
-            content: Text items
-            title: Widget's title, `None` for same as content
+            title (str): Widget's title
+            content: Items' texts
             color: Text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
-            select: text or index of item to select initially
+            select: Text or index of item to select initially
         """
-        super().__init__(content, title, select=select, color=color)
+        super().__init__(title_and_content, content, color=color, select=select)
```

### Comparing `midiscripter-0.3/midiscripter/gui/gui_widgets/mixins.py` & `midiscripter-0.4/midiscripter/gui/gui_widgets/mixins.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.3/midiscripter/keyboard/keyboard_msg.py` & `midiscripter-0.4/midiscripter/keyboard/keyboard_msg.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,50 +26,53 @@
     pynput.keyboard.Key.ctrl_l: pynput.keyboard.Key.ctrl,
     pynput.keyboard.Key.ctrl_r: pynput.keyboard.Key.ctrl,
     pynput.keyboard.Key.shift_l: pynput.keyboard.Key.shift,
     pynput.keyboard.Key.shift_r: pynput.keyboard.Key.shift,
 }
 
 
-class KeyEventType(midiscripter.base.msg_base.AttrEnum):
-    KEY_PRESS = 'KEY_PRESS'
-    KEY_RELEASE = 'KEY_RELEASE'
-    KEY_TAP = 'KEY_TAP'
-    """Key press and release. Isn't assigned by [`KeyIn`][midiscripter.KeyIn]. 
-       Use it for message declarations in calls."""
+class KeyEvent(midiscripter.base.msg_base.AttrEnum):
+    """Keyboard event message type enumerator
+    to use as [`KeyMsg`][midiscripter.KeyMsg] `type` attribute."""
+
+    PRESS = 'PRESS'
+    RELEASE = 'RELEASE'
+    TAP = 'TAP'
+    """Key press and release. Isn't assigned by [`KeyIn`][midiscripter.KeyIn]
+       but can be sent with [`KeyOut`][midiscripter.KeyOut]."""
 
 
 class KeyMsg(midiscripter.base.msg_base.Msg):
     """Keyboard event message"""
 
     __match_args__ = ('type', 'shortcut')
 
-    type: KeyEventType
+    type: KeyEvent
     """Keyboard event type"""
 
     keycodes: list[pynput.keyboard.Key]
     """Keycodes in the order they were pressed. Use when press order matters."""
 
     source: 'None | KeyIn'
 
     def __init__(
         self,
-        type: KeyEventType,
+        type: KeyEvent,
         shortcut_or_keycodes: str | Iterable[pynput.keyboard.Key],
         *,
         source: 'None | KeyIn' = None,
     ):
         """
         Args:
             type: Keyboard event type
             shortcut_or_keycodes: keyboard shortcut description or event key codes
-            source (KeyIn): The [`KeyIn`][midiscripter.KeyIn] instance that generated the message
+            source: The [`KeyIn`][midiscripter.KeyIn] instance that generated the message
 
         Tip:
-            Run GUI and Enable keyboard input. Use log to get messages with shortcuts you need.
+            Run GUI and enable keyboard input. Use log to get messages with shortcuts you need.
         """
         super().__init__(type, source)
         self.__shortcut_cache = ''
         self.__cached_keycodes = None
 
         if isinstance(shortcut_or_keycodes, str):
             self.shortcut = shortcut_or_keycodes.lower()
@@ -112,11 +115,11 @@
                 key = pynput.keyboard.KeyCode.from_char(key)
             else:
                 key = getattr(pynput.keyboard.Key, key)
             self.keycodes.append(key)
 
     def matches(
         self,
-        type: 'None | Container[KeyEventType] | KeyEventType' = None,
+        type: 'None | Container[KeyEvent] | KeyEvent' = None,
         shortcut: 'None | Container[str] | str' = None,
     ) -> bool:
         return super().matches(type, shortcut)
```

### Comparing `midiscripter-0.3/midiscripter/logger/console_sink.py` & `midiscripter-0.4/midiscripter/logger/console_sink.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.3/midiscripter/logger/html_sink.py` & `midiscripter-0.4/midiscripter/logger/html_sink.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     def __call__(self, log_entries: list[tuple[str, dict]]):
         html_entries = []
         for entry in log_entries:
             text = entry[0]
             kwargs = entry[1]
 
             text = text.replace('\n', '<br>')
-            text = text.replace(' ', '&nbsp;')
 
             if '_color' in kwargs:
                 text = to_html_colored_text(text, f'dark{kwargs["_color"]}')
 
             for arg_name, arg_object in kwargs.items():
                 for obj_type in (Input, Output, Msg):
                     if isinstance(arg_object, obj_type):
```

### Comparing `midiscripter-0.3/midiscripter/logger/log.py` & `midiscripter-0.4/midiscripter/logger/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 import threading
 import time
 from typing import TYPE_CHECKING
 
-import midiscripter.base.shared
+import midiscripter.shared
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from midiscripter.logger.console_sink import ConsoleSink
     from midiscripter.logger.html_sink import HtmlSink
 
 
@@ -49,22 +49,15 @@
                       Passed [inputs][midiscripter.base.port_base.Input],
                       [outputs][midiscripter.base.port_base.Output],
                       [messages][midiscripter.base.msg_base.Msg] and callables are highlighted.
         """
         if not self.is_enabled:
             return
 
-        precise_time = midiscripter.base.shared.precise_epoch_time()
-        time_string = time.strftime('%H:%M:%S', time.localtime(precise_time))
-
-        # >1.5 times faster than datetime
-        after_dot = repr(precise_time).split('.')[1][:6].ljust(6, '0')
-        milisec_part = after_dot[:3]
-        microsec_part = after_dot[3:]
-        kwargs['_ctime_str'] = f'{time_string}.{milisec_part},{microsec_part}'
+        kwargs['_ctime_str'] = self._get_current_precise_time_stamp()
 
         self.__buffer.append((str(text), kwargs))
 
     @property
     def _sink(self) -> 'Callable':
         """A callable that receives a list of log strings to print them for user.
         Set by starter. Can be altered to customize the logger."""
@@ -85,28 +78,43 @@
             time.sleep(self.FLUSH_DELAY)
             self.__wait_counter += self.FLUSH_DELAY
             if self.__buffer:
                 self._flush()
 
     def _flush(self) -> None:
         """Sends buffered messages to sink"""
+        if not self.__sink:
+            return
+
         output_entries = []
 
         if self.__wait_counter > self.ADD_SPACER_THRESHOLD_SEC:
             output_entries.append(('', {}))
         self.__wait_counter = 0
 
         while self.__buffer:
             output_entries.append(self.__buffer.popleft())  # for thread safety
 
         try:
             self._sink(output_entries)
-        except (TypeError, RuntimeError):  # ignore Qt error on widget destruction at app exit
+        except RuntimeError:  # ignore Qt error on widget destruction at app exit
             pass
 
+    @staticmethod
+    def _get_current_precise_time_stamp() -> str:
+        """Returns current timestamp with microsecond precision as a string"""
+        precise_time = midiscripter.shared.precise_epoch_time()
+        time_string = time.strftime('%H:%M:%S', time.localtime(precise_time))
+
+        # >1.5 times faster than datetime
+        after_dot = repr(precise_time).split('.')[1][:6].ljust(6, '0')
+        milisec_part = after_dot[:3]
+        microsec_part = after_dot[3:]
+        return f'{time_string}.{milisec_part},{microsec_part}'
+
     def red(self, text: str, **kwargs) -> None:
         """Print red log message."""
         self(text, _color='red', **kwargs)
 
     def blue(self, text: str, **kwargs) -> None:
         """Print blue log message."""
         self(text, _color='blue', **kwargs)
```

### Comparing `midiscripter-0.3/midiscripter/metronome/metronome_port.py` & `midiscripter-0.4/midiscripter/metronome/metronome_port.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,84 @@
 import time
+from typing import overload
 
 import midiscripter.base.port_base
-import midiscripter.base.shared
+import midiscripter.shared
 from midiscripter.base.msg_base import Msg
 from midiscripter.base.port_base import Output
 from midiscripter.logger import log
 
 
 class MetronomeIn(midiscripter.base.port_base.Input):
-    """The input port that sends messages with set interval."""
+    """The input port that sends messages with set interval
 
-    def __init__(self, name_or_bpm: str | float, bpm: float = 60, msg_to_send: Msg = Msg('Click')):  # noqa: B008
+    Notes:
+        `Metronome` sets extra `bpm` and `number` attributes to any message it sends
+    """
+
+    @overload
+    def __init__(self, name: str, bpm: float = 60, *, msg_to_send: Msg = Msg('Click')): ...  # noqa: B008
+
+    @overload
+    def __init__(self, bpm: float, *, msg_to_send: Msg = Msg('Click')): ...  # noqa: B008
+
+    def __init__(
+        self,
+        name_or_bpm: str | float,
+        bpm: float = 60,
+        *,
+        msg_to_send: Msg = Msg('Click'),  # noqa: B008
+    ):
         """
+        **Overloads:**
+            ``` python
+            MetronomeIn(name: str, bpm: float = 60, msg_to_send: Msg = Msg('Click'))
+            ```
+            ``` python
+            MetronomeIn(bpm: float, *, msg_to_send: Msg = Msg('Click'))
+            ```
+
         Args:
-            name_or_bpm: Metronome name, if it's a number it will also set bpm interval
+            name (str): Metronome name
             bpm: Message sending interval in beats per minute
-            msg_to_send: Message that the port will send
+            msg_to_send: Message the port will send
         """
         super().__init__(name_or_bpm)
         try:
             self.bpm = float(name_or_bpm)
         except ValueError:
             self.bpm = bpm
 
         self.msg_to_send = msg_to_send
-        self.msg_to_send.source = self
-
-        self.attached_passthrough_outs: list[Output] = []
-        """[`Output`][midiscripter.base.port_base.Output] ports attached 
-           as pass-through ports to send metronome messages"""
 
     @property
     def bpm(self) -> float:
         """Message sending interval in beats per minute."""
         return 60 / self.__interval_sec
 
     @bpm.setter
     def bpm(self, bpm: float) -> None:
         self.__interval_sec = 60 / bpm
 
-    def passthrough_out(self, output: Output) -> None:
-        """Attach output port as a pass-through port to send metronome messages.
-        The output port should be compatible to send messages.
-
-        Args:
-            output: [`Output`][midiscripter.base.port_base.Output] port to use for pass-through
-        """
-        if output not in self.attached_passthrough_outs:
-            self.attached_passthrough_outs.append(output)
-            log('{input} input will pass through {output}', input=self, output=output)
-
     def _open(self) -> None:
         self.is_enabled = True
-        midiscripter.base.shared.thread_executor.submit(self.__send_clicks_worker)
-        log(f'Started metronome at {self.bpm} bpm')
+        midiscripter.shared.thread_executor.submit(self.__send_clicks_worker)
+        log('Started {input} at {bpm}', input=self, bpm=self.bpm)
 
     def __send_clicks_worker(self) -> None:
+        msg_counter = 1
         while self.is_enabled:
             time.sleep(self.__interval_sec)
-            self.msg_to_send.ctime = midiscripter.base.shared.precise_epoch_time()
 
-            for output in self.attached_passthrough_outs:
-                output.send(self.msg_to_send)
+            self.msg_to_send.source = self
+            self.msg_to_send.ctime = midiscripter.shared.precise_epoch_time()
+            self.msg_to_send.bpm = self.bpm
+            self.msg_to_send.number = msg_counter
 
             self._send_input_msg_to_calls(self.msg_to_send)
 
-        log(f'Stopped metronome at {self.bpm} bpm')
+            msg_counter += 1
+
+        log('Stopped {input}', input=self)
 
     def _close(self) -> None:
         self.is_enabled = False
```

### Comparing `midiscripter-0.3/midiscripter/midi/midi_note_data.py` & `midiscripter-0.4/midiscripter/midi/midi_note_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,28 +36,28 @@
     'A#',
     'B',
 )
 _NOTE_INT_TO_NOTE_NAME_MAP_FLATS = ('C', 'Db', 'D', 'Eb', 'E', 'F', 'Gb', 'G', 'Ab', 'A', 'Bb', 'B')
 
 
 class NoteData:
-    """Optional wrapper for MIDI note data for readable representation.
-    When using it as `int` - it's note MIDI data, when using as `str` - it's note name.
+    """Optional wrapper for readable representation of MIDI note data.
+    When using it as `int` - it's note's MIDI data, when using as `str` - it's note's name.
     """
 
     middle_c_octave_n = 3
     """Octave number for middle C to use as reference for note naming"""
 
     __note_name_re = re.compile(r'([A-G][#|b]?)(-?[0-9])')
 
     def __init__(self, int_or_name: int | str, use_flats: bool = False):
         """
         Args:
             int_or_name: note MIDI data (0-127) or note name (like 'C#3' or 'Db3')
-            use_flats: True to use flats in note name (Db3), False to use sharps (C#3)
+            use_flats: `True` to use flats in note name (Db3), `False` to use sharps (C#3)
         """
         if isinstance(int_or_name, int):
             self.__int = int_or_name
             self.__str = self.__covert_to_str(self.__int, use_flats)
         elif isinstance(int_or_name, str):
             self.__str = int_or_name
             self.__int = self.__covert_to_int(self.__str)
```

### Comparing `midiscripter-0.3/midiscripter/midi/midi_port.py` & `midiscripter-0.4/midiscripter/midi/midi_port.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import platform
-from collections.abc import Callable
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, overload
 
 import rtmidi
 import rtmidi.midiconstants
 
 import midiscripter.base.port_base
 from midiscripter.logger import log
 from midiscripter.midi.midi_msg import MidiType
 
 if TYPE_CHECKING:
+    from collections.abc import Callable, Container
     from midiscripter.midi.midi_msg import MidiMsg
 
+
 BYTE_TO_TYPE_MAP = {
     rtmidi.midiconstants.NOTE_ON: MidiType.NOTE_ON,
     rtmidi.midiconstants.NOTE_OFF: MidiType.NOTE_OFF,
     rtmidi.midiconstants.PITCH_BEND: MidiType.PITCH_BEND,
     rtmidi.midiconstants.PROGRAM_CHANGE: MidiType.PROGRAM_CHANGE,
     rtmidi.midiconstants.CONTROLLER_CHANGE: MidiType.CONTROL_CHANGE,
     rtmidi.midiconstants.POLY_PRESSURE: MidiType.POLYTOUCH,
@@ -47,50 +48,55 @@
         port_names_without_prefixes = [
             port_name[port_name.find(':') + 1 :] for port_name in persistent_port_names
         ]
         return port_names_without_prefixes
 
 
 class _MidiPortMixin(midiscripter.base.port_base.Port):
+    name: str
+    """MIDI port name"""
+
     # Attrs provided by the class that inherits from MidiPortMixin
     is_enabled: bool
     _available_names: list[str]
     _is_virtual = False
 
     # noinspection PyMissingConstructor
-    def __init__(self, port_name: str, input_callback: Callable | None = None):
-        self.__port_name = port_name
+    def __init__(self, port_name: str, input_callback: 'Callable | None' = None):
+        self.name = port_name
+        self.name: str
+        """MIDI port name"""
 
         if input_callback:
             self._rtmidi_port = rtmidi.MidiIn()
             self._rtmidi_port.ignore_types(sysex=False)
             self._rtmidi_port.set_callback(input_callback)
         else:
             self._rtmidi_port = rtmidi.MidiOut()
 
     @property
     def _is_available(self) -> bool:
         """Port is available and can be opened."""
-        return self.__port_name in self._available_names
+        return self.name in self._available_names
 
     def _open(self) -> None:
         if self._rtmidi_port.is_port_open():
             self.is_enabled = True
             return
 
         try:
-            port_index = self._available_names.index(self.__port_name)
+            port_index = self._available_names.index(self.name)
             self._rtmidi_port.open_port(port_index)
             self.is_enabled = True
             log('Opened {port}', port=self)
         except ValueError:
             if platform.system() == 'Windows':
                 log.red("Can't find port {port}. Check the port name.", port=self)
             else:
-                self._rtmidi_port.open_virtual_port(self.__port_name)
+                self._rtmidi_port.open_virtual_port(self.name)
                 self._is_virtual = True
                 self.is_enabled = True
                 log('Created and opened virtual port {port}', port=self)
         except Exception:
             log.red('Failed to open {port}', port=self)
 
     def _close(self) -> None:
@@ -115,15 +121,15 @@
         """
         Args:
             port_name: MIDI input port name
         """
         _MidiPortMixin.__init__(self, port_name, self.__callback)
         midiscripter.base.port_base.Input.__init__(self, port_name)
 
-        self.attached_passthrough_outs: list['MidiOut'] = []
+        self.attached_passthrough_outs: 'list[MidiOut]' = []
         """[`MidiOut`][midiscripter.MidiOut] ports attached as pass-through ports
         which will send all incoming messages as soon as they arrive before sending them to calls"""
 
     def passthrough_out(self, midi_output: 'MidiOut') -> None:
         """Attach [`MidiOut`][midiscripter.MidiOut] as a pass-through port
         to send all incoming messages as soon as they arrive,
         before sending them to calls. This can greatly reduce latency.
@@ -131,14 +137,35 @@
         Args:
             midi_output: [`MidiOut`][midiscripter.MidiOut] port to use for pass-through
         """
         if midi_output not in self.attached_passthrough_outs:
             self.attached_passthrough_outs.append(midi_output)
             log('{input} input will pass through {output}', input=self, output=midi_output)
 
+    @overload
+    def subscribe(self, call: 'Callable[[MidiMsg], None]') -> 'Callable': ...
+
+    @overload
+    def subscribe(
+        self,
+        type: 'None | Container | MidiType' = None,
+        channel: 'None | Container | int | tuple[int, ...]' = None,
+        data1: 'None | Container | int | tuple[int, ...]' = None,
+        data2: 'None | Container | int | tuple[int, ...]' = None,
+    ) -> 'Callable': ...
+
+    def subscribe(
+        self,
+        type: 'None | Container | MidiType' = None,
+        channel: 'None | Container | int | tuple[int, ...]' = None,
+        data1: 'None | Container | int | tuple[int, ...]' = None,
+        data2: 'None | Container | int | tuple[int, ...]' = None,
+    ) -> 'Callable':
+        return super().subscribe(type, channel, data1, data2)
+
     def __callback(self, rt_midi_input: tuple[tuple[hex, ...], float], _: list) -> None:
         if not self.is_enabled:
             return
 
         rt_midi_data, _ = rt_midi_input
         [output._passthrough_send(rt_midi_data) for output in self.attached_passthrough_outs]
         self._send_input_msg_to_calls(self.__convert_to_msg(rt_midi_data))
```

### Comparing `midiscripter-0.3/midiscripter/midi/midi_ports_update.py` & `midiscripter-0.4/midiscripter/midi/midi_ports_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 import time
+from typing import ClassVar
 
 import rtmidi
 
-import midiscripter.base.msg_base
 import midiscripter.base.port_base
-import midiscripter.base.shared
+import midiscripter.shared
 import midiscripter.logger
+from midiscripter.base.msg_base import Msg
 
 
 class MidiPortsChangedIn(midiscripter.base.port_base.Input):
-    """MIDI ports change watcher. Produces [`Msg`][midiscripter.base.msg_base.Msg] objects
-    with `MIDI Ports Changed` as `type` on any MIDI port connection or disconnection.
+    """MIDI ports change watcher. Produces base [`Msg`][midiscripter.Msg] objects.
 
     Used as a service port for `Restart on new MIDI port found` GUI option.
-
-    Notes:
-        Can be used to restart CLI scripts on ports change by:
-        `MidiPortsChangedIn().subscribe(restart_script)`.
     """
 
-    REFRESH_RATE_SEC = 1
-    """MIDI ports polling rate."""
+    refresh_rate_sec: float = 1
+    """MIDI ports polling rate in seconds"""
 
-    _force_uid = 'MIDI Ports Change'
+    _force_uid: ClassVar[str] = 'MIDI Ports Change'
 
     def __init__(self):
+        """"""
         super().__init__(self._force_uid)
         self.__dummy_midi_input = rtmidi.MidiIn()
         self.__dummy_midi_output = rtmidi.MidiOut()
 
         self.__last_check_inputs = self.__dummy_midi_input.get_ports()
         self.__last_check_outputs = self.__dummy_midi_output.get_ports()
 
     def _open(self) -> None:
         self.is_enabled = True
-        midiscripter.base.shared.thread_executor.submit(self.__updater_worker)
+        midiscripter.shared.thread_executor.submit(self.__updater_worker)
         midiscripter.logger.log('Started MIDI ports change watcher')
 
     def _close(self) -> None:
         self.is_enabled = False
 
     def __updater_worker(self) -> None:
         while self.is_enabled:
-            time.sleep(self.REFRESH_RATE_SEC)
+            time.sleep(self.refresh_rate_sec)
 
             current_inputs = self.__dummy_midi_input.get_ports()
             current_outputs = self.__dummy_midi_output.get_ports()
 
             if (
                 self.__last_check_inputs != current_inputs
                 or self.__last_check_outputs != current_outputs
             ):
+                msg = Msg('MIDI Ports Changed', self)
+                self._send_input_msg_to_calls(msg)
+
                 self.__last_check_inputs = current_inputs
                 self.__last_check_outputs = current_outputs
-                self._send_input_msg_to_calls(midiscripter.base.msg_base.Msg('MIDI Ports Changed'))
```

### Comparing `midiscripter-0.3/midiscripter/osc/osc_msg.py` & `midiscripter-0.4/midiscripter/osc/osc_msg.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,21 +28,19 @@
         *,
         source: 'None | OscIn' = None,
     ):
         """
         Args:
             address: Open Sound Control message address
             data: Open Sound Control message data
-            source (OscIn): The [`OscIn`][midiscripter.OscIn] instance
-                            that generated the message
+            source: The [`OscIn`][midiscripter.OscIn] instance that generated the message
         """
         super().__init__(self.type, source)
         self.address = address
         self.data = data
 
     def matches(
         self,
-        address: 'None | Container[str] | str' = None,
-        data: 'None | Container[str | bytes | bool | int | float | list | tuple] | \
-               str | bytes | bool | int | float | list | tuple' = None,
+        address: 'None | Container | str' = None,
+        data: 'None | Container | str | bytes | bool | int | float | list | tuple' = None,
     ) -> bool:
         return super().matches(self.type, address, data)
```

### Comparing `midiscripter-0.3/midiscripter/osc/osc_port.py` & `midiscripter-0.4/midiscripter/osc/osc_port.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from typing import TYPE_CHECKING, overload
+
 import pythonosc.osc_server
 import pythonosc.udp_client
 
 import midiscripter.base.port_base
-import midiscripter.base.shared
+import midiscripter.shared
 import midiscripter.osc.osc_msg
 from midiscripter.logger import log
 from midiscripter.osc.osc_msg import OscMsg
 
+if TYPE_CHECKING:
+    from collections.abc import Container, Callable
+
 
 def _parse_ip_port(ip_port: str | int) -> (str, int):
     """Parses 'ip:port' or local port to get ip and port
 
     Args:
         ip_port: 'ip:port' or local port
     Returns:
@@ -56,23 +61,40 @@
 
         self.__dispatcher = pythonosc.osc_server.Dispatcher()
         self.__dispatcher.set_default_handler(self.__osc_server_msg_handler)
         self._osc_server = pythonosc.osc_server.BlockingOSCUDPServer(
             (self.listener_ip_address, self.listener_port), self.__dispatcher
         )
 
-        midiscripter.base.shared.thread_executor.submit(self._osc_server.serve_forever)
+        midiscripter.shared.thread_executor.submit(self._osc_server.serve_forever)
         self.is_enabled = True
         log('Opened {input}', input=self)
 
     def _close(self) -> None:
         self._osc_server.shutdown()
         self.is_enabled = False
         log('Stopped {input}', input=self)
 
+    @overload
+    def subscribe(self, call: 'Callable[[OscMsg], None]') -> 'Callable': ...
+
+    @overload
+    def subscribe(
+        self,
+        address: 'None | Container | str' = None,
+        data: 'None | Container | str | bytes | bool | int | float | list | tuple' = None,
+    ) -> 'Callable': ...
+
+    def subscribe(
+        self,
+        address: 'None | Container | str' = None,
+        data: 'None | Container | str | bytes | bool | int | float | list | tuple' = None,
+    ) -> 'Callable':
+        return super().subscribe(address, data)
+
 
 class OscOut(midiscripter.base.port_base.Output):
     """Open Sound Control output port. Sends [`OscMsg`][midiscripter.OscMsg] objects."""
 
     def __init__(self, target_ip_port: str | int):
         """
         Args:
```

### Comparing `midiscripter-0.3/midiscripter/osc/osc_query_maker.py` & `midiscripter-0.4/midiscripter/osc/osc_query_maker.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.3/midiscripter/resources/icon.ico` & `midiscripter-0.4/midiscripter/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `midiscripter-0.3/midiscripter/resources/icon.svg` & `midiscripter-0.4/midiscripter/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `midiscripter-0.3/LICENSE` & `midiscripter-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `midiscripter-0.3/README.md` & `midiscripter-0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,84 @@
-# MIDI Scripter
+# <img src="docs/icon.svg" width="24"/> MIDI Scripter
 
-MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound
-Control (OSC) input and output with only a few lines of Python code.
+MIDI Scripter is a framework filtering, modifying, routing and any other
+scripting for MIDI, Open Sound Control (OSC), keyboard and mouse input and
+output with Python.
 
-MIDI Scripter listens to selected input ports and feed incoming messages to
+MIDI Scripter listens to the input ports and feeds incoming messages to
 subscribed callables (functions, methods, etc.). These callables or any
-other Python code can send modified or brand-new messages with
-output ports. MIDI Scripter can act as a proxy to filter and transform and
-convert the input.
-
-MIDI Scripter included customizable GUI that provides messages logging,
-"ready to paste" port and message declarations and one line of code widgets for
-monitoring / controlling scripts.
+other Python code can send modified or created messages with output ports. 
+MIDI Scripter can act as a proxy to filter, transform and convert the input.
+
+MIDI Scripter includes customizable GUI for message logging, coding
+assistance and GUI controls and indicators to use in scripts.
 
 An octave transposer with GUI controls in 10 lines of code:
 
 ``` python
 from midiscripter import *
 
 midi_keyboard = MidiIn('MIDI Keyboard')  # GUI will provide you with port names
-proxy_output = MidiOut('To DAW')  # using virtual port for output
+proxy_output = MidiOut('To DAW')  # using virtual proxy port for output
 
 # GUI control in a single line
 octave_selector = GuiButtonSelectorH(('-2', '-1', '0', '+1', '+2'), select='0')
 
 @midi_keyboard.subscribe  # decorated function will receive port's messages
 def transpose(msg: MidiMsg) -> None:
 	if msg.type == MidiType.NOTE_ON or msg.type == MidiType.NOTE_OFF:  # filter
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
-		proxy_output.send(msg)  # route
+	proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
 ![Screenshot after some widget arrangement](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
 
 [You can find more examples here.](https://github.com/Maboroshy/midi-scripter/tree/master/examples)
 
-[Scripting guide and API documentation available.](https://maboroshy.github.io/midi-scripter)
+[Overview and API documentation available.](https://maboroshy.github.io/midi-scripter)
+
+The average measured roundtrip latency for the script above is less than 0.25 
+milliseconds.
 
 Currently MIDI Scripter is at "beta" development stage. It's fully
-functional but needs more user feedback. It works on Windows and Linx and
+functional but needs more user feedback. It works on Windows and Linux and
 should work on macOS.
 
 ## What it can do
 
-For writing Python code:
+The basics:
 
-- Prepare MIDI, OSC and keyboard inputs and outputs with a single line,
-  without boilerplate code.
-- Feed input messages to functions or any callables by "decorating" them.
-- Work with common message objects instead of raw data different for each port
-  type.
-- Send MIDI, OSC and keyboard output messages.
-- Create GUI widgets with one line and arrange them with mouse on your script's
-  dashboard.
+- Receive MIDI, OSC, keyboard and mouse input messages.
+- Filter, modify and do anything Python can with the messages.
+- Send out modified or generated MIDI, OSC, keyboard and mouse messages.
 
-For live performance setups:
+For performance MIDI setups:
 
-- Make extra layers to multiply MIDI controls.
+- Make extra banks and layers to multiply MIDI controls.
 - Organize mappings into sets / scenes with GUI dashboard.
 - Make an extra overlay mappings on top of MIDI controller's DAW integration by
   using proxies.
-- Create and map complex macros.
-
-For MIDI related apps:
-
-- Make custom sequencers or MIDI output generators.
-- Make basic music training GUI applications based on MIDI input.
 
 For software control and automation:
 
+- Map or convert the messages to each other with any conditions and logic.
 - Use MIDI controllers or keyboard shortcuts to run any Python code.
-- Use keyboard macros to control apps.
+- Use keyboard and mouse macros.
+
+For writing MIDI related Python code:
+
+- Prepare MIDI, OSC keyboard and mouse inputs and outputs with a single line,
+  without boilerplate code.
+- Feed input messages to functions or any callables by decorators.
+- Work with message objects instead of raw data different for each input type.
+- Create GUI widgets with a single line and arrange them with mouse.
+- Write basic MIDI related GUI applications with very little Python code.
 
 ## Installation
 
 1. Install [Python 3.11+](https://www.python.org/downloads/) including pip.
 2. Run `pip install midiscripter`.
 
 Extra steps for Windows:
@@ -85,19 +86,20 @@
 1. Enable `Add python .exe to PATH` option in Python installer.
 2. Install [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html)
    and set required virtual MIDI ports inside it.
 
 ## Quick Start
 
 1. Paste [script template](examples/script_template.py) to Python IDE or plain
-   text editor. IDE is greatly recommended.
-2. Run unaltered template script from IDE or by `python` command to open GUI for
-   more info on available ports and their input.
-3. Turn on available ports' checkboxes to enable them, and watch the log for
+   text editor. IDE is recommended.
+2. Run template script as-is from IDE or by `python your_script.py` command to
+   open GUI for more info on available ports and incoming input.
+3. Turn on available ports' checkboxes to enable them, watch the log for
    input messages.
-4. Click on port names and messages to copy their declarations to the clipboard.
-   Paste the declarations to your script.
-5. Write the functions you need. Subscribe them to input messages with
-   `@input_port.subscribe` decorator. Use `log('messages')` for debugging.
-   Use `output_port.send(msg)` to send modified or created messages from a
-   function.
+4. Click on port names and messages in log to copy their declarations to the
+   clipboard. Paste the declarations to your script.
+5. Modify the template function to make it do what you want.
+   Use `log('messages')` for debugging.
 6. Restart the script from GUI to check how in works.
+7. Write more complex scripts. Use more inputs, outputs and functions
+   (callables). Subscribe callables to input messages with
+   `@input_port.subscribe` decorator.
```

### Comparing `midiscripter-0.3/pyproject.toml` & `midiscripter-0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'midiscripter'
-version = '0.3'
+version = '0.4'
 description = 'Framework for scripting MIDI, keyboard and Open Sound Control input and output'
 readme = 'README.md'
 requires-python = '>=3.11'
 license = {file = "LICENSE"}
 keywords = ['MIDI', 'OSC', 'script', 'automation', 'input']
 authors = [{name = 'Maboroshy'}]
 classifiers = [
```

### Comparing `midiscripter-0.3/PKG-INFO` & `midiscripter-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: midiscripter
-Version: 0.3
+Version: 0.4
 Summary: Framework for scripting MIDI, keyboard and Open Sound Control input and output
 Project-URL: Documentation, https://maboroshy.github.io/midi-scripter
 Project-URL: Issues, https://github.com/Maboroshy/midi-scripter/issues
 Project-URL: Source, https://github.com/Maboroshy/midi-scripter
 Author: Maboroshy
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -192,90 +192,91 @@
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: griffe-inherited-docstrings; extra == 'doc'
 Requires-Dist: mkdocs-material; extra == 'doc'
 Requires-Dist: mkdocstrings; extra == 'doc'
 Description-Content-Type: text/markdown
 
-# MIDI Scripter
+# <img src="docs/icon.svg" width="24"/> MIDI Scripter
 
-MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound
-Control (OSC) input and output with only a few lines of Python code.
+MIDI Scripter is a framework filtering, modifying, routing and any other
+scripting for MIDI, Open Sound Control (OSC), keyboard and mouse input and
+output with Python.
 
-MIDI Scripter listens to selected input ports and feed incoming messages to
+MIDI Scripter listens to the input ports and feeds incoming messages to
 subscribed callables (functions, methods, etc.). These callables or any
-other Python code can send modified or brand-new messages with
-output ports. MIDI Scripter can act as a proxy to filter and transform and
-convert the input.
-
-MIDI Scripter included customizable GUI that provides messages logging,
-"ready to paste" port and message declarations and one line of code widgets for
-monitoring / controlling scripts.
+other Python code can send modified or created messages with output ports. 
+MIDI Scripter can act as a proxy to filter, transform and convert the input.
+
+MIDI Scripter includes customizable GUI for message logging, coding
+assistance and GUI controls and indicators to use in scripts.
 
 An octave transposer with GUI controls in 10 lines of code:
 
 ``` python
 from midiscripter import *
 
 midi_keyboard = MidiIn('MIDI Keyboard')  # GUI will provide you with port names
-proxy_output = MidiOut('To DAW')  # using virtual port for output
+proxy_output = MidiOut('To DAW')  # using virtual proxy port for output
 
 # GUI control in a single line
 octave_selector = GuiButtonSelectorH(('-2', '-1', '0', '+1', '+2'), select='0')
 
 @midi_keyboard.subscribe  # decorated function will receive port's messages
 def transpose(msg: MidiMsg) -> None:
 	if msg.type == MidiType.NOTE_ON or msg.type == MidiType.NOTE_OFF:  # filter
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
-		proxy_output.send(msg)  # route
+	proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
 ![Screenshot after some widget arrangement](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
 
 [You can find more examples here.](https://github.com/Maboroshy/midi-scripter/tree/master/examples)
 
-[Scripting guide and API documentation available.](https://maboroshy.github.io/midi-scripter)
+[Overview and API documentation available.](https://maboroshy.github.io/midi-scripter)
+
+The average measured roundtrip latency for the script above is less than 0.25 
+milliseconds.
 
 Currently MIDI Scripter is at "beta" development stage. It's fully
-functional but needs more user feedback. It works on Windows and Linx and
+functional but needs more user feedback. It works on Windows and Linux and
 should work on macOS.
 
 ## What it can do
 
-For writing Python code:
+The basics:
 
-- Prepare MIDI, OSC and keyboard inputs and outputs with a single line,
-  without boilerplate code.
-- Feed input messages to functions or any callables by "decorating" them.
-- Work with common message objects instead of raw data different for each port
-  type.
-- Send MIDI, OSC and keyboard output messages.
-- Create GUI widgets with one line and arrange them with mouse on your script's
-  dashboard.
+- Receive MIDI, OSC, keyboard and mouse input messages.
+- Filter, modify and do anything Python can with the messages.
+- Send out modified or generated MIDI, OSC, keyboard and mouse messages.
 
-For live performance setups:
+For performance MIDI setups:
 
-- Make extra layers to multiply MIDI controls.
+- Make extra banks and layers to multiply MIDI controls.
 - Organize mappings into sets / scenes with GUI dashboard.
 - Make an extra overlay mappings on top of MIDI controller's DAW integration by
   using proxies.
-- Create and map complex macros.
-
-For MIDI related apps:
-
-- Make custom sequencers or MIDI output generators.
-- Make basic music training GUI applications based on MIDI input.
 
 For software control and automation:
 
+- Map or convert the messages to each other with any conditions and logic.
 - Use MIDI controllers or keyboard shortcuts to run any Python code.
-- Use keyboard macros to control apps.
+- Use keyboard and mouse macros.
+
+For writing MIDI related Python code:
+
+- Prepare MIDI, OSC keyboard and mouse inputs and outputs with a single line,
+  without boilerplate code.
+- Feed input messages to functions or any callables by decorators.
+- Work with message objects instead of raw data different for each input type.
+- Create GUI widgets with a single line and arrange them with mouse.
+- Write basic MIDI related GUI applications with very little Python code.
 
 ## Installation
 
 1. Install [Python 3.11+](https://www.python.org/downloads/) including pip.
 2. Run `pip install midiscripter`.
 
 Extra steps for Windows:
@@ -283,19 +284,20 @@
 1. Enable `Add python .exe to PATH` option in Python installer.
 2. Install [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html)
    and set required virtual MIDI ports inside it.
 
 ## Quick Start
 
 1. Paste [script template](examples/script_template.py) to Python IDE or plain
-   text editor. IDE is greatly recommended.
-2. Run unaltered template script from IDE or by `python` command to open GUI for
-   more info on available ports and their input.
-3. Turn on available ports' checkboxes to enable them, and watch the log for
+   text editor. IDE is recommended.
+2. Run template script as-is from IDE or by `python your_script.py` command to
+   open GUI for more info on available ports and incoming input.
+3. Turn on available ports' checkboxes to enable them, watch the log for
    input messages.
-4. Click on port names and messages to copy their declarations to the clipboard.
-   Paste the declarations to your script.
-5. Write the functions you need. Subscribe them to input messages with
-   `@input_port.subscribe` decorator. Use `log('messages')` for debugging.
-   Use `output_port.send(msg)` to send modified or created messages from a
-   function.
+4. Click on port names and messages in log to copy their declarations to the
+   clipboard. Paste the declarations to your script.
+5. Modify the template function to make it do what you want.
+   Use `log('messages')` for debugging.
 6. Restart the script from GUI to check how in works.
+7. Write more complex scripts. Use more inputs, outputs and functions
+   (callables). Subscribe callables to input messages with
+   `@input_port.subscribe` decorator.
```

