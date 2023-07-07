# Comparing `tmp/exchange_calendars_extensions-0.2.1.tar.gz` & `tmp/exchange_calendars_extensions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions-0.2.1.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions-0.3.0.tar", max compression
```

## Comparing `exchange_calendars_extensions-0.2.1.tar` & `exchange_calendars_extensions-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/LICENSE
--rw-r--r--   0        0        0    22327 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/README.md
--rw-r--r--   0        0        0    22374 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/__init__.py
--rw-r--r--   0        0        0    27151 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/changeset.py
--rw-r--r--   0        0        0     6780 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/holiday.py
--rw-r--r--   0        0        0    37920 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/holiday_calendar.py
--rw-r--r--   0        0        0     1674 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/observance.py
--rw-r--r--   0        0        0     5720 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/offset.py
--rw-r--r--   0        0        0     2611 2023-05-31 11:16:15.831594 exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/util.py
--rw-r--r--   0        0        0     1485 2023-05-31 11:16:28.649816 exchange_calendars_extensions-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    23639 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 08:09:05.766729 exchange_calendars_extensions-0.3.0/LICENSE
+-rw-r--r--   0        0        0    30234 2023-07-07 08:09:05.766729 exchange_calendars_extensions-0.3.0/README.md
+-rw-r--r--   0        0        0    26680 2023-07-07 08:09:05.766729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/__init__.py
+-rw-r--r--   0        0        0    19576 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/changeset.py
+-rw-r--r--   0        0        0     6780 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday.py
+-rw-r--r--   0        0        0    40255 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday_calendar.py
+-rw-r--r--   0        0        0     5673 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/offset.py
+-rw-r--r--   0        0        0     2595 2023-07-07 08:09:05.770729 exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/util.py
+-rw-r--r--   0        0        0     2888 2023-07-07 08:09:20.482809 exchange_calendars_extensions-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    31729 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.3.0/PKG-INFO
```

### Comparing `exchange_calendars_extensions-0.2.1/LICENSE` & `exchange_calendars_extensions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/__init__.py` & `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import functools
 from datetime import time
-from typing import Optional, Callable, Type, Union
-from typing_extensions import ParamSpec, Concatenate
+from typing import Optional, Callable, Type, Union, Any
 
-import pandas as pd
 from exchange_calendars import calendar_utils, register_calendar_type, ExchangeCalendar, get_calendar_names
 from exchange_calendars.calendar_utils import _default_calendar_factories
 from exchange_calendars.exchange_calendar_asex import ASEXExchangeCalendar
 from exchange_calendars.exchange_calendar_xams import XAMSExchangeCalendar
 from exchange_calendars.exchange_calendar_xbru import XBRUExchangeCalendar
 from exchange_calendars.exchange_calendar_xbud import XBUDExchangeCalendar
 from exchange_calendars.exchange_calendar_xcse import XCSEExchangeCalendar
@@ -26,17 +24,18 @@
 from exchange_calendars.exchange_calendar_xpra import XPRAExchangeCalendar
 from exchange_calendars.exchange_calendar_xsto import XSTOExchangeCalendar
 from exchange_calendars.exchange_calendar_xswx import XSWXExchangeCalendar
 from exchange_calendars.exchange_calendar_xtae import XTAEExchangeCalendar
 from exchange_calendars.exchange_calendar_xtse import XTSEExchangeCalendar
 from exchange_calendars.exchange_calendar_xwar import XWARExchangeCalendar
 from exchange_calendars.exchange_calendar_xwbo import XWBOExchangeCalendar
+from typing_extensions import ParamSpec, Concatenate
 
-from .changeset import ChangeSet, HolidaysAndSpecialSessions, DaySpec, DaySpecWithTime
-from .holiday_calendar import extend_class, ExtendedExchangeCalendar
+from .changeset import ChangeSet, DayType, DaySpec, DayWithTimeSpec
+from .holiday_calendar import extend_class, ExtendedExchangeCalendar, ExchangeCalendarExtensions
 
 # Dictionary that maps from exchange key to ExchangeCalendarChangeSet. Contains all changesets to apply when creating a
 # new calendar instance.
 _changesets = dict()
 
 # Dictionary that maps from exchange key to ExtendedExchangeCalendar. Contains all extended calendars classes that
 # replace the vanilla classes in exchange_calendars when calling apply_extensions().
@@ -68,32 +67,79 @@
     "XTAE": (XTAEExchangeCalendar, 4),
     "XTSE": (XTSEExchangeCalendar, 4),
     "XWAR": (XWARExchangeCalendar, 4),
     "XWBO": (XWBOExchangeCalendar, 4),
 }
 
 
+_original_classes = dict()
+
+
 def apply_extensions() -> None:
     """
     Apply extensions to exchange_calendars.
 
     This registers all extended calendars in exchange_calendars, overwriting the respective vanilla calendars.
     """
+    if len(_original_classes) > 0:
+        # Extensions have already been applied.
+        return
+
     calendar_names = set(get_calendar_names())
 
+    def get_changeset_fn(name: str) -> Callable[[], ChangeSet]:
+        def fn() -> ChangeSet:
+            return _changesets.get(name)
+        return fn
+
+    print('Applying generic extension for calendars that have no explicit extension defined.')
     for k in calendar_names - set(_extensions.keys()):
         cls = _default_calendar_factories.get(k)
         if cls is not None:
-            cls = extend_class(cls, day_of_week_expiry=None, changeset_provider=lambda: _changesets.get(k))
+            # Store the original class for later use.
+            _original_classes[k] = cls
+            # Create extended class.
+            print(f'Extending {k}: {cls}')
+            cls = extend_class(cls, day_of_week_expiry=None, changeset_provider=get_changeset_fn(k))
+            # Register extended class.
             register_calendar_type(k, cls, force=True)
+            # Remove original class from factory cache.
+            _remove_calendar_from_factory_cache(k)
 
+    print('Applying extension for calendars with explicit extension defined.')
     for k, v in _extensions.items():
         cls, day_of_week_expiry = v
-        cls = extend_class(cls, day_of_week_expiry=day_of_week_expiry, changeset_provider=lambda: _changesets.get(k))
+        # Store the original class for later use.
+        _original_classes[k] = cls
+        # Create extended class.
+        print(f'Extending {k}: {cls} day_of_week_expiry={day_of_week_expiry}')
+        cls = extend_class(cls, day_of_week_expiry=day_of_week_expiry, changeset_provider=get_changeset_fn(k))
+        # Register extended class.
         register_calendar_type(k, cls, force=True)
+        # Remove original class from factory cache.
+        _remove_calendar_from_factory_cache(k)
+
+
+def remove_extensions() -> None:
+    """
+    Remove extensions from exchange_calendars.
+
+    This removes all extended calendars from exchange_calendars, restoring the respective vanilla calendars.
+    """
+    if len(_original_classes) == 0:
+        # Extensions have not been applied.
+        return
+
+    for k, v in _original_classes.items():
+        # Register original class.
+        register_calendar_type(k, v, force=True)
+        # Remove extended class from factory cache.
+        _remove_calendar_from_factory_cache(k)
+
+    _original_classes.clear()
 
 
 def register_extension(name: str, cls: Type[ExchangeCalendar], day_of_week_expiry: Optional[int] = None) -> None:
     """
     Register an extended calendar class for a given exchange key and a given base class.
 
     This creates and then registers an extended calendar class based on the given class, with support for all
@@ -157,446 +203,547 @@
     def wrapper(exchange: str, *args: P.args, **kwargs: P.kwargs) -> None:
         # Retrieve changeset for key, create new empty one, if required.
         cs: ChangeSet = _changesets.get(exchange, ChangeSet())
 
         # Call wrapped function with changeset as first positional argument.
         cs = f(cs, *args, **kwargs)
 
-        if not cs.is_consistent():
-            raise ValueError(f'Changeset for {str} is inconsistent: {cs}.')
+#        if not cs.is_consistent():
+#            raise ValueError(f'Changeset for {str} is inconsistent: {cs}.')
 
         # Save changeset back to _changesets.
         _changesets[exchange] = cs
 
         # Remove calendar for exchange key from factory cache.
         _remove_calendar_from_factory_cache(exchange)
 
         # Return result of wrapped function.
         return None
 
     return wrapper
 
 
 @_with_changeset
-def _add_day(cs: ChangeSet, day_type: HolidaysAndSpecialSessions, date: pd.Timestamp, value: Union[DaySpec, DaySpecWithTime], strict: bool) -> ChangeSet:
+def _add_day(cs: ChangeSet, date: Any, value: Union[DaySpec, DayWithTimeSpec, dict], day_type: DayType, strict: bool) -> ChangeSet:
     """
     Add a day of a given type to the changeset for a given exchange calendar.
 
     Parameters
     ----------
     cs : ChangeSet
         The changeset to which to add the day.
-    day_type : HolidaysAndSpecialSessions
-        The type of the day to add.
-    date : pd.Timestamp
-        The date to add.
-    value : Union[DaySpec, DaySpecWithTime]
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
+    value : Union[DaySpec, DaySpecWithTime, dict]
         The properties to add for the day. Must match the properties required by the given day type.
+    day_type : DayType
+        The type of the day to add.
     strict : bool
         Whether to raise an error if the changeset would be inconsistent after adding the day.
 
     Returns
     -------
     ChangeSet
         The changeset with the added day.
 
     Raises
     ------
     ValueError
         If the changeset would be inconsistent after adding the day.
     """
-    return cs.add_day(date, value, day_type, strict=strict)
+    if not strict:
+        cs.clear_day(date)
+
+    return cs.add_day(date, value, day_type)
 
 
-def add_day(exchange: str, day_type: HolidaysAndSpecialSessions, date: pd.Timestamp, value: Union[DaySpec, DaySpecWithTime], strict: bool = False) -> None:
+def add_day(exchange: str, date: Any, value: Union[DaySpec, DayWithTimeSpec], day_type: DayType, strict: bool = False) -> None:
     """
     Add a day of a given type to the given exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    day_type : HolidaysAndSpecialSessions
-        The type of the day to add.
-    date : pd.Timestamp
-        The date to add.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
     value : Union[DaySpec, DaySpecWithTime]
         The properties to add for the day. Must match the properties required by the given day type.
+    day_type : DayType
+        The type of the day to add.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after adding the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after adding the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, day_type, date, value, strict=strict)
+    _add_day(exchange, date, value, day_type, strict=strict)
 
 
 @_with_changeset
-def _clear_day(cs: ChangeSet, date: pd.Timestamp, day_type: Optional[HolidaysAndSpecialSessions] = None) -> ChangeSet:
+def _remove_day(cs: ChangeSet, date: Any, day_type: DayType, strict: bool) -> ChangeSet:
     """
-    Clear a day of a given type from the changeset for a given exchange calendar.
+    Remove a day of a given type from the changeset for a given exchange calendar.
 
     Parameters
     ----------
     cs : ChangeSet
-        The changeset from which to clear the day.
-    date : pd.Timestamp
-        The date to clear.
-    day_type : Optional[HolidaysAndSpecialSessions]
-        The type of the day to clear. If None, clears all types of days.
+        The changeset from which to remove the day.
+    date : Any
+        The date to remove. Must be convertible to pandas.Timestamp.
+    day_type : DayType
+        The type of the day to remove.
+    strict : bool
+        Whether to raise an error if the changeset would be inconsistent after removing the day.
 
     Returns
     -------
     ChangeSet
-        The changeset with the cleared day.
+        The changeset with the removed day.
+
+    Raises
+    ------
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
-    return cs.clear_day(date, day_type)
+    if not strict:
+        cs.clear_day(date)
+
+    return cs.remove_day(date, day_type)
 
 
-def clear_day(exchange: str, date: pd.Timestamp, day_type: Optional[HolidaysAndSpecialSessions] = None) -> None:
+def remove_day(exchange: str, date: Any, day_type: Optional[DayType] = None, strict: bool = False) -> None:
     """
