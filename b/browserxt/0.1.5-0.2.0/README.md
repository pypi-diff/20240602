# Comparing `tmp/browserxt-0.1.5.tar.gz` & `tmp/browserxt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserxt-0.1.5.tar", last modified: Sat Jun  1 13:40:06 2024, max compression
+gzip compressed data, was "browserxt-0.2.0.tar", last modified: Sun Jun  2 17:43:35 2024, max compression
```

## Comparing `browserxt-0.1.5.tar` & `browserxt-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    16725 2024-06-01 13:39:50.584096 browserxt-0.1.5/LICENSE
--rw-r--r--   0        0        0     3035 2024-06-01 13:39:50.584096 browserxt-0.1.5/README.md
--rw-r--r--   0        0        0     2296 2024-06-01 13:40:06.796067 browserxt-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       72 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/__init__.py
--rwxr-xr-x   0        0        0     4978 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/browser.py
--rw-r--r--   0        0        0     1324 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/cli.py
--rw-r--r--   0        0        0        0 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/py.typed
--rw-r--r--   0        0        0     5681 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/scripts/detect_browsers.ps1
--rw-r--r--   0        0        0     1024 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/settings.py
--rwxr-xr-x   0        0        0    11178 2024-06-01 13:39:50.592096 browserxt-0.1.5/src/browserxt/utils.py
--rw-r--r--   0        0        0       25 2024-06-01 13:39:50.592096 browserxt-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      448 2024-06-01 13:39:50.592096 browserxt-0.1.5/tests/cli_test.py
--rw-r--r--   0        0        0      136 2024-06-01 13:39:50.592096 browserxt-0.1.5/tests/pkg_test.py
--rw-r--r--   0        0        0      338 2024-06-01 13:39:50.592096 browserxt-0.1.5/tests/settings_test.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 browserxt-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-06-02 17:43:20.596677 browserxt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3035 2024-06-02 17:43:20.596677 browserxt-0.2.0/README.md
+-rw-r--r--   0        0        0     2032 2024-06-02 17:43:35.592883 browserxt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/__init__.py
+-rwxr-xr-x   0        0        0     5168 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/browser.py
+-rw-r--r--   0        0        0     2894 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/cli.py
+-rwxr-xr-x   0        0        0     4427 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/constants.py
+-rwxr-xr-x   0        0        0     2220 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/globals.py
+-rwxr-xr-x   0        0        0     2104 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/profiles.py
+-rw-r--r--   0        0        0        0 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/py.typed
+-rw-r--r--   0        0        0     1024 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/settings.py
+-rwxr-xr-x   0        0        0    11176 2024-06-02 17:43:20.600677 browserxt-0.2.0/src/browserxt/utils.py
+-rw-r--r--   0        0        0       25 2024-06-02 17:43:20.600677 browserxt-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      448 2024-06-02 17:43:20.600677 browserxt-0.2.0/tests/cli_test.py
+-rw-r--r--   0        0        0      136 2024-06-02 17:43:20.600677 browserxt-0.2.0/tests/pkg_test.py
+-rw-r--r--   0        0        0      338 2024-06-02 17:43:20.600677 browserxt-0.2.0/tests/settings_test.py
+-rw-r--r--   0        0        0     3576 1970-01-01 00:00:00.000000 browserxt-0.2.0/PKG-INFO
```

### Comparing `browserxt-0.1.5/LICENSE` & `browserxt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.5/README.md` & `browserxt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.5/pyproject.toml` & `browserxt-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 [build-system]
 build-backend = "pdm.backend"
 requires = [
     "pdm-backend==2.3.0",
 ]
 
 [project]
-authors = [
-    { email = "nsyntych@punkops.dev", name = "Nick Syntychakis" },
-]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.11",
-]
 dependencies = [
     "pydantic-settings",
     "typer[all]",
-    "wslPath",
 ]
 description = "A simple extensible browser runner"
 dynamic = []
 keywords = [
     "copier-template",
     "full-development-lifecycle",
     "project-template",
     "serious-scaffold",
+    "winreg; sys_platform == 'win32'",
 ]
 name = "browserxt"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.1.5"
