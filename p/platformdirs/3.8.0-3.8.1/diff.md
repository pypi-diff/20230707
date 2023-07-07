# Comparing `tmp/platformdirs-3.8.0.tar.gz` & `tmp/platformdirs-3.8.1.tar.gz`

## Comparing `platformdirs-3.8.0.tar` & `platformdirs-3.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tox.ini
--rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/conftest.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_android.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_main.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.8.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.8.0/LICENSE
--rw-r--r--   0        0        0     8955 2020-02-02 00:00:00.000000 platformdirs-3.8.0/README.rst
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.8.0/pyproject.toml
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 platformdirs-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tox.ini
+-rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/android.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 platformdirs-3.8.1/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/test_android.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/test_main.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 platformdirs-3.8.1/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.8.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.8.1/LICENSE
+-rw-r--r--   0        0        0     8955 2020-02-02 00:00:00.000000 platformdirs-3.8.1/README.rst
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 platformdirs-3.8.1/PKG-INFO
```

### Comparing `platformdirs-3.8.0/tox.ini` & `platformdirs-3.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/src/platformdirs/__init__.py` & `platformdirs-3.8.1/src/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/src/platformdirs/__main__.py` & `platformdirs-3.8.1/src/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/src/platformdirs/android.py` & `platformdirs-3.8.1/src/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/src/platformdirs/api.py` & `platformdirs-3.8.1/src/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/src/platformdirs/macos.py` & `platformdirs-3.8.1/src/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/src/platformdirs/unix.py` & `platformdirs-3.8.1/src/platformdirs/unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,20 +149,23 @@
     @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g. ``/run/user/$(id -u)/$appname/$version`` or
          ``$XDG_RUNTIME_DIR/$appname/$version``.
 
          For FreeBSD/OpenBSD/NetBSD, it would return ``/var/run/user/$(id -u)/$appname/$version`` if
-         ``$XDG_RUNTIME_DIR`` is not set.
+         exists, otherwise ``/tmp/runtime-$(id -u)/$appname/$version``, if``$XDG_RUNTIME_DIR``
+         is not set.
         """
         path = os.environ.get("XDG_RUNTIME_DIR", "")
         if not path.strip():
             if sys.platform.startswith(("freebsd", "openbsd", "netbsd")):
                 path = f"/var/run/user/{getuid()}"
+                if not Path(path).exists():
+                    path = f"/tmp/runtime-{getuid()}"  # noqa: S108
             else:
                 path = f"/run/user/{getuid()}"
         return self._append_app_name_and_version(path)
 
     @property
     def site_data_path(self) -> Path:
         """:return: data path shared by users. Only return first item, even if ``multipath`` is set to ``True``"""
@@ -206,16 +209,15 @@
             parser.read_string(f"[top]\n{stream.read()}")
 
         if key not in parser["top"]:
             return None
 
         path = parser["top"][key].strip('"')
         # Handle relative home paths
-        path = path.replace("$HOME", os.path.expanduser("~"))  # noqa: PTH111
-        return path
+        return path.replace("$HOME", os.path.expanduser("~"))  # noqa: PTH111
 
     return None
 
 
 __all__ = [
     "Unix",
 ]
```

### Comparing `platformdirs-3.8.0/src/platformdirs/windows.py` & `platformdirs-3.8.1/src/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/tests/conftest.py` & `platformdirs-3.8.1/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,14 +29,13 @@
 def func(request: SubRequest) -> str:
     return cast(str, request.param)
 
 
 @pytest.fixture(params=PROPS)
 def func_path(request: SubRequest) -> str:
     prop = cast(str, request.param)
-    prop = prop.replace("_dir", "_path")
-    return prop
+    return prop.replace("_dir", "_path")
 
 
 @pytest.fixture()
 def props() -> tuple[str, ...]:
     return PROPS
```

### Comparing `platformdirs-3.8.0/tests/test_android.py` & `platformdirs-3.8.1/tests/test_android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/tests/test_api.py` & `platformdirs-3.8.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.8.1/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/tests/test_macos.py` & `platformdirs-3.8.1/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/tests/test_unix.py` & `platformdirs-3.8.1/tests/test_unix.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,25 +139,24 @@
 
     monkeypatch.setenv(xdg_variable.name, "/custom-dir")
     result = getattr(dirs_instance, func)
     assert result == "/custom-dir"
 
 
 @pytest.mark.usefixtures("_getuid")
-def test_platform_on_bsd(monkeypatch: pytest.MonkeyPatch, mocker: MockerFixture) -> None:
+@pytest.mark.parametrize("platform", ["freebsd", "openbsd", "netbsd"])
+def test_platform_on_bsd(monkeypatch: pytest.MonkeyPatch, mocker: MockerFixture, platform: str) -> None:
     monkeypatch.delenv("XDG_RUNTIME_DIR", raising=False)
-    mocker.patch("sys.platform", "freebsd")
-    expected_path = "/var/run/user/1234"
-    assert Unix().user_runtime_dir == expected_path
+    mocker.patch("sys.platform", platform)
 
-    mocker.patch("sys.platform", "openbsd")
-    assert Unix().user_runtime_dir == expected_path
+    mocker.patch("pathlib.Path.exists", return_value=True)
+    assert Unix().user_runtime_dir == "/var/run/user/1234"
 
-    mocker.patch("sys.platform", "netbsd")
-    assert Unix().user_runtime_dir == expected_path
+    mocker.patch("pathlib.Path.exists", return_value=False)
+    assert Unix().user_runtime_dir == "/tmp/runtime-1234"  # noqa: S108
 
 
 def test_platform_on_win32(monkeypatch: pytest.MonkeyPatch, mocker: MockerFixture) -> None:
     monkeypatch.delenv("XDG_RUNTIME_DIR", raising=False)
     mocker.patch("sys.platform", "win32")
     prev_unix = unix
     importlib.reload(unix)
```

### Comparing `platformdirs-3.8.0/LICENSE` & `platformdirs-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/README.rst` & `platformdirs-3.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/pyproject.toml` & `platformdirs-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `platformdirs-3.8.0/PKG-INFO` & `platformdirs-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.8.0
+Version: 3.8.1
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
```