-    Clear a day of a given type from the given exchange calendar.
+    Remove a day of a given type from the given exchange calendar.
 
     Parameters
     ----------
     exchange : str
-        The exchange key for which to clear the day.
-    date : pd.Timestamp
-        The date to clear.
-    day_type : Optional[HolidaysAndSpecialSessions]
-        The type of the day to clear. If None, clears all types of days.
+        The exchange key for which to remove the day.
+    date : Any
+        The date to remove. Must be convertible to pandas.Timestamp.
+    day_type : Optional[DayType]
+        The type of the day to remove. If None, removes the day for all types of days.
+    strict : bool
+        Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
 
     Returns
     -------
     None
+
+    Raises
+    ------
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
-    _clear_day(exchange, date, day_type)
+    _remove_day(exchange, date, day_type, strict=strict)
 
 
 @_with_changeset
-def _remove_day(cs: ChangeSet, date: pd.Timestamp, day_type: HolidaysAndSpecialSessions, strict: bool) -> ChangeSet:
+def _reset_day(cs: ChangeSet, date: Any, day_type: Optional[DayType] = None) -> ChangeSet:
     """
-    Remove a day of a given type from the changeset for a given exchange calendar.
+    Clear a day of a given type from the changeset for a given exchange calendar.
 
     Parameters
     ----------
     cs : ChangeSet
-        The changeset from which to remove the day.
-    date : pd.Timestamp
-        The date to remove.
-    day_type : HolidaysAndSpecialSessions
-        The type of the day to remove.
-    strict : bool
-        Whether to raise an error if the changeset would be inconsistent after removing the day.
+        The changeset from which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+    day_type : Optional[DayType]
+        The type of the day to clear. If None, clears all types of days.
 
     Returns
     -------
     ChangeSet
-        The changeset with the removed day.
-
-    Raises
-    ------
-    ValueError
-        If the changeset would be inconsistent after removing the day.
+        The changeset with the cleared day.
     """
-    return cs.remove_day(date, day_type, strict=strict)
+    return cs.clear_day(date, day_type)
 
 
-def remove_day(exchange: str, date: pd.Timestamp, day_type: Optional[HolidaysAndSpecialSessions] = None, strict: bool = False) -> None:
+def reset_day(exchange: str, date: Any, day_type: Optional[DayType] = None) -> None:
     """
-    Remove a day of a given type from the given exchange calendar.
+    Clear a day of a given type from the given exchange calendar.
 
     Parameters
     ----------
     exchange : str
-        The exchange key for which to remove the day.
-    date : pd.Timestamp
-        The date to remove.
-    day_type : Optional[HolidaysAndSpecialSessions]
-        The type of the day to remove. If None, removes the day for all types of days.
-    strict : bool
-        Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
+        The exchange key for which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+    day_type : Optional[DayType]
+        The type of the day to clear. If None, clears all types of days.
 
     Returns
     -------
     None
-
-    Raises
-    ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after removing the day.
     """
-    _remove_day(exchange, date, day_type, strict=strict)
+    _reset_day(exchange, date, day_type)
 
 
-def add_holiday(exchange: str, date: pd.Timestamp, name: str = "Holiday", strict: bool = False) -> None:
+def add_holiday(exchange: str, date: Any, name: str = "Holiday", strict: bool = False) -> None:
     """
     Add a holiday to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    date : pd.Timestamp
-        The date of the holiday.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
     name : str
         The name of the holiday.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after adding the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after adding the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, HolidaysAndSpecialSessions.HOLIDAY, date, {"name": name}, strict=strict)
+    _add_day(exchange, date, {"name": name}, DayType.HOLIDAY, strict=strict)
 
 
-def remove_holiday(exchange: str, date: pd.Timestamp, strict: bool = False) -> None:
+def remove_holiday(exchange: str, date: Any, strict: bool = False) -> None:
     """
     Remove a holiday from an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to remove the day.
-    date : pd.Timestamp
-        The date of the holiday to remove.
+    date : Any
+        The date to remove. Must be convertible to pandas.Timestamp.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after removing the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
-    _remove_day(exchange, date, HolidaysAndSpecialSessions.HOLIDAY, strict=strict)
+    _remove_day(exchange, date, DayType.HOLIDAY, strict=strict)
 
 
-def add_special_open(exchange: str, date: pd.Timestamp, t: time, name: str = "Special Open", strict: bool = False) -> None:
+def reset_holiday(exchange: str, date: Any) -> None:
+    """
+    Clear a holiday from an exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange key for which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+
+    Returns
+    -------
+    None
+    """
+    _reset_day(exchange, date, DayType.HOLIDAY)
+
+
+def add_special_open(exchange: str, date: Any, t: Union[time, str], name: str = "Special Open", strict: bool = False) -> None:
     """
     Add a special open to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    date : pd.Timestamp
-        The date of the special open.
-    t : time
-        The time of the special open.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
+    t : Union[time, str]
+        The time of the special open. If a string, must be in the format 'HH:MM' or 'HH:MM:SS'.
     name : str
         The name of the special open.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after adding the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after adding the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, HolidaysAndSpecialSessions.SPECIAL_OPEN, date, {"name": name, "time": t}, strict=strict)
+    _add_day(exchange, date, {"name": name, "time": t}, DayType.SPECIAL_OPEN, strict=strict)
 
 
-def remove_special_open(exchange: str, date: pd.Timestamp, strict: bool = False) -> None:
+def remove_special_open(exchange: str, date: Any, strict: bool = False) -> None:
     """
     Remove a special close from an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to remove the day.
-    date : pd.Timestamp
-        The date of the special open to remove.
+    date : Any
+        The date to remove. Must be convertible to pandas.Timestamp.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after removing the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
-    _remove_day(exchange, date, HolidaysAndSpecialSessions.SPECIAL_OPEN, strict=strict)
+    _remove_day(exchange, date, DayType.SPECIAL_OPEN, strict=strict)
 
 
-def add_special_close(exchange: str, date: pd.Timestamp, t: time, name: str = "Special Close", strict: bool = False) -> None:
+def reset_special_open(exchange: str, date: Any) -> None:
+    """
+    Clear a special open from an exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange key for which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+
+    Returns
+    -------
+    None
+    """
+    _reset_day(exchange, date, DayType.SPECIAL_OPEN)
+
+
+def add_special_close(exchange: str, date: Any, t: Union[time, str], name: str = "Special Close", strict: bool = False) -> None:
     """
     Add a special close to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    date : pd.Timestamp
-        The date of the special close.
-    t : time
-        The time of the special close.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
+    t : Union[time, str]
+        The time of the special close. If a string, must be in the format 'HH:MM' or 'HH:MM:SS'.
     name : str
         The name of the special close.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after adding the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after adding the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, HolidaysAndSpecialSessions.SPECIAL_CLOSE, date, {"name": name, "time": t}, strict=strict)
+    _add_day(exchange, date, {"name": name, "time": t}, DayType.SPECIAL_CLOSE, strict=strict)
 
 
-def remove_special_close(exchange: str, date: pd.Timestamp, strict: bool = False) -> None:
+def remove_special_close(exchange: str, date: Any, strict: bool = False) -> None:
     """
     Remove a special close from an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to remove the day.
-    date : pd.Timestamp
-        The date of the special close to remove.
+    date : Any
+        The date to remove. Must be convertible to pandas.Timestamp.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after removing the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
-    _remove_day(exchange, date, HolidaysAndSpecialSessions.SPECIAL_CLOSE, strict=strict)
+    _remove_day(exchange, date, DayType.SPECIAL_CLOSE, strict=strict)
 
 
-def add_quarterly_expiry(exchange: str, date: pd.Timestamp, name: str = "Quarterly Expiry", strict: bool = False) -> None:
+def reset_special_close(exchange: str, date: Any) -> None:
+    """
+    Clear a special close from an exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange key for which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+
+    Returns
+    -------
+    None
+    """
+    _reset_day(exchange, date, DayType.SPECIAL_CLOSE)
+
+
+def add_quarterly_expiry(exchange: str, date: Any, name: str = "Quarterly Expiry", strict: bool = False) -> None:
     """
     Add a quarterly expiry to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    date : pd.Timestamp
-        The date of the quarterly expiry.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
     name : str
         The name of the quarterly expiry.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after adding the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after adding the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, HolidaysAndSpecialSessions.QUARTERLY_EXPIRY, date, {"name": name}, strict=strict)
+    _add_day(exchange, date, {"name": name}, DayType.QUARTERLY_EXPIRY, strict=strict)
 
 
-def remove_quarterly_expiry(exchange: str, date: pd.Timestamp, strict: bool = False) -> None:
+def remove_quarterly_expiry(exchange: str, date: Any, strict: bool = False) -> None:
     """
     Remove a quarterly expiry from an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to remove the day.
-    date : pd.Timestamp
-        The date of the quarterly expiry to remove.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
 
     Returns
     -------
     None
+
+    Raises
+    ------
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
+    """
+    _remove_day(exchange, date, DayType.QUARTERLY_EXPIRY, strict=strict)
+
+
+def reset_quarterly_expiry(exchange: str, date: Any) -> None:
+    """
+    Clear a quarterly expiry from an exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange key for which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+
+    Returns
+    -------
+    None
     """
-    _remove_day(exchange, date, HolidaysAndSpecialSessions.QUARTERLY_EXPIRY, strict=strict)
+    _reset_day(exchange, date, DayType.QUARTERLY_EXPIRY)
 
 
-def add_monthly_expiry(exchange: str, date: pd.Timestamp, name: str = "Monthly Expiry", strict: bool = False) -> None:
+def add_monthly_expiry(exchange: str, date: Any, name: str = "Monthly Expiry", strict: bool = False) -> None:
     """
     Add a monthly expiry to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    date : pd.Timestamp
-        The date of the monthly expiry.
+    date : Any
+        The date to add. Must be convertible to pandas.Timestamp.
     name : str
         The name of the monthly expiry.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after adding the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after adding the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, HolidaysAndSpecialSessions.MONTHLY_EXPIRY, date, {"name": name}, strict=strict)
+    _add_day(exchange, date, {"name": name}, DayType.MONTHLY_EXPIRY, strict=strict)
 
     
-def remove_monthly_expiry(exchange: str, date: pd.Timestamp, strict: bool = False) -> None:
+def remove_monthly_expiry(exchange: str, date: Any, strict: bool = False) -> None:
     """
     Remove a monthly expiry from an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to remove the day.
-    date : pd.Timestamp
-        The date of the monthly expiry to remove.
+    date : Any
+        The date to remove. Must be convertible to pandas.Timestamp.
     strict : bool
         Whether to raise an error if the changeset for the exchange would be inconsistent after removing the day.
 
     Returns
     -------
     None
 
     Raises
     ------
-    ValueError
-        If the changeset for the exchange would be inconsistent after removing the day.
+    ValidationError
+        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
-    _remove_day(exchange, date, HolidaysAndSpecialSessions.MONTHLY_EXPIRY)
+    _remove_day(exchange, date, DayType.MONTHLY_EXPIRY, strict=strict)
+
+
+def reset_monthly_expiry(exchange: str, date: Any) -> None:
+    """
+    Clear a monthly expiry from an exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange key for which to clear the day.
+    date : Any
+        The date to clear. Must be convertible to pandas.Timestamp.
+
+    Returns
+    -------
+    None
+    """
+    _reset_day(exchange, date, DayType.MONTHLY_EXPIRY)
+
 
-    
 @_with_changeset
 def _reset_calendar(cs: ChangeSet) -> None:
     """
     Reset an exchange calendar to its original state.
 
     Parameters
     ----------
