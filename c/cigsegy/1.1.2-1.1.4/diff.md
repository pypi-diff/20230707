# Comparing `tmp/cigsegy-1.1.2.tar.gz` & `tmp/cigsegy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cigsegy-1.1.2.tar", last modified: Sat May 27 10:07:05 2023, max compression
+gzip compressed data, was "cigsegy-1.1.4.tar", last modified: Fri Jul  7 06:45:51 2023, max compression
```

## Comparing `cigsegy-1.1.2.tar` & `cigsegy-1.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.649687 cigsegy-1.1.2/
--rw-r--r--   0 roger     (1000) roger     (1000)     1066 2023-05-27 10:03:26.000000 cigsegy-1.1.2/LICENSE
--rw-r--r--   0 roger     (1000) roger     (1000)      133 2023-05-27 10:03:07.000000 cigsegy-1.1.2/MANIFEST.in
--rw-rw-r--   0 roger     (1000) roger     (1000)      264 2023-05-27 10:07:05.645687 cigsegy-1.1.2/PKG-INFO
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/cigsegy.egg-info/
--rw-rw-r--   0 roger     (1000) roger     (1000)      264 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/PKG-INFO
--rw-rw-r--   0 roger     (1000) roger     (1000)      606 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/SOURCES.txt
--rw-rw-r--   0 roger     (1000) roger     (1000)        1 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/dependency_links.txt
--rw-rw-r--   0 roger     (1000) roger     (1000)        8 2023-05-27 10:07:05.000000 cigsegy-1.1.2/cigsegy.egg-info/top_level.txt
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/include/
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/include/fmt/
--rw-r--r--   0 roger     (1000) roger     (1000)    34822 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/chrono.h
--rw-r--r--   0 roger     (1000) roger     (1000)    22421 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/color.h
--rw-r--r--   0 roger     (1000) roger     (1000)    19898 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/compile.h
--rw-r--r--   0 roger     (1000) roger     (1000)    50435 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/core.h
--rw-r--r--   0 roger     (1000) roger     (1000)    50189 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/format-inl.h
--rw-r--r--   0 roger     (1000) roger     (1000)   118325 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/format.h
--rw-r--r--   0 roger     (1000) roger     (1000)     2870 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/locale.h
--rw-r--r--   0 roger     (1000) roger     (1000)     4607 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/ostream.h
--rw-r--r--   0 roger     (1000) roger     (1000)     9025 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/posix.h
--rw-r--r--   0 roger     (1000) roger     (1000)    21823 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/printf.h
--rw-r--r--   0 roger     (1000) roger     (1000)    11858 2023-05-27 09:59:48.000000 cigsegy-1.1.2/include/fmt/ranges.h
--rw-r--r--   0 roger     (1000) roger     (1000)      114 2023-05-27 10:03:36.000000 cigsegy-1.1.2/pyproject.toml
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/python/
--rw-r--r--   0 roger     (1000) roger     (1000)    12791 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/PySegy.cpp
--rw-r--r--   0 roger     (1000) roger     (1000)      427 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/__init__.py
--rw-r--r--   0 roger     (1000) roger     (1000)    10680 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/cigsegy.pyi
--rw-r--r--   0 roger     (1000) roger     (1000)      695 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/setup.py
--rw-r--r--   0 roger     (1000) roger     (1000)    11284 2023-05-27 09:54:05.000000 cigsegy-1.1.2/python/tools.py
--rw-r--r--   0 roger     (1000) roger     (1000)       79 2023-05-27 10:07:05.000000 cigsegy-1.1.2/python/version.py
--rw-rw-r--   0 roger     (1000) roger     (1000)       38 2023-05-27 10:07:05.649687 cigsegy-1.1.2/setup.cfg
--rw-r--r--   0 roger     (1000) roger     (1000)     2281 2023-05-27 09:54:05.000000 cigsegy-1.1.2/setup.py
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/src/
-drwxrwxr-x   0 roger     (1000) roger     (1000)        0 2023-05-27 10:07:05.645687 cigsegy-1.1.2/src/include/
--rw-r--r--   0 roger     (1000) roger     (1000)    59855 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/mio.hpp
--rw-r--r--   0 roger     (1000) roger     (1000)     6009 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/progressbar.hpp
--rw-r--r--   0 roger     (1000) roger     (1000)     6496 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/segy.h
--rw-r--r--   0 roger     (1000) roger     (1000)    17167 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/include/utils.h
--rw-r--r--   0 roger     (1000) roger     (1000)    37107 2023-05-27 09:54:04.000000 cigsegy-1.1.2/src/segy.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.348249 cigsegy-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-05-27 10:03:26.000000 cigsegy-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-27 10:03:07.000000 cigsegy-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-07 06:45:51.344248 cigsegy-1.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.344248 cigsegy-1.1.4/cigsegy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-07 06:45:51.000000 cigsegy-1.1.4/cigsegy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-07 06:45:51.000000 cigsegy-1.1.4/cigsegy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 06:45:51.000000 cigsegy-1.1.4/cigsegy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-07 06:45:51.000000 cigsegy-1.1.4/cigsegy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.340248 cigsegy-1.1.4/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.344248 cigsegy-1.1.4/include/fmt/
+-rw-r--r--   0 root         (0) root         (0)    34822 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/chrono.h
+-rw-r--r--   0 root         (0) root         (0)    22421 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/color.h
+-rw-r--r--   0 root         (0) root         (0)    19898 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/compile.h
+-rw-r--r--   0 root         (0) root         (0)    50435 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/core.h
+-rw-r--r--   0 root         (0) root         (0)    50189 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/format-inl.h
+-rw-r--r--   0 root         (0) root         (0)   118325 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/format.h
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/locale.h
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/ostream.h
+-rw-r--r--   0 root         (0) root         (0)     9025 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/posix.h
+-rw-r--r--   0 root         (0) root         (0)    21823 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/printf.h
+-rw-r--r--   0 root         (0) root         (0)    11858 2023-05-27 09:59:48.000000 cigsegy-1.1.4/include/fmt/ranges.h
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-27 10:03:36.000000 cigsegy-1.1.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.344248 cigsegy-1.1.4/python/
+-rw-r--r--   0 root         (0) root         (0)    19218 2023-07-07 06:45:51.000000 cigsegy-1.1.4/python/PySegy.cpp
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-07 06:45:51.000000 cigsegy-1.1.4/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13173 2023-07-07 06:45:51.000000 cigsegy-1.1.4/python/cigsegy.pyi
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-07 06:45:51.000000 cigsegy-1.1.4/python/setup.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2023-07-07 06:45:51.000000 cigsegy-1.1.4/python/tools.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-07 06:45:51.000000 cigsegy-1.1.4/python/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 06:45:51.348249 cigsegy-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-07 06:45:51.000000 cigsegy-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.344248 cigsegy-1.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:51.344248 cigsegy-1.1.4/src/include/
+-rw-r--r--   0 root         (0) root         (0)    59855 2023-07-07 06:45:51.000000 cigsegy-1.1.4/src/include/mio.hpp
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-07-07 06:45:51.000000 cigsegy-1.1.4/src/include/progressbar.hpp
+-rw-r--r--   0 root         (0) root         (0)     6937 2023-07-07 06:45:51.000000 cigsegy-1.1.4/src/include/segy.h
+-rw-r--r--   0 root         (0) root         (0)    17149 2023-07-07 06:45:51.000000 cigsegy-1.1.4/src/include/utils.h
+-rw-r--r--   0 root         (0) root         (0)    54328 2023-07-07 06:45:51.000000 cigsegy-1.1.4/src/segy.cpp
```

### Comparing `cigsegy-1.1.2/LICENSE` & `cigsegy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/cigsegy.egg-info/SOURCES.txt` & `cigsegy-1.1.4/cigsegy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/chrono.h` & `cigsegy-1.1.4/include/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/color.h` & `cigsegy-1.1.4/include/fmt/color.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/compile.h` & `cigsegy-1.1.4/include/fmt/compile.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/core.h` & `cigsegy-1.1.4/include/fmt/core.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/format-inl.h` & `cigsegy-1.1.4/include/fmt/format-inl.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/format.h` & `cigsegy-1.1.4/include/fmt/format.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/locale.h` & `cigsegy-1.1.4/include/fmt/locale.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/ostream.h` & `cigsegy-1.1.4/include/fmt/ostream.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/posix.h` & `cigsegy-1.1.4/include/fmt/posix.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/printf.h` & `cigsegy-1.1.4/include/fmt/printf.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/include/fmt/ranges.h` & `cigsegy-1.1.4/include/fmt/ranges.h`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/python/PySegy.cpp` & `cigsegy-1.1.4/python/PySegy.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,113 @@
 /*********************************************************************
-** Copyright (c) 2022 Roger Lee.
+** Copyright (c) 2023 Roger Lee.
 ** Computational and Interpretation Group (CIG),
 ** University of Science and Technology of China (USTC).
 **
 ** @File: PySegy.cpp
-** @Time: 2022/12/05 14:36:48
-** @Version: 1.0
 ** @Description :
 *********************************************************************/
 
 #include "segy.h"
+#include <iostream>
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
 #include <stdexcept>
 
 namespace py = pybind11;
 
 class Pysegy : public segy::SegyIO {
 public:
   using segy::SegyIO::create;
+  using segy::SegyIO::cut;
   using segy::SegyIO::read;
   using segy::SegyIO::read_cross_slice;
   using segy::SegyIO::read_inline_slice;
   using segy::SegyIO::read_time_slice;
   using segy::SegyIO::read_trace;
   using segy::SegyIO::SegyIO;
 
   py::array_t<int> get_traceInfo(int n);
   py::array_t<int> get_traceInfo(int beg, int end);
+  py::array_t<int> get_lineInfo();
 
   py::array_t<float> read(int startZ, int endZ, int startY, int endY,
                           int startX, int endX);
   py::array_t<float> read();
   py::array_t<float> read_inline_slice(int iZ);
   py::array_t<float> read_cross_slice(int iY);
   py::array_t<float> read_time_slice(int iX);
   py::array_t<float> read_trace(int iZ, int iY);
 
-  void create(const std::string &segy_out_name, const py::array_t<float> &src);
+  void cut(const std::string &outname, int startZ, int endZ, int startY,
+           int endY, int startX, int endX,
+           const py::list &custom_info = py::list());
+  void cut(const std::string &outname, int startZ, int endZ, int startY,
+           int endY, const py::list &custom_info = py::list());
+  void cut(const std::string &outname, int startX, int endX,
+           const py::list &custom_info = py::list());
+
+  void create(const std::string &segy_out_name, const py::array_t<float> &src,
+              const py::list &custom_info = py::list());
+  void create(const std::string &segy_out_name,
+              const py::list &custom_info = py::list());
 };
 
 py::array_t<int> Pysegy::get_traceInfo(int n) {
   py::array_t<int> traceinfo(4);
   int *ptr = static_cast<int *>(traceinfo.request().ptr);
   get_TraceInfo(n, ptr);
+  if (!is_crossline_fast_order()) {
+    int t = ptr[0];
+    ptr[0] = ptr[1];
+    ptr[1] = t;
+  }
   return traceinfo;
 }
 
 py::array_t<int> Pysegy::get_traceInfo(int beg, int end) {
   if (beg < 0 || beg >= trace_count() || end <= beg || end > trace_count()) {
     throw std::runtime_error("Invalid index");
   }
   int n = end - beg;
   py::array_t<int> traceinfo({n, 4});
   int *ptr = static_cast<int *>(traceinfo.request().ptr);
 
   for (int i = beg; i < end; i++) {
     get_TraceInfo(i, ptr);
+    if (!is_crossline_fast_order()) {
+      int t = ptr[0];
+      ptr[0] = ptr[1];
+      ptr[1] = t;
+    }
     ptr += 4;
   }
   return traceinfo;
 }
 
+py::array_t<int> Pysegy::get_lineInfo() {
+  // [inline, crossline_start, crossline_end,
+  //  trace_strat, trace_end, count]
+  auto info = line_info();
+  int n = info.size();
+  py::array_t<int> out({n, 6});
+  int *outptr = static_cast<int *>(out.request().ptr);
+  memcpy(outptr, info.data(), sizeof(int) * 6 * n);
+  if (!is_crossline_fast_order()) {
+    std::cout
+        << "[Warining] As the fast order of your segy file "
+           "is inline order (default is crossline order). So the lineInfo "
+           "you obtained is seems as [crossline, inline_start, inline_end, "
+           "trace_start, trace_end, count]\n"
+        << std::endl;
+  }
+  return out;
+}
+
 // Be careful the order of the dimensions
 // In segy, X (time) is the first, but when you read into python,
 // Z (inline) is the first. If need change it to X first,
 // use data.transpose() in python
 py::array_t<float> Pysegy::read(int startZ, int endZ, int startY, int endY,
                                 int startX, int endX) {
 
@@ -120,56 +162,132 @@
   py::array_t<float> out(shape(0));
   auto buff = out.request();
   float *ptr = static_cast<float *>(buff.ptr);
   read_trace(ptr, iY, iZ);
   return out;
 }
 
+void Pysegy::cut(const std::string &outname, int startZ, int endZ, int startY,
+                 int endY, int startX, int endX, const py::list &custom_info) {
+  auto customvec = custom_info.cast<std::vector<std::string>>();
+  cut(outname, startX, endX, startY, endY, startZ, endZ, customvec);
+}
+
+void Pysegy::cut(const std::string &outname, int startZ, int endZ, int startY,
+                 int endY, const py::list &custom_info) {
+  auto customvec = custom_info.cast<std::vector<std::string>>();
+  cut(outname, startY, endY, startZ, endZ, customvec);
+}
+
+void Pysegy::cut(const std::string &outname, int startX, int endX,
+                 const py::list &custom_info) {
+  auto customvec = custom_info.cast<std::vector<std::string>>();
+  cut(outname, startX, endX, customvec);
+}
+
 void Pysegy::create(const std::string &segy_out_name,
-                    const py::array_t<float> &src) {
+                    const py::array_t<float> &src,
+                    const py::list &custom_info) {
   auto buff = src.request();
   if (buff.ndim != 3) {
     throw std::runtime_error("Input data must be a 3D data.");
   }
   auto r = src.unchecked<3>();
   set_size(r.shape(2), r.shape(1), r.shape(0));
+  auto customvec = custom_info.cast<std::vector<std::string>>();
 
   float *ptr = static_cast<float *>(buff.ptr);
-  create(segy_out_name, ptr);
+  create(segy_out_name, ptr, customvec);
+}
+
+void Pysegy::create(const std::string &segy_out_name,
+                    const py::list &custom_info) {
+  auto customvec = custom_info.cast<std::vector<std::string>>();
+  create(segy_out_name, customvec);
 }
 
 void create_by_sharing_header(const std::string &segy_name,
                               const std::string &header_segy,
                               const py::array_t<float> &src, int iline = 189,
-                              int xline = 193, int istep = 1, int xstep = 1) {
+                              int xline = 193, int istep = 1, int xstep = 1,
+                              const py::object &offset = py::none(),
+                              const py::list &custom_info = py::list()) {
   auto buff = src.request();
   if (buff.ndim != 3) {
     throw std::runtime_error("Input data must be a 3D data.");
   }
 
   auto r = src.unchecked<3>();
   float *ptr = static_cast<float *>(buff.ptr);
 
-  segy::create_by_sharing_header(segy_name, header_segy, ptr, r.shape(2),
-                                 r.shape(1), r.shape(0), iline, xline, istep,
-                                 xstep);
+  if (offset.is_none()) {
+    segy::create_by_sharing_header(segy_name, header_segy, ptr, r.shape(2),
+                                   r.shape(1), r.shape(0), iline, xline, istep,
+                                   xstep);
+  } else {
+    int offsetX, offsetY, offsetZ;
+    if (py::isinstance<py::dict>(offset)) {
+      py::dict off = offset.cast<py::dict>();
+      offsetZ = off["iline"].cast<int>();
+      offsetY = off["xline"].cast<int>();
+      offsetX = off["time"].cast<int>();
+    } else if (py::isinstance<py::sequence>(offset)) {
+      py::sequence off = offset.cast<py::sequence>();
+      offsetX = py::cast<int>(off[2]);
+      offsetY = py::cast<int>(off[1]);
+      offsetZ = py::cast<int>(off[0]);
+    } else {
+      throw std::runtime_error("Unkown type of offset");
+    }
+    auto customvec = custom_info.cast<std::vector<std::string>>();
+
+    segy::create_by_sharing_header(segy_name, header_segy, ptr, r.shape(2),
+                                   r.shape(1), r.shape(0), iline, xline, istep,
+                                   xstep, offsetX, offsetY, offsetZ, customvec);
+  }
 }
 
 void create_by_sharing_header(const std::string &segy_name,
                               const std::string &header_segy,
                               const std::string &src_file,
                               const py::sequence &shape, int iline = 189,
-                              int xline = 193, int istep = 1, int xstep = 1) {
+                              int xline = 193, int istep = 1, int xstep = 1,
+                              const py::object &offset = py::none(),
+                              const py::list &custom_info = py::list()) {
   if (shape.size() != 3) {
     throw std::runtime_error("dimensions must be 3");
   }
-  segy::create_by_sharing_header(
-      segy_name, header_segy, src_file, py::cast<int>(shape[2]),
-      py::cast<int>(shape[1]), py::cast<int>(shape[0]), iline, xline, istep,
-      xstep);
+
+  if (offset.is_none()) {
+    segy::create_by_sharing_header(
+        segy_name, header_segy, src_file, py::cast<int>(shape[2]),
+        py::cast<int>(shape[1]), py::cast<int>(shape[0]), iline, xline, istep,
+        xstep);
+  } else {
+    int offsetX, offsetY, offsetZ;
+    if (py::isinstance<py::dict>(offset)) {
+      py::dict off = offset.cast<py::dict>();
+      offsetZ = off["iline"].cast<int>();
+      offsetY = off["xline"].cast<int>();
+      offsetX = off["time"].cast<int>();
+    } else if (py::isinstance<py::sequence>(offset)) {
+      py::sequence off = offset.cast<py::sequence>();
+      offsetX = py::cast<int>(off[2]);
+      offsetY = py::cast<int>(off[1]);
+      offsetZ = py::cast<int>(off[0]);
+    } else {
+      throw std::runtime_error("Unkown type of offset");
+    }
+    auto customvec = custom_info.cast<std::vector<std::string>>();
+
+    segy::create_by_sharing_header(
+        segy_name, header_segy, src_file, py::cast<int>(shape[2]),
+        py::cast<int>(shape[1]), py::cast<int>(shape[0]), iline, xline, istep,
+        xstep, offsetX, offsetY, offsetZ, customvec);
+  }
 }
 
 py::array_t<float> fromfile_ignore_header(const std::string &segy_name,
                                           int sizeZ, int sizeY, int sizeX,
                                           int format = 5) {
   py::array_t<float> out({sizeZ, sizeY, sizeX});
   auto buff = out.request();
@@ -218,19 +336,21 @@
 using overload_cast_ = pybind11::detail::overload_cast_impl<Args...>;
 
 PYBIND11_MODULE(cigsegy, m) {
   py::class_<Pysegy>(m, "Pysegy")
       .def(py::init<std::string>())
       .def(py::init<int, int, int>())
       .def(py::init<std::string, int, int, int>())
-      .def("trace_cout", &Pysegy::trace_count)
+      .def("is_crossline_fast_order", &Pysegy::is_crossline_fast_order)
+      .def("trace_count", &Pysegy::trace_count)
       .def("get_traceInfo", overload_cast_<int>()(&Pysegy::get_traceInfo),
            py::arg("n"))
       .def("get_traceInfo", overload_cast_<int, int>()(&Pysegy::get_traceInfo),
            py::arg("beg"), py::arg("end"))
+      .def("get_lineInfo", &Pysegy::get_lineInfo)
       .def("setInlineLocation", &Pysegy::setInlineLocation, py::arg("iline"))
       .def("setCrosslineLocation", &Pysegy::setCrosslineLocation,
            py::arg("xline"))
       .def("setXLocation", &Pysegy::setXLocation, py::arg("xfield"))
       .def("setYLocation", &Pysegy::setYLocation, py::arg("yfield"))
       .def("setInlineStep", &Pysegy::setInlineStep, py::arg("step"))
       .def("setCrosslineStep", &Pysegy::setCrosslineStep, py::arg("step"))
@@ -249,36 +369,61 @@
            "read inline slice", py::arg("iZ"))
       .def("read_cross_slice", overload_cast_<int>()(&Pysegy::read_cross_slice),
            "read crossline slice", py::arg("iY"))
       .def("read_time_slice", overload_cast_<int>()(&Pysegy::read_time_slice),
            "read time slice", py::arg("iX"))
       .def("read_trace", overload_cast_<int, int>()(&Pysegy::read_trace),
            "read trace", py::arg("iZ"), py::arg("iY"))
+      .def("cut",
+           overload_cast_<const std::string &, int, int, int, int, int, int,
+                          const py::list &>()(&Pysegy::cut),
+           "cut a sub volume to a segy", py::arg("outname"), py::arg("startZ"),
+           py::arg("endZ"), py::arg("startY"), py::arg("endY"),
+           py::arg("startX"), py::arg("endX"),
+           py::arg("custom_info") = py::list())
+      .def("cut",
+           overload_cast_<const std::string &, int, int, int, int,
+                          const py::list &>()(&Pysegy::cut),
+           "cut a sub volume to a segy", py::arg("outname"), py::arg("startZ"),
+           py::arg("endZ"), py::arg("startY"), py::arg("endY"),
+           py::arg("custom_info") = py::list())
+      .def("cut",
+           overload_cast_<const std::string &, int, int, const py::list &>()(
+               &Pysegy::cut),
+           "cut a sub volume to a segy", py::arg("outname"), py::arg("startX"),
+           py::arg("endX"), py::arg("custom_info") = py::list())
       .def("setSampleInterval", &Pysegy::setSampleInterval, py::arg("dt"))
       .def("setDataFormatCode", &Pysegy::setDataFormatCode, py::arg("format"))
       .def("setStartTime", &Pysegy::setStartTime, py::arg("start_time"))
       .def("setXInterval", &Pysegy::setXInterval, py::arg("dx"))
       .def("setYInterval", &Pysegy::setYInterval, py::arg("dy"))
       .def("setMinInline", &Pysegy::setMinInline, py::arg("minInline"))
       .def("setMinCrossline", &Pysegy::setMinCrossline, py::arg("minXline"))
       .def("textual_header", &Pysegy::textual_header)
       .def("metaInfo", &Pysegy::metaInfo)
- //     .def("create", overload_cast_<const std::string &>()(&Pysegy::create),
- //          "create a segy", py::arg("segy_out_name"))
- //     .def("create",
- //          overload_cast_<const std::string &,
- //                         const pybind11::array_t<float> &>()(&Pysegy::create),
- //          "create a segy from memory", py::arg("segy_out_name"),
- //          py::arg("src"))
-      .def("create", static_cast<void (Pysegy::*)(const std::string &)>(&Pysegy::create),
-           "create a segy", py::arg("segy_out_name"))
+      //     .def("create", overload_cast_<const std::string
+      //     &>()(&Pysegy::create),
+      //          "create a segy", py::arg("segy_out_name"))
+      //     .def("create",
+      //          overload_cast_<const std::string &,
+      //                         const pybind11::array_t<float>
+      //                         &>()(&Pysegy::create),
+      //          "create a segy from memory", py::arg("segy_out_name"),
+      //          py::arg("src"))
+      .def("create",
+           static_cast<void (Pysegy::*)(const std::string &, const py::list &)>(
+               &Pysegy::create),
+           "create a segy", py::arg("segy_out_name"),
+           py::arg("custom_info") = py::list())
       .def("create",
-          static_cast<void (Pysegy::*)(const std::string&, const py::array_t<float>&)>(&Pysegy::create),
+           static_cast<void (Pysegy::*)(const std::string &,
+                                        const py::array_t<float> &,
+                                        const py::list &)>(&Pysegy::create),
            "create a segy from memory", py::arg("segy_out_name"),
-           py::arg("src"))
+           py::arg("src"), py::arg("custom_info") = py::list())
       .def("set_size", &Pysegy::set_size, py::arg("sizeX"), py::arg("sizeY"),
            py::arg("sizeZ"))
       .def("close_file", &Pysegy::close_file);
 
   m.def("fromfile_ignore_header", &fromfile_ignore_header,
         "read by ignoring header and specify shape", py::arg("segy_name"),
         py::arg("sizeZ"), py::arg("sizeY"), py::arg("sizeX"),
@@ -294,21 +439,25 @@
         py::arg("out_name"), py::arg("iline") = 189, py::arg("xline") = 193,
         py::arg("istep") = 1, py::arg("xstep") = 1);
   m.def("collect", &collect, "colloct all trace (data and location)",
         py::arg("segy_in"), py::arg("iline") = 189, py::arg("xline") = 193,
         py::arg("xfield") = 73, py::arg("yfield") = 77);
   m.def("create_by_sharing_header",
         overload_cast_<const std::string &, const std::string &,
-                       const py::array_t<float> &, int, int, int, int>()(
+                       const py::array_t<float> &, int, int, int, int,
+                       const py::object &, const py::list &>()(
             &create_by_sharing_header),
         "create a segy file using a existed segy header", py::arg("segy_name"),
         py::arg("header_segy"), py::arg("src"), py::arg("iline") = 189,
-        py::arg("xline") = 193, py::arg("istep") = 1, py::arg("xstep") = 1);
+        py::arg("xline") = 193, py::arg("istep") = 1, py::arg("xstep") = 1,
+        py::arg("offset") = py::none(), py::arg("custom_info") = py::list());
   m.def("create_by_sharing_header",
         overload_cast_<const std::string &, const std::string &,
                        const std::string &, const py::sequence &, int, int, int,
-                       int>()(&create_by_sharing_header),
+                       int, const py::object &, const py::list &>()(
+            &create_by_sharing_header),
         "create a segy file using a existed segy header", py::arg("segy_name"),
         py::arg("header_segy"), py::arg("src_file"), py::arg("shape"),
         py::arg("iline") = 189, py::arg("xline") = 193, py::arg("istep") = 1,
-        py::arg("xstep") = 1);
+        py::arg("xstep") = 1, py::arg("offset") = py::none(),
+        py::arg("custom_info") = py::list());
 }
```

