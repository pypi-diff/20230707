# Comparing `tmp/pyppms-3.2.1.tar.gz` & `tmp/pyppms-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-3.2.1.tar", max compression
+gzip compressed data, was "pyppms-3.3.0.tar", max compression
```

## Comparing `pyppms-3.2.1.tar` & `pyppms-3.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.2.1/README.md
--rw-r--r--   0        0        0     1146 2023-06-30 08:33:10.446721 pyppms-3.2.1/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.2.1/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5895 2023-06-30 08:32:08.949246 pyppms-3.2.1/src/pyppms/booking.py
--rw-r--r--   0        0        0     7859 2023-06-22 14:39:34.090209 pyppms-3.2.1/src/pyppms/common.py
--rw-r--r--   0        0        0      130 2023-06-21 14:22:58.508961 pyppms-3.2.1/src/pyppms/exceptions.py
--rw-r--r--   0        0        0    47431 2023-06-30 08:32:08.953246 pyppms-3.2.1/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.2.1/src/pyppms/system.py
--rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.2.1/src/pyppms/user.py
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.3.0/README.md
+-rw-r--r--   0        0        0     1146 2023-07-07 13:55:41.400238 pyppms-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.3.0/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-07 13:54:38.067533 pyppms-3.3.0/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7859 2023-06-22 14:39:34.090209 pyppms-3.3.0/src/pyppms/common.py
+-rw-r--r--   0        0        0      130 2023-06-21 14:22:58.508961 pyppms-3.3.0/src/pyppms/exceptions.py
+-rw-r--r--   0        0        0    48216 2023-07-07 13:54:38.067533 pyppms-3.3.0/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.3.0/src/pyppms/system.py
+-rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.3.0/src/pyppms/user.py
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.3.0/PKG-INFO
```

### Comparing `pyppms-3.2.1/README.md` & `pyppms-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.1/pyproject.toml` & `pyppms-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "A Python package to communicate with Stratocore's PUMAPI."
 name = "pyppms"
-version = "3.2.1"
+version = "3.3.0"
 
 license = "GPLv3"
 
 authors = [
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
   "Laurent Guerard <laurent.guerard@unibas.ch>",
 ]
```

### Comparing `pyppms-3.2.1/src/pyppms/booking.py` & `pyppms-3.3.0/src/pyppms/booking.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             self.session = lines[2]
         except Exception as err:
             log.error("Parsing booking response failed ({}), text was:\n{}", err, text)
             raise
 
         log.trace(str(self))
 
+    # FIXME: date is of type datetime.datetime, NOT datetime.date !!!
     @classmethod
     def from_runningsheet(cls, entry, system_id, username, date):
         """Alternative constructor using a (parsed) getrunningsheet response.
 
         Parameters
         ----------
         entry : dict
```

### Comparing `pyppms-3.2.1/src/pyppms/common.py` & `pyppms-3.3.0/src/pyppms/common.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.1/src/pyppms/ppms.py` & `pyppms-3.3.0/src/pyppms/ppms.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,17 @@
         log.trace("{} groups in the PPMS database: {}", len(groups), ", ".join(groups))
         return groups
 
     def get_next_booking(self, system_id):
         """Wrapper for `get_booking()` with 'booking_type' set to 'next'."""
         return self.get_booking(system_id, "next")
 
-    def get_running_sheet(self, core_facility_ref, date, ignore_uncached_users=False):
+    def get_running_sheet(
+        self, core_facility_ref, date, ignore_uncached_users=False, localisation=""
+    ):
         """Get the running sheet for a specific day on the given facility.
 
         The so-called "running-sheet" consists of all bookings / reservations of
         a facility on a specifc day.
 
         WARNING: PUMAPI doesn't return a proper unique user identifier with the
         'getrunningsheet' request, instead the so called "full name" is given to
@@ -581,14 +583,17 @@
             The core facility ID for PPMS.
         date : datetime.datetime
             The date to request the running sheet for, e.g. ``datetime.now()`` or
             similar. Note that only the date part is relevant, time will be ignored.
         ignore_uncached_users : bool, optional
             If set to `True` any booking for a user that is not present in the instance
             attribute `fullname_mapping` will be ignored in the resulting list.
+        localisation : str, optional
+            If given, the runningsheet will be limited to systems where the
+            `localisation` (~"room") field matches the given value.
 
         Returns
         -------
         list(pyppms.booking.PpmsBooking)
             A list with `PpmsBooking` objects for the given day. Empty in case
             there are no bookings or parsing the response failed.
         """
@@ -624,16 +629,27 @@
                 log.error("PPMS doesn't seem to know user [{}], skipping", full)
                 continue
 
             log.trace(
                 f"Booking for user '{self.fullname_mapping[full]}' ({full}) found"
             )
             system_name = entry["Object"]
-            system_ids = self.get_systems_matching("", [system_name])
-            if len(system_ids) != 1:
+            # FIXME: add a test with one system name being a subset of another system
+            # (this will result in more than one result and should be fixed e.g. by
+            # adding an optional parameter "exact" to get_systems_matching() or
+            # similar)
+            system_ids = self.get_systems_matching(localisation, [system_name])
+            if len(system_ids) < 1:
+                if localisation:
+                    log.debug(f"Given criteria return zero systems for [{system_name}]")
+                else:
+                    log.warning(f"No systems matching criteria for [{system_name}]")
+                continue
+
+            if len(system_ids) > 1:
                 # NOTE: more than one result should not happen as PPMS doesn't allow for
                 # multiple systems having the same name - no result might happen though!
                 log.error("Ignoring booking for unknown system [{}]", system_name)
                 continue
 
             booking = PpmsBooking.from_runningsheet(
                 entry,
```

### Comparing `pyppms-3.2.1/src/pyppms/system.py` & `pyppms-3.3.0/src/pyppms/system.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.1/src/pyppms/user.py` & `pyppms-3.3.0/src/pyppms/user.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.2.1/PKG-INFO` & `pyppms-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 3.2.1
+Version: 3.3.0
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
```