@@ -624,15 +771,15 @@
     None
     """
     _reset_calendar(exchange)
 
 
 @_with_changeset
 def _update_calendar(_: ChangeSet, changes: dict) -> ChangeSet:
-    return ChangeSet.from_dict(changes)
+    return ChangeSet(**changes)
 
 
 def update_calendar(exchange: str, changes: dict) -> None:
     """
     Apply changes to an exchange calendar.
 
     Parameters
@@ -644,32 +791,33 @@
     -------
     None
     """
     _update_calendar(exchange, changes)
 
 
 # Declare public names.
-__all__ = ["apply_extensions", "register_extension", "extend_class", "HolidaysAndSpecialSessions", "add_day",
-           "remove_day", "DaySpec", "DaySpecWithTime", "add_holiday", "remove_holiday", "add_special_close",
-           "remove_special_close", "add_special_open", "remove_special_open", "add_quarterly_expiry",
-           "remove_quarterly_expiry", "add_monthly_expiry", "remove_monthly_expiry", "reset_calendar",
-           "update_calendar", "ExtendedExchangeCalendar"]
+__all__ = ["apply_extensions", "remove_extensions", "register_extension", "extend_class", "DayType", "add_day",
+           "remove_day", "reset_day", "DaySpec", "DayWithTimeSpec", "add_holiday", "remove_holiday", "reset_holiday",
+           "add_special_close", "remove_special_close", "reset_special_close", "add_special_open",
+           "remove_special_open", "reset_special_open", "add_quarterly_expiry", "remove_quarterly_expiry",
+           "reset_quarterly_expiry", "add_monthly_expiry", "remove_monthly_expiry", "reset_monthly_expiry",
+           "reset_calendar", "update_calendar", "ExtendedExchangeCalendar", "ExchangeCalendarExtensions"]
 
 __version__ = None
 
 try:
     from importlib.metadata import version
     # get version from installed package
     __version__ = version("exchange_calendars_extensions")
 except ImportError:
     pass
 
 if __version__ is None:
     try:
-        # if package not installed, get version as set when package built
+        # if package not installed, get version as set when package built.
         from ._version import version
     except Exception:
         # If package not installed and not built, leave __version__ as None
         pass
     else:
         __version__ = version
```

### Comparing `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/changeset.py` & `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/changeset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,439 +1,323 @@
 import datetime as dt
-import itertools
 from copy import deepcopy
-from dataclasses import dataclass
-from enum import Enum
-from types import MappingProxyType
-from typing import Set, Generic, TypeVar, Any, Dict, TypedDict, Union, Optional
-from typing_extensions import Self
-
+from enum import Enum, unique
+from typing import Set, Generic, TypeVar, Dict, Union, Optional, Any
 
 import pandas as pd
-import schema as s
+from pydantic import BaseModel, Field, model_validator, ValidationInfo
+from pydantic.functional_validators import BeforeValidator
+from typing_extensions import Self, Annotated
 
-T = TypeVar('T')
 
+class DaySpec(BaseModel, extra='forbid'):
+    """
+    A model for a simple special day specification, for example, holidays.
+    """
+    name: str  # The name of the special day.
 
-@dataclass
-class Changes(Generic[T]):
+
+def _to_time(value: Union[dt.time, str]):
     """
-    Generic internal class to represent a set of changes to a calendar.
+    Convert value to time.
 
-    Changes consist of a set of dates to remove and a dictionary of dates to add. The type parameter T is the type of
-    the value for dates to add to the calendar. For example, for a holiday calendar, T would be a type containing
-    just the name of the holiday, while for special open/close days, T would be a type containing the name of the
-    special day and the open/close time.
+    Parameters
+    ----------
+    value : Union[dt.time, str]
+        The value to convert.
+
+    Returns
+    -------
+    dt.time
+        The converted value.
+
+    Raises
+    ------
+    ValueError
+        If the value cannot be converted to dt.time.
     """
+    if not isinstance(value, dt.time):
+        for f in ('%H:%M', '%H:%M:%S'):
+            try:
+                value = dt.datetime.strptime(value, f).time()
+                break
+            except ValueError:
+                pass
 
-    @property
-    def add(self) -> Dict[pd.Timestamp, T]:
-        # Return a read-only view of the dictionary of dates to add.
-        return MappingProxyType(self._add)
+        if not isinstance(value, dt.time):
+            raise ValueError(f'Failed to convert {value} to {dt.time}.')
 
-    @property
-    def remove(self) -> Set[pd.Timestamp]:
-        # Return a read-only view of the set of dates to remove.
-        return frozenset(self._remove)
+    return value
 
-    def __init__(self, schema: s.Schema) -> None:
-        """
-        Constructor.
 
-        Parameters
-        ----------
-        schema : Schema
-            The schema to use to validate the values to add.
+# A type alias for dt.time that allows initialisation from suitably formatted string values.
+TimeLike = Annotated[dt.time, BeforeValidator(_to_time)]
 
-        Returns
-        -------
-        None
-        """
-        # Save schema.
-        self._schema = schema
-        # Initialize properties.
-        self._add = dict()
-        self._remove = set()
 
-    def _remove_from_add(self, date: pd.Timestamp) -> None:
-        """
-        Remove a date from the dictionary of dates to add.
+class DayWithTimeSpec(BaseModel, extra='forbid'):
+    """
+    A model for a special day specification that includes a time, for example, special opens.
+    """
+    name: str  # The name of the special day.
+    time: TimeLike  # The open/close time of the special day.
 
-        Gracefully returns directly if the given date is not in the dictionary of dates to add.
 
-        Parameters
-        ----------
-        date : pd.Timestamp
-            The date to remove.
+DaySpecT = TypeVar('DaySpecT')
 
-        Returns
-        -------
-        None
-        """
-        # Check if holiday to remove is already in the dictionary of holidays to add.
-        if self._add.get(date) is not None:
-            # Remove element from the dictionary.
-            del self._add[date]
 
-    def _remove_from_remove(self, date: pd.Timestamp) -> None:
-        """
-        Remove a date from the set of dates to remove.
+def _to_timestamp(value: Union[pd.Timestamp, str]) -> pd.Timestamp:
+    """
+    Convert value to Pandas timestamp.
 
-        Gracefully returns directly if the given date is not in the set of dates to remove.
+    Parameters
+    ----------
+    value : Union[pd.Timestamp, str]
+        The value to convert.
 
-        Parameters
-        ----------
-        date : pd.Timestamp
-            The date to remove.
+    Returns
+    -------
+    pd.Timestamp
+        The converted value.
 
-        Returns
-        -------
-        None
-        """
-        # Check if holiday to add is already in the set of holidays to remove.
-        if date in self._remove:
-            # Remove the holiday from the set of holidays to remove.
-            self._remove.remove(date)
+    Raises
+    ------
+    ValueError
+        If the value cannot be converted to pd.Timestamp.
+    """
+    # Check if value is a valid timestamp.
+    if not isinstance(value, pd.Timestamp):
+        try:
+            # Convert value to timestamp.
+            value = pd.Timestamp(value)
+        except ValueError as e:
+            # Failed to convert key to timestamp.
+            raise ValueError(f'Failed to convert {value} to {pd.Timestamp}.') from e
+    return value
+
+
+# A type alias for pd.Timestamp that allows initialisation from suitably formatted string values.
+TimestampLike = Annotated[pd.Timestamp, BeforeValidator(_to_timestamp)]
+
+
+class Changes(BaseModel, Generic[DaySpecT], extra='forbid', arbitrary_types_allowed=True, validate_assignment=True):
+    """
+    Generic internal class to represent a set of calendar changes for a specific day type.
+
+    Changes consist of a set of dates to remove and a dictionary of dates to add. The type parameter T specifies the
+    properties to hold for the dates to add. For example, for a holiday calendar, T would be a type containing
+    just the name of the holiday. For special open/close days, T would be a type containing the name of the respective
+    special day and the associated open/close time.
+    """
+    add: Dict[TimestampLike, DaySpecT] = Field(default=dict())  # The dictionary of dates to add.
+    remove: Set[TimestampLike] = Field(default=set())  # The set of dates to remove.
+
+    # noinspection PyMethodParameters
+    @model_validator(mode='after')
+    def _validate_consistency(cls, info: Union[dict, 'Changes']) -> Any:
+        # Check if there are any dates that are both added and removed.
+        duplicates = info['add'].keys() & info['remove'] if isinstance(info, dict) else info.add.keys() & info.remove
+
+        if duplicates:
+            raise ValueError(f'Inconsistent changes: Dates {", ".join([d.date().isoformat() for d in duplicates])} are '
+                             f'both added and removed.')
 
-    def add_day(self, date: pd.Timestamp, value: T, strict: bool) -> Self:
+        return info
+
+    def add_day(self, date: TimestampLike, value: Union[DaySpecT, dict]) -> Self:
         """
         Add a date to the set of dates to add.
 
         If strict is True, raise ValueError if the given date is already in the set of days to remove. If strict is
         False, gracefully remove the date from the set of days to remove, if required, and then add it to the days to
         add. Effectively, setting strict to True raises an Exception before any inconsistent changes are made while
         setting strict to False enforces consistency by removing the date from the set of days to remove before adding.
 
         Adding the same day twice will overwrite the previous value without raising an exception.
 
         Parameters
         ----------
-        date : pd.Timestamp
-            The date to add.
+        date : Any
+            The date to add. Must be convertible to pandas.Timestamp.
         value : T
             The value to add.
-        strict : bool, optional
-            If True, raise ValueError if the given date is already in the set of days to remove. If False, gracefully
-            remove the date from the set of days to remove, if required, and then add it to the days to add.
 
         Returns
         -------
         Changes : self
 
         Raises
         ------
-        SchemaError
-            If the value does not match the schema.
-        ValueError
-            If strict is True and the given date is already in the set of days to remove.
+        ValidationError
+            If value is not of the expected type or adding date would make the changes inconsistent.
         """
-        # Validate value against schema.
-        value = self._schema.validate(value)
+        # Validate date.
+        date = TimestampLike(date)
 
-        # Ensure consistency by removing from days to remove, maybe.
-        if strict:
-            if date in self._remove:
-                raise ValueError(f'Date {date} is already in the set of days to remove.')
-        else:
-            self._remove_from_remove(date)
+        # Save previous value for key. Note that an existing value cannot be None, so we can use it to indicate absence.
+        previous = self.add.get(date, None)
+
+        # Add new key and value.
+        self.add[date] = value
+
+        try:
+            # Trigger validation.
+            self.add = self.add
+        except Exception as e:
+            if previous is None:
+                # Delete new entry.
+                del self.add[date]
+            else:
+                # Restore previous entry.
+                self.add[date] = previous
 
-        # Add the holiday to the set of holidays to add. Also overwrites any previous entry for the date.
-        self._add[date] = value
+            # Re-raise exception.
+            raise e
 
         return self
 
-    def remove_day(self, date: pd.Timestamp, strict: bool) -> Self:
+    def remove_day(self, date: TimestampLike) -> Self:
         """
         Add a date to the set of dates to remove.
 
         If strict is True, raise ValueError if the given date is already in the set of days to add. If strict is
         False, gracefully remove the date from the set of days to add, if required, and then add it to the days to
         remove. Effectively, setting strict to True raises an Exception before any inconsistent changes are made while
         setting strict to False enforces consistency by removing the date from the set of days to add before removing.
 
         Removing the same day twice will be a no-op without raising an exception.
 
         Parameters
         ----------