+version = "0.2.0"
 
 [project.license]
 text = "MPL-2.0"
 
 [project.scripts]
 browserxt = "browserxt.cli:app"
 
@@ -97,39 +88,20 @@
 addopts = "-l -s --durations=0"
 log_cli = true
 log_cli_level = "info"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 log_format = "%(asctime)s %(levelname)s %(message)s"
 minversion = "6.0"
 
-[tool.ruff]
-fix = true
-src = [
-    "src",
-]
-
-[tool.ruff.lint]
-select = [
-    "B",
-    "D",
-    "E",
-    "F",
-    "I",
-    "RUF100",
-    "S",
-    "SIM",
-    "UP",
-    "W",
-]
-
-[tool.ruff.lint.per-file-ignores]
-"tests/*" = [
-    "S101",
-]
-
-[tool.ruff.lint.pydocstyle]
-convention = "google"
-
 [tool.tomlsort]
+authors = [
+    { email = "nsyntych@punkops.dev", name = "Nick Syntychakis" },
+]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.11",
+]
 all = true
 in_place = true
 trailing_comma_inline_array = true
```

### Comparing `browserxt-0.1.5/src/browserxt/browser.py` & `browserxt-0.2.0/src/browserxt/browser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import os
 import subprocess
 
-from browserxt.utils import is_running_in_wsl, nt_to_wsl_path, detect_nt, detect_posix
+from browserxt.utils import nt_to_wsl_path, sort_tryoder, detect_standard_browsers
 
-# Default order for browsers to check, chosen according to popularity (kind of)
-DEFAULT_SORTING = [
-    "default",
-    "chrome",
-    "chromium",
-    "firefox",
-    "brave",
-    "opera",
-    "vivaldi",
-    "edge",
-    "safari",
-    "unknown",
-]
+from browserxt.profiles import (
+    get_chromium_profile_options,
+    get_firefox_profile_options,
+)
+
+from browserxt.globals import GLOBALS
 
 
 class ExtensibleBrowser:
     def __init__(
-        self, name: str, path: str, options: list[str] = [], family: str = "unknown"
+        self,
+        name: str,
+        path: str,
+        options: list[str] = [],
+        family: str = "unknown",
+        profile: str = "",
+        user_data_path: str = "",
     ) -> None:
         self.name = name
         self.family = family
         self.path = path
-        self.set_options(options)
+        self.set_options(options.copy())
+        if profile != "":
+            self.set_profile_options(profile, user_data_path)
 
     def set_options(self, options: list[str]) -> None:
         self.options = options
 
+    # Dummy method to be overridden by subclasses
+    def set_profile_options(self, name: str, user_data_path: str = "") -> None:
+        pass
+
+    def is_running_in_wsl(self) -> bool:
+        return GLOBALS.IS_WSL and not self.path.startswith("/mnt")
+
     def open(self, url: str) -> bool:
         cmdline = [self.path] + self.options + [url]
         try:
             if os.name == "nt":
                 p = subprocess.Popen(
                     cmdline, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT
                 )
@@ -46,26 +54,46 @@
                 )
             return True
         except OSError:
             return False
 
 
 class ChromiumBrowser(ExtensibleBrowser):
-    def __init__(self, name: str, path: str, options: list[str] = []) -> None:
-        super().__init__(name, path, options, "chromium")
+    def __init__(
+        self,
+        name: str,
+        path: str,
+        options: list[str] = [],
+        profile: str = "",
+        user_data_path: str = "",
+    ) -> None:
+        super().__init__(name, path, options, "chromium", profile, user_data_path)
+
+    def set_profile_options(self, name: str, user_data_path: str = "") -> None:
+        self.options += get_chromium_profile_options(name, user_data_path)
 
     def set_options(self, options: list[str]) -> None:
         super().set_options(options)
         if self.name == "edge":
             self.options = [arg.replace("incognito", "inprivate") for arg in options]
 
 
 class FirefoxBrowser(ExtensibleBrowser):
