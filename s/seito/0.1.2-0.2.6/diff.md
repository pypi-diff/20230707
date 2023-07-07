# Comparing `tmp/seito-0.1.2.tar.gz` & `tmp/seito-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seito-0.1.2.tar", max compression
+gzip compressed data, was "seito-0.2.6.tar", last modified: Fri Jul  7 14:51:52 2023, max compression
```

## Comparing `seito-0.1.2.tar` & `seito-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0     1232 2022-05-03 09:26:06.866421 seito-0.1.2/README.md
--rw-r--r--   0        0        0      656 2022-05-03 09:26:06.866421 seito-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      211 2022-05-03 09:26:06.866421 seito-0.1.2/seito/__init__.py
--rw-r--r--   0        0        0     2343 2022-05-03 09:26:06.866421 seito-0.1.2/seito/http.py
--rw-r--r--   0        0        0     1362 2022-05-03 09:26:06.866421 seito-0.1.2/seito/json.py
--rw-r--r--   0        0        0        0 2022-05-03 09:26:06.866421 seito-0.1.2/seito/monad/__init__.py
--rw-r--r--   0        0        0     4153 2022-05-03 09:26:06.866421 seito-0.1.2/seito/monad/async_opt.py
--rw-r--r--   0        0        0      195 2022-05-03 09:26:06.866421 seito-0.1.2/seito/monad/func.py
--rw-r--r--   0        0        0     6656 2022-05-03 09:26:06.866421 seito-0.1.2/seito/monad/opt.py
--rw-r--r--   0        0        0     1337 2022-05-03 09:26:06.866421 seito-0.1.2/seito/monad/try_.py
--rw-r--r--   0        0        0        0 2022-05-03 09:26:06.866421 seito-0.1.2/seito/py.typed.py
--rw-r--r--   0        0        0     2031 2022-05-03 09:26:15.866470 seito-0.1.2/setup.py
--rw-r--r--   0        0        0     1772 2022-05-03 09:26:15.866820 seito-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6217 2023-07-07 14:51:29.951137 seito-0.2.6/README.md
+-rw-r--r--   0        0        0      677 2023-07-07 14:51:52.271046 seito-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:51:29.955137 seito-0.2.6/seito/__init__.py
+-rw-r--r--   0        0        0     2744 2023-07-07 14:51:29.955137 seito-0.2.6/seito/http.py
+-rw-r--r--   0        0        0     2049 2023-07-07 14:51:29.955137 seito-0.2.6/seito/json.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/__init__.py
+-rw-r--r--   0        0        0     9796 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/async_result.py
+-rw-r--r--   0        0        0     1580 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/container.py
+-rw-r--r--   0        0        0      795 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/effect.py
+-rw-r--r--   0        0        0     6110 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/func.py
+-rw-r--r--   0        0        0     7792 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/option.py
+-rw-r--r--   0        0        0     7095 2023-07-07 14:51:29.955137 seito-0.2.6/seito/monad/result.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:51:29.955137 seito-0.2.6/seito/py.typed.py
+-rw-r--r--   0        0        0     4371 2023-07-07 14:51:29.955137 seito-0.2.6/tests/test_async_try.py
+-rw-r--r--   0        0        0     1825 2023-07-07 14:51:29.955137 seito-0.2.6/tests/test_http.py
+-rw-r--r--   0        0        0      523 2023-07-07 14:51:29.955137 seito-0.2.6/tests/test_impure.py
+-rw-r--r--   0        0        0     1835 2023-07-07 14:51:29.955137 seito-0.2.6/tests/test_json.py
+-rw-r--r--   0        0        0     8132 2023-07-07 14:51:29.955137 seito-0.2.6/tests/test_option.py
+-rw-r--r--   0        0        0     3008 2023-07-07 14:51:29.955137 seito-0.2.6/tests/test_result.py
+-rw-r--r--   0        0        0     6465 1970-01-01 00:00:00.000000 seito-0.2.6/PKG-INFO
```

### Comparing `seito-0.1.2/seito/monad/opt.py` & `seito-0.2.6/seito/monad/option.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,284 +1,352 @@
-from abc import ABC, abstractmethod
+import typing as t
 from dataclasses import dataclass
-from typing import Any, TypeVar, Generic, Callable, NoReturn
 
-import pampy
-from aflowey import lift
-from pampy.pampy import match_dict as pampy_dict_matcher
+from seito.monad.container import CommonContainer, EmptyError
+from seito.monad.func import apply
 