-        date : pd.Timestamp
-            The date to remove.
-        strict : bool, optional
-            If True, raise ValueError if the given date is already in the set of days to add. If False, gracefully
-            remove the date from the set of days to add, if required, and then add it to the days to remove.
+        date : Any
+            The date to remove. Must be convertible to pandas.Timestamp.
 
         Returns
         -------
         Changes : self
 
         Raises
         ------
-        ValueError
-            If strict is True and the given date is already in the set of days to add.
+        ValidationError
+            If removing date would make the changes inconsistent.
         """
-        # Ensure consistency by removing from days to add, maybe.
-        if strict:
-            if self._add.get(date) is not None:
-                raise ValueError(f'Date {date} is already in the set of days to add.')
-        else:
-            self._remove_from_add(date)
+        # Validate date.
+        date = TimestampLike(date)
 
-        # Add the holiday to the set of holidays to remove. Will be a no-op if the date is already in the set.
-        self._remove.add(date)
+        # Add the holiday to the set of holidays to remove.
+        self.remove.add(date)
+
+        try:
+            # Trigger validation.
+            self.remove = self.remove
+        except Exception as e:
+            # Remove the date from the set again. Since an exception was thrown, the date could not have been in the set
+            # in the first place.
+            self.remove.remove(date)
+
+            # Re-raise exception.
+            raise e
 
         return self
 
-    def clear_day(self, date: pd.Timestamp) -> Self:
+    def clear_day(self, date: TimestampLike) -> Self:
         """
         Reset a date so that it is neither in the set of dates to add nor the set of dates to remove.
 
         Parameters
         ----------
-        date : pd.Timestamp
-            The date to reset.
+        date : Any
+            The date to remove. Must be convertible to pandas.Timestamp.
 
         Returns
         -------
         Changes
             Self
         """
+        # Validate date.
+        date = TimestampLike(date)
+
         # Remove the holiday from the set of holidays to add.
-        self._remove_from_add(date)
+
+        # Check if holiday to remove is already in the dictionary of holidays to add.
+        if self.add.get(date) is not None:
+            # Remove element from the dictionary.
+            del self.add[date]
 
         # Remove the holiday from the set of holidays to remove.
-        self._remove_from_remove(date)
+
+        # Check if holiday to add is already in the set of holidays to remove.
+        if date in self.remove:
+            # Remove the holiday from the set of holidays to remove.
+            self.remove.remove(date)
 
         return self
 
     def clear(self) -> Self:
         """
         Clear all changes.
 
         Returns
         -------
         Changes : self
         """
-        self._add.clear()
-        self._remove.clear()
+        self.add.clear()
+        self.remove.clear()
 
         return self
 
-    def is_consistent(self) -> bool:
-        """
-        Return whether the changes are consistent.
+    def __len__(self) -> int:
+        return len(self.add) + len(self.remove)
 
-        Changes are consistent if and only if dates to add and dates to remove do not overlap.
-
-        Returns
-        -------
-        bool
-            True if the changes are consistent, False otherwise.
-        """
-        # Check if any dates are in both the set of holidays to add and the set of holidays to remove.
-        return len(self.add.keys() & self.remove) == 0
-
-    def is_empty(self) -> bool:
-        """
-        Check if the changes are empty.
-
-        Changes are empty when both the set of dates to add and the set of dates to remove are empty.
-
-        Returns
-        -------
-        bool
-            True if the changes are empty, False otherwise.
-        """
-        return len(self.add) == 0 and len(self.remove) == 0
+    def __bool__(self):
+        return len(self) > 0
 
     def __eq__(self, other) -> bool:
         # Check if other is an instance of Changes.
         if not isinstance(other, Changes):
             return False
 
         # Check if the dictionaries of dates to add and the sets of dates to remove are both equal.
         return self.add == other.add and self.remove == other.remove
 
-    def __copy__(self):
-        c = Changes()
-        c._add = self._add
-        c_remove = self._remove
-        return c
-
-    def __deepcopy__(self, memo):
-        c = Changes(self._schema)
-        c._add = deepcopy(self._add, memo)
-        c._remove = deepcopy(self._remove, memo)
-        return c
-
-    @staticmethod
-    def _format_dict(d: Dict[pd.Timestamp, T]) -> str:
-        """
-        Format a dictionary of dates to values as a string.
-
-        Parameters
-        ----------
-        d : Dict[pd.Timestamp, T]
-            The dictionary to format.
-
-        Returns
-        -------
-        str
-            The formatted string.
-        """
-        return '{' + ', '.join([f'{k.date().isoformat()}: {v}' for k, v in d.items()]) + '}'
-
-    @staticmethod
-    def _format_set(s: Set[pd.Timestamp]) -> str:
-        """
-        Format a set of dates as a string.
 
-        Parameters
-        ----------
-        s : Set[pd.Timestamp]
-            The set to format.
-
-        Returns
-        -------
-        str
-            The formatted string.
-        """
-        return '{' + ', '.join([d.date().isoformat() for d in s]) + '}'
-
-    def __str__(self) -> str:
-        return f'Changes(add={self._format_dict(self._add)}, remove={self._format_set(self._remove)})'
-
-
-def _to_time(input: Union[str, dt.time]) -> dt.time:
-    """
-    Gracefully convert an input value to a datetime.time.
-
-    Parameters
-    ----------
-    input : Union[str, dt.time]
-        The input value to convert.
-
-    Returns
-    -------
-    dt.time
-        The converted value.
-
-    Raises
-    ------
-    ValueError
-        If the input value cannot be converted to a datetime.time.
-    """
-    if isinstance(input, dt.time):
-        return input
-    try:
-        return dt.datetime.strptime(input, '%H:%M').time()
-    except ValueError:
-        return dt.datetime.strptime(input, '%H:%M:%S').time()
-    
-
-def _to_timestamp(input: Union[str, pd.Timestamp]) -> pd.Timestamp:
-    """
-    Gracefully convert an input value to a pandas.Timestamp.
-
-    Parameters
-    ----------
-    input : Union[str, pd.Timestamp]
-        The input value to convert.
-
-    Returns
-    -------
-    pd.Timestamp
-        The converted value.
-
-    Raises
-    ------
-    ValueError
-        If the input value cannot be converted to a pandas.Timestamp.
-    """
-    if isinstance(input, pd.Timestamp):
-        return input
-    return pd.Timestamp(input)
-
-
-# Define types and schemas for the different types of holidays and special sessions.
-DaySpec = TypedDict('DAY_SPEC', {'name': str})
-_DaySchema = s.Schema({'name': str})
-DaySpecWithTime = TypedDict('DAY_SPEC_WITH_TIME', {'name': str, 'time': dt.time})
-_DayWithTimeSchema = s.Schema({'name': str, 'time': s.Use(_to_time)})
-
-
-class HolidaysAndSpecialSessions(Enum):
+@unique
+class DayType(str, Enum):
     """
     Enum for the different types of holidays and special sessions.
 
     HOLIDAY: A holiday.
     SPECIAL_OPEN: A special session with a special opening time.
     SPECIAL_CLOSE: A special session with a special closing time.
     MONTHLY_EXPIRY: A monthly expiry.
     QUARTERLY_EXPIRY: A quarterly expiry.
+    """
+    HOLIDAY = 'holiday'
+    SPECIAL_OPEN = 'special_open'
+    SPECIAL_CLOSE = 'special_close'
+    MONTHLY_EXPIRY = 'monthly_expiry'
+    QUARTERLY_EXPIRY = 'quarterly_expiry'
 
-    Each enum value is a tuple of the following form:
-    (id, type, schema)
-    where
-    id: int
-        Unique int to ensure enum value uniqueness.
-    type: Type[Union[DaySpec, DaySpecWithTime]]
-        Type of the value of the enum value.
-    schema: Schema
-        Schema for the value of the enum value.
-    """
-    HOLIDAY = (1, DaySpec, _DaySchema)
-    SPECIAL_OPEN = (2, DaySpecWithTime, _DayWithTimeSchema)
-    SPECIAL_CLOSE = (3, DaySpecWithTime, _DayWithTimeSchema)
-    MONTHLY_EXPIRY = (4, DaySpec, _DaySchema)
-    QUARTERLY_EXPIRY = (5, DaySpec, _DaySchema)
-
-    @staticmethod
-    def to_enum(key: Union[str, 'HolidaysAndSpecialSessions']):
-        """
-        Return the enum value corresponding to the given key. Case-insensitive.
-
-        Parameters
-        ----------
-        key : Union[str, HolidaysAndSpecialSessions]
-            The key to look up.
-
-        Returns
-        -------
-        HolidaysAndSpecialSessions
-            The enum value corresponding to the given key.
-        """
-        if isinstance(key, HolidaysAndSpecialSessions):
-            return key
-
-        return HolidaysAndSpecialSessions[key.upper()]
 
-    def __copy__(self):
-        # Enums are immutable, so return self.
-        return self
+def _to_day_type(value: Union[DayType, str]) -> DayType:
+    if not isinstance(value, DayType):
+        try:
+            # Lookup via lower-case value.
+            value = DayType(value.lower())
+        except ValueError as e:
+            # Failed to convert value to DayType.
+            raise ValueError(f'Failed to convert {value} to {DayType}.') from e
 
-    def __deepcopy__(self, memodict={}):
-        # Enums are immutable, so return self.
-        return self
+    return value
 
 
-# Define a schema for a dictionary to represent a changeset containing changes to an exchange calendar. Note that the
-# schema only defines the expected structure, i.e. the keys and the types of the values. It does not validate the values
-# themselves. A dictionary that is valid with respect to this schema may still contain an invalid combination of dates.
-# For example, it may contain a date that is in the set of dates to add for two different types of days like holidays
-# and special open. This is obviously inconsistent as the same day can only be one of those two types of days.
-_SCHEMA = s.Schema({
-    s.Optional('holiday'): {s.Optional('add'): [{'date': s.Use(_to_timestamp), 'value': _DaySchema}], s.Optional('remove'): [s.Use(_to_timestamp)]},
-    s.Optional('special_open'): {s.Optional('add'): [{'date': s.Use(_to_timestamp), 'value': _DayWithTimeSchema}], s.Optional('remove'): [s.Use(_to_timestamp)]},
-    s.Optional('special_close'): {s.Optional('add'): [{'date': s.Use(_to_timestamp), 'value': _DayWithTimeSchema}], s.Optional('remove'): [s.Use(_to_timestamp)]},
-    s.Optional('monthly_expiry'): {s.Optional('add'): [{'date': s.Use(_to_timestamp), 'value': _DaySchema}], s.Optional('remove'): [s.Use(_to_timestamp)]},
-    s.Optional('quarterly_expiry'): {s.Optional('add'): [{'date': s.Use(_to_timestamp), 'value': _DaySchema}], s.Optional('remove'): [s.Use(_to_timestamp)]},
-})
+# A type alias for DayType that allows initialisation from suitably formatted string values.
+DayTypeLike = Annotated[DayType, BeforeValidator(DayType.HOLIDAY)]
 
 
-@dataclass
-class ChangeSet:
+class ChangeSet(BaseModel, extra='forbid', validate_assignment=True):
     """
     Represents a modification to an existing exchange calendar.
 
     A changeset consists of a set of dates to add and a set of dates to remove, respectively, for each of the following
     types of days:
     - holidays
     - special open
@@ -469,216 +353,159 @@
     To resolve this issue, the date 2020-01-01 could be added to the changeset, respectively, for all day types (except
     special opens) as a day to remove. Now, if the changeset is applied to the original calendar, 2020-01-01 will no
     longer be a holiday and therefore no longer conflict with the new special open day. This form of sanitization
     ensures that a consistent changeset can be applied safely to any exchange calendar. Effectively, normalization
     ensures that adding a new day for a given day type becomes an upsert operation, i.e. the day is added if it does not
     already exist in any day type category, and updated/moved to the new day type if it does.
     """