-    def __init__(self, name: str, path: str, options: list[str] = []) -> None:
-        super().__init__(name, path, options, "firefox")
+    def __init__(
+        self,
+        name: str,
+        path: str,
+        options: list[str] = [],
+        profile: str = "",
+        user_data_path: str = "",
+    ) -> None:
+        super().__init__(name, path, options, "firefox", profile, user_data_path)
+
+    def set_profile_options(self, name: str, user_data_path: str = "") -> None:
+        self.options += get_firefox_profile_options(name, user_data_path)
 
 
 class UnknownBrowser(ExtensibleBrowser):
     def __init__(self, name: str, path: str, options: list[str] = []) -> None:
         super().__init__(name, path, options)
 
 
@@ -80,48 +108,43 @@
 
 
 class Browser:
     def __init__(
         self,
         prefered: list[str] = [],
         options: list[str] = [],
-        wsl: bool = False,
         ignore_default: bool = False,
+        profile: str = "",
+        user_data_path: str = "",
     ) -> None:
         self.options = options.copy()
         self._platform = os.name
-        self._wsl = wsl
         self._ignore_default = ignore_default
         self._prefered = prefered.copy()
         self._tryorder: list[str] = []
         self._browsers: dict[str, ExtensibleBrowser] = {}
+        self._profile = profile
+        self._user_data_path = user_data_path
         self.detect_browsers()
-        self._fix_tryoder()
+        self._tryorder = sort_tryoder(self._tryorder)
 
     def detect_browsers(self) -> None:
-        if self._platform == "nt" or (is_running_in_wsl() and not self._wsl):
-            default, browsers = detect_nt()
-            for name, browser in browsers.items():
-                path = browser.get("path", "")
-                family = browser.get("family", "")
-                if is_running_in_wsl():
-                    path = nt_to_wsl_path(path)
-                self.register(name, get_browser_class(family)(name, path, self.options))
-            default_instance = self._browsers.get(default, None)
-            if default_instance and not self._ignore_default:
-                self.register("default", default_instance)
-        else:
-            default, browsers = detect_posix()
-            for name, browser in browsers.items():
-                path = browser.get("path", "")
-                family = browser.get("family", "")
-                self.register(name, get_browser_class(family)(name, path, self.options))
-            default_instance = self._browsers.get(default, None)
-            if default_instance and not self._ignore_default:
-                self.register("default", default_instance)
+        default, browsers = detect_standard_browsers()
+        for name, browser in browsers.items():
+            path = browser.get("path", "")
+            family = browser.get("family", "")
+            self.register(
+                name,
+                get_browser_class(family)(
+                    name, path, self.options, self._profile, self._user_data_path
+                ),
+            )
+        default_instance = self._browsers.get(default, None)
+        if default_instance and not self._ignore_default:
+            self.register("default", default_instance)
 
     def open(self, url: str, using: str = "") -> bool:
         browser = self.get(using)
         if browser:
             return browser.open(url)
         return False
 
@@ -138,17 +161,7 @@
 
     def register(self, name: str, instance: ExtensibleBrowser) -> None:
         self._browsers[name] = instance
         if name == "default":
             self._tryorder.insert(0, name)
         else:
             self._tryorder.append(name)