-from seito.monad.func import identity
+T_co = t.TypeVar("T_co", covariant=True)
+U = t.TypeVar("U")
+V = t.TypeVar("V")
+P = t.ParamSpec("P")
 
 
-class EmptyError(ValueError):
-    ...
-
-
-class MatchError(TypeError):
-    ...
-
-
-def apply(f: Callable[..., Any] | Any = identity, *args: Any, **kwargs: Any) -> Any:
-    if callable(f):
-        return f(*args, **kwargs)
-    return f
-
+class OptionContainer(CommonContainer[T_co], t.Protocol):
+    def is_some(self) -> bool:  # pragma: no cover
+        ...
 
-_ = pampy._
+    def is_empty(self) -> bool:  # pragma: no cover
+        ...
 
+    def or_if_falsy(
+        self, obj: t.Callable[P, t.Any] | t.Any, *args: P.args, **kwargs: P.kwargs
+    ) -> t.Any:  # pragma: no cover
+        """ """
+        ...
 
-class When:
-    def __init__(self, value):
-        self.value = value
-        self.action = None
-
-    def then(self, f):
-        self.action = f
-        return self
-
-    def __repr__(self):
-        return repr(self.value)
 
+Q = t.TypeVar("Q")
 
-when = When
 
+Nested: t.TypeAlias = "Some[Q | Nested[Q]]"
 
-@dataclass
-class Default:
-    def __init__(self):
-        self.action = None
 
-    def __rshift__(self, other) -> "Default":
-        self.action = other
-        return self
+@dataclass(unsafe_hash=True, frozen=True)
+class Some(OptionContainer[T_co]):
+    """ """
 
+    _under: T_co
 
-default = Default
+    def get(self) -> T_co:
+        """
+        get the value of the Some container
 
+        Returns:
+            T: _description_
+        """
+        return self._under
 
-class Option(ABC):
-    @abstractmethod
-    def get(self) -> Any:
-        ...  # pragma: no cover
+    def is_some(self) -> bool:
+        """
+        Check if the container is a Some.
+
+        Returns:
+            bool: _description_
+        """
+        return True
 
-    @abstractmethod
     def is_empty(self) -> bool:
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def or_else(self, obj: Callable[..., Any] | Any, *args: Any, **kwargs: Any) -> Any:
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def or_if_falsy(
-        self, obj: Callable[..., Any] | Any, *args: Any, **kwargs: Any
-    ) -> Any:
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def or_none(self) -> Any:
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def or_raise(self, exc: Exception | None = None):
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def map(self, func: Callable[..., Any], *args: Any, **kwargs: Any) -> "Option":
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def __iter__(self):
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def __getattr__(self, name: str) -> Any:
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def __call__(self, *args: Any, **kwargs: Any):
-        ...  # pragma: no cover
-
-    @abstractmethod
-    def __str__(self) -> str:
-        ...  # pragma: no cover
-
-    def __rshift__(self, other) -> When:
-        return when(self).then(other)
+        """
+        Check if the container is empty.
 
-    def match(self, *whens: When | Default):
-        for w in whens:
-            if isinstance(w, when):
-                if w.value.__class__ == self.__class__:
-                    match_dict, self_dict = w.value.__dict__, self.__dict__
-                    is_a_match, extracted = pampy_dict_matcher(match_dict, self_dict)
-                    if not is_a_match:
-                        continue
-                    if extracted:
-                        return apply(w.action, *extracted)
-                    return apply(w.action)
-            else:
-                return apply(w.action)
-        raise MatchError(f"No default guard found, enable to match {self}")
-
-
-T = TypeVar("T")
-M = TypeVar("M")
-
-
-@dataclass
-class Some(Generic[T], Option):
-    _under: T
-
-    def get(self) -> T:
-        return self._under
-
-    def is_empty(self) -> bool:
+        Returns:
+            bool: True if the container is empty, False otherwise.
+        """
         return False
 
-    def or_else(self, obj: Callable[..., Any], *args: Any, **kwargs: Any) -> T:
+    @t.overload
+    def flatten(self: "Nested[Empty]") -> "Empty":
+        ...
+
+    @t.overload
+    def flatten(self: "Nested[Q]") -> "Some[Q]":
+        ...
+
+    def flatten(self) -> "Some | Empty":
+        """
+        Flatten the container i.e. transform Some(Some(x)) into Some(x).
+
+        Returns:
+            Some | Empty: _description_
+        """
+        x = self._under
+        while isinstance(x, (Some, Empty)):
+            x = x._under  # type: ignore
+        return opt(x)
+
+    @t.overload
+    def or_else(
+        self, obj: t.Callable[P, t.Any], *args: P.args, **kwargs: P.kwargs
+    ) -> T_co:
+        ...
+
+    @t.overload
+    def or_else(self, obj: t.Any) -> T_co:
+        ...
+
+    def or_else(
+        self, obj: t.Callable[P, t.Any] | t.Any, *args: P.args, **kwargs: P.kwargs
+    ) -> T_co:
+        """
+        Apply a function to the value of the container.
+        Args:
+            obj (t.Callable[P, t.Any]): _description_
+
+        Returns:
+            T: _description_
+        """
         return self._under
 