+    holiday: Changes[DaySpec] = Changes[DaySpec]()
+    special_open: Changes[DayWithTimeSpec] = Changes[DayWithTimeSpec]()
+    special_close: Changes[DayWithTimeSpec] = Changes[DayWithTimeSpec]()
+    monthly_expiry: Changes[DaySpec] = Changes[DaySpec]()
+    quarterly_expiry: Changes[DaySpec] = Changes[DaySpec]()
+
+    # noinspection PyMethodParameters
+    @model_validator(mode='after')
+    def _validate_consistency(cls, info: ValidationInfo) -> ValidationInfo:
+        # Maps each date to add to the corresponding day type(s) it appears in.
+        date2day_types = dict()
+
+        for day_type in cls.model_fields.keys():
+            c: Changes = info[day_type] if isinstance(info, dict) else getattr(info, day_type)
+            dates = c.add.keys()
+            for d in dates:
+                date2day_types[d] = date2day_types.get(d, set()) | {day_type}
+
+        # Remove all entries from date2day_types that only appear in one day type.
+        date2day_types = {k: v for k, v in date2day_types.items() if len(v) > 1}
+
+        # Check if there are any dates that appear in multiple day types.
+        if len(date2day_types) > 0:
+            raise ValueError(f'Inconsistent changes: Dates '
+                             f'{", ".join([d.date().isoformat() for d in date2day_types.keys()])} are each added for '
+                             f'more than one day type.')
 
-    @property
-    def changes(self) -> Dict[HolidaysAndSpecialSessions, Changes[Union[DaySpec, DaySpecWithTime]]]:
-        """
-        The changes.
-
-        Returns
-        -------
-        Dict[HolidaysAndSpecialSessions, Changes[Any]]
-            The changes.
-        """
-        # Return a read-only view of the _changes dictionary.
-        return MappingProxyType(self._changes)
-
-    def __init__(self) -> None:
-        """
-        Initialize a new instance of ChangeSet.
-        """
-        # Initialize the _changes dictionary.
-        self._changes: Dict[HolidaysAndSpecialSessions, Changes[Any]] = {k: Changes[k.value[1]](schema=k.value[2]) for k in HolidaysAndSpecialSessions}
+        return info
 
-    def clear_day(self, date: pd.Timestamp, day_type: Optional[HolidaysAndSpecialSessions] = None) -> Self:
-        """
-        Clear a day from the change set.
-
-        Parameters
-        ----------
-        date : pd.Timestamp
-            The date to clear.
-        day_type : Optional[HolidaysAndSpecialSessions]
-            The day type to clear. If None, all day types will be cleared.
-
-        Returns
-        -------
-        ExchangeCalendarChangeSet : self
-        """
-        if day_type is None:
-            # Clear for all day types.
-            for c in self.changes.values():
-                c.clear_day(date)
-        else:
-            # Clear for the given day type.
-            self.changes[day_type].clear_day(date)
-
-        return self
-
-    def clear(self) -> Self:
-        """
-        Clear all changes.
-
-        Returns
-        -------
-        ExchangeCalendarChangeSet : self
-        """
-        # Clear all changes for all day types.
-        for c in self.changes.values():
-            c.clear()
-
-        return self
-
-    def add_day(self, date: pd.Timestamp, value: Any, day_type: HolidaysAndSpecialSessions, strict: bool = False) -> Self:
+    def add_day(self, date: Any, value: Union[DaySpec, DayWithTimeSpec, dict], day_type: DayTypeLike) -> Self:
         """
         Add a day to the change set.
 
         Parameters
         ----------
-        date : pd.Timestamp
-            The date to add.
+        date : Any
+            The date to add. Must be convertible to pandas.Timestamp.
         value : Any
             The value to add.
-        day_type : HolidaysAndSpecialSessions
+        day_type : Union[str, DayType]
             The day type to add.
-        strict : bool
-            If True, raise ValueError if adding the given date would make the changeset inconsistent. If False, ensure
-            that the changeset remains consistent with the day added, by removing the date anywhere else in the
-            changeset, where required.
 
         Returns
         -------
         ExchangeCalendarChangeSet : self
         """
-        # Check if the given date is already added somewhere.
-        is_added = any(date in c.add.keys() and k != day_type for k, c in self.changes.items())
+        # Convert to string representation.
+        day_type = DayTypeLike(day_type).value
+
+        # Add day to set of changes for day type. If this fails, the set of changes should be unmodified as a result, so
+        # that the changeset remains consistent. Just let the exception bubble up.
+        getattr(self, day_type).add_day(date, value)
 
-        # Exit early if strict is True and the date is already added somewhere.
-        if strict and is_added:
-            raise ValueError(f'Adding the given date {date} for day type {day_type} would make the changeset inconsistent.')
-
-        # Add the day to the change set. This may raise ValueError if the date is already in the days to remove for the
-        # given day type.
-        self.changes[day_type].add_day(date, value, strict)
-
-        if not strict and is_added:
-            # Remove the date from the changeset for all other day types.
-            for k, c in self.changes.items():
-                if k != day_type and date in c.add.keys():
-                    c.clear_day(date)
+        # If we get here, then the day has been added to the set of changes successfully.
+
+        # Trigger validation of the entire changeset.
+        try:
+            setattr(self, day_type, getattr(self, day_type))
+        except Exception as e:
+            # If the changeset is no longer consistent, then this can only be because the day was already a day to
+            # add for another day type before and this call added it to the given day type as well, leading to an
+            # invalid second add entry.
+
+            # Restore the state before the call by clearing the day from the given day type.
+            getattr(self, day_type).clear_day(date)
+
+            # Let exception bubble up.
+            raise e
 
         return self
 
-    def remove_day(self, date: pd.Timestamp, day_type: Optional[HolidaysAndSpecialSessions] = None, strict: bool = False) -> Self:
+    def remove_day(self, date: Any, day_type: Optional[DayTypeLike] = None) -> Self:
         """
         Remove a day from the change set.
 
         Parameters
         ----------
-        date : pd.Timestamp
-            The date to remove.
-        day_type : HolidaysAndSpecialSessions
+        date : Any
+            The date to add. Must be convertible to pandas.Timestamp.
+        day_type : Union[str, DayType]
             The day type to remove.
-        strict : bool
-            If True, raise ValueError if removing the given date would make the changeset inconsistent. If False, ensure
-            that the changeset remains consistent by removing the day from the dates to add for any day type where it is
-            going to be added to the days to remove.
 
         Returns
         -------
         ExchangeCalendarChangeSet : self
 
         Raises
         ------
         ValueError
             If removing the given date would make the changeset inconsistent.
         """
-        if day_type is not None:
-            self.changes[day_type].remove_day(date, strict)
-        else:
-            # Remove for all day types.
-            for c in self.changes.values():
-                c.remove_day(date, strict)
+        # Determine which day types to remove day from.
+        day_types = (DayTypeLike(day_type).value,) if day_type is not None else tuple(self.model_fields.keys())
 
-        return self
+        for k in day_types:
+            getattr(self, k).remove_day(date)
 
-    def is_empty(self):
-        """
-        Return True if there are no changes.
-
-        Returns
-        -------
-        bool
-            True if there are no changes.
-        """
-        return not any(changes.add or changes.remove for changes in self.changes.values())
+        return self
 
-    def is_consistent(self):
+    def clear_day(self, date: Any, day_type: Optional[DayTypeLike] = None) -> Self:
         """
-        Return True if the change set is consistent.
+        Clear a day from the change set.
 
-        A change set is consistent iff
-        - the dates of all days to add do not overlap across the different day types, and
-        - the dates to add and the days to remove do not overlap for each day type, respectively.
+        Parameters
+        ----------
+        date : Any
+            The date to add. Must be convertible to pandas.Timestamp.
+        day_type : Optional[Union[str, DayType]]
+            The day type to clear. If None, all day types will be cleared.
 
         Returns
         -------
-        bool
-            True if the change set is consistent, False otherwise.
+        ExchangeCalendarChangeSet : self
         """
-        # Check if all contained changes are consistent for each day type.
-        if not all(changes.is_consistent() for changes in self.changes.values()):
-            return False
+        # Determine which day types to clear.
+        day_types = (DayTypeLike(day_type).value,) if day_type is not None else tuple(self.model_fields.keys())
 
-        # Get all dates to add.
-        dates_to_add = sorted(list(itertools.chain.from_iterable(changes.add.keys() for changes in self.changes.values())))
-
-        # Check if there are any overlapping dates to add.
-        if len(dates_to_add) != len(set(dates_to_add)):
-            # Duplicates in the dates to add. This is invalid since the same day cannot be added multiple times with a
-            # different day type each.
-            return False
-
-        if any([changes.add.keys() & changes.remove for changes in self.changes.values()]):
-            return False
+        for k in day_types:
+            # Clear for the given day type.
+            getattr(self, k).clear_day(date)
 
-        return True
+        return self
 
-    def __copy__(self) -> 'ChangeSet':
+    def clear(self) -> Self:
         """
-        Return a shallow copy of the change set.
+        Clear all changes.
 
         Returns
         -------
-        ChangeSet
-            The shallow copy.
+        ExchangeCalendarChangeSet : self
         """
-        cs = ChangeSet()
-        cs._changes = self.changes
+        # Clear all changes for all day types.
+        for k in self.model_fields.keys():
+            getattr(self, k).clear()
 
-        return cs
+        return self
 
-    def __deepcopy__(self, memo) -> 'ChangeSet':
-        """
-        Return a deep copy of the change set.
+    def __len__(self):
+        return sum(len(getattr(self, k)) for k in self.model_fields.keys())
 
-        Returns
-        -------
-        ChangeSet
-            The deep copy.
-        """
-        cs = ChangeSet()
-        cs._changes = deepcopy(self._changes)
+    def __eq__(self, other):
+        if not isinstance(other, ChangeSet):
+            return False
 