-
-    def _fix_tryoder(self) -> None:
-        self._tryorder = sorted(
-            self._tryorder,
-            key=lambda x: (
-                DEFAULT_SORTING.index(x)
-                if x in DEFAULT_SORTING
-                else len(DEFAULT_SORTING)
-            ),
-        )
```

### Comparing `browserxt-0.1.5/src/browserxt/settings.py` & `browserxt-0.2.0/src/browserxt/settings.py`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.5/src/browserxt/utils.py` & `browserxt-0.2.0/src/browserxt/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,372 +1,345 @@
+# mypy: disable-error-code = attr-defined
 import os
-import sys
 import json
 import shutil
-import platform
 import subprocess
 import configparser
+from browserxt.globals import GLOBALS
+from browserxt.constants import (
+    DEFAULT_SORTING,
+    DESKTOP_DIRS,
+    NT_BROWSERS,
+    POSIX_BROWSERS,
+)
 
-POSIX_BROWSERS = {
-    "chrome": {
-        "paths": [
-            "google-chrome",
-            "google-chrome-stable",
-            "chrome",
-            "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
-        ],
-        "family": "chromium",
-    },
-    "firefox": {
-        "paths": [
-            "firefox",
-            "firefox-bin",
-            "/Applications/Firefox.app/Contents/MacOS/firefox",
-        ],
-        "family": "firefox",
-    },
-    "chromium": {
-        "paths": [
-            "chromium",
-            "chromium-browser",
-            "/Applications/Chromium.app/Contents/MacOS/Chromium",
-        ],
-        "family": "chromium",
-    },
-    "opera": {
-        "paths": ["opera", "/Applications/Opera.app/Contents/MacOS/Opera"],
-        "family": "chromium",
-    },
-    "brave": {
-        "paths": [
-            "brave",
-            "brave-browser",
-            "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser",
-        ],
-        "family": "chromium",
-    },
-    "edge": {
-        "paths": [
-            "microsoft-edge",
-            "microsoft-edge-stable",
-            "edge",
-            "msedge",
-            "/Applications/Microsoft Edge.app/Contents/MacOS/Microsoft Edge",
-        ],
-        "family": "chromium",
-    },
-    "safari": {
-        "paths": ["safari", "/Applications/Safari.app/Contents/MacOS/Safari"],
-        "family": "safari",
-    },
-    "vivaldi": {
-        "paths": ["vivaldi", "/Applications/Vivaldi.app/Contents/MacOS/Vivaldi"],
-        "family": "chromium",
-    },
-}
 
+def sort_tryoder(tryorder: list[str]) -> list[str]:
+    return sorted(
+        tryorder.copy(),
+        key=lambda x: (
+            DEFAULT_SORTING.index(x) if x in DEFAULT_SORTING else len(DEFAULT_SORTING)
+        ),
+    )
 
-def get_posix_default_browser() -> str | None:
-    # Check xdg-settings (Linux)
-    try:
-        result = subprocess.run(
-            ["xdg-settings", "get", "default-web-browser"],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            return result.stdout.strip()
-    except FileNotFoundError:
-        pass
-
-    # Check macOS defaults
-    try:
-        result = subprocess.run(
-            [
-                "defaults",
-                "read",
-                "com.apple.LaunchServices/com.apple.launchservices.secure",
-                "LSHandlers",
-            ],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            output = result.stdout.strip()
-            # Implement parsing to find the default browser if necessary
-            return output
-    except FileNotFoundError:
-        pass
-
-    # Check GNOME settings
-    try:
-        result = subprocess.run(
-            [
-                "gsettings",
-                "get",
-                "org.gnome.system.default-applications.browser",
-                "exec",
-            ],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            return result.stdout.strip().strip("'")
-    except FileNotFoundError:
-        pass
-
-    # Check KDE settings
-    try:
-        result = subprocess.run(
-            ["xdg-mime", "query", "default", "x-scheme-handler/http"],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            return result.stdout.strip()
-    except FileNotFoundError:
-        pass
-
-    # Check XFCE settings
-    try:
-        result = subprocess.run(
-            [
-                "xfconf-query",
-                "--channel",
-                "xfce4-session",
-                "--property",
-                "/sessions/Failsafe/Client0_Command",
-            ],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            return result.stdout.strip()
-    except FileNotFoundError:
-        pass
-
-    # Check LXDE settings
-    try:
-        lxde_config = os.path.expanduser("~/.config/lxsession/LXDE/autostart")
-        if os.path.exists(lxde_config):
-            with open(lxde_config, "r") as file:
-                for line in file:
-                    if line.startswith("@"):
-                        return line.strip("@").split()[0]
-    except Exception as e:
-        pass
-
-    # Check Cinnamon settings
-    try:
-        result = subprocess.run(
-            [
-                "gsettings",
-                "get",
-                "org.cinnamon.desktop.default-applications.browser",
-                "exec",
-            ],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            return result.stdout.strip().strip("'")
-    except FileNotFoundError:
-        pass
-
-    # Check MATE settings
-    try:
-        result = subprocess.run(
-            ["gsettings", "get", "org.mate.applications-browser", "exec"],
-            capture_output=True,
-            text=True,
-        )
-        if result.returncode == 0:
-            return result.stdout.strip().strip("'")
-    except FileNotFoundError:
-        pass
-
-    # Method 10: Check i3 settings
-    try:
-        i3_config = os.path.expanduser("~/.config/i3/config")
-        if os.path.exists(i3_config):
-            with open(i3_config, "r") as file:
-                for line in file:
-                    if "browser" in line:
-                        return line.split()[-1].strip()
-    except Exception as e:
-        pass
-
-    # Method 11: Check Sway settings
-    try:
-        sway_config = os.path.expanduser("~/.config/sway/config")
-        if os.path.exists(sway_config):
-            with open(sway_config, "r") as file:
-                for line in file:
-                    if "browser" in line:
-                        return line.split()[-1].strip()
-    except Exception as e:
-        pass
-
-    # Method 12: Check XMonad settings
-    try:
-        xmonad_config = os.path.expanduser("~/.xmonad/xmonad.hs")
-        if os.path.exists(xmonad_config):
-            with open(xmonad_config, "r") as file:
-                for line in file:
-                    if "browser" in line:
-                        return line.split()[-1].strip()
-    except Exception as e:
-        pass
 
+def get_nt_default_browser() -> str | None:
+    if GLOBALS.IS_WSL:
+        try:
+            result = subprocess.run(
+                [
+                    "cmd.exe",
+                    "/c",
+                    "reg",
+                    "query",
+                    "HKEY_CURRENT_USER\\Software\\Microsoft\\Windows\\Shell\\Associations\\UrlAssociations\\http\\UserChoice",
+                    "/v",
+                    "Progid",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if result.returncode == 0:
+                output = result.stdout.strip()
+                if "Progid" in output:
+                    return output.split()[-1]
+        except FileNotFoundError:
+            pass
+        return None
+    elif GLOBALS.IS_WINDOWS:
+        import winreg
+
+        try:
+            with winreg.OpenKey(
+                winreg.HKEY_CURRENT_USER,
+                r"Software\Microsoft\Windows\Shell\Associations\UrlAssociations\http\UserChoice",
+            ) as key:
+                prog_id = str(winreg.QueryValueEx(key, "Progid")[0])
+                return prog_id
+        except FileNotFoundError:
+            pass
+        except Exception:
+            pass
     return None
 
 
-def get_binary_path_from_desktop_entry(browser: str | None) -> str | None:
-    if not browser:
+def _posix_default_browser() -> str | None:
+    # if system is macOS
+    if GLOBALS.IS_MACOS:
+        # Check macOS defaults
+        try:
+            result = subprocess.run(
+                [
+                    "defaults",
+                    "read",
+                    "com.apple.LaunchServices/com.apple.launchservices.secure",
+                    "LSHandlers",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if result.returncode == 0:
+                output = result.stdout.strip()
+                return output
+        except FileNotFoundError:
+            pass
         return None
-    # If the browser is not a .desktop file, return it as is
-    if not browser.endswith(".desktop"):
-        return browser
 
-    # Common directories for .desktop files
-    desktop_dirs = [
-        "/usr/share/applications/",
-        "/usr/local/share/applications/",
-        os.path.expanduser("~/.local/share/applications/"),
-        "/etc/profiles/per-user/$USER/share/applications/",
-        "/run/current-system/sw/share/applications/",
-        os.path.expanduser("~/.nix-profile/share/applications/"),
-    ]
-
-    for directory in desktop_dirs:
-        desktop_file_path = os.path.join(directory, browser)
-        if os.path.exists(desktop_file_path):
-            config = configparser.ConfigParser(interpolation=None)
-            config.read(desktop_file_path)
-
-            # The desktop file format has sections like [Desktop Entry]
-            if "Desktop Entry" in config and "Exec" in config["Desktop Entry"]:
-                exec_command = config["Desktop Entry"]["Exec"]
-
-                # Extract the binary path from the exec command
-                binary_path = exec_command.split()[0]
-
-                # Resolve to full path if binary is in PATH
-                binary_full_path = shutil.which(binary_path)
-                if binary_full_path:
-                    return binary_full_path
-                else:
-                    return binary_path
+    # if system is linux or BSD
+    if GLOBALS.IS_UNIX:
+        # Check xdg-settings
+        try:
+            result = subprocess.run(
+                ["xdg-settings", "get", "default-web-browser"],
+                capture_output=True,
+                text=True,
+            )
+            if result.returncode == 0:
+                default_browser = result.stdout.strip()
+        except FileNotFoundError:
+            pass
+
+        # Check GNOME settings
+        try:
+            settings = subprocess.run(
+                [
+                    "gsettings",
+                    "get",
+                    "org.gnome.desktop.default-applications.web",
+                    "schemes",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if settings.returncode == 0:
+                default_browser = settings.stdout.strip().strip("'")
+                if default_browser:
+                    return default_browser
+        except FileNotFoundError:
+            pass
+
+        try:
+            settings = subprocess.run(
+                [
+                    "gsettings",
+                    "get",
+                    "org.gnome.system.default-applications.browser",
+                    "exec",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if settings.returncode == 0:
+                default_browser = settings.stdout.strip().strip("'")
+                if default_browser:
+                    return default_browser
+        except FileNotFoundError:
+            pass
+
+        # Check KDE settings
+        try:
+            settings = subprocess.run(
+                [
+                    "kreadconfig5",
+                    "--file",
+                    "kdeglobals",
+                    "--group",
+                    "General",
+                    "--key",
+                    "Browser",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if settings.returncode == 0:
+                default_browser = settings.stdout.strip().strip("'")
+                if default_browser:
+                    return default_browser
+        except FileNotFoundError:
+            pass
+
+        # Check XFCE settings
+        try:
+            settings = subprocess.run(
+                [
+                    "xfconf-query",
+                    "-c",
+                    "xfce4-session",
+                    "-p",
+                    "/sessions/Failsafe/Client0_Command",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if settings.returncode == 0:
+                default_browser = settings.stdout.strip().strip("'")
+                if default_browser:
+                    return default_browser
+        except FileNotFoundError:
+            pass
+
+        # Check LXDE settings
+        try:
+            lxde_config = os.path.expanduser("~/.config/lxsession/LXDE/autostart")
+            if os.path.exists(lxde_config):
+                with open(lxde_config, "r") as file:
+                    for line in file:
+                        if line.startswith("@"):
+                            return line.strip("@").split()[0]
+        except Exception:
+            pass
+
+        # Check Cinnamon settings
+        try:
+            settings = subprocess.run(
+                [
+                    "gsettings",
+                    "get",
+                    "org.cinnamon.desktop.default-applications.browser",
+                    "exec",
+                ],
+                capture_output=True,
+                text=True,
+            )
+            if settings.returncode == 0:
+                default_browser = settings.stdout.strip().strip("'")
+                if default_browser:
+                    return default_browser
+        except FileNotFoundError:
+            pass
+
+        # Check MATE settings
+        try:
+            settings = subprocess.run(
+                ["gsettings", "get", "org.mate.applications-browser", "exec"],
+                capture_output=True,
+                text=True,
+            )
+            if settings.returncode == 0:
+                default_browser = settings.stdout.strip().strip("'")
+                if default_browser:
+                    return default_browser
+        except FileNotFoundError:
+            pass
+
+        # Check i3 settings
+        try:
+            i3_config = os.path.expanduser("~/.config/i3/config")
+            if os.path.exists(i3_config):
+                with open(i3_config, "r") as file:
+                    for line in file:
+                        if "browser" in line:
+                            return line.split()[-1].strip()
+        except Exception:
+            pass
+
+        # Check Sway settings
+        try:
+            sway_config = os.path.expanduser("~/.config/sway/config")
+            if os.path.exists(sway_config):
+                with open(sway_config, "r") as file:
+                    for line in file:
+                        if "browser" in line:
+                            return line.split()[-1].strip()
+        except Exception:
+            pass
+
+        # Check XMonad settings
+        try:
+            xmonad_config = os.path.expanduser("~/.xmonad/xmonad.hs")
+            if os.path.exists(xmonad_config):
+                with open(xmonad_config, "r") as file:
+                    for line in file:
+                        if "browser" in line:
+                            return line.split()[-1].strip()
+        except Exception:
+            pass
 
     return None
 
 
-def get_posix_browser_name(path: str | None) -> str:
-    if not path:
-        return ""
-    for name, browser in POSIX_BROWSERS.items():
-        for binary in browser.get("paths", []):
-            if binary in path:
-                return name
+def _binary_path_from_desktop_entry(browser: str | None) -> str | None:
+    if browser:
+        # If the browser is not a .desktop file, return it as is
+        if not browser.endswith(".desktop"):
+            return browser
+
+        for directory in DESKTOP_DIRS:
+            desktop_file_path = os.path.join(directory, browser)
+            if os.path.exists(desktop_file_path):
+                config = configparser.ConfigParser(interpolation=None)
+                config.read(desktop_file_path)
+
+                # The desktop file format has sections like [Desktop Entry]
+                if "Desktop Entry" in config and "Exec" in config["Desktop Entry"]:
+                    exec_command = config["Desktop Entry"]["Exec"]
+
+                    # Extract the binary path from the exec command
+                    binary_path = exec_command.split()[0]
+
+                    # Resolve to full path if binary is in PATH
+                    binary_full_path = shutil.which(binary_path)
+                    if binary_full_path:
+                        return binary_full_path
+                    else:
+                        return binary_path
+    return None
+
+
+def _posix_browser_name(path: str | None) -> str:
+    if path:
+        for name, browser in POSIX_BROWSERS.items():
+            for binary in browser.get("paths", []):
+                if binary in path or path in binary:
+                    return name
     return ""
 
 
+def get_posix_default_browser() -> str | None:
+    return _posix_browser_name(
+        _binary_path_from_desktop_entry(_posix_default_browser())
+    )
+
+
+def get_default_browser() -> str | None:
+    return get_nt_default_browser() if GLOBALS.IS_NT else get_posix_default_browser()
+
+
 def get_default_from_env_vars() -> str:
     browser = os.getenv("BROWSER") or os.getenv("DEFAULT_BROWSER")
     if browser:
         return browser
     return ""
 
 
 # Function to check if a browser is installed and map its name
-def detect_posix() -> tuple[str, dict[str, dict[str, str]]]:
+def detect_standard_browsers() -> tuple[str, dict[str, dict[str, str]]]:
     installed_browsers: dict[str, dict[str, str]] = {}
-    for name, browser in POSIX_BROWSERS.items():
+    browsers = NT_BROWSERS.items()
+    if not GLOBALS.IS_NT:
+        browsers = POSIX_BROWSERS.items()
+    for name, browser in browsers:
         for binary in browser.get("paths", []):
+            if GLOBALS.IS_WSL:
+                binary = nt_to_wsl_path(binary)
             path = shutil.which(binary)
             if path:
                 installed_browsers[name] = {}
                 installed_browsers[name]["path"] = path
                 installed_browsers[name]["family"] = str(browser.get("family", ""))
                 break  # Stop at the first detected binary for a browser
 
     default_browser = get_default_from_env_vars()
     if default_browser in installed_browsers:
         return default_browser, installed_browsers
 
-    default_browser = get_posix_browser_name(
-        get_binary_path_from_desktop_entry(get_posix_default_browser())
-    )
+    default_browser = get_default_browser() or ""
     return default_browser, installed_browsers
 
 
-def detect_nt() -> tuple[str, dict[str, dict[str, str]]]:
-    # Path to the PowerShell script
-    powershell_script_path = os.path.join(
-        os.path.dirname(__file__), "scripts/detect_browsers.ps1"
-    )
-    try:
-        # Run the PowerShell script
-        result = subprocess.run(
-            [
-                "powershell.exe",
-                "-NoProfile",
-                "-ExecutionPolicy",
-                "Bypass",
-                "-File",
-                powershell_script_path,
-            ],
-            capture_output=True,
-            text=True,
-            check=True,
-        )
-        # Load the JSON output into a Python dictionary
-        json_output = json.loads(result.stdout)
-
-        default_browser = get_default_from_env_vars()
-        if default_browser in json_output.get("browsers", {}):
-            return default_browser, json_output.get("browsers", {})
-
-        return json_output.get("default", ""), json_output.get("browsers", {})
-    except subprocess.CalledProcessError as e:
-        print(f"An error occurred while running the PowerShell script: {e}")
-    except json.JSONDecodeError as e:
-        print(f"Failed to decode JSON output: {e}")
-
-    return "", {}
-
-
-def get_windows_username() -> str | None:
-    return (
-        os.popen("powershell.exe '$env:UserName'").read().strip()
-        if is_running_in_wsl() and os.name != "nt"
-        else None
-    )
-
-
-def is_running_in_wsl() -> bool:
-    if (os.environ.get("SKIP_WSL_CHECK") != None) | (sys.platform != "linux"):
-        return False
-    try:
-        with open("/proc/version") as f:
-            version_info = f.read()
-            if "microsoft" in version_info and "WSL" in version_info:
-                return True
-    except FileNotFoundError:
-        pass
-
-    if "WSL_DISTRO_NAME" in os.environ:
-        return True
-
-    if "WT_SESSION" in os.environ and "Windows Terminal" in platform.system():
-        return True
-
-    return False
-
-
 def nt_to_wsl_path(nt_path: str) -> str:
     # Replace backslashes with forward slashes
     wsl_path = nt_path.replace("\\", "/")
 
     # Replace drive letter (e.g., C:) with /mnt/c
     if ":" in wsl_path:
         drive, path = wsl_path.split(":", 1)
```

### Comparing `browserxt-0.1.5/PKG-INFO` & `browserxt-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 Metadata-Version: 2.1
 Name: browserxt
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple extensible browser runner
-Keywords: copier-template,full-development-lifecycle,project-template,serious-scaffold
-Author-Email: Nick Syntychakis <nsyntych@punkops.dev>
+Keywords: copier-template,full-development-lifecycle,project-template,serious-scaffold,winreg; sys_platform == 'win32'
 License: MPL-2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://browserxt.punkops.dev
 Project-URL: Issue, https://github.com/punkops/browserxt/issues
 Project-URL: Repository, https://github.com/punkops/browserxt
 Requires-Python: >=3.11
 Requires-Dist: pydantic-settings
 Requires-Dist: typer[all]
-Requires-Dist: wslPath
 Description-Content-Type: text/markdown
 
 # BrowserXT
 
 A simple extensible browser runner
 
 [![CI](https://github.com/punkops/browserxt/actions/workflows/ci.yml/badge.svg)](https://github.com/punkops/browserxt/actions/workflows/ci.yml)
```