+    unwrap_or_else = or_else
+
     def or_if_falsy(
-        self, obj: Callable[..., Any], *args: Any, **kwargs: Any
-    ) -> T | Any:
+        self, obj: t.Callable[P, U], *args: P.args, **kwargs: P.kwargs
+    ) -> T_co | U:
+        """
+        Apply a function to the value of the container if it is falsy.
+
+        Args:
+            obj (t.Callable[P, U]): _description_
+
+        Returns:
+            T | U: _description_
+        """
         return self._under or apply(obj, *args, **kwargs)
 
-    def or_none(self) -> T:
+    def or_none(self) -> T_co:
+        """
+        Return the value of the container if it is not None.
+
+        Returns:
+            T: _description_
+        """
         return self._under
 
-    def or_raise(self, exc: Exception | None = None) -> T:
+    def or_raise(self, exc: Exception | None = None) -> T_co:
+        """
+        Return the value of the container if it is not None.
+
+        Args:
+            exc (Exception | None, optional): _description_. Defaults to None.
+
+        Returns:
+            T: _description_
+        """
         return self._under
 
-    def map(
-        self, f: Callable[[T, ...], M], *args: Any, **kwargs: Any
-    ) -> "Some[M] | Empty":
-        inst = self
-        while isinstance(inst._under, Option):
-            inst = inst._under
-        return opt(apply(f, inst._under, *args, **kwargs))
-
-    def __iter__(self):
-        under = self._under
-        while under is not None:
-            if isinstance(under, Option):
-                under = under._under
-            else:
-                yield under
-                under = None
-
-    def __getattr__(self, name: str) -> "Some[Any] | Empty | Callable[..., Any]":
+    def map(self, func: t.Callable[[T_co], U]) -> "Some[U]":
+        """
+        Apply a function to the value of the container.
+
+        Args:
+            func (t.Callable[[T], U]): _description_
+
+        Returns:
+            Some[U]: _description_
+        """
+        result = apply(func, self._under)
+        result = opt(result)
+        return result
+
+    def __iter__(self) -> t.Generator[T_co, t.Any, None]:
+        """
+        Iterate over the value of the container.
+
+        Returns:
+            t.Iterator[T]: _description_
+
+        Yields:
+            Iterator[t.Iterator[T]]: _description_
+        """
+        yield self.flatten().get()
+
+    def __getattr__(self, name: str) -> "Some | Empty | t.Callable":
+        """
+        Get an attribute of the value of the container.
+
+        Args:
+            name (str): _description_
+
+        Returns:
+            Some | Empty | t.Callable: _description_
+        """
         try:
             attr = getattr(self._under, name)
         except AttributeError:
             return none
         if callable(attr):
 
-            def wrapper(*args: Any, **kwargs: Any) -> "Some | Empty":
+            def wrapper(*args: t.Any, **kwargs: t.Any) -> "Some[t.Any] | Empty":
                 return opt(attr(*args, **kwargs))
 
             return wrapper
         return opt(attr)
 
-    def __call__(self, *args: Any, **kwargs: Any) -> "Some[T]":
-        return self
-
     def __str__(self) -> str:
+        """
+        Return the string representation of the container.
+
+        Returns:
+            str: _description_
+        """
         return f"<Some {str(self._under)}>"
 
 
-@dataclass
-class Empty(Option):
-    _under = None
+@dataclass(unsafe_hash=True)
+class Empty(OptionContainer[None]):
+    """ """
 
-    def get(self) -> NoReturn:
+    _under: None = None
+
+    def get(self) -> t.NoReturn:
         raise EmptyError("Option is empty")
 
+    def is_some(self) -> bool:
+        return False
+
     def is_empty(self) -> bool:
         return True
 
-    def or_else(self, obj: Callable[..., M] | M, *args: Any, **kwargs: Any) -> M:
-        return apply(obj, *args, **kwargs)
+    def or_(self, obj: U) -> U:
+        return obj
 
-    def or_if_falsy(self, obj: Callable[..., M] | M, *args, **kwargs) -> M:
+    @t.overload
+    def or_else(self, obj: t.Callable[P, U], *args: P.args, **kwargs: P.kwargs) -> U:
+        ...
+
+    @t.overload
+    def or_else(self, obj: U) -> U:
+        ...
+
+    def or_else(
+        self, obj: t.Callable[P, U] | U, *args: P.args, **kwargs: P.kwargs
+    ) -> U:
         return apply(obj, *args, **kwargs)
 