-        return cs
+        return all(getattr(self, k) == getattr(other, k) for k in self.model_fields.keys())
 
     def normalize(self, inplace: bool = False) -> Self:
         """
         Normalize the change set.
 
         A change set is normalized if
         1) It is consistent.
@@ -697,78 +524,19 @@
         if inplace:
             # This instance.
             cs: ChangeSet = self
         else:
             # A copy of this instance.
             cs: ChangeSet = deepcopy(self)
 
-        for day_type in HolidaysAndSpecialSessions:
+        for day_type in DayType:
             # Get the dates to add for the day type.
-            dates_to_add = cs._changes[day_type].add.keys()
+            dates_to_add = getattr(cs, day_type).add.keys()
+
             # Loop over all day types.
-            for day_type0 in HolidaysAndSpecialSessions:
+            for day_type0 in DayType.__members__.values():
                 if day_type0 != day_type:
                     # Add the dates to add for day_type to the dates to remove for day_type0.
                     for date in dates_to_add:
-                        cs.remove_day(date, day_type0, strict=True)
-
-        return cs
-
-    def __eq__(self, other):
-        if not isinstance(other, ChangeSet):
-            return False
-
-        return self.changes == other.changes
-
-    def __str__(self):
-        changes_str = ", ".join([f'{k.name}: {c}' for k, c in self.changes.items() if not c.is_empty()])
-        return f'ChangeSet({changes_str})'
-
-    @classmethod
-    def from_dict(cls, d: dict) -> "ChangeSet":
-        """
-        Create a change set from a dictionary.
-
-        The changes represented by the input dictionary need to result in a consistent change set. Otherwise, a
-        ValueError is raised.
-
-        Parameters
-        ----------
-        d : dict
-            The dictionary to create the change set from.
-
-        Returns
-        -------
-        ExchangeCalendarChangeSet
-            The created change set.
-
-        Raises
-        ------
-        ValueError
-            If the given dictionary does not represent a consistent change set.
-        """
-        try:
-            # Validate the input dictionary.
-            d = _SCHEMA.validate(d)
-        except Exception as e:
-            raise ValueError(f"Dictionary does not satisfy expected schema.") from e
-
-        # Create empty change set.
-        cs: ChangeSet = cls()
-
-        # Add the changes for each day type.
-        for day_type_str, changes_incoming in d.items():
-            try:
-                # Convert the day type string to the corresponding enum value.
-                day_type: HolidaysAndSpecialSessions = HolidaysAndSpecialSessions.to_enum(day_type_str)
-            except ValueError as e:
-                raise ValueError(f"Invalid day type '{day_type_str}' in dictionary.") from e
-
-            if changes_incoming.get('add') is not None:
-                for item in changes_incoming.get('add'):
-                    cs.add_day(date=item['date'], value=item['value'], day_type=day_type, strict=True)
-
-            if changes_incoming.get('remove') is not None:
-                for date in changes_incoming.get('remove'):
-                    cs.remove_day(date=date, day_type=day_type, strict=True)
+                        cs.remove_day(date, day_type0)
 
         return cs
```

### Comparing `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/holiday.py` & `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/holiday_calendar.py` & `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/holiday_calendar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
 from abc import ABC
+from copy import copy
 from dataclasses import field, dataclass
 from functools import reduce
 from typing import Iterable, Optional, Callable, Union, Type, Protocol, List, Tuple, runtime_checkable
 
 import pandas as pd
 from exchange_calendars import ExchangeCalendar
 from exchange_calendars.exchange_calendar import HolidayCalendar as ExchangeCalendarsHolidayCalendar
 from exchange_calendars.pandas_extensions.holiday import Holiday
 from exchange_calendars.pandas_extensions.holiday import Holiday as ExchangeCalendarsHoliday
 from pandas.tseries.holiday import Holiday as PandasHoliday
 
-from exchange_calendars_extensions import ChangeSet, HolidaysAndSpecialSessions
+from exchange_calendars_extensions import ChangeSet
 from exchange_calendars_extensions.holiday import get_monthly_expiry_holiday, DayOfWeekPeriodicHoliday, \
     get_last_day_of_month_holiday
-from exchange_calendars_extensions.observance import get_roll_backward_observance
 
 
 class HolidayCalendar(ExchangeCalendarsHolidayCalendar):
     """
     A subclass of exchange_calendars.exchange_calendar.HolidayCalendar that supports overlapping rules, i.e. rules that
     apply to the same date.
 
@@ -41,39 +41,101 @@
         # Drop duplicates, keeping the first occurrence.
         if return_name:
             return holidays[~holidays.index.duplicated()]
         else:
             return holidays.drop_duplicates()
 
 
+def get_conflicts(holidays_dates: List[pd.Timestamp], other_holidays: pd.DatetimeIndex, weekend_days: Iterable[int]) -> List[int]:
+    """
+    Get the indices of holidays that coincide with holidays from the other calendar or the given weekend days.
+
+    Parameters
+    ----------
+    holidays_dates : List[pd.Timestamp]
+        The dates of the holidays.
+    other_holidays : pd.DatetimeIndex
+        The dates of the holidays from the other calendar.
+    weekend_days : Iterable[int]
+        The days of the week that are considered weekend days.
+
+    Returns
+    -------
+    List[int]
+        The indices of holidays that coincide with holidays from the other calendar or the given weekend days.
+    """
+
+    # Determine the indices of holidays that coincide with holidays from the other calendar.
+    return [i for i in range(len(holidays_dates)) if holidays_dates[i] in other_holidays or holidays_dates[i].weekday() in weekend_days]
+
+
+class AdjustedHolidayCalendar(ExchangeCalendarsHolidayCalendar):
+
+    def __init__(self, rules, other: ExchangeCalendarsHolidayCalendar, weekmask: str) -> None:
+        super().__init__(rules=rules)
+        self.other = other
+        self.weekend_days = {d for d in range(7) if weekmask[d] == '0'}
+
+    def holidays(self, start=None, end=None, return_name=False):
+        # Get the holidays from the parent class.
+        holidays = super().holidays(start=start, end=end, return_name=return_name)
+
+        # Get the holidays from the other calendar.
+        other_holidays = self.other.holidays(start=start, end=end, return_name=False)
+
+        holidays_dates = list(holidays.index if return_name else holidays)
+
+        conflicts = get_conflicts(holidays_dates, other_holidays, self.weekend_days)
+
+        if len(conflicts) == 0:
+            return holidays
+
+        while True:
+            # For each index of a conflicting holiday, adjust the date by one day into the past.
+            for i in conflicts:
+                holidays_dates[i] = holidays_dates[i] - pd.Timedelta(days=1)
+
+            conflicts = get_conflicts(holidays_dates, other_holidays, self.weekend_days)
+
+            if len(conflicts) == 0:
+                break
+
+        holidays_index = pd.DatetimeIndex(holidays_dates)
+
+        if return_name:
+            return pd.Series(holidays.values, index=holidays_index)
+        else:
+            return holidays_index
+
+
 def get_holiday_calendar_from_timestamps(timestamps: Iterable[pd.Timestamp],
-                                         name: Optional[str] = None) -> HolidayCalendar:
+                                         name: Optional[str] = None) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with holidays given by a collection of timestamps.
 
     If name is specified, each holiday will use that given name.
 
     Parameters
     ----------
     timestamps : Iterable[pd.Timestamp]
         The timestamps of the holidays.
     name : Optional[str], optional
         The name to use for each holiday, by default None.
 
     Returns
     -------
-    HolidayCalendar
+    ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar object as specified.
     """
     # Generate list of rules, one for each timestamp.
-    rules = [Holiday(name, year=ts.year, month=ts.month, day=ts.day) for ts in
-             list(dict.fromkeys(timestamps))]  # As of Python 3.7, dict preserves insertion order.
+    rules = [Holiday(name, year=ts.year, month=ts.month, day=ts.day, start_date=ts, end_date=ts) for ts in
+             set(dict.fromkeys(timestamps))]  # As of Python 3.7, dict preserves insertion order.
 
     # Return a new HolidayCalendar with the given rules.
-    return HolidayCalendar(rules=rules)
+    return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
 def get_holiday_calendar_from_day_of_week(day_of_week: int, name: Optional[str] = None) -> HolidayCalendar:
     """
     Return a holiday calendar with a periodic holiday occurring on each instance of the given day of the week.
 
     Parameters
@@ -86,61 +148,61 @@
     # Generate list of rules. Actually contains only one rule for the given day of the week.
     rules = [DayOfWeekPeriodicHoliday(name, day_of_week)]
 
     # Return a new HolidayCalendar with the given rules.
     return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
-def merge_calendars(calendars: Iterable[HolidayCalendar]) -> HolidayCalendar:
+def merge_calendars(calendars: Iterable[ExchangeCalendarsHolidayCalendar]) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all holidays from the given calendars merged into a single HolidayCalendar.
 
     The rules of the returned calendar will be the concatenation of the rules of the given calendars. Note that rules
     that occur earlier take precedence in case of conflicts, i.e. rules that apply to the same date.
     """
     x = reduce(lambda x, y: HolidayCalendar(rules=[r for r in x.rules] + [r for r in y.rules]), calendars,
-               HolidayCalendar(rules=[]))
+               ExchangeCalendarsHolidayCalendar(rules=[]))
     return x
 
 
-def get_holidays_calendar(exchange_calendar: ExchangeCalendar) -> HolidayCalendar:
+def get_holidays_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
     """
-    Return a holiday calendar with all holidays, regular and ad-hoc, from the given exchange calendar merged into a single
-    HolidayCalendar.
+    Return a holiday calendar with all holidays, regular and ad-hoc, from the given exchange calendar merged into a
+    single calendar.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
         The exchange calendar to use.
 
     Returns
     -------
-    HolidayCalendar
+    ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar with all holidays from the given EchangeCalendar.
     """
     holiday_calendars = [get_holiday_calendar_from_timestamps(exchange_calendar.adhoc_holidays, name='ad-hoc holiday'),
                          exchange_calendar.regular_holidays]
 
     # Merge all calendars by reducing the list of calendars into one, calling the merge method on each pair.
     return merge_calendars(holiday_calendars)
 
 
-def get_special_opens_calendar(exchange_calendar: ExchangeCalendar) -> HolidayCalendar:
+def get_special_opens_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
     """
-    Return a holiday calendar with all special opens, regular and ad-hoc, from the given exchange calendar merged into a single
-    HolidayCalendar.
+    Return a holiday calendar with all special opens, regular and ad-hoc, from the given exchange calendar merged into a
+    single calendar.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
         The exchange calendar to use.
 
     Returns
     -------
-    HolidayCalendar
+    ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar with all special opens from the given EchangeCalendar.
     """
     holiday_calendars = []
 
     # Add ad-hoc special opens.
     for item in exchange_calendar.special_opens_adhoc:
         _, definition = item
@@ -154,27 +216,27 @@
         elif isinstance(definition, int):
             holiday_calendars.append(get_holiday_calendar_from_day_of_week(definition, name='special open'))
 
     # Merge all calendars by reducing the list of calendars into one, calling the merge method on each pair.
     return merge_calendars(holiday_calendars)
 
 
-def get_special_closes_calendar(exchange_calendar: ExchangeCalendar) -> HolidayCalendar:
+def get_special_closes_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
     """
-    Return a holiday calendar with all special closes, regular and ad-hoc, from the given exchange calendar merged into a single
-    HolidayCalendar.
+    Return a holiday calendar with all special closes, regular and ad-hoc, from the given exchange calendar merged into
+    a single calendar.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
         The exchange calendar to use.
 
     Returns
     -------
-    HolidayCalendar
+    ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar with all special closes from the given EchangeCalendar.
     """
     holiday_calendars = []
 
     # Add ad-hoc special closes.
     for item in exchange_calendar.special_closes_adhoc:
         _, definition = item
@@ -188,195 +250,192 @@
         elif isinstance(definition, int):
             holiday_calendars.append(get_holiday_calendar_from_day_of_week(definition, name='special close'))
 
     # Merge all calendars by reducing the list of calendars into one, calling the merge method on each pair.
     return merge_calendars(holiday_calendars)
 
 
-def get_weekend_days_calendar(exchange_calendar: ExchangeCalendar) -> HolidayCalendar:
+def get_weekend_days_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all weekend days from the given exchange calendar as holidays.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
         The exchange calendar to use.
 
     Returns
     -------
-    HolidayCalendar
+    ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar with all weekend days from the given EchangeCalendar.
     """
     rules = [DayOfWeekPeriodicHoliday('weekend day', day_of_week) for day_of_week, v in
              enumerate(exchange_calendar.weekmask) if v == '0']
     return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
