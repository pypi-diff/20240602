# Comparing `tmp/pynboard-0.0.2.tar.gz` & `tmp/pynboard-0.0.3.tar.gz`

## Comparing `pynboard-0.0.2.tar` & `pynboard-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pynboard-0.0.2/requirements.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/pynboard.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/actions.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/core.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/html_buffer.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pynboard-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pynboard-0.0.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynboard-0.0.2/README.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pynboard-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pynboard-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pynboard-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/pynboard.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pynboard-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pynboard-0.0.3/examples/scratch_00.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/__init__.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/actions.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/core.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/html_buffer.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pynboard-0.0.3/src/pynboard/utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pynboard-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pynboard-0.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynboard-0.0.3/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pynboard-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pynboard-0.0.3/PKG-INFO
```

### Comparing `pynboard-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `pynboard-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.2/src/pynboard/__init__.py` & `pynboard-0.0.3/src/pynboard/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
-from core import Board
-from utils import create_default_board
+from pynboard.core import Board
+from pynboard.utils import create_default_board
 
 _active_board: Optional[Board] = None
 
 __all__ = [
     "append",
     "render",
     "render_obj",
```

### Comparing `pynboard-0.0.2/src/pynboard/actions.py` & `pynboard-0.0.3/src/pynboard/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tempfile
 import webbrowser
 from pathlib import Path
 from typing import Optional
 
-from core import Buffer
-from html_buffer import HtmlBuffer
+from pynboard.core import Buffer
+from pynboard.html_buffer import HtmlBuffer
 
 
 def _gen_tempfile(suffix: Optional[str] = None):
     temp_dir = Path.home() / "tmp" / "pynboard"
     if not temp_dir.exists():
         temp_dir.mkdir(parents=True)
```

### Comparing `pynboard-0.0.2/src/pynboard/core.py` & `pynboard-0.0.3/src/pynboard/core.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.2/src/pynboard/html_buffer.py` & `pynboard-0.0.3/src/pynboard/html_buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 import warnings
-from typing import Iterable
 from typing import List
 from typing import Optional
-from typing import Protocol
-
-import numpy as np
-import pandas as pd
-
-from pathlib import Path
-import warnings
-import webbrowser
 
 import numpy as np
 import pandas as pd
 import pandas.io.formats.style
-import plotly.io as pio
 import plotly.graph_objects as go
-
-import tempfile
+import plotly.io as pio
 
 
 class HtmlBuffer:
     _buffer_data: List[str]
     _rendered: Optional[str] = None
 
     def __init__(self):
@@ -43,17 +32,17 @@
         self._rendered = None
 
 
 # region html conversion
 
 def _obj_to_html(obj, **kwargs) -> str:
     if isinstance(obj, (list, tuple)):
-        out_html = _obj_grid_to_html(obj)
+        out_html = _obj_grid_to_html(obj, **kwargs)
     else:
-        out_html = _obj_single_to_html(obj)
+        out_html = _obj_single_to_html(obj, **kwargs)
     return out_html
 
 
 def _obj_single_to_html(obj, **kwargs):
     if isinstance(obj, go.Figure):
         html0 = pio.to_html(obj, full_html=False)
     elif isinstance(obj, pandas.io.formats.style.Styler):
```

### Comparing `pynboard-0.0.2/LICENSE` & `pynboard-0.0.3/LICENSE`

 * *Files identical despite different names*