### Comparing `cigsegy-1.1.2/python/cigsegy.pyi` & `cigsegy-1.1.4/python/cigsegy.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import cigsegy
 import typing
+from typing import List, Tuple
 import numpy
 
 _Shape = typing.Tuple[int, ...]
 
 __all__ = [
     "Pysegy", "fromfile", "fromfile_ignore_header", "tofile",
     "tofile_ignore_header", "collect", "create_by_sharing_header"
@@ -43,27 +44,35 @@
         - binary_name: the input binary file name,
         - sizeX: the number of samples per trace,
         - sizeY: the number of crossline,
         - sizeZ: the number of inline.
         """
 
     @typing.overload
-    def create(self, segy_out_name: str) -> None:
+    def create(self, segy_out_name: str, custom_info: List[str] = []) -> None:
         """
         create a segy
 
         Parameters:
         - segy_out_name: the output file name to create segy format
+        - custom_info: textual header info by user custom, max: 12 rows
+                each row is less than 76 chars
         """
 
     @typing.overload
-    def create(self, segy_out_name: str,
-               src: numpy.ndarray[numpy.float32]) -> None:
+    def create(self,
+               segy_out_name: str,
+               src: numpy.ndarray[numpy.float32],
+               custom_info: List[str] = []) -> None:
         """
         create a segy from src
+
+        Parameters:
+        - custom_info: textual header info by user custom, max: 12 rows
+                each row is less than 76 chars
         """
 
     def metaInfo(self) -> str:
         """ 
         the meta info for the whole segy file
         """
 
@@ -99,14 +108,50 @@
         """
 
     def read_trace(self, iZ: int, iY: int) -> numpy.ndarray[numpy.float32]:
         """
         read a trace with index
         """
 
+    def cut(self,
+            outname: str,
+            startZ: int,
+            endZ: int,
+            startY: int,
+            endY: int,
+            startX: int,
+            endX: int,
+            custom_info: List[str] = []) -> None:
+        """
+        - custom_info: textual header info by user custom, max: 12 rows
+                each row is less than 76 chars
+        """
+
+    def cut(self,
+            outname: str,
+            startZ: int,
+            endZ: int,
+            startY: int,
+            endY: int,
+            custom_info: List[str] = []) -> None:
+        """
+        - custom_info: textual header info by user custom, max: 12 rows
+                each row is less than 76 chars
+        """
+
+    def cut(self,
+            outname: str,
+            startX: int,
+            endX: int,
+            custom_info: List[str] = []) -> None:
+        """
+        - custom_info: textual header info by user custom, max: 12 rows
+                each row is less than 76 chars
+        """
+
     def scan(self) -> None:
         """
         scan the whole segy file
         """
 
     def setCrosslineLocation(self, xline: int) -> None:
         """ 
@@ -230,19 +275,31 @@
         """
 
     def get_traceInfo(self, beg: int, end: int) -> numpy.ndarray[int]:
         """
         get traceinfo from beg to end traces: [beg, end)
         """
 
+    def get_lineInfo(self) -> numpy.ndarray:
+        """
+        get lineinfo: [sizeZ, 6]
+        each raw: [inline, crossline_start, crossline_end, 
+        trace_start, trace_end, count]
+        """
+
     def trace_count(self) -> int:
         """
         get the total traces
         """
 
+    def is_crossline_fast_order(self) -> bool:
+        """
+        The fast order is crossline order or not
+        """
+
     pass
 
 
 def fromfile(segy_name: str,
              iline: int = 189,
              xline: int = 193,
              istep: int = 1,
@@ -330,55 +387,67 @@
     - iline: int, the inline number field
     - xline: int, the crossline number field
     - xfield: int, the X field
     - yfield: int, the Y field
 
     Returns:
     a tuple, 
-    - the first element is the data (numpy.ndarray), its shape = (trace_cout, n-time)
+    - the first element is the data (numpy.ndarray), its shape = (trace_count, n-time)
     - the second element is the header, 
-    its shape = (trace_count, 4) = trace_cout * (iline, xline, x, y)
+    its shape = (trace_count, 4) = trace_count * (iline, xline, x, y)
     """
 
 
 def create_by_sharing_header(segy_name: str,
                              header_segy: str,
                              src: numpy.ndarray[numpy.float32],
                              iline: int = 189,
                              xline: int = 193,
                              istep: int = 1,
-                             xstep: int = 1) -> None:
+                             xstep: int = 1,
+                             offset: list or dict = None,
+                             custom_info: List[str] = []) -> None:
     """
     create a segy and its header is from an existed segy.
 
     Parameters:
     - segy_name: str, the out segy name
     - header_segy: str, the header segy file
     - src: numpy.ndarray, source data
     - iline: int, the inline number field of header segy
     - xline: int, the crossline number field of header segy
     - istep: the step of inline numbers
     - xstep: the step of crossline numbers
+    - offset: the offset of a sub data from a original data, 
+            e.g., dsub = d[256:400, 500: 100:], offset = [256, 500, 100]
+    - custom_info: textual header info by user custom, max: 12 rows
+            each row is less than 76 chars, use it when offset is not None
     """
 
 
 def create_by_sharing_header(segy_name: str,
                              header_segy: str,
                              src_file: str,
                              shape: tuple or list,
                              iline: int = 189,
                              xline: int = 193,
                              istep: int = 1,
-                             xstep: int = 1) -> None:
+                             xstep: int = 1,
+                             offset: list or dict = None,
+                             custom_info: List[str] = []) -> None:
     """
     create a segy and its header is from an existed segy.
 
     Parameters:
     - segy_name: str, the out segy name
     - header_segy: str, the header segy file
     - src_file: source data file
     - shape: tuple or list, like: (sizeZ, sizeY, sizeX) or (iline, xline, nt)
     - iline: int, the inline number field of header segy
     - xline: int, the crossline number field of header segy
     - istep: the step of inline numbers
     - xstep: the step of crossline numbers
+    - offset: the offset of a sub data from a original data, 
+            e.g., dsub = d[256:400, 500: 100:], offset = [256, 500, 100]
+    - custom_info: textual header info by user custom, max: 12 rows
+            each row is less than 76 chars, use it when offset is not None
     """
```

### Comparing `cigsegy-1.1.2/python/setup.py` & `cigsegy-1.1.4/python/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             _bdist_wheel.finalize_options(self)
             self.root_is_pure = False
 except ImportError:
     bdist_wheel = None
 
 setup(
     name='cigsegy',
-    version='1.1.2',
+    version='1.1.4',
     description=
     'A tool for segy-format file reading and segy-format creating from binary file',
     author='roger',
     url='https://github.com/JintaoLee-Roger/cigsegy',
     license='MIT',
     cmdclass={'bdist_wheel': bdist_wheel},
     packages=find_packages(),
```

### Comparing `cigsegy-1.1.2/python/tools.py` & `cigsegy-1.1.4/python/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy
-from typing import Tuple
+from typing import List, Tuple
 from .cigsegy import (Pysegy, collect, fromfile, tofile,
                       create_by_sharing_header)
 import warnings
 
 
 def create(segy_out: str,
            binary_in: str or numpy.ndarray,
@@ -12,15 +12,16 @@
            sizeX: int,
            format: int = 5,
            dt: int = 2000,
            start_time: int = 0,
            X_interval: float = 25,
            Y_interval: float = 25,
            min_iline: int = 1,
-           min_xline: int = 1):
+           min_xline: int = 1,
+           custom_info: List[str] = []) -> None:
     """
     Create a segy format file from a binary file or numpy.ndarray
     
     Parameters:
         - segy_out: str, out segy format file path
         - binary_in: str or numpy.array, the input binary file or array
         - sizeZ: int, number of inline
@@ -29,14 +30,16 @@
         - format: int, the data format code, 1 for 4 bytes IBM float, 5 for 4 bytes IEEE float
         - dt: int, data sample interval, 2000 means 2ms
         - start_time: int, start time for each trace
         - X_interval: int
         - Y_interval: int
         - min_iline: int, the start inline number
         - min_xline: int, the start crossline number
+        - custom_info: textual header info by user custom, max: 12 rows
+            each row is less than 76 chars
     """
     if isinstance(binary_in, str):
         segy_create = Pysegy(binary_in, sizeX, sizeY, sizeZ)
     elif isinstance(binary_in, numpy.ndarray):
         if binary_in.shape == (sizeZ, sizeY, sizeX):
             segy_create = Pysegy(sizeX, sizeY, sizeZ)
         else:
@@ -50,87 +53,24 @@
     segy_create.setSampleInterval(dt)
     segy_create.setStartTime(start_time)
     segy_create.setXInterval(X_interval)
     segy_create.setYInterval(Y_interval)
     segy_create.setMinInline(min_iline)
     segy_create.setMinCrossline(min_xline)
     if isinstance(binary_in, str):
-        segy_create.create(segy_out)
+        segy_create.create(segy_out, custom_info)
     else:
-        segy_create.create(segy_out, binary_in)
+        segy_create.create(segy_out, binary_in, custom_info)
 
 
-def is_sorted(header: numpy.ndarray) -> bool:
-    for i in range(header.shape[0] - 1):
-        if (header[i, 0], header[i, 1]) >= (header[i + 1, 0], header[i + 1,
-                                                                     1]):
-            return False
-
-    return True
-
-
-def step(header: numpy.ndarray) -> Tuple[int, int]:
-    warnings.warn(
-        "`step()` function is deprecated and will be removed in the future.",
-        stacklevel=2)
-    iline = numpy.unique(header[:, 0])
-    xline = numpy.unique(header[:, 1])
-    step1 = iline[2] - iline[1]
-    step2 = xline[2] - xline[1]
-    if ((iline + step1)[:-1] == iline[1:]).all() and ((xline + step2)[:-1]
-                                                      == xline[1:]).all():
-        return (step1, step2)
-    else:
-        return (-1, -1)
-
-
-def read_unstrict(segy_name, iline, xline) -> numpy.ndarray:
-    warnings.warn(
-        "`read_unstrict` function is deprecated and will be removed in the future."
-        "Please consider use `fromfile(...)` instead.",
-        stacklevel=2)
-    data, header = collect(segy_name, iline, xline)
-    if not is_sorted(header):
-        raise RuntimeError("the segy file is unsorted, don't supprt now")
-
-    step1, step2 = step(header)
-    if step1 != -1 and step2 != -1:
-        ni = (header[:, 0].max() - header[:, 0].min()) / step1 + 1
-        nx = (header[:, 1].max() - header[:, 1].min()) / step2 + 1
-        nt = data.shape[1]
-        if ni * nx != data.shape[0]:
-            raise RuntimeError(
-                "n-inline * n-crossline != trace_count in this settings")
-
-        data = data.reshape(int(ni), int(nx), nt)
-        return data
-    else:
-        raise RuntimeError("Please use `cigsegy.fromfile()` function")
-
-
-def read_with_step(segy_name, iline, xline, iline_step,
-                   xline_step) -> numpy.ndarray:
-    warnings.warn(
-        "`read_unstrict` function is deprecated and will be removed in the future."
-        "Please consider use `fromfile(..., istep, xstep)` instead.",
-        stacklevel=2)
-    data, header = collect(segy_name, iline, xline)
-    ni = (header[:, 0].max() - header[:, 0].min()) / iline_step + 1
-    nx = (header[:, 1].max() - header[:, 1].min()) / xline_step + 1
-    nt = data.shape[1]
-    if ni * nx != data.shape[0]:
-        raise RuntimeError(
-            "n-inline * n-crossline != trace_count in this settings")
-
-    data = data.reshape(int(ni), int(nx), nt)
-    return data
-
-
-def eval_xline(segy: Pysegy):
-    tracecout = segy.trace_cout()
+def eval_xline(segy: Pysegy) -> List:
+    """
+    To guess the crossline location of the segy
+    """
+    tracecout = segy.trace_count()
     options = [193, 17, 21]
     select = [193, 17, 21]
     for op in options:
         segy.setCrosslineLocation(op)
         l = []
         l.append(segy.get_traceInfo(0)[1])
         l.append(segy.get_traceInfo(1)[1])
@@ -150,16 +90,19 @@
 
     if select == []:
         raise RuntimeError("Cannot evaluate crossline location")
 
     return select
 
 
-def eval_iline(segy: Pysegy):
-    tracecout = segy.trace_cout()
+def eval_iline(segy: Pysegy) -> List:
+    """
+    To guess the inline location of the segy
+    """
+    tracecout = segy.trace_count()
     options = [189, 5, 9, 221]
     select = [189, 5, 9, 221]
     for op in options:
         segy.setInlineLocation(op)
         l0 = segy.get_traceInfo(0)[0]
         ll = segy.get_traceInfo(tracecout - 1)[0]
         l2 = segy.get_traceInfo(tracecout // 2)[0]
@@ -180,27 +123,33 @@
 
     if select == []:
         raise RuntimeError("Cannot evaluate inline location")
 
     return select
 
 
-def eval_xstep(segy: Pysegy, xline):
+def eval_xstep(segy: Pysegy, xline: int) -> int:
+    """
+    To guess the crossline step
+    """
     segy.setCrosslineLocation(xline)
     l0 = segy.get_traceInfo(0)[1]
     l1 = segy.get_traceInfo(1)[1]
     l2 = segy.get_traceInfo(2)[1]
 
     if l2 - l1 != l1 - l0:
         return 0
     else:
         return l2 - l1
 
 
-def eval_istep(segy: Pysegy, iline):
+def eval_istep(segy: Pysegy, iline: int) -> int:
+    """
+    To guess the inline step
+    """
     segy.setInlineLocation(iline)
     i0 = segy.get_traceInfo(0)[0]
     x1 = 1
     while segy.get_traceInfo(x1)[0] == i0:
         x1 += 1
     i1 = segy.get_traceInfo(x1)[0]
 
@@ -211,26 +160,31 @@
 
     if i2 - i1 != i1 - i0:
         return 0
     else:
         return i2 - i1
 
 
-def guess(segy_name: str):
+def guess(segy_name: str or Pysegy) -> List:
     """
     guess the locations and steps of inline and crossline
 
     Parameters:
         - segy_name: str, the input segy file
 
     return:
     locs: [loc1, loc2, ...], all possible loctaions,
           each location is like: [iline, xline, istep, xstep]
     """
-    segy = Pysegy(segy_name)
+    if isinstance(segy_name, str):
+        segy = Pysegy(segy_name)
+    elif isinstance(segy_name, Pysegy):
+        segy = segy_name
+    else:
+        raise TypeError("Invalid type of `segy_name`")
     xlines = eval_xline(segy)
     ilines = eval_iline(segy)
     xselect = []
     iselect = []
     xsteps = []
     isteps = []
 
@@ -263,32 +217,39 @@
 
     if out == []:
         raise RuntimeError("cannot guess the location and steps")
 
     return out
 
 
-def textual_header(segy_name: str):
+def textual_header(segy_name: str) -> None:
+    """
+    Print segy file's 3200 bytes textual header.
+    """
     segy = Pysegy(segy_name)
     print(segy.textual_header())
     segy.close_file()
 
 
 def metaInfo(segy_name: str,
              iline: int = 189,
              xline: int = 193,
              istep: int = 1,
              xstep: int = 1,
-             use_guess: bool = False):
+             xloc: int = 73,
+             yloc: int = 77,
+             use_guess: bool = False) -> None:
     if use_guess:
         [iline, xline, istep, xstep] = guess(segy_name)[0]
     segy = Pysegy(segy_name)
     segy.setInlineLocation(iline)
     segy.setCrosslineLocation(xline)
     segy.setSteps(istep, xstep)
+    segy.setXLocation(xloc)
+    segy.setYLocation(yloc)
     print(segy.metaInfo())
     segy.close_file()
 
 
 def fromfile_by_guess(segy_name: str) -> numpy.ndarray:
     """
     reading from a segy file.
@@ -321,53 +282,129 @@
     """
     loc = guess(segy_name)
     finish = False
 
     for l in loc:
         try:
             metaInfo(segy_name, l[0], l[1], l[2], l[3])
-            tofile(segy_name, l[0], l[1], l[2], l[3])
+            tofile(out_name, l[0], l[1], l[2], l[3])
             finish = True
             break
         except:
             continue
 
     if not finish:
         raise RuntimeError(
             "Cannot read by guess location, please specify the location")
 
 
 def create_by_sharing_header_guess(segy_name: str,
                                    header_segy: str,
                                    src: numpy.ndarray or str,
-                                   shape=None) -> None:
+                                   shape: list or tuple = None,
+                                   offset: list or tuple or dict = None,
+                                   custom_info: List[str] = []) -> None:
     """
     create a segy and its header is from an existed segy.
 
     Parameters:
     - segy_name: str, the out segy name
     - header_segy: str, the header segy file
     - src: numpy.ndarray, source data
     - shape: if src is str, shape must be specify
+    - offset: the offset of a sub data from a original data, 
+            e.g., dsub = d[256:400, 500: 100:], offset = [256, 500, 100]
+    - custom_info: textual header info by user custom, max: 12 rows
+            each row is less than 76 chars, use it when offset is not None
     """
     if isinstance(src, str) and shape is None:
         raise ValueError("Shape is None!")
 
     loc = guess(header_segy)
     finish = False
 
     for l in loc:
         try:
             if isinstance(src, str):
-                create_by_sharing_header(segy_name, header_segy, src, shape,
-                                         l[0], l[1], l[2], l[3])
+                create_by_sharing_header(segy_name,
+                                         header_segy,
+                                         src,
+                                         shape,
+                                         l[0],
+                                         l[1],
+                                         l[2],
+                                         l[3],
+                                         offset=offset,
+                                         custom_info=custom_info)
             else:
-                create_by_sharing_header(segy_name, header_segy, src, l[0],
-                                         l[1], l[2], l[3])
+                create_by_sharing_header(segy_name,
+                                         header_segy,
+                                         src,
+                                         l[0],
+                                         l[1],
+                                         l[2],
+                                         l[3],
+                                         offset=offset,
+                                         custom_info=custom_info)
             finish = True
             break
         except:
             continue
 
     if not finish:
         raise RuntimeError(
             "Cannot read by guess location, please specify the location")
+
+
+def plot_region(segy, loc: list = None, save: str = None) -> None:
+    if isinstance(segy, Pysegy):
+        try:
+            segy.scan()
+        except:
+            loc = guess(segy)[0]
+            segy.setInlineLocation(loc[0])
+            segy.setCrosslineLocation(loc[1])
+            segy.setSteps(loc[2], loc[3])
+            segy.scan()
+        lineinfo = segy.get_lineInfo()
+        is_xline_fast = segy.is_crossline_fast_order()
+    elif isinstance(segy, str):
+        if loc is None:
+            loc = guess(segy)[0]
+        segyc = Pysegy(segy)
+        segyc.setInlineLocation(loc[0])
+        segyc.setCrosslineLocation(loc[1])
+        segyc.setSteps(loc[2], loc[3])
+        segyc.scan()
+        lineinfo = segyc.get_lineInfo()
+        is_xline_fast = segyc.is_crossline_fast_order()
+    else:
+        raise RuntimeError("Invalid type of `segy`")
+
+    x = numpy.concatenate((lineinfo[:, 0], lineinfo[::-1, 0]))
+    y = numpy.concatenate((lineinfo[:, 1], lineinfo[::-1, 2]))
+    x = numpy.append(x, x[0])
+    y = numpy.append(y, y[0])
+
+    istep = x[1] - x[0]
+    xstep = (lineinfo[0, 2] - lineinfo[0, 1]) // (lineinfo[0, 5] - 1)
+    if not is_xline_fast:
+        istep, xstep = xstep, istep
+
+    import matplotlib.pyplot as plt
+
+    plt.fill(x, y, color=(0.9, 0.9, 0.9))
+    plt.plot(x, y)
+    plt.gca().invert_yaxis()
+    # plt.gca().xaxis.set_ticks_position('top')
+
+    plt.grid(True, linestyle='--')
+    xlabel = f"Inline Number/interval={istep}"
+    ylabel = f"Crossline Number/interval={xstep}"
+    if not is_xline_fast:
+        xlabel, ylabel = ylabel, xlabel
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.title('Region')
+    if save:
+        plt.savefig(save, dpi=200, bbox_inches='tight', pad_inches=0.0)
+    plt.show()
```

### Comparing `cigsegy-1.1.2/setup.py` & `cigsegy-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         # fmt_root = v.removeprefix('--fmt_root=')
         fmt_root = v[11:]
         break
 
 cwd = Path(__file__).resolve().parent
 
 package_name = "cigsegy"
-version = "1.1.2"
+version = "1.1.4"
 git_hash = "unknown"
 
 try:
     git_hash = (subprocess.check_output(["git", "rev-parse", "HEAD"],
                                         cwd=cwd).decode().strip())
 except (FileNotFoundError, subprocess.CalledProcessError):
     pass
```

### Comparing `cigsegy-1.1.2/src/include/mio.hpp` & `cigsegy-1.1.4/src/include/mio.hpp`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/src/include/progressbar.hpp` & `cigsegy-1.1.4/src/include/progressbar.hpp`

 * *Files identical despite different names*

### Comparing `cigsegy-1.1.2/src/include/segy.h` & `cigsegy-1.1.4/src/include/segy.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 /*********************************************************************
-** Copyright (c) 2022 Roger Lee.
+** Copyright (c) 2023 Roger Lee.
 ** Computational and Interpretation Group (CIG),
 ** University of Science and Technology of China (USTC).
 **
 ** @File: segy.h
-** @Time: 2022/11/16 11:30:42
-** @Version: 1.0
 ** @Description :
 *********************************************************************/
 
 #ifndef CIG_SEGY_H
 #define CIG_SEGY_H
 
 #include <stdexcept>
@@ -51,16 +49,18 @@
 
   int inline_step = 1;
   int crossline_step = 1;
 };
 
 struct LineInfo {
   int line_num;
-  uint64_t trace_start;
-  uint64_t trace_end;
+  int crossline_start;
+  int crossline_end;
+  int trace_start;
+  int trace_end;
   int count;
 };
 
 struct TraceInfo {
   int inline_num;
   int crossline_num;
   int X;
@@ -86,90 +86,94 @@
     } else if (dimension == 2) {
       return m_metaInfo.sizeZ;
     } else {
       throw std::runtime_error("shape(dim), dim can be only {0, 1, 2}");
     }
   }
 
-  inline int64_t trace_count() { return m_metaInfo.trace_count; }
+  int64_t trace_count();
+  void set_size(int x, int y, int z);
 
-  inline void set_size(int x, int y, int z) {
-    m_metaInfo.sizeX = x;
-    m_metaInfo.sizeY = y;
-    m_metaInfo.sizeZ = z;
-    if (isReadSegy) {
-      m_metaInfo.isNormalSegy = true;
-      isScan = true;
-      int64_t trace_count =
-          (m_source.size() - kTextualHeaderSize - kBinaryHeaderSize) /
-          (kTraceHeaderSize + x * sizeof(float));
-      if ((int64_t)y * z != (trace_count)) {
-        throw std::runtime_error("invalid shape. inline * crossline != "
-                                 "total_trace_count");
-      }
-    }
-  }
-
-  void collect(float *data, int *header);
-
-  std::string textual_header();
-  std::string metaInfo();
   inline std::vector<LineInfo> line_info() { return m_lineInfo; }
   inline MetaInfo get_metaInfo() { return m_metaInfo; }
+  inline bool is_crossline_fast_order() { return is_crossline_fast; }
 
+  // read segy
   void setInlineLocation(int loc);
   void setCrosslineLocation(int loc);
   void setXLocation(int loc);
   void setYLocation(int loc);
-
   void setInlineStep(int step);
   void setCrosslineStep(int step);
   void setSteps(int istep, int xstep);
-
-  // read segy
   void setFillNoValue(float noValue);
-  void scan();
-  void tofile(const std::string &binary_out_name);
-  void read(float *dst, int startX, int endX, int startY, int endY, int startZ,
-            int endZ);
-  void read(float *dst);
-  void read_inline_slice(float *dst, int iZ);
-  void read_cross_slice(float *dst, int iY);
-  void read_time_slice(float *dst, int iX);
-  void read_trace(float *dst, int iY, int iZ);
-
-  // binary header & trace header
-  void get_TraceInfo(int n, int *traceinfo);
 
   // create segy
   void setSampleInterval(int interval);
   void setDataFormatCode(int fdormat);
   void setStartTime(int start_time);
   void setXInterval(float dz);
   void setYInterval(float dy);
   void setMinInline(int in);
   void setMinCrossline(int cross);
 
-  void create(const std::string &segy_out_name, const float *src);
-  void create(const std::string &segy_out_name);
+  std::string textual_header();
+  std::string metaInfo();
+  // binary header & trace header
+  void get_TraceInfo(int n, int *traceinfo);
+
+  void collect(float *data, int *header);
+
+  // read segy
+  void scan();
+  void read(float *dst, int startX, int endX, int startY, int endY, int startZ,
+            int endZ);
+  void read(float *dst);
+  void read_inline_slice(float *dst, int iZ);
+  void read_cross_slice(float *dst, int iY);
+  void read_time_slice(float *dst, int iX);
+  void read_trace(float *dst, int iY, int iZ);
+  void tofile(const std::string &binary_out_name);
+  void
+  cut(const std::string &outname, int startX, int endX, int startY, int endY,
+      int startZ, int endZ,
+      const std::vector<std::string> &custom_info = std::vector<std::string>());
+  void
+  cut(const std::string &outname, int startY, int endY, int startZ, int endZ,
+      const std::vector<std::string> &custom_info = std::vector<std::string>());
+  void
+  cut(const std::string &outname, int startX, int endX,
+      const std::vector<std::string> &custom_info = std::vector<std::string>());
+
+  // create
+  void create(
+      const std::string &segy_out_name, const float *src,
+      const std::vector<std::string> &custom_info = std::vector<std::string>());
+  void create(
+      const std::string &segy_out_name,
+      const std::vector<std::string> &custom_info = std::vector<std::string>());
 
   void close_file();
 
 private:
-  bool isReadSegy{};
+  bool isReadSegy;
   bool isScan = false;
+  bool is_crossline_fast = true;
   mio::mmap_source m_source;
   mio::mmap_sink m_sink;
   std::vector<LineInfo> m_lineInfo;
   MetaInfo m_metaInfo;
 
   void scanBinaryHeader();
   void initMetaInfo();
+  void check_order();
   void initTraceHeader(TraceHeader *trace_header);
-  void write_textual_header(char *dst, const std::string &segy_out_name);
+  void write_textual_header(
+      char *dst, const std::string &segy_out_name,
+      const std::vector<std::string> &custom_info = std::vector<std::string>());
   void write_binary_header(char *dst);
   void write_trace_header(char *dst, TraceHeader *trace_header, int32_t iY,
                           int32_t iZ, int32_t x, int32_t y);
 
   inline void _get_TraceInfo(uint64_t n, TraceInfo &tmetaInfo) {
     const char *field =
         m_source.data() + kTextualHeaderSize + kBinaryHeaderSize +
@@ -179,34 +183,38 @@
     tmetaInfo.crossline_num =
         swap_endian(*(int32_t *)(field + m_metaInfo.crossline_field - 1));
     tmetaInfo.X = swap_endian(*(int32_t *)(field + m_metaInfo.X_field - 1));
     tmetaInfo.Y = swap_endian(*(int32_t *)(field + m_metaInfo.Y_field - 1));
   }
 };
 
-void read_ignore_header(const std::string &segy_name, float *dst, int sizeX,
-                        int sizeY, int sizeZ, int format = 5);
-void tofile_ignore_header(const std::string &segy_name,
-                          const std::string &out_name, int sizeX, int sizeY,
-                          int sizeZ, int format = 5);
+void read(const std::string &segy_name, float *dst,
+          int iline = kDefaultInlineField, int xline = kDefaultCrosslineField,
+          int istep = 1, int xstep = 1);
 
 void tofile(const std::string &segy_name, const std::string &out_name,
             int iline = kDefaultInlineField, int xline = kDefaultCrosslineField,
             int istep = 1, int xstep = 1);
 
-void read(const std::string &segy_name, float *dst,
-          int iline = kDefaultInlineField, int xline = kDefaultCrosslineField,
-          int istep = 1, int xstep = 1);
+void read_ignore_header(const std::string &segy_name, float *dst, int sizeX,
+                        int sizeY, int sizeZ, int format = 5);
+
+void tofile_ignore_header(const std::string &segy_name,
+                          const std::string &out_name, int sizeX, int sizeY,
+                          int sizeZ, int format = 5);
 
-void create_by_sharing_header(const std::string &segy_name,
-                              const std::string &header_segy, const float *src,
-                              int sizeX, int sizeY, int sizeZ, int iline = 189,
-                              int xline = 193, int istep = 1, int xstep = 1);
-
-void create_by_sharing_header(const std::string &segy_name,
-                              const std::string &header_segy,
-                              const std::string &src_file, int sizeX, int sizeY,
-                              int sizeZ, int iline = 189, int xline = 193,
-                              int istep = 1, int xstep = 1);
+void create_by_sharing_header(
+    const std::string &segy_name, const std::string &header_segy,
+    const float *src, int sizeX, int sizeY, int sizeZ, int iline = 189,
+    int xline = 193, int istep = 1, int xstep = 1, int offsetX = -1,
+    int offsetY = -1, int offsetZ = -1,
+    const std::vector<std::string> &custom_info = std::vector<std::string>());
+
+void create_by_sharing_header(
+    const std::string &segy_name, const std::string &header_segy,
+    const std::string &src_file, int sizeX, int sizeY, int sizeZ,
+    int iline = 189, int xline = 193, int istep = 1, int xstep = 1,
+    int offsetX = -1, int offsetY = -1, int offsetZ = -1,
+    const std::vector<std::string> &custom_info = std::vector<std::string>());
 } // namespace segy
 
 #endif
```

### Comparing `cigsegy-1.1.2/src/include/utils.h` & `cigsegy-1.1.4/src/include/utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 /*********************************************************************
-** Copyright (c) 2022 Roger Lee.
+** Copyright (c) 2023 Roger Lee.
 ** Computational and Interpretation Group (CIG),
 ** University of Science and Technology of China (USTC).
 **
 ** @File: utils.h
-** @Time: 2022/11/16 11:12:32
-** @Version: 1.0
 ** @Description :
 *********************************************************************/
 #ifndef CIG_UTILS_H
 #define CIG_UTILS_H
 
 #include <cctype>
 #include <climits>
@@ -34,15 +32,16 @@
 
 // const binary header field
 const int kBSampleIntervalField = 17;
 const int kBSampleCountField = 21;
 const int kBSampleFormatField = 25;
 
 // const trace header field
-const int kTStartTimeField = 111; // TODO(Jintao): check
+const int kTStartTimeField = 105; // in ms
+const int kTDelayTimeField = 109; // in ms
 const int kTScalarField = 71;
 const int kTSampleCountField = 115;
 const int kTSampleIntervalField = 117;
 
 const int kDefaultInlineField = 189;
 const int kDefaultCrosslineField = 193;
 const int kDefaultXField = 73;
```

### Comparing `cigsegy-1.1.2/src/segy.cpp` & `cigsegy-1.1.4/src/segy.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,312 @@
 /*********************************************************************
-** Copyright (c) 2022 Roger Lee.
+** Copyright (c) 2023 Roger Lee.
 ** Computational and Interpretation Group (CIG),
 ** University of Science and Technology of China (USTC).
 **
 ** @File: segy.cpp
-** @Time: 2022/11/18 16:28:37
-** @Version: 1.0
 ** @Description :
 *********************************************************************/
 
 #include "segy.h"
+#include <cassert>
 #include <chrono>
 #include <cstring>
+#include <numeric>
+#include <vector>
 #define FMT_HEADER_ONLY
 #include <fmt/format.h>
+#include <fstream>
 #include <stdexcept>
 
-#ifdef WIN32
-#include <fcntl.h>
-#include <io.h>
-#define open _open
-#define lseek _lseek
-#define close _close
-#define write _write
-#define O_RDWR _O_RDWR
-#define O_CREAT _O_CREAT
-#define O_TRUNC _O_TRUNC
-#endif
+// #ifdef WIN32
+// #include <fcntl.h>
+// #include <io.h>
+// #define open _open
+// #define lseek _lseek
+// #define close _close
+// #define write _write
+// #define O_RDWR _O_RDWR
+// #define O_CREAT _O_CREAT
+// #define O_TRUNC _O_TRUNC
+// #endif
 
 #include "mio.hpp"
 #include "progressbar.hpp"
 #include "utils.h"
 
 namespace segy {
 
+/********************* static functions ***************************/
+
+static inline void updatebar(progressbar &bar, int n) {
+  for (int i = 0; i < n; i++) {
+    bar.update();
+  }
+}
+
+static inline std::string field_str(int field, int len = 2) {
+  return fmt::format("{}-{}", field, field + len - 1);
+}
+
+static inline int32_t getCrossline(const char *source, int field) {
+  return swap_endian(*(int32_t *)(source + field - 1));
+}
+
+static inline std::string align_80(const std::string &s) {
+  return fmt::format("{:<76}", s);
+}
+
+static inline std::string catstr(const std::string &s1, const std::string &s2) {
+  return s1 + s2;
+}
+
+static inline std::string create_textual_header(
+    const MetaInfo &meta_info, const std::string &segyname = "",
+    const std::vector<std::string> &custom_info = std::vector<std::string>()) {
+  std::vector<std::string> header;
+
+  auto now =
+      std::chrono::system_clock::to_time_t(std::chrono::system_clock::now());
+  std::string time_string(25, ' ');
+  std::strftime(&time_string[0], time_string.size(), "%Y-%m-%d %H:%M:%S",
+                std::localtime(&now));
+
+  float Y_interval, Z_interval;
+  if (meta_info.scalar != 0) {
+    Y_interval = meta_info.scalar > 0
+                     ? meta_info.Y_interval * meta_info.scalar
+                     : meta_info.Y_interval / -meta_info.scalar;
+    Z_interval = meta_info.scalar > 0
+                     ? meta_info.Z_interval * meta_info.scalar
+                     : meta_info.Z_interval / -meta_info.scalar;
+  }
+
+  std::string dformat = meta_info.data_format == 1
+                            ? "4-bytes IBM floating-point"
+                            : "4-bytes IEEE floating-point";
+
+  if (custom_info.size() > 12) {
+    fmt::print("The max rows of custom_info header are 12 rows, but the vector "
+               "contian {} strings. We will drop the last strings.",
+               custom_info.size());
+  }
+
+  if (custom_info.size() > 0) {
+    for (int i = 0; i < 12; i++) {
+      if (i >= custom_info.size()) {
+        header.push_back(align_80(""));
+      } else {
+        header.push_back(align_80(custom_info[i]));
+      }
+    }
+  } else {
+    header.push_back(
+        align_80("Create By CIGSEGY software (CIG, USTC, 2023), see:"));
+    header.push_back(
+        align_80("github: https://github.com/JintaoLee-Roger/cigsegy"));
+    header.push_back(align_80(""));
+    header.push_back(align_80(fmt::format("Name: {}", segyname)));
+    header.push_back(align_80(
+        fmt::format("Type: 3D seismic  Created Time: {}", time_string)));
+    header.push_back(align_80(""));
+    header.push_back(align_80(""));
+    header.push_back(align_80(""));
+    header.push_back(align_80(""));
+    header.push_back(align_80(""));
+    header.push_back(align_80(""));
+    header.push_back(align_80(""));
+  }
+
+  header.push_back(align_80(fmt::format(
+      "Inline range:    {} - {}", meta_info.min_inline, meta_info.max_inline)));
+  header.push_back(
+      align_80(fmt::format("Crossline range: {} - {}", meta_info.min_crossline,
+                           meta_info.max_crossline)));
+  header.push_back(
+      align_80(fmt::format("Inline step: {}, Crossline step: {}",
+                           meta_info.inline_step, meta_info.crossline_step)));
+  header.push_back(align_80(
+      fmt::format("shape: (n-time, n-crossline, n-time) = ({}, {}, {})",
+                  meta_info.sizeX, meta_info.sizeY, meta_info.sizeZ)));
+  header.push_back(align_80(
+      fmt::format("Number of samples per data trace: {}", meta_info.sizeX)));
+  header.push_back(
+      align_80(fmt::format("Sample nterval: {} ", meta_info.sample_interval)));
+  header.push_back(align_80(fmt::format("Data sample format: {}", dformat)));
+  header.push_back(align_80(fmt::format(
+      "X interval: {} meters, Y interval: {} meters", Y_interval, Z_interval)));
+  header.push_back(
+      align_80(fmt::format("Time start: {}", meta_info.start_time)));
+
+  header.push_back(align_80(""));
+  header.push_back(align_80(""));
+  header.push_back(align_80(""));
+  header.push_back(align_80("Binary header locations:"));
+  header.push_back(
+      align_80(fmt::format("Sample interval             : bytes {}",
+                           field_str(kBSampleIntervalField))));
+  header.push_back(
+      align_80(fmt::format("Number of samples per trace : bytes {}",
+                           field_str(kBSampleCountField))));
+  header.push_back(
+      align_80(fmt::format("Data sample format code     : bytes {}",
+                           field_str(kBSampleFormatField))));
+  header.push_back(align_80(""));
+  header.push_back(align_80(""));
+  header.push_back(align_80("Trace header locations:"));
+  header.push_back(
+      align_80(fmt::format("Inline number               : bytes {}",
+                           field_str(meta_info.inline_field, 4))));
+  header.push_back(
+      align_80(fmt::format("Crossline number            : bytes {}",
+                           field_str(meta_info.crossline_field, 4))));
+  header.push_back(
+      align_80(fmt::format("X coordinate                : bytes {}",
+                           field_str(meta_info.X_field, 4))));
+  header.push_back(
+      align_80(fmt::format("Y coordinate                : bytes {}",
+                           field_str(meta_info.Y_field, 4))));
+  header.push_back(align_80(fmt::format(
+      "Trace start time/depth      : bytes {}", field_str(kTStartTimeField))));
+  header.push_back(
+      align_80(fmt::format("Number of samples per trace : bytes {}",
+                           field_str(kTSampleCountField))));
+  header.push_back(
+      align_80(fmt::format("Sample interval             : bytes {}",
+                           field_str(kTSampleIntervalField))));
+  header.push_back(align_80(""));
+  header.push_back(align_80(""));
+
+  assert(header.size() == kTextualRows);
+
+  for (int i = 0; i < header.size(); i++) {
+    header[i] = fmt::format("C{:02} ", i + 1) + header[i];
+  }
+
+  std::string out =
+      std::accumulate(header.begin(), header.end(), std::string{}, catstr);
+
+  assert(out.length() == kTextualHeaderSize);
+
+  for (auto &s : out) {
+    s = getEBCIDfromASCII(s);
+  }
+
+  return out;
+}
+
+static inline void modify_traceheader(char *trace_header, int sizeX,
+                                      int start_time = -1) {
+  int16_t *int_header = reinterpret_cast<int16_t *>(trace_header);
+  int_header[(kTSampleCountField - 1) / 2] =
+      swap_endian(static_cast<int16_t>(sizeX));
+  if (start_time > 0) {
+    int_header[(kTStartTimeField - 1) / 2] =
+        swap_endian(static_cast<int16_t>(start_time));
+    int_header[(kTDelayTimeField - 1) / 2] =
+        swap_endian(static_cast<int16_t>(start_time));
+  }
+}
+
+static int64_t copy_traces(const mio::mmap_source &header,
+                           const std::vector<LineInfo> &line_info,
+                           const MetaInfo &meta_info, const float *src,
+                           char *outptr, int sizeX, int sizeY, int sizeZ,
+                           int offsetX, int offsetY, int offsetZ,
+                           int start_time) {
+  // trace header and data
+  char *start_outptr = outptr;
+
+  int trace_count = 0;
+
+  int step = sizeZ >= 100 ? 1 : 100 / sizeZ + 1;
+  int nbar = sizeZ >= 100 ? sizeZ : step * sizeZ;
+  progressbar bar(nbar);
+
+  int trace_size = kTraceHeaderSize + sizeX * sizeof(float);
+  int trace_size_ori = kTraceHeaderSize + meta_info.sizeX * sizeof(float);
+
+  for (int iz = 0; iz < sizeZ; iz++) {
+    updatebar(bar, step);
+
+    const float *srcopy = src + iz * sizeY * sizeX;
+
+    int izo = iz + offsetZ;
+    const char *header_ptr = header.data() + kTextualHeaderSize +
+                             kBinaryHeaderSize +
+                             trace_size_ori * line_info[izo].trace_start;
+
+    int count_in_line = 0;
+    int xyzspace_start = 0;
+    int xyzspace_end = 0;
+    for (int iyo = 0; iyo < line_info[izo].count; iyo++) {
+      int srct = iyo;
+      if (line_info[izo].count != meta_info.sizeY) {
+        const int32_t *tmp = reinterpret_cast<const int32_t *>(header_ptr);
+        srct = swap_endian(
+                   tmp[(iyo * trace_size_ori + meta_info.crossline_field - 1) /
+                       4]) -
+               meta_info.min_crossline;
+
+        srct /= meta_info.crossline_step;
+      }
+      if (iyo == 0) {
+        xyzspace_start = srct;
+      }
+      if (iyo == line_info[izo].count) {
+        xyzspace_end = srct + 1;
+      }
+
+      if (srct >= offsetY && srct < (offsetY + sizeY)) {
+        count_in_line++;
+        trace_count++;
+        int iy = srct - offsetY;
+
+        // copy header & modify sample count and start time
+        memcpy(outptr, header_ptr + iyo * trace_size_ori, kTraceHeaderSize);
+        if (sizeX != meta_info.sizeX) {
+          modify_traceheader(outptr, sizeX, start_time);
+        }
+        outptr += kTraceHeaderSize;
+
+        // copy data
+        memcpy(outptr, srcopy + iy * sizeX, sizeX * sizeof(float));
+        float *floatptr = reinterpret_cast<float *>(outptr);
+        for (int ix = 0; ix < sizeX; ix++) {
+          if (meta_info.data_format == 1) {
+            floatptr[ix] = ieee_to_ibm(floatptr[ix], true);
+          }
+          floatptr[ix] = swap_endian(floatptr[ix]);
+        }
+        floatptr = nullptr;
+        outptr += (sizeX * sizeof(float));
+      }
+    }
+    if (count_in_line == 0) {
+      throw std::runtime_error(fmt::format(
+          "Can not copy headers through the index, becuase the line {} "
+          "contains 0 trace if use the offsetY and sizeY."
+          "In line {}, the header file's crossline range: "
+          "[{}, {}], in the 3D volume space, y axis is range:"
+          "[{}, {}), while your binary is range: [offsetY, offsetY+sizeY] "
+          "= [{}, {}).",
+          izo, izo, line_info[izo].crossline_start,
+          line_info[izo].crossline_end, xyzspace_start, xyzspace_end, offsetY,
+          offsetY + sizeY));
+    }
+  }
+  assert((outptr - start_outptr) == (trace_count * trace_size));
+  fmt::print("\n");
+
+  return trace_count * trace_size;
+}
+
+/********************* SegyIO public ***************************/
+
 SegyIO::SegyIO(const std::string &segyname) {
   this->isReadSegy = true;
   memset(&this->m_metaInfo, 0, sizeof(MetaInfo));
   std::error_code error;
   this->m_source.map(segyname, error);
   if (error) {
     throw std::runtime_error("Cannot mmap segy file");
@@ -70,35 +339,42 @@
 
 SegyIO::~SegyIO() {
   if (m_source.is_mapped()) {
     m_source.unmap();
   }
 }
 
+int64_t SegyIO::trace_count() { return m_metaInfo.trace_count; }
+
+void SegyIO::set_size(int x, int y, int z) {
+  m_metaInfo.sizeX = x;
+  m_metaInfo.sizeY = y;
+  m_metaInfo.sizeZ = z;
+  if (isReadSegy) {
+    m_metaInfo.isNormalSegy = true;
+    isScan = true;
+    int64_t trace_count =
+        (m_source.size() - kTextualHeaderSize - kBinaryHeaderSize) /
+        (kTraceHeaderSize + x * sizeof(float));
+    if ((int64_t)y * z != (trace_count)) {
+      throw std::runtime_error("invalid shape. inline * crossline != "
+                               "total_trace_count");
+    }
+  }
+}
+
 void SegyIO::setInlineLocation(int loc) {
-  // if (loc != 5 && loc != 9 && loc != 189) {
-  //   fmt::print("[Warning]: You set a unusual inline field: {}, the best
-  //   choice "
-  //              "is setting it as 189 or 5 or 9.\n",
-  //              loc);
-  // }
   if (loc <= 0) {
     throw std::runtime_error("Invalid location (must > 0)");
   }
   m_metaInfo.inline_field = loc;
   isScan = false;
 }
 
 void SegyIO::setCrosslineLocation(int loc) {
-  // if (loc != 193 && loc != 17 && loc != 21) {
-  //   fmt::print(
-  //       "[Warning]: You set a unusual crossline field: {}, the best choice "
-  //       "is set it as 193 or 17 or 21.\n",
-  //       loc);
-  // }
   if (loc <= 0) {
     throw std::runtime_error("Invalid location (must > 0)");
   }
   m_metaInfo.crossline_field = loc;
   isScan = false;
 }
 
@@ -206,32 +482,144 @@
     throw std::runtime_error("Invalid crossline number (must > 0)");
   }
   m_metaInfo.min_crossline = cross;
   m_metaInfo.max_crossline = cross + m_metaInfo.sizeY - 1;
   isScan = false;
 }
 
-void SegyIO::scanBinaryHeader() {
-  const auto *binary_header = reinterpret_cast<const BinaryHeader *>(
-      m_source.data() + kTextualHeaderSize);
-  m_metaInfo.data_format = swap_endian(binary_header->data_format);
-  m_metaInfo.sizeX = swap_endian(binary_header->trace_length);
-  m_metaInfo.sample_interval = swap_endian(binary_header->sample_interval);
-  m_metaInfo.trace_count =
-      (m_source.size() - kTextualHeaderSize - kBinaryHeaderSize) /
-      (kTraceHeaderSize + m_metaInfo.sizeX * sizeof(float));
+std::string SegyIO::textual_header() {
+  if (!isReadSegy && m_sink.size() < kTextualHeaderSize) {
+    throw std::runtime_error(
+        "No textual header, because this is not a segy "
+        "file (read mode) or you don't create textual header (create mode)");
+  }
+  const char *textual_header = nullptr;
+  if (isReadSegy) {
+    textual_header = m_source.data();
+  } else {
+    textual_header = m_sink.data();
+  }
+  char out[kTextualHeaderSize + kTextualRows];
+  bool isEBCDIC = isTextInEBCDICFormat(textual_header, kTextualHeaderSize);
+  for (int iRow = 0; iRow < kTextualRows; iRow++) {
+    int offset = iRow * kTextualColumns;
+    for (int iCol = 0; iCol < kTextualColumns; iCol++) {
+      if (isEBCDIC) {
+        out[iCol + offset + iRow] =
+            getASCIIfromEBCDIC(textual_header[iCol + offset]);
+      } else {
+        out[iCol + offset + iRow] = textual_header[iCol + offset];
+      }
+    }
+    if (iRow < kTextualRows - 1) {
+      out[(iRow + 1) * (kTextualColumns + 1) - 1] = '\n';
+    }
+  }
+
+  return std::string(out);
+}
+
+std::string SegyIO::metaInfo() {
+  if (!isScan && isReadSegy) {
+    scan();
+  }
+
+  float Y_interval = 0;
+  float Z_interval = 0;
+
+  if (m_metaInfo.scalar != 0) {
+
+    Y_interval = m_metaInfo.scalar > 0
+                     ? m_metaInfo.Y_interval * m_metaInfo.scalar
+                     : m_metaInfo.Y_interval / -m_metaInfo.scalar;
+    Z_interval = m_metaInfo.scalar > 0
+                     ? m_metaInfo.Z_interval * m_metaInfo.scalar
+                     : m_metaInfo.Z_interval / -m_metaInfo.scalar;
+  }
+
+  if (!is_crossline_fast) {
+    float t = Y_interval;
+    Y_interval = Z_interval;
+    Z_interval = t;
+  }
+
+  int sizeY, sizeZ, ifield, xfield, istart, iend, xstart, xend, istep, xstep;
+  sizeY = is_crossline_fast ? m_metaInfo.sizeY : m_metaInfo.sizeZ;
+  sizeZ = is_crossline_fast ? m_metaInfo.sizeZ : m_metaInfo.sizeY;
+  ifield =
+      is_crossline_fast ? m_metaInfo.inline_field : m_metaInfo.crossline_field;
+  xfield =
+      is_crossline_fast ? m_metaInfo.crossline_field : m_metaInfo.inline_field;
+  istart = is_crossline_fast ? m_metaInfo.min_inline : m_metaInfo.min_crossline;
+  iend = is_crossline_fast ? m_metaInfo.max_inline : m_metaInfo.max_crossline;
+  xstart = is_crossline_fast ? m_metaInfo.min_crossline : m_metaInfo.min_inline;
+  xend = is_crossline_fast ? m_metaInfo.max_crossline : m_metaInfo.max_inline;
+  istep =
+      is_crossline_fast ? m_metaInfo.inline_step : m_metaInfo.crossline_step;
+  xstep =
+      is_crossline_fast ? m_metaInfo.crossline_step : m_metaInfo.inline_step;
+
+  std::string shapeinfo =
+      is_crossline_fast
+          ? fmt::format(
+                "In python, the shape is (n-inline, n-crossline, n-time) "
+                "= ({}, {}, {}).\n\n",
+                sizeZ, sizeY, m_metaInfo.sizeX)
+          : fmt::format(
+                "In python, the shape is (n-crossline, n-inline, n-time) "
+                "= ({}, {}, {}), as the fast order is inline\n"
+                "You need transpose it manully, "
+                "such as, in numpy, `d = d.transpose(1, 0, 2)`\n\n",
+                sizeY, sizeZ, m_metaInfo.sizeX);
+
+  std::string dformat = m_metaInfo.data_format == 1
+                            ? "4-bytes IBM floating-point"
+                            : "4-bytes IEEE floating-point";
+  return fmt::format("{}shape: (n-time, n-crossline, n-inline) = ({}, {}, {})\n"
+                     "sample interval: {}, data format code: {}\n"
+                     "inline range: {} - {}, crossline range: {} - {}\n"
+                     "X interval: {:.1f}, Y interval: {:.1f}, time start: {}\n"
+                     "inline field: {}, crossline field: {}\n"
+                     "inline step: {}, crossline step: {}\n"
+                     "Is regular file (no missing traces): {}",
+                     shapeinfo, m_metaInfo.sizeX, sizeY, sizeZ,
+                     m_metaInfo.sample_interval, dformat, istart, iend, xstart,
+                     xend, Y_interval, Z_interval, m_metaInfo.start_time,
+                     ifield, xfield, istep, xstep, m_metaInfo.isNormalSegy);
 }
 
 void SegyIO::get_TraceInfo(int n, int *traceinfo) {
   if (m_metaInfo.trace_count <= n || n < 0) {
     throw std::runtime_error("the trace number must be in [0, ntrace-1)");
   }
   _get_TraceInfo(n, *reinterpret_cast<TraceInfo *>(traceinfo));
 }
 
+void SegyIO::collect(float *data, int *header) {
+  const char *source = m_source.data() + kTextualHeaderSize + kBinaryHeaderSize;
+  int32_t trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
+  progressbar bar(100);
+  for (int i = 0; i < m_metaInfo.trace_count; i++) {
+    if (i % (m_metaInfo.trace_count / 100) == 0) {
+      bar.update();
+    }
+    _get_TraceInfo(i, *reinterpret_cast<TraceInfo *>(header));
+    memcpy(data, source + kTraceHeaderSize, m_metaInfo.sizeX * sizeof(float));
+    for (int j = 0; j < m_metaInfo.sizeX; j++) {
+      if (m_metaInfo.data_format == 1) {
+        data[j] = ibm_to_ieee(data[j], true);
+      } else {
+        data[j] = swap_endian(data[j]);
+      }
+    }
+    data += m_metaInfo.sizeX;
+    header += 4;
+  }
+}
+
 void SegyIO::scan() {
   if (!isReadSegy) {
     throw std::runtime_error(
         "'scan()' function only used in reading segy mode.");
   }
 
   isScan = true;
@@ -261,14 +649,20 @@
   int trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
   const char *start = m_source.data() + kTextualHeaderSize + kBinaryHeaderSize;
   m_metaInfo.start_time = swap_endian(
       *reinterpret_cast<const int16_t *>(start + kTStartTimeField - 1));
   m_metaInfo.scalar = swap_endian(
       *reinterpret_cast<const int16_t *>(start + kTScalarField - 1));
 
+  // check order, is the fast order inline or crossline?
+  // the default is crossline
+  // if the fast order is inline, then exchange the location
+  // of inline and crossline
+  check_order();
+
   // line x: ... trace1
   // line x+1: trace2 ...
   TraceInfo trace1{}, trace2{};
   _get_TraceInfo(0, trace1);
   _get_TraceInfo(m_metaInfo.trace_count - 1, trace2);
 
   m_metaInfo.sizeZ =
@@ -286,24 +680,26 @@
         "Size Z (inline number) is invalid, don't support. Maybe the "
         "inline location is wrong, use 'setInlineLocation(loc)' to set.");
   }
 
   m_metaInfo.isNormalSegy =
       m_metaInfo.trace_count % m_metaInfo.sizeZ == 0 ? true : false;
   m_lineInfo.resize(m_metaInfo.sizeZ);
+  m_lineInfo[m_metaInfo.sizeZ - 1].crossline_end = trace2.crossline_num;
 
   // fill m_lineInfo
   int jump = m_metaInfo.trace_count / m_metaInfo.sizeZ;
   m_metaInfo.sizeY = jump;
-  int64_t itrace = 0;
+  int itrace = 0;
   _get_TraceInfo(0, trace2);
   for (int i = 0; i < m_metaInfo.sizeZ - 1; i++) {
     m_lineInfo[i].trace_start = itrace;
     m_lineInfo[i].line_num = trace2.inline_num;
     m_lineInfo[i].count = 1;
+    m_lineInfo[i].crossline_start = trace2.crossline_num;
 
     if (trace2.crossline_num < m_metaInfo.min_crossline) {
       m_metaInfo.min_crossline = trace2.crossline_num;
     }
 
     itrace += jump;
     if (itrace >= m_metaInfo.trace_count) {
@@ -325,14 +721,15 @@
         if (jump > kMaxSizeOneDimemsion || itrace >= m_metaInfo.trace_count) {
           throw std::runtime_error(
               "inline/crossline location is wrong, use "
               "'setInlineLocation(loc)'/'setCrosslineLocation(loc)' to set");
         }
         _get_TraceInfo(itrace, trace2);
       }
+      _get_TraceInfo(itrace - 1, trace1);
       // if (jump > m_metaInfo.sizeY) {
       //   m_metaInfo.sizeY = jump;
       // }
     } else if (trace1.inline_num > m_lineInfo[i].line_num) {
       m_metaInfo.isNormalSegy = false;
       while (trace1.inline_num != m_lineInfo[i].line_num && itrace > 0 &&
              jump > 0) {
@@ -342,56 +739,59 @@
           throw std::runtime_error(
               "inline/crossline location is wrong, use "
               "'setInlineLocation(loc)'/'setCrosslineLocation(loc)' to set");
         }
         trace2 = trace1;
         _get_TraceInfo(itrace - 1, trace1);
       }
+      _get_TraceInfo(itrace, trace2);
     }
 
-    m_metaInfo.sizeY = m_metaInfo.max_crossline - m_metaInfo.min_crossline + 1;
+    m_metaInfo.sizeY = (m_metaInfo.max_crossline - m_metaInfo.min_crossline) /
+                           m_metaInfo.crossline_step +
+                       1;
 
     if (trace2.inline_num == m_lineInfo[i].line_num + m_metaInfo.inline_step &&
         trace1.inline_num == m_lineInfo[i].line_num) {
       if (trace1.crossline_num > m_metaInfo.max_crossline) {
         m_metaInfo.max_crossline = trace1.crossline_num;
       }
       m_lineInfo[i].trace_end = itrace - 1;
       m_lineInfo[i].count = itrace - m_lineInfo[i].trace_start;
+      m_lineInfo[i].crossline_end = trace1.crossline_num;
     } else {
       throw std::runtime_error("Cannot analysis this segy file, "
                                "may inline step != 1");
     }
   }
 
   // the last line
   m_lineInfo[m_metaInfo.sizeZ - 1].trace_start = itrace;
   m_lineInfo[m_metaInfo.sizeZ - 1].line_num = trace2.inline_num;
   m_lineInfo[m_metaInfo.sizeZ - 1].trace_end = m_metaInfo.trace_count - 1;
   m_lineInfo[m_metaInfo.sizeZ - 1].count = m_metaInfo.trace_count - itrace;
+  m_lineInfo[m_metaInfo.sizeZ - 1].crossline_start = trace2.crossline_num;
 
   // cal x, y interval
   _get_TraceInfo(0, trace1);
   _get_TraceInfo(m_lineInfo[0].trace_end, trace2);
+  // float scale =
+  //     m_metaInfo.scalar < 0 ? -1.0 / m_metaInfo.scalar : m_metaInfo.scalar;
   m_metaInfo.Y_interval = std::sqrt(std::pow(trace2.X - trace1.X, 2) +
                                     std::pow(trace2.Y - trace1.Y, 2)) /
-                          m_lineInfo[0].count;
+                          (m_lineInfo[0].count - 1);
   int num = m_metaInfo.trace_count > 10 ? 10 : m_metaInfo.trace_count - 1;
   _get_TraceInfo(m_lineInfo[num].trace_start, trace2);
   m_metaInfo.Z_interval =
       std::sqrt(std::pow(trace2.X - trace1.X, 2) +
                 std::pow(trace2.Y - trace1.Y, 2) -
-                std::pow((trace2.crossline_num - trace1.crossline_num) *
-                             m_metaInfo.Y_interval,
+                std::pow(float(trace2.crossline_num - trace1.crossline_num) /
+                             m_metaInfo.crossline_step * m_metaInfo.Y_interval,
                          2)) /
-      (trace2.inline_num - trace1.inline_num);
-}
-
-static inline int32_t getCrossline(const char *source, int field) {
-  return swap_endian(*(int32_t *)(source + field - 1));
+      ((trace2.inline_num - trace1.inline_num) / float(m_metaInfo.inline_step));
 }
 
 void SegyIO::read(float *dst, int startX, int endX, int startY, int endY,
                   int startZ, int endZ) {
   if (!isReadSegy) {
     throw std::runtime_error(
         "'read()' function used only in reading segy mode");
@@ -408,15 +808,18 @@
   int trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
 
   int sizeX = endX - startX;
   int sizeY = endY - startY;
   int sizeZ = endZ - startZ;
   int offset = startX * sizeof(float) + kTraceHeaderSize;
 
-  progressbar bar(sizeZ);
+  int step = sizeZ >= 100 ? 1 : 100 / sizeZ + 1;
+  int nbar = sizeZ >= 100 ? sizeZ : step * sizeZ;
+  progressbar bar(nbar);
+
   auto time_start = std::chrono::high_resolution_clock::now();
 
   // #pragma omp parallel for
   for (int iZ = startZ; iZ < endZ; iZ++) {
     int istart = startY;
     float *dstline = dst + static_cast<uint64_t>(iZ - startZ) * sizeX * sizeY;
     uint64_t trace_start = m_metaInfo.isNormalSegy
@@ -456,15 +859,15 @@
         }
         istart++;
       } else {
         std::fill(dsttrace, dsttrace + sizeX, m_metaInfo.fillNoValue);
       }
     }
     // #pragma omp critical
-    bar.update();
+    updatebar(bar, step);
   }
   fmt::print("\n");
 
   auto time_end = std::chrono::high_resolution_clock::now();
 
   fmt::print("need time: {}s\n",
              std::chrono::duration_cast<std::chrono::nanoseconds>(time_end -
@@ -510,146 +913,238 @@
 
 void SegyIO::tofile(const std::string &binary_out_name) {
   if (!isScan) {
     scan();
   }
   uint64_t need_size = static_cast<uint64_t>(m_metaInfo.sizeX) *
                        m_metaInfo.sizeY * m_metaInfo.sizeZ * sizeof(float);
-  int fd = open(binary_out_name.c_str(), O_RDWR | O_CREAT | O_TRUNC, 00644);
+  std::ofstream ffst(binary_out_name, std::ios::binary);
+  if (!ffst) {
+    throw std::runtime_error("create file failed");
+  }
   for (int i = 0; i < int(need_size / kMaxLSeekSize) + 1; i++) {
     uint64_t move_point = need_size > kMaxLSeekSize ? kMaxLSeekSize : need_size;
-    if (lseek(fd, move_point - 1, SEEK_END) < 0) {
-      throw std::runtime_error("create file failed");
-    }
-    if (write(fd, "", 1) < 0) {
-      throw std::runtime_error("create file failed");
-    }
-    if (need_size > kMaxLSeekSize) {
-      need_size -= kMaxLSeekSize;
-    }
+    ffst.seekp(move_point - 1, std::ios_base::cur);
+    ffst.put(0);
+    need_size -= move_point;
+  }
+  if (need_size != 0) {
+    throw std::runtime_error("create file failed");
   }
-  close(fd);
+  ffst.close();
 
   std::error_code error;
   mio::mmap_sink rw_mmap = mio::make_mmap_sink(binary_out_name, error);
   if (error) {
     throw std::runtime_error("mmap fail when write data");
   }
   // or need split into serveral chunks?
   read(reinterpret_cast<float *>(rw_mmap.data()));
   rw_mmap.unmap();
 }
 
-std::string SegyIO::metaInfo() {
-  if (!isScan && isReadSegy) {
+void SegyIO::cut(const std::string &outname, int startX, int endX, int startY,
+                 int endY, int startZ, int endZ,
+                 const std::vector<std::string> &custom_info) {
+  if (!isScan) {
     scan();
   }
 
-  float Y_interval = 0;
-  float Z_interval = 0;
+  if (startX >= endX || startY >= endY || startZ >= endZ) {
+    throw std::runtime_error("Index 'end' must large than 'start'");
+  }
+  if (startX < 0 || endX > m_metaInfo.sizeX || startY < 0 ||
+      endY > m_metaInfo.sizeY || startZ < 0 || endZ > m_metaInfo.sizeZ) {
+    throw std::runtime_error("Index out of range");
+  }
 
-  if (m_metaInfo.scalar != 0) {
+  int sizeX, sizeY, sizeZ;
+  sizeX = endX - startX;
+  sizeY = endY - startY;
+  sizeZ = endZ - startZ;
+  int start_time =
+      m_metaInfo.start_time + startX * m_metaInfo.sample_interval / 1000;
+
+  std::fstream out_(outname, std::ios::binary | std::ios::out);
+  if (!out_.is_open()) {
+    throw std::runtime_error("create file failed");
+  }
+
+  // textual header
+  MetaInfo subinfo = m_metaInfo;
+  subinfo.sizeX = sizeX;
+  subinfo.sizeY = sizeY;
+  subinfo.sizeZ = sizeZ;
+  subinfo.start_time = start_time;
+  subinfo.min_inline = m_metaInfo.min_inline + startZ * m_metaInfo.inline_step;
+  subinfo.min_crossline =
+      m_metaInfo.min_crossline + startY * m_metaInfo.crossline_step;
+  subinfo.max_inline =
+      subinfo.min_inline + (sizeZ - 1) * m_metaInfo.inline_step;
+  subinfo.max_crossline =
+      subinfo.min_crossline + (sizeY - 1) * m_metaInfo.crossline_step;
+
+  std::string textual_header =
+      create_textual_header(subinfo, outname, custom_info);
+  out_.write(textual_header.data(), kTextualHeaderSize);
+
+  // binary header
+  std::vector<char> tmp(kBinaryHeaderSize, 0);
+  memcpy(tmp.data(), m_source.data() + kTextualHeaderSize, kBinaryHeaderSize);
+  if (sizeX != m_metaInfo.sizeX) {
+    int16_t *int16ptr = reinterpret_cast<int16_t *>(tmp.data());
+    int16ptr[(kBSampleCountField - 1) / 2] =
+        swap_endian(static_cast<int16_t>(sizeX));
+    int16ptr = nullptr;
+  }
+  out_.write(tmp.data(), kBinaryHeaderSize);
+
+  int step = sizeZ >= 100 ? 1 : 100 / sizeZ + 1;
+  int nbar = sizeZ >= 100 ? sizeZ : step * sizeZ;
+  progressbar bar(nbar);
+
+  int trace_size = kTraceHeaderSize + sizeX * sizeof(float);
+  int trace_size_ori = kTraceHeaderSize + m_metaInfo.sizeX * sizeof(float);
+  tmp.resize(trace_size);
+  tmp.assign(trace_size, 0);
+  int tracecount = 0;
+
+  // iy: sub-voume dat space
+  // iyo: full segy trace space
+  // srct: full-volume dat space
+  for (int iz = 0; iz < sizeZ; iz++) {
+    updatebar(bar, step);
 
-    Y_interval = m_metaInfo.scalar > 0
-                     ? m_metaInfo.Y_interval * m_metaInfo.scalar
-                     : m_metaInfo.Y_interval / -m_metaInfo.scalar;
-    Z_interval = m_metaInfo.scalar > 0
-                     ? m_metaInfo.Z_interval * m_metaInfo.scalar
-                     : m_metaInfo.Z_interval / -m_metaInfo.scalar;
-  }
+    int izo = iz + startZ;
+    const char *srcptr = m_source.data() + kTextualHeaderSize +
+                         kBinaryHeaderSize +
+                         trace_size_ori * m_lineInfo[izo].trace_start;
+    int count_in_line = 0;
+    int xyzspace_start = 0;
+    int xyzspace_end = 0;
+    for (int iyo = 0; iyo < m_lineInfo[izo].count; iyo++) {
+      const char *traceptr = srcptr + iyo * trace_size_ori;
+      int srct = iyo;
+      if (m_lineInfo[izo].count != m_metaInfo.sizeY) {
+        const int32_t *trace_tmp = reinterpret_cast<const int32_t *>(traceptr);
+        srct = swap_endian(trace_tmp[(m_metaInfo.crossline_field - 1) / 4]) -
+               m_metaInfo.min_crossline;
+        srct /= m_metaInfo.crossline_step; // in dat space
+      }
+      if (iyo == 0) {
+        xyzspace_start = srct;
+      }
+      if (iyo == m_lineInfo[izo].count - 1) {
+        xyzspace_end = srct + 1;
+      }
 
-  std::string dformat = m_metaInfo.data_format == 1
-                            ? "4-bytes IBM floating-point"
-                            : "4-bytes IEEE floating-point";
-  return fmt::format("shape: (n-time, n-crossline, n-inline) = ({}, {}, {})\n"
-                     "sample interval: {}, data format code: {}\n"
-                     "inline start: {}, crossline start: {}\n"
-                     "X interval: {:.1f}, Y interval: {:.1f}, time start: {}\n"
-                     "inline field: {}, crossline field: {}\n"
-                     "inline step: {}, crossline step: {}\n"
-                     "Is regular file (no missing traces): {}",
-                     m_metaInfo.sizeX, m_metaInfo.sizeY, m_metaInfo.sizeZ,
-                     m_metaInfo.sample_interval, dformat, m_metaInfo.min_inline,
-                     m_metaInfo.min_crossline, Y_interval, Z_interval,
-                     m_metaInfo.start_time, m_metaInfo.inline_field,
-                     m_metaInfo.crossline_field, m_metaInfo.inline_step,
-                     m_metaInfo.crossline_step, m_metaInfo.isNormalSegy);
+      if (srct >= startY && srct < endY) {
+        tracecount++;
+        count_in_line++;
+        if (sizeX == m_metaInfo.sizeX) {
+          memcpy(tmp.data(), traceptr, trace_size);
+          out_.write(tmp.data(), trace_size);
+        } else {
+          memcpy(tmp.data(), traceptr, kTraceHeaderSize);
+          memcpy(tmp.data() + kTraceHeaderSize,
+                 traceptr + kTraceHeaderSize + startX * sizeof(float),
+                 sizeX * sizeof(float));
+          modify_traceheader(tmp.data(), sizeX, start_time);
+          out_.write(tmp.data(), trace_size);
+        }
+      }
+    } // end iyo
+
+    if (count_in_line == 0) {
+      throw std::runtime_error(
+          fmt::format("Can not cut through the index, becuase the line {} "
+                      "contains 0 trace if use the startY and endY. "
+                      "In line {}, the original crossline range: "
+                      "[{}, {}], in the 3D volume space, y axis is range:"
+                      "[{}, {}), while your cut is range of: [{}, {}).",
+                      izo, izo, m_lineInfo[izo].crossline_start,
+                      m_lineInfo[izo].crossline_end, xyzspace_start,
+                      xyzspace_end, startY, endY));
+    }
+  } // end iz
+  auto pos = out_.tellp();
+  assert(pos ==
+         (kTextualHeaderSize + kBinaryHeaderSize + tracecount * trace_size));
+  out_.close();
+  fmt::print("\n");
 }
 
-std::string SegyIO::textual_header() {
-  if (!isReadSegy && m_sink.size() < kTextualHeaderSize) {
-    throw std::runtime_error(
-        "No textual header, because this is not a segy "
-        "file (read mode) or you don't create textual header (create mode)");
-  }
-  const char *textual_header = nullptr;
-  if (isReadSegy) {
-    textual_header = m_source.data();
-  } else {
-    textual_header = m_sink.data();
+void SegyIO::cut(const std::string &outname, int startY, int endY, int startZ,
+                 int endZ, const std::vector<std::string> &custom_info) {
+  if (!isScan) {
+    scan();
   }
-  char out[kTextualHeaderSize + kTextualRows];
-  bool isEBCDIC = isTextInEBCDICFormat(textual_header, kTextualHeaderSize);
-  for (int iRow = 0; iRow < kTextualRows; iRow++) {
-    int offset = iRow * kTextualColumns;
-    for (int iCol = 0; iCol < kTextualColumns; iCol++) {
-      if (isEBCDIC) {
-        out[iCol + offset + iRow] =
-            getASCIIfromEBCDIC(textual_header[iCol + offset]);
-      } else {
-        out[iCol + offset + iRow] = textual_header[iCol + offset];
-      }
-    }
-    if (iRow < kTextualRows - 1) {
-      out[(iRow + 1) * (kTextualColumns + 1) - 1] = '\n';
-    }
+
+  cut(outname, 0, m_metaInfo.sizeX, startY, endY, startZ, endZ, custom_info);
+}
+
+void SegyIO::cut(const std::string &outname, int startX, int endX,
+                 const std::vector<std::string> &custom_info) {
+  if (!isScan) {
+    scan();
   }
 
-  return std::string(out);
+  cut(outname, startX, endX, 0, m_metaInfo.sizeY, 0, m_metaInfo.sizeZ,
+      custom_info);
 }
 
-void SegyIO::create(const std::string &segy_out_name, const float *src) {
+void SegyIO::create(const std::string &segy_out_name, const float *src,
+                    const std::vector<std::string> &custom_info) {
   if (isReadSegy) {
     throw std::runtime_error(
         "'create() function only can be used for creating segy file.'");
   }
   uint64_t need_size =
       kTextualHeaderSize + kBinaryHeaderSize +
       static_cast<uint64_t>(m_metaInfo.sizeY) * m_metaInfo.sizeZ *
           (m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize);
-  int fd = open(segy_out_name.c_str(), O_RDWR | O_CREAT | O_TRUNC, 00644);
-  // lseek(int, long, ), check whether need size > max number of long
+  std::ofstream ffst(segy_out_name, std::ios::binary);
+  if (!ffst) {
+    throw std::runtime_error("create file failed");
+  }
+  // int fd = open(binary_out_name.c_str(), O_RDWR | O_CREAT | O_TRUNC, 00644);
   for (int i = 0; i < int(need_size / kMaxLSeekSize) + 1; i++) {
     uint64_t move_point = need_size > kMaxLSeekSize ? kMaxLSeekSize : need_size;
-    if (lseek(fd, move_point - 1, SEEK_END) < 0) {
-      throw std::runtime_error("create file failed");
-    }
-    if (write(fd, "", 1) < 0) {
-      throw std::runtime_error("create file failed");
-    }
-    if (need_size > kMaxLSeekSize) {
-      need_size -= kMaxLSeekSize;
-    }
+    // if (lseek(fd, move_point - 1, SEEK_END) < 0) {
+    //   throw std::runtime_error("create file failed");
+    // }
+    // if (write(fd, "", 1) < 0) {
+    //   throw std::runtime_error("create file failed");
+    // }
+    ffst.seekp(move_point - 1, std::ios_base::cur);
+    ffst.put(0);
+    need_size -= move_point;
   }
-  close(fd);
+  if (need_size != 0) {
+    throw std::runtime_error("create file failed");
+  }
+  ffst.close();
 
   std::error_code error;
   mio::mmap_sink rw_mmap = mio::make_mmap_sink(segy_out_name, error);
   if (error) {
     throw std::runtime_error("mmap fail when write data");
   }
 
-  write_textual_header(rw_mmap.data(), segy_out_name);
+  write_textual_header(rw_mmap.data(), segy_out_name, custom_info);
   write_binary_header(rw_mmap.data() + kTextualHeaderSize);
   TraceHeader trace_header{};
   initTraceHeader(&trace_header);
   char *dst = rw_mmap.data() + kTextualHeaderSize + kBinaryHeaderSize;
   char *dstline = dst;
 
-  progressbar bar(m_metaInfo.sizeZ);
+  int step = m_metaInfo.sizeZ >= 100 ? 1 : 100 / m_metaInfo.sizeZ + 1;
+  int nbar =
+      m_metaInfo.sizeZ >= 100 ? m_metaInfo.sizeZ : step * m_metaInfo.sizeZ;
+  progressbar bar(nbar);
 
   int trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
   // #pragma omp parallel for
   for (int iZ = 0; iZ < m_metaInfo.sizeZ; iZ++) {
     for (int iY = 0; iY < m_metaInfo.sizeY; iY++) {
       // write header
       int64_t x = iY * m_metaInfo.Y_interval + 5200;
@@ -669,31 +1164,34 @@
         }
         dstdata[iX] = swap_endian(dstdata[iX]);
       }
 
       dstline += trace_size;
     }
     // #pragma omp critical
-    bar.update();
+    updatebar(bar, step);
   }
   fmt::print("\n");
   rw_mmap.unmap();
 }
 
-void SegyIO::create(const std::string &segy_out_name) {
+void SegyIO::create(const std::string &segy_out_name,
+                    const std::vector<std::string> &custom_info) {
   if (isReadSegy) {
     throw std::runtime_error("Now is read segy mode, cannot create a segy");
   }
   if (!m_source.is_mapped()) {
     throw std::runtime_error("You need to read a binary file before create, or "
                              "you can create from memory");
   }
-  create(segy_out_name, (float *)m_source.data());
+  create(segy_out_name, (float *)m_source.data(), custom_info);
 }
 
+/********************** SegyIO private *******************************/
+
 void SegyIO::initMetaInfo() {
   m_metaInfo.isNormalSegy = true;
   m_metaInfo.crossline_field = kDefaultCrosslineField;
   m_metaInfo.inline_field = kDefaultInlineField;
   m_metaInfo.min_inline = 1;
   m_metaInfo.max_inline = m_metaInfo.min_inline + m_metaInfo.sizeZ - 1;
   m_metaInfo.min_crossline = 1;
@@ -704,108 +1202,82 @@
   m_metaInfo.Z_interval = 25 * 100;
   m_metaInfo.scalar = -100;
   m_metaInfo.start_time = 0;
   m_metaInfo.X_field = kDefaultXField;
   m_metaInfo.Y_field = kDefaultYField;
 }
 
-static inline std::string field_str(int field, int len = 2) {
-  return fmt::format("{}-{}", field, field + len - 1);
+void SegyIO::scanBinaryHeader() {
+  const auto *binary_header = reinterpret_cast<const BinaryHeader *>(
+      m_source.data() + kTextualHeaderSize);
+  m_metaInfo.data_format = swap_endian(binary_header->data_format);
+  m_metaInfo.sizeX = swap_endian(binary_header->trace_length);
+  m_metaInfo.sample_interval = swap_endian(binary_header->sample_interval);
+  m_metaInfo.trace_count =
+      (m_source.size() - kTextualHeaderSize - kBinaryHeaderSize) /
+      (kTraceHeaderSize + m_metaInfo.sizeX * sizeof(float));
 }
 
-void SegyIO::write_textual_header(char *dst, const std::string &segy_out_name) {
-  auto now =
-      std::chrono::system_clock::to_time_t(std::chrono::system_clock::now());
-  std::string time_string(25, ' ');
-  std::strftime(&time_string[0], time_string.size(), "%Y-%m-%d %H:%M:%S",
-                std::localtime(&now));
-  // std::string time_string = fmt::format("{:<30}", time_string0);
-
-  std::string dformat = m_metaInfo.data_format == 1
-                            ? "4-bytes IBM floating-point"
-                            : "4-bytes IEEE floating-point";
-  std::string textual_header = fmt::format(
-      "C01 Create By CIGSEGY software (CIG, USTC, 2022), see:              "
-      "            "
-      "C02 github: https://github.com/JintaoLee-Roger/cigsegy              "
-      "            "
-      "C03                                                                 "
-      "            "
-      "C04 Name: {:<70}"                           // 10 + 70
-      "C05 Type: 3D seismic  Created Time: {:<44}" // 36 + 44
-      "C06                                                                 "
-      "            "
-      "C07 First inline: {:<10}  Last inline: {:<37}" // 36 + 10 + 34
-      "C08 First xline:  {:<10}  Last xline:  {:<37}"
-      "C09                                                                 "
-      "            "
-      "C10 nt, nx, ni = {:>6}, {:>6}, {:<38}         " // 30 + 6 + 6 + 38
-      "C11 Number of samples per data trace: {:<42}"   // 38 + 42
-      "C12 Sample interval: {:<10}   microsecond                           "
-      "        " // 70 + 10
-      "C13 X interval: {:<10} meters, Y interval: {:<10} meters            "
-      "    " // 60 + 10 + 10
-      "C14 Byte endian: BIG_ENDIAN                                         "
-      "            "
-      "C15 Data sample format: {:<56}" // 24 + 56
-      "C16                                                                 "
-      "            "
-      "C17                                                                 "
-      "            "
-      "C18 Binary header locations:                                        "
-      "            "
-      "C19 Sample interval             : bytes {:<40}" // 40 + 40
-      "C20 Number of samples per trace : bytes {:<40}" // 40 + 40
-      "C21 Data sample format code     : bytes {:<40}" // 40 + 40
-      "C22                                                                 "
-      "            "
-      "C23 Trace header locations:                                         "
-      "            "
-      "C24 Inline number               : bytes {:<40}" // 40 + 40
-      "C25 Xline number                : bytes {:<40}"
-      "C26 X coordinate                : bytes {:<40}"
-      "C27 Y coordinate                : bytes {:<40}"
-      "C28 Trace start time/depth      : bytes {:<40}"
-      "C29 Number of samples per trace : bytes {:<40}"
-      "C30 Sample interval             : bytes {:<40}"
-      "C31                                                                 "
-      "            "
-      "C32                                                                 "
-      "            "
-      "C33                                                                 "
-      "            "
-      "C34                                                                 "
-      "            "
-      "C35                                                                 "
-      "            "
-      "C36                                                                 "
-      "            "
-      "C37                                                                 "
-      "            "
-      "C38                                                                 "
-      "            "
-      "C39                                                                 "
-      "            "
-      "C40 END EBCDIC                                                      "
-      "            ",
-      segy_out_name, time_string.substr(0, 19), m_metaInfo.min_inline,
-      m_metaInfo.max_inline, m_metaInfo.min_crossline, m_metaInfo.max_crossline,
-      m_metaInfo.sizeX, m_metaInfo.sizeY, m_metaInfo.sizeZ, m_metaInfo.sizeX,
-      m_metaInfo.sample_interval, m_metaInfo.Z_interval / 100,
-      m_metaInfo.Y_interval / 100, dformat, field_str(kBSampleIntervalField),
-      field_str(kBSampleCountField), field_str(kBSampleFormatField),
-      field_str(m_metaInfo.inline_field, 4),
-      field_str(m_metaInfo.crossline_field, 4),
-      field_str(m_metaInfo.X_field, 4), field_str(m_metaInfo.Y_field, 4),
-      field_str(kTStartTimeField), field_str(kTSampleCountField),
-      field_str(kTSampleIntervalField));
-
-  for (auto &s : textual_header) {
-    s = getEBCIDfromASCII(s);
+void SegyIO::check_order() {
+  int i1, x1, i2, x2, i3, x3;
+  TraceInfo trace{};
+  _get_TraceInfo(0, trace);
+  i1 = trace.inline_num;
+  x1 = trace.crossline_num;
+  _get_TraceInfo(1, trace);
+  i2 = trace.inline_num;
+  x2 = trace.crossline_num;
+  _get_TraceInfo(2, trace);
+  i3 = trace.inline_num;
+  x3 = trace.crossline_num;
+
+  if (x1 == x2 && x1 == x3) {
+    if (i1 != i2 && i1 != i3 && i2 != i3) {
+      is_crossline_fast = false;
+      int t = m_metaInfo.inline_field;
+      int t2 = m_metaInfo.inline_step;
+      m_metaInfo.inline_field = m_metaInfo.crossline_field;
+      m_metaInfo.crossline_field = t;
+      m_metaInfo.inline_step = m_metaInfo.crossline_step;
+      m_metaInfo.crossline_step = t2;
+
+      fmt::print(
+          "[Warining] The fast order of you segy file "
+          "is inline order (default is crossline order). This means "
+          "the file you obtain (numpy array or a binary file in disk) "
+          "is shape as (n-time, n-inline, n-crossline) (in python numpy array"
+          ", the shape is (n-crossline, n-inline, n-time)). "
+          "You need to transpose it manully, such as "
+          "`d = d.transpose(1, 0, 2)`\n\n");
+    } else {
+      throw std::runtime_error(fmt::format(
+          "Cannot check the fast order (default is crossline). "
+          "We check the first three traces, now the crossline numbers "
+          "are constant, the inline numbers must be different if "
+          "the file is valid (fast order is inline). "
+          "But the inline number is {}, {}, {}. May be the locations "
+          "is wrong.\n\n",
+          i1, i2, i3));
+    }
+  } else if (i1 != i2 || i1 != i3 || i2 != i3) {
+    throw std::runtime_error(fmt::format(
+        "Cannot check the fast order (default is crossline). "
+        "We check the first three traces, and can not evaluate "
+        "the fast order, becuase the inline and crossline numbers are "
+        "both different. The inline numbers: {}, {}, {}"
+        "The crossline numbers: {}, {}, {}. Maybe the locations is "
+        "wrong, or the file is small\n\n",
+        i1, i2, i3, x1, x2, x3));
   }
+}
+
+void SegyIO::write_textual_header(char *dst, const std::string &segy_out_name,
+                                  const std::vector<std::string> &custom_info) {
+  std::string textual_header =
+      create_textual_header(m_metaInfo, segy_out_name, custom_info);
 
   memcpy(dst, textual_header.c_str(), kTextualHeaderSize);
 }
 
 void SegyIO::write_binary_header(char *dst) {
   memset(dst, 0, kBinaryHeaderSize);
   BinaryHeader binary_header{};
@@ -830,15 +1302,16 @@
   trace_header->trace_num_in_orig = swap_endian(int32_t(1));
   trace_header->trace_num_in_ensemble = swap_endian(int32_t(1));
   trace_header->trace_ID_code = swap_endian(int16_t(1));
   trace_header->data_used_for = swap_endian(int16_t(1));
   trace_header->scalar_for_elev_and_depth = swap_endian(int16_t(1));
   trace_header->scalar_for_coord = swap_endian(m_metaInfo.scalar);
   trace_header->coord_units = swap_endian(int16_t(1));
-  trace_header->mute_time_start = swap_endian(m_metaInfo.start_time);
+  trace_header->lag_time_A = swap_endian(m_metaInfo.start_time);
+  trace_header->delay_record_time = swap_endian(m_metaInfo.start_time);
   trace_header->num_sample = swap_endian(int16_t(m_metaInfo.sizeX));
   trace_header->sample_interval = swap_endian(m_metaInfo.sample_interval);
   trace_header->correlated = swap_endian(int16_t(1));
   trace_header->sweep_type_code = swap_endian(int16_t(1));
   trace_header->taper_type = swap_endian(int16_t(1));
 }
 
@@ -859,35 +1332,15 @@
 
 void SegyIO::close_file() {
   if (m_source.is_mapped()) {
     m_source.unmap();
   }
 }
 
-void SegyIO::collect(float *data, int *header) {
-  const char *source = m_source.data() + kTextualHeaderSize + kBinaryHeaderSize;
-  int32_t trace_size = m_metaInfo.sizeX * sizeof(float) + kTraceHeaderSize;
-  progressbar bar(100);
-  for (int i = 0; i < m_metaInfo.trace_count; i++) {
-    if (i % (m_metaInfo.trace_count / 100) == 0) {
-      bar.update();
-    }
-    _get_TraceInfo(i, *reinterpret_cast<TraceInfo *>(header));
-    memcpy(data, source + kTraceHeaderSize, m_metaInfo.sizeX * sizeof(float));
-    for (int j = 0; j < m_metaInfo.sizeX; j++) {
-      if (m_metaInfo.data_format == 1) {
-        data[j] = ibm_to_ieee(data[j], true);
-      } else {
-        data[j] = swap_endian(data[j]);
-      }
-    }
-    data += m_metaInfo.sizeX;
-    header += 4;
-  }
-}
+/************** Usefual function, need to be binded ******************/
 
 void read(const std::string &segy_name, float *dst, int iline, int xline,
           int istep, int xstep) {
   SegyIO segy_data(segy_name);
   segy_data.setInlineLocation(iline);
   segy_data.setCrosslineLocation(xline);
   segy_data.setSteps(istep, xstep);
@@ -925,128 +1378,154 @@
   segy_data.tofile(out_name);
   segy_data.close_file();
 }
 
 void create_by_sharing_header(const std::string &segy_name,
                               const std::string &header_segy, const float *src,
                               int sizeX, int sizeY, int sizeZ, int iline,
-                              int xline, int istep, int xstep) {
+                              int xline, int istep, int xstep, int offsetX,
+                              int offsetY, int offsetZ,
+                              const std::vector<std::string> &custom_info) {
   SegyIO header(header_segy);
   header.setInlineLocation(iline);
   header.setCrosslineLocation(xline);
   header.setSteps(istep, xstep);
   header.scan();
   auto line_info = header.line_info();
   auto meta_info = header.get_metaInfo();
   auto trace_count = header.trace_count();
   header.close_file();
 
-  if (meta_info.sizeY != sizeY || meta_info.sizeZ != sizeZ ||
-      meta_info.sizeX != sizeX) {
-    throw std::runtime_error(fmt::format(
-        "shape of header: {} x {} x {}, but shape of source: {} x {} x {}",
-        meta_info.sizeZ, meta_info.sizeY, meta_info.sizeX, sizeZ, sizeY,
-        sizeX));
-  }
-
-  uint64_t need_size = kTextualHeaderSize + kBinaryHeaderSize +
-                       trace_count * (sizeX * sizeof(float) + kTraceHeaderSize);
-  int fd = open(segy_name.c_str(), O_RDWR | O_CREAT | O_TRUNC, 00644);
-  // lseek(int, long, ), check whether need size > max number of long
-  for (int i = 0; i < int(need_size / kMaxLSeekSize) + 1; i++) {
-    uint64_t move_point = need_size > kMaxLSeekSize ? kMaxLSeekSize : need_size;
-    if (lseek(fd, move_point - 1, SEEK_END) < 0) {
-      throw std::runtime_error("create file failed");
-    }
-    if (write(fd, "", 1) < 0) {
-      throw std::runtime_error("create file failed");
-    }
-    if (need_size > kMaxLSeekSize) {
-      need_size -= kMaxLSeekSize;
-    }
-  }
-  close(fd);
-
   std::error_code error;
-  mio::mmap_sink rw_mmap = mio::make_mmap_sink(segy_name, error);
-  if (error) {
-    throw std::runtime_error("mmap fail when write data");
-  }
-
   mio::mmap_source m_source;
   m_source.map(header_segy, error);
   if (error) {
     throw std::runtime_error("Cannot mmap segy file");
   }
 
-  // copy textual header and binary header
-  std::copy(m_source.begin(),
-            m_source.begin() + kTextualHeaderSize + kBinaryHeaderSize,
-            rw_mmap.begin());
-
-  // trace header and data
-  progressbar bar(sizeZ);
-  int64_t trace_size = sizeX + kTraceHeaderSize / 4;
-  for (int iz = 0; iz < sizeZ; iz++) {
-    bar.update();
-    int64_t trace_loc = kTextualHeaderSize + kBinaryHeaderSize +
-                        trace_size * 4 * line_info[iz].trace_start;
-
-    const float *srcopy = src + iz * sizeY * sizeX;
-
-    const float *m_src =
-        reinterpret_cast<const float *>(m_source.data() + trace_loc);
-    float *m_dst = reinterpret_cast<float *>(rw_mmap.data() + trace_loc);
-
-    for (int iy = 0; iy < line_info[iz].count; iy++) {
-      int srct = iy;
-      if (line_info[iz].count != sizeY) {
-        const int *tmp = reinterpret_cast<const int *>(m_src);
-        srct = swap_endian(
-                   tmp[iy * trace_size + (meta_info.crossline_field - 1) / 4]) -
-               meta_info.min_crossline;
-      }
+  if (offsetX < 0 || offsetY < 0 || offsetZ < 0) {
+    // full copy
+    if (meta_info.sizeY != sizeY || meta_info.sizeZ != sizeZ ||
+        meta_info.sizeX != sizeX) {
+      throw std::runtime_error(fmt::format(
+          "shape of header: {} x {} x {}, but shape of source: {} x {} x {}",
+          meta_info.sizeZ, meta_info.sizeY, meta_info.sizeX, sizeZ, sizeY,
+          sizeX));
+    }
 
-      // copy trace header
-      std::copy(m_src + iy * trace_size,
-                m_src + iy * trace_size + kTraceHeaderSize / 4,
-                m_dst + iy * trace_size);
+    uint64_t need_size =
+        kTextualHeaderSize + kBinaryHeaderSize +
+        trace_count * (sizeX * sizeof(float) + kTraceHeaderSize);
+    std::ofstream ffst(segy_name, std::ios::binary);
+    if (!ffst) {
+      throw std::runtime_error("create file failed");
+    }
+    for (int i = 0; i < int(need_size / kMaxLSeekSize) + 1; i++) {
+      uint64_t move_point =
+          need_size > kMaxLSeekSize ? kMaxLSeekSize : need_size;
+      ffst.seekp(move_point - 1, std::ios_base::cur);
+      ffst.put(0);
+      need_size -= move_point;
+    }
+    if (need_size != 0) {
+      throw std::runtime_error("create file failed");
+    }
+    ffst.close();
 
-      // copy data
-      float *t_dst = m_dst + iy * trace_size + kTraceHeaderSize / 4;
-      std::copy(srcopy + srct * sizeX, srcopy + srct * sizeX + sizeX, t_dst);
-      // convert each value to big endian and its format
-      for (int ix = 0; ix < sizeX; ix++) {
-        if (meta_info.data_format == 1) {
-          t_dst[ix] = ieee_to_ibm(t_dst[ix], true);
-        }
-        t_dst[ix] = swap_endian(t_dst[ix]);
-      }
+    mio::mmap_sink rw_mmap = mio::make_mmap_sink(segy_name, error);
+    if (error) {
+      throw std::runtime_error("mmap fail when write data");
+    }
+
+    char *outptr = rw_mmap.data();
+    memcpy(outptr, m_source.data(), kTextualHeaderSize + kBinaryHeaderSize);
+    outptr += (kTextualHeaderSize + kBinaryHeaderSize);
+
+    copy_traces(m_source, line_info, meta_info, src, outptr, sizeX, sizeY,
+                sizeZ, 0, 0, 0, -1);
+
+    rw_mmap.unmap();
+
+  } else if (offsetX >= 0 && offsetY >= 0 && offsetZ >= 0) {
+    // subset data
+    if (sizeX + offsetX > meta_info.sizeX ||
+        sizeY + offsetY > meta_info.sizeY ||
+        sizeZ + offsetZ > meta_info.sizeZ) {
+      throw std::runtime_error("size_{src} + offset > size_{header}");
+    }
+
+    int max_size = kTextualHeaderSize + kBinaryHeaderSize +
+                   (kTraceHeaderSize + sizeX * sizeof(float)) * (sizeY * sizeZ);
+    std::vector<char> outsegy(max_size, 0);
+    char *outptr = outsegy.data();
+    int start_time =
+        meta_info.start_time + offsetX * meta_info.sample_interval / 1000;
+    MetaInfo msub = meta_info;
+    msub.sizeX = sizeX;
+    msub.sizeY = sizeY;
+    msub.sizeZ = sizeZ;
+    msub.start_time = start_time;
+    msub.min_inline = meta_info.min_inline + offsetZ * meta_info.inline_step;
+    msub.min_crossline =
+        meta_info.min_crossline + offsetY * meta_info.crossline_step;
+    msub.max_inline = msub.min_inline + (sizeZ - 1) * meta_info.inline_step;
+    msub.max_crossline =
+        msub.min_crossline + (sizeY - 1) * meta_info.crossline_step;
+
+    std::string textual_header =
+        create_textual_header(msub, segy_name, custom_info);
+    memcpy(outptr, textual_header.c_str(), kTextualHeaderSize);
+    outptr += kTextualHeaderSize;
+
+    // copy binary header & modify sample count
+    memcpy(outptr, m_source.data() + kTextualHeaderSize, kBinaryHeaderSize);
+    int16_t *int16ptr = reinterpret_cast<int16_t *>(outptr);
+    int16ptr[(kBSampleCountField - 1) / 2] =
+        swap_endian(static_cast<int16_t>(sizeX));
+    int16ptr = nullptr;
+    outptr += kBinaryHeaderSize;
+
+    int64_t size =
+        copy_traces(m_source, line_info, meta_info, src, outptr, sizeX, sizeY,
+                    sizeZ, offsetX, offsetY, offsetZ, start_time);
+
+    outsegy.resize(kTextualHeaderSize + kBinaryHeaderSize + size);
+
+    std::ofstream file(segy_name, std::ios::binary | std::ios::out);
+    if (file.is_open()) {
+      file.write(outsegy.data(), outsegy.size());
+      file.close();
+    } else {
+      throw std::runtime_error("create file failed");
     }
+  } else {
+    throw std::runtime_error(
+        fmt::format("offset (X, Y, Z) must be both positive or negetive, "
+                    "but now is: {}, {}, {}",
+                    offsetX, offsetY, offsetZ));
   }
-  fmt::print("\n");
-
   m_source.unmap();
-  rw_mmap.unmap();
 }
 
 // if src is very huge, memmap it
 void create_by_sharing_header(const std::string &segy_name,
                               const std::string &header_segy,
                               const std::string &src_file, int sizeX, int sizeY,
                               int sizeZ, int iline, int xline, int istep,
-                              int xstep) {
+                              int xstep, int offsetX, int offsetY, int offsetZ,
+                              const std::vector<std::string> &custom_info) {
   mio::mmap_source m_src;
   std::error_code error;
   m_src.map(src_file, error);
   if (error) {
     throw std::runtime_error("Cannot mmap segy file");
   }
 
   const float *src = reinterpret_cast<const float *>(m_src.data());
   create_by_sharing_header(segy_name, header_segy, src, sizeX, sizeY, sizeZ,
-                           iline, xline, istep, xstep);
+                           iline, xline, istep, xstep, offsetX, offsetY,
+                           offsetZ, custom_info);
 
   m_src.unmap();
 }
 
 } // namespace segy
```