-def get_monthly_expiry_calendar(day_of_week: int,
-                                observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None) -> HolidayCalendar:
+def get_monthly_expiry_rules(day_of_week: int,
+                             observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None) -> List[Holiday]:
     """
-    Return a holiday calendar with a holiday for each month's expiry, but excluding quarterly expiry days.
+    Return a list of rules for a calendar with a holiday for each month's expiry, but excluding quarterly expiry days.
 
     Parameters
     ----------
     day_of_week : int
         The day of the week to use, where 0 is Monday and 6 is Sunday.
     observance : Optional[Callable[[pd.Timestamp], pd.Timestamp]], optional
         The observance function to use, by default None.
 
     Returns
     -------
-    HolidayCalendar
-        A new HolidayCalendar with a holiday for each month's expiry, but excluding quarterly expiry days.
+    List[Holiday]
+        A list of rules for a calendar with a holiday for each month's expiry, but excluding quarterly expiry days.
     """
-    rules = [get_monthly_expiry_holiday('monthly expiry', day_of_week, month, observance) for month in
+    return [get_monthly_expiry_holiday('monthly expiry', day_of_week, month, observance) for month in
              [1, 2, 4, 5, 7, 8, 10, 11]]
-    return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
-def get_quadruple_witching_calendar(day_of_week: int, observance: Optional[
-    Callable[[pd.Timestamp], pd.Timestamp]] = None) -> HolidayCalendar:
+def get_quadruple_witching_rules(day_of_week: int,
+                                 observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None) -> List[Holiday]:
     """
-    Return a holiday calendar with a holiday for each quarterly expiry aka quadruple witching.
+    Return a list of rules for a calendar with a holiday for each quarterly expiry aka quadruple witching.
 
     Parameters
     ----------
     day_of_week : int
         The day of the week to use, where 0 is Monday and 6 is Sunday.
     observance : Optional[Callable[[pd.Timestamp], pd.Timestamp]], optional
         The observance function to use, by default None.
 
     Returns
     -------
-    HolidayCalendar
-        A new HolidayCalendar with a holiday for each quarterly expiry.
+    List[Holiday]
+        A list of rules for a calendar with a holiday for each quarterly expiry aka quadruple witching.
     """
-    rules = [get_monthly_expiry_holiday('quarterly expiry', day_of_week, month, observance) for month in [3, 6, 9, 12]]
-    return ExchangeCalendarsHolidayCalendar(rules=rules)
+    return [get_monthly_expiry_holiday('quarterly expiry', day_of_week, month, observance) for month in [3, 6, 9, 12]]
 
 
-def get_last_day_of_month_calendar(name: Optional[str] = 'last trading day of month', observance: Optional[
-    Callable[[pd.Timestamp], pd.Timestamp]] = None) -> HolidayCalendar:
+def get_last_day_of_month_rules(name: Optional[str] = 'last trading day of month', observance: Optional[
+    Callable[[pd.Timestamp], pd.Timestamp]] = None) -> List[Holiday]:
     """
-    Return a holiday calendar with a holiday for each last trading day of the month.
+    Return a list of rules for a calendar with a holiday for each last trading day of the month.
 
     Parameters
     ----------
     name : Optional[str], optional
         The name to use for the holidays, by default 'last trading day of month'.
     observance : Optional[Callable[[pd.Timestamp], pd.Timestamp]], optional
         The observance function to use, by default None.
 
     Returns
     -------
-    HolidayCalendar
-        A new HolidayCalendar with a holiday for each last trading day of the month.
+    List[Holiday]
+        A list of rules for a calendar with a holiday for each last trading day of the month.
     """
-    rules = [get_last_day_of_month_holiday(name, i, observance=observance) for i in range(1, 13)]
-    return ExchangeCalendarsHolidayCalendar(rules=rules)
+    return [get_last_day_of_month_holiday(name, i, observance=observance) for i in range(1, 13)]
 
 
 @runtime_checkable
 class ExchangeCalendarExtensions(Protocol):
     """
     A protocol for extensions to the exchange_calendars.ExchangeCalendar class.
     """
 
     @property
-    def weekend_days(self) -> HolidayCalendar:
+    def weekend_days(self) -> ExchangeCalendarsHolidayCalendar:
         """
         Return holiday calendar containing all weekend days as holidays.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with all weekend days as holidays.
         """
         ...  # pragma: no cover
 
     @property
-    def holidays_all(self) -> HolidayCalendar:
+    def holidays_all(self) -> ExchangeCalendarsHolidayCalendar:
         """
         Return a holiday calendar containing all holidays, regular and ad-hoc.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with all holidays.
         """
         ...  # pragma: no cover
 
     @property
-    def special_opens_all(self) -> HolidayCalendar:
+    def special_opens_all(self) -> ExchangeCalendarsHolidayCalendar:
         """
         Return a holiday calendar with all special opens, regular and ad-hoc.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with all special opens.
         """
         ...  # pragma: no cover
 
     @property
-    def special_closes_all(self) -> HolidayCalendar:
+    def special_closes_all(self) -> ExchangeCalendarsHolidayCalendar:
         """
         Return a holiday calendar with all special closes, regular and ad-hoc.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with all special closes.
         """
         ...  # pragma: no cover
 
     @property
-    def monthly_expiries(self) -> Union[HolidayCalendar, None]:
+    def monthly_expiries(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
         """
         Return a holiday calendar with a holiday for each monthly expiry, but excluding quarterly expiry days.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each monthly expiry.
         """
         ...  # pragma: no cover
 
     @property
-    def quarterly_expiries(self) -> Union[HolidayCalendar, None]:
+    def quarterly_expiries(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
         """
         Return a holiday calendar with a holiday for each quarterly expiry aka quadruple witching.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each quarterly expiry.
         """
         ...  # pragma: no cover
 
     @property
-    def last_trading_days_of_months(self) -> Union[HolidayCalendar, None]:
+    def last_trading_days_of_months(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
         """
         Return a holiday calendar with a holiday for each last trading day of the month.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each last trading day of the month.
         """
         ...  # pragma: no cover
 
     @property
-    def last_regular_trading_days_of_months(self) -> Union[HolidayCalendar, None]:
+    def last_regular_trading_days_of_months(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
         """
         Return a holiday calendar with a holiday for each last regular trading day of the month.
 
         Returns
         -------
-        HolidayCalendar
+        ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each last regular trading day of the month.
         """
         ...
 
 
 @dataclass
 class AdjustedProperties:
@@ -681,166 +740,164 @@
         # Remove empty DateTime indices.
         adhoc_special_sessions = [(t, adhoc_ts) for t, adhoc_ts in adhoc_special_sessions if not adhoc_ts.empty]
 
         return regular_special_sessions, adhoc_special_sessions
 
     def __init__(self, *args, **kwargs):
         # Save adjusted properties. Initialize with copies of the original properties.
-        a = AdjustedProperties(regular_holidays=regular_holidays_orig(self).rules.copy(),
-                               adhoc_holidays=adhoc_holidays_orig(self).copy(),
-                               special_closes=[(t, d if isinstance(d, int) else d.rules.copy()) for t, d in
-                                               special_closes_orig(self).copy()],
-                               adhoc_special_closes=adhoc_special_closes_orig(self).copy(),
-                               special_opens=[(t, d if isinstance(d, int) else d.rules.copy()) for t, d in
-                                              special_opens_orig(self).copy()],
-                               adhoc_special_opens=adhoc_special_opens_orig(self).copy())
+        a = AdjustedProperties(regular_holidays=list(copy(regular_holidays_orig(self).rules)),
+                               adhoc_holidays=list(copy(adhoc_holidays_orig(self))),
+                               special_closes=[(t, d if isinstance(d, int) else list(copy(d.rules))) for t, d in
+                                               copy(special_closes_orig(self))],
+                               adhoc_special_closes=list(copy(adhoc_special_closes_orig(self))),
+                               special_opens=[(t, d if isinstance(d, int) else list(copy(d.rules))) for t, d in
+                                              copy(special_opens_orig(self))],
+                               adhoc_special_opens=list(copy(adhoc_special_opens_orig(self))))
 
         # Get changeset from provider, maybe.
         changeset: ChangeSet = changeset_provider() if changeset_provider is not None else None
 
         # Set changeset to None if it is empty.
-        if changeset is not None and changeset.is_empty():
+        if changeset is not None and len(changeset) <= 0:
             changeset = None
 
         # Normalize changeset, maybe.
         if changeset is not None:
             # Creates a normalized copy of the changeset.
             changeset = changeset.normalize()
 
         if changeset is not None:
             # Apply all changes pertaining to regular exchange calendar properties.
 
             # Remove holidays.
-            for ts in changeset.changes[HolidaysAndSpecialSessions.HOLIDAY].remove:
+            for ts in changeset.holiday.remove:
                 a.regular_holidays, a.adhoc_holidays = remove_holiday(ts, a.regular_holidays, a.adhoc_holidays)
 
             # Add holidays.
-            for ts, spec in changeset.changes[HolidaysAndSpecialSessions.HOLIDAY].add.items():
-                name = spec['name']
+            for ts, spec in changeset.holiday.add.items():
+                name = spec.name
+
                 # Remove existing holiday, maybe.
                 a.regular_holidays, a.adhoc_holidays = remove_holiday(ts, a.regular_holidays, a.adhoc_holidays)
 
                 # Add the holiday.
                 a.regular_holidays.append(Holiday(name, year=ts.year, month=ts.month, day=ts.day))
 
             # Remove special opens.
-            for ts in changeset.changes[HolidaysAndSpecialSessions.SPECIAL_OPEN].remove:
+            for ts in changeset.special_open.remove:
                 a.special_opens, a.adhoc_special_opens = remove_special_session(ts, a.special_opens,
                                                                                 a.adhoc_special_opens)
 
             # Add special opens.
-            for ts, spec in changeset.changes[HolidaysAndSpecialSessions.SPECIAL_OPEN].add.items():
-                name, t = spec['name'], spec['time']
+            for ts, spec in changeset.special_open.add.items():
+                name, t = spec.name, spec.time
 
                 # Remove existing special open, maybe.
                 a.special_opens, a.adhoc_special_opens = remove_special_session(ts, a.special_opens,
                                                                                 a.adhoc_special_opens)
 
                 # Add the special open.
                 a.special_opens = add_special_session(name, ts, t, a.special_opens)
 
             # Remove special closes.
-            for ts in changeset.changes[HolidaysAndSpecialSessions.SPECIAL_CLOSE].remove:
+            for ts in changeset.special_close.remove:
                 a.special_closes, a.adhoc_special_closes = remove_special_session(ts, a.special_closes,
                                                                                   a.adhoc_special_closes)
 
             # Add special closes.
-            for ts, spec in changeset.changes[HolidaysAndSpecialSessions.SPECIAL_CLOSE].add.items():
-                name, t = spec['name'], spec['time']
+            for ts, spec in changeset.special_close.add.items():
+                name, t = spec.name, spec.time
 
                 # Remove existing special close, maybe.
                 a.special_closes, a.adhoc_special_closes = remove_special_session(ts, a.special_closes,
                                                                                   a.adhoc_special_closes)
 
                 # Add the special close.
                 a.special_closes = add_special_session(name, ts, t, a.special_closes)
 
         self._adjusted_properties = a
 
         # Call upstream init method.
         init_orig(self, *args, **kwargs)
 
-        # All weekend days and holidays.
-        weekends_and_holidays = merge_calendars([get_weekend_days_calendar(self), get_holidays_calendar(self)])
-
-        # All weekend days, holidays and special business days.
-        weekends_holidays_and_special_business_days = merge_calendars(
-            [weekends_and_holidays, get_special_opens_calendar(self), get_special_closes_calendar(self)])
-
-        a.quarterly_expiries = get_quadruple_witching_calendar(day_of_week_expiry, get_roll_backward_observance(
-            weekends_holidays_and_special_business_days)).rules.copy() if day_of_week_expiry is not None else []
-        a.monthly_expiries = get_monthly_expiry_calendar(day_of_week_expiry, get_roll_backward_observance(
-            weekends_holidays_and_special_business_days)).rules.copy() if day_of_week_expiry is not None else []
+        a.quarterly_expiries = get_quadruple_witching_rules(day_of_week_expiry) if day_of_week_expiry is not None else []
+        a.monthly_expiries = get_monthly_expiry_rules(day_of_week_expiry) if day_of_week_expiry is not None else []
 
         if changeset is not None:
 
             # Remove quarterly expiries.
 
             # Loop over quarterly expiries to remove.
-            for ts in changeset.changes[HolidaysAndSpecialSessions.QUARTERLY_EXPIRY].remove:
+            for ts in changeset.quarterly_expiry.remove:
                 a.quarterly_expiries, _ = remove_holiday(ts, a.quarterly_expiries)
 
             # Add quarterly expiries.
 
             # Loop over quarterly expiries to add.
-            for ts, spec in changeset.changes[HolidaysAndSpecialSessions.QUARTERLY_EXPIRY].add.items():
-                name = spec['name']
+            for ts, spec in changeset.quarterly_expiry.add.items():
+                name = spec.name
+
                 # Remove existing quarterly expiry, maybe.
                 a.quarterly_expiries, _ = remove_holiday(ts, a.quarterly_expiries)
 
                 # Add the quarterly expiry.
                 a.quarterly_expiries.append(Holiday(name, year=ts.year, month=ts.month, day=ts.day))
 
             # Remove monthly expiries.
 
             # Loop over monthly expiries to remove.
-            for ts in changeset.changes[HolidaysAndSpecialSessions.MONTHLY_EXPIRY].remove:
+            for ts in changeset.monthly_expiry.remove:
                 a.monthly_expiries, _ = remove_holiday(ts, a.monthly_expiries)
 
             # Add monthly expiries.
 
             # Loop over monthly expiries to add.
-            for ts, spec in changeset.changes[HolidaysAndSpecialSessions.MONTHLY_EXPIRY].add.items():
-                name = spec['name']
+            for ts, spec in changeset.monthly_expiry.add.items():
+                name = spec.name
+
                 # Remove existing monthly expiry, maybe.
                 a.monthly_expiries, _ = remove_holiday(ts, a.monthly_expiries)
 
                 # Add the monthly expiry.
                 a.monthly_expiries.append(Holiday(name, year=ts.year, month=ts.month, day=ts.day))
 
-        a.last_trading_days_of_months = get_last_day_of_month_calendar('last trading day of month',
-                                                                       get_roll_backward_observance(
-                                                                           weekends_and_holidays)).rules.copy()
-        a.last_regular_trading_days_of_months = get_last_day_of_month_calendar('last regular trading day of month',
-                                                                               get_roll_backward_observance(
-                                                                                   weekends_holidays_and_special_business_days)).rules.copy()
+        a.last_trading_days_of_months = get_last_day_of_month_rules('last trading day of month')
+        a.last_regular_trading_days_of_months = get_last_day_of_month_rules('last regular trading day of month')
+
+        # Save a calendar with all holidays and another one with all holidays and special business days for later use.
+        # These calendars are needed to generate calendars for monthly expiries, quarterly expiries, last trading days
+        # of the month, and last regular trading days of the month. Each of these calendars defines contains days that
+        # need to be rolled back to a previous business day if they fall on a holiday and/or special business day.
+        self._holidays_shared = get_holidays_calendar(self)
+        self._holidays_and_special_business_days_shared = merge_calendars(
+            [get_holidays_calendar(self), get_special_opens_calendar(self), get_special_closes_calendar(self)])
 
     @property
     def regular_holidays(self) -> Union[HolidayCalendar, None]:
         return HolidayCalendar(rules=self._adjusted_properties.regular_holidays)
 
     @property
     def adhoc_holidays(self) -> List[pd.Timestamp]:
-        return self._adjusted_properties.adhoc_holidays.copy()
+        return copy(self._adjusted_properties.adhoc_holidays)
 
     @property
     def special_closes(self) -> List[Tuple[datetime.time, Union[HolidayCalendar, int]]]:
         return [(t, HolidayCalendar(rules=rules)) for t, rules in self._adjusted_properties.special_closes]
 
     @property
     def special_closes_adhoc(self) -> List[Tuple[datetime.time, pd.DatetimeIndex]]:
-        return self._adjusted_properties.adhoc_special_closes.copy()
+        return copy(self._adjusted_properties.adhoc_special_closes)
 
     @property
     def special_opens(self) -> List[Tuple[datetime.time, Union[HolidayCalendar, int]]]:
         return [(t, HolidayCalendar(rules=rules)) for t, rules in self._adjusted_properties.special_opens]
 
     @property
     def special_opens_adhoc(self) -> List[Tuple[datetime.time, pd.DatetimeIndex]]:
-        return self._adjusted_properties.adhoc_special_opens.copy()
+        return copy(self._adjusted_properties.adhoc_special_opens)
 
     @property
     def weekend_days(self) -> Union[HolidayCalendar, None]:
         return get_weekend_days_calendar(self)
 
     @property
     def holidays_all(self) -> Union[HolidayCalendar, None]:
@@ -852,27 +909,27 @@
 
     @property
     def special_closes_all(self) -> Union[HolidayCalendar, None]:
         return get_special_closes_calendar(self)
 
     @property
     def monthly_expiries(self) -> Union[HolidayCalendar, None]:
-        return HolidayCalendar(rules=self._adjusted_properties.monthly_expiries)
+        return AdjustedHolidayCalendar(rules=self._adjusted_properties.monthly_expiries, other=self._holidays_and_special_business_days_shared, weekmask=self.weekmask)
 
     @property
     def quarterly_expiries(self) -> Union[HolidayCalendar, None]:
-        return HolidayCalendar(rules=self._adjusted_properties.quarterly_expiries)
+        return AdjustedHolidayCalendar(rules=self._adjusted_properties.quarterly_expiries, other=self._holidays_and_special_business_days_shared, weekmask=self.weekmask)
 
     @property
     def last_trading_days_of_months(self) -> Union[HolidayCalendar, None]:
-        return HolidayCalendar(rules=self._adjusted_properties.last_trading_days_of_months)
+        return AdjustedHolidayCalendar(rules=self._adjusted_properties.last_trading_days_of_months, other=self._holidays_shared, weekmask=self.weekmask)
 
     @property
     def last_regular_trading_days_of_months(self) -> Union[HolidayCalendar, None]:
-        return HolidayCalendar(rules=self._adjusted_properties.last_regular_trading_days_of_months)
+        return AdjustedHolidayCalendar(rules=self._adjusted_properties.last_regular_trading_days_of_months, other=self._holidays_and_special_business_days_shared, weekmask=self.weekmask)
 
     # Use type to create a new class.
     extended = type(cls.__name__ + "Extended", (cls, ExtendedExchangeCalendar), {
         "__init__": __init__,
         "regular_holidays": regular_holidays,
         "adhoc_holidays": adhoc_holidays,
         "special_closes": special_closes,
```

### Comparing `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/offset.py` & `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/offset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+from abc import ABC, abstractmethod
 from datetime import datetime, date
-from typing import Type, Callable
+from typing import Type
 
 import pandas as pd
 from pandas._libs.tslibs import localize_pydatetime
 from pandas._libs.tslibs.offsets import Easter, apply_wraps
 
 from exchange_calendars_extensions.util import get_month_name, get_day_of_week_name, third_day_of_week_in_month, \
     last_day_in_month
 
 
-class AbstractHolidayOffset(Easter):
+class AbstractHolidayOffset(Easter, ABC):
 
     @staticmethod
     def _is_normalized(dt):
         if dt.hour != 0 or dt.minute != 0 or dt.second != 0 or dt.microsecond != 0:
             # Regardless of whether dt is datetime vs Timestamp
             return False
         if isinstance(dt, pd.Timestamp):
             return dt.nanosecond == 0
         return True
 
-    @property
-    def holiday(self, year: int):
+    @abstractmethod
+    def holiday(self, year: int) -> date:
         """
         Return the Gregorian date for the holiday in a given Gregorian calendar
         year.
         """
         ...  # pragma: no cover
 
     @apply_wraps
@@ -79,20 +80,19 @@
 
     Returns
     -------
     Type[AbstractHolidayOffset]
         A new class that represents the offset.
     """
 
-    @property
-    def holiday(self) -> Callable[[int], pd.Timestamp]:
+    def holiday(self, year) -> date:
         """
         Return a function that returns the third instance of the given day of the week in the given month and year.
         """
-        return lambda year: third_day_of_week_in_month(day_of_week, month, year)
+        return third_day_of_week_in_month(day_of_week, month, year)
 
     # Get name of day of week.
     day_of_week_name = get_day_of_week_name(day_of_week)
 
     # Get name of month.
     month_name = get_month_name(month)
 
@@ -132,20 +132,19 @@
         The month, where 1 is January and 12 is December.
 
     Returns
     -------
     Type[AbstractHolidayOffset]
         A new class that represents the offset.
     """
-    @property
-    def holiday(self) -> Callable[[int], pd.Timestamp]:
+    def holiday(self, year) -> date:
         """
         Return a function that returns the last day of the month for a given year.
         """
-        return lambda year: last_day_in_month(month, year)
+        return last_day_in_month(month, year)
 
     # Get name of month.
     month_name = get_month_name(month)
 
     # Create the new class.
     offset = type(f"LastDayOfMonth{month_name}Offset", (AbstractHolidayOffset,), {
         "holiday": holiday,
```

### Comparing `exchange_calendars_extensions-0.2.1/exchange_calendars_extensions/util.py` & `exchange_calendars_extensions-0.3.0/exchange_calendars_extensions/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 from datetime import date
 from datetime import timedelta
 
 
 def get_month_name(month: int) -> str:
     """
     Convert month to capitalized name of month.
```

### Comparing `exchange_calendars_extensions-0.2.1/pyproject.toml` & `exchange_calendars_extensions-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,95 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions"
-version = "0.2.1"
+version = "0.3.0"
 description = "Extensions of the exchange-calendars package"
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/"
 keywords = ["exchange", "calendar", "trading", "holidays"]
 classifiers = [
 	"Development Status :: 4 - Beta",
+    "License :: OSI Approved :: Apache Software License",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Financial and Insurance Industry",
+    "Intended Audience :: Information Technology",
+    "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "License :: OSI Approved :: Apache Software License",
-    "Intended Audience :: Science/Research",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Mathematics",
-    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [{include = "exchange_calendars_extensions"}]
 
 [tool.poetry.dependencies]
 python = "~=3.8"
 exchange-calendars = ">=4.0.1"
-schema = "~=0.7.5"
-typing-extensions = "~=4.6.2"
+typing-extensions = ">=4.6.2,<4.8.0"
+pydantic = "~=2.0.2"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "~=7.3.1"
+pytest = ">=7.3.1,<7.5.0"
 pytest-cov = "~=4.1.0"
+pre-commit = "~=3.3.3"
+
 
 [tool.pytest.ini_options]
 addopts = "--cov=exchange_calendars_extensions --cov-report=term-missing"
+
+[tool.ruff]
+# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
+select = ["E", "F"]
+ignore = ["E501"]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+unfixable = []
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".git-rewrite",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+
+# Same as Black.
+line-length = 88
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.10.
+target-version = "py38"
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
```