+    def unwrap_or_else(
+        self, obj: t.Callable[P, U], *args: P.args, **kwargs: P.kwargs
+    ) -> U:
+        return self.or_else(obj, *args, **kwargs)
+
+    def or_if_falsy(
+        self, obj: t.Callable[P, U] | U, *args: P.args, **kwargs: P.kwargs
+    ) -> U:
+        x = apply(obj, *args, **kwargs)
+        return x
+
     def or_none(self) -> None:
         return None
 
-    def or_raise(self, exc: Exception | None = None) -> NoReturn:
+    def or_raise(self, exc: Exception | None = None) -> t.NoReturn:
         if exc is None:
-            raise ValueError("Empty value !")
+            raise EmptyError("Option is empty")
         raise exc
 
-    def map(self, func, *args, **kwargs) -> "Empty":
+    def map(
+        self,
+        func: t.Callable,
+    ) -> "Empty":
         return self
 
-    def __iter__(self):
+    def __iter__(self) -> "t.Iterator[Empty]":
         return self
 
     def __next__(self):
         raise StopIteration()
 
     def __getattr__(self, name: str) -> "Empty":
         return self
 
-    def __call__(self, *args: Any, **kwargs: Any) -> "Empty":
+    def __call__(self, *args: t.Any, **kwargs: t.Any) -> "Empty":
         return self
 
     def __str__(self) -> str:
-        return "<Empty >"
+        return "<Empty>"
 
 
-E = TypeVar("E", bound=Exception)
+T_err = t.TypeVar("T_err", bound=Exception, covariant=True)
 
 
-@dataclass
-class Err(Empty, Generic[E]):
-    _under: E
+# @t.overload
+# def unravel_container(
+#    value: T,  # not a some
+#    last_container: T | None = None,
+# ) -> tuple[T, T | None]:
+#    ...
 
-    def __str__(self):
-        return f"<Err {repr(self._under)} >"
 
-    def unwrap(self):
-        return self._under
+# @t.overload
+# def unravel_container(
+#    value: Some[Some[Some[U]]],
+# ) -> tuple[U, Some[U]]:
+#    ...
 
-    recover_with = Empty.or_else
 
-    def or_raise(self, exc: Exception | None = None) -> NoReturn:
-        if exc is not None:
-            raise exc from self._under
-        raise self._under
+# @t.overload
+# def unravel_container(
+#    value: t.Any,
+#    last_container: t.Any | None = None,
+# ) -> tuple[t.Any, t.Any]:
+#    ...
 
 
-def unravel_opt(value):
-    if not isinstance(value, Option):
-        return value
-    inst = value._under
-    while isinstance(inst, Option):  # pragma: no cover
-        inst = inst._under
-    return inst
+# @t.overload
+# def unravel_container(
+#    value: Some[Some[T]],
+# ) -> Some[T]:
+#    ...
+
+
+def unravel_container(value):
+    match value:
+        case Some(under) | Empty(under):
+            return unravel_container(under)
+        case _:
+            return value
+
+
+OPT_MATCHABLE_CLASSES = {Some, Empty}
+Some.__matchable_classes__ = OPT_MATCHABLE_CLASSES
+Empty.__matchable_classes__ = OPT_MATCHABLE_CLASSES
+
+
+T_opt = t.TypeVar("T_opt")
+
+
+@t.overload
+def option(value: None) -> Empty:
+    ...
+
+
+@t.overload
+def option(value: T_opt) -> Some[T_opt]:
+    ...
 
 
-def option(value: Any) -> Some[Any] | Empty:
-    if isinstance(value, Exception):
-        return Err(value)
-    new_val = unravel_opt(value)
-    return none if new_val is None else Some(new_val)
+def option(value: T_opt) -> Some[T_opt] | Empty:
+    """ """
+    return Null if value is None else Some(value)
 
 
-def opt_from_call(f, *args, **kwargs):
-    exc = kwargs.pop("exc", Exception)
-    try:
-        return opt(f(*args, **kwargs))
-    except exc:
-        return Err(exc)
+def lift_opt(f: t.Callable[P, U]) -> t.Callable[P, Some[U] | Empty]:
+    """ """
 
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Some[U] | Empty:
+        val: U = f(*args, **kwargs)
+        return opt(val)
 
-def lift_opt(f):
-    return lift(f, opt_from_call)
+    return wrapper
 
 
 # aliases
-none = nope = empty = Empty()
+none = nope = empty = Null = Empty(None)
 opt = option
-err = Err
```

