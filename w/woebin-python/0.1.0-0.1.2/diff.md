# Comparing `tmp/woebin-python-0.1.0.tar.gz` & `tmp/woebin-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woebin-python-0.1.0.tar", last modified: Mon Jul  3 09:15:16 2023, max compression
+gzip compressed data, was "woebin-python-0.1.2.tar", last modified: Fri Jul  7 05:31:29 2023, max compression
```

## Comparing `woebin-python-0.1.0.tar` & `woebin-python-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:15:16.462588 woebin-python-0.1.0/
--rw-rw-rw-   0        0        0      188 2023-07-03 09:15:16.462588 woebin-python-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-07-03 08:34:39.000000 woebin-python-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 09:15:16.463588 woebin-python-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-07-03 09:13:50.000000 woebin-python-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:15:16.445441 woebin-python-0.1.0/target/
-drwxrwxrwx   0        0        0        0 2023-07-03 09:15:16.454579 woebin-python-0.1.0/target/release/
--rw-rw-rw-   0        0        0   224768 2023-07-03 08:38:42.000000 woebin-python-0.1.0/target/release/woebin.dll
-drwxrwxrwx   0        0        0        0 2023-07-03 09:15:16.456586 woebin-python-0.1.0/woebin/
--rw-rw-rw-   0        0        0     3321 2023-07-03 09:04:59.000000 woebin-python-0.1.0/woebin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:15:16.461589 woebin-python-0.1.0/woebin_python.egg-info/
--rw-rw-rw-   0        0        0      188 2023-07-03 09:15:16.000000 woebin-python-0.1.0/woebin_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-07-03 09:15:16.000000 woebin-python-0.1.0/woebin_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:15:16.000000 woebin-python-0.1.0/woebin_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 09:15:16.000000 woebin-python-0.1.0/woebin_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 05:31:29.524427 woebin-python-0.1.2/
+-rw-rw-rw-   0        0        0     1498 2023-07-07 05:31:29.523426 woebin-python-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1271 2023-07-04 18:46:47.000000 woebin-python-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 05:31:29.524427 woebin-python-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-07-07 05:31:01.000000 woebin-python-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:31:29.499159 woebin-python-0.1.2/target/
+drwxrwxrwx   0        0        0        0 2023-07-07 05:31:29.504156 woebin-python-0.1.2/target/release/
+-rw-rw-rw-   0        0        0   224768 2023-07-03 10:57:03.000000 woebin-python-0.1.2/target/release/woebin.dll
+drwxrwxrwx   0        0        0        0 2023-07-07 05:31:29.506156 woebin-python-0.1.2/woebin/
+-rw-rw-rw-   0        0        0     3690 2023-07-07 05:27:38.000000 woebin-python-0.1.2/woebin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:31:29.522418 woebin-python-0.1.2/woebin_python.egg-info/
+-rw-rw-rw-   0        0        0     1498 2023-07-07 05:31:29.000000 woebin-python-0.1.2/woebin_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-07-07 05:31:29.000000 woebin-python-0.1.2/woebin_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 05:31:29.000000 woebin-python-0.1.2/woebin_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 05:31:29.000000 woebin-python-0.1.2/woebin_python.egg-info/top_level.txt
```

### Comparing `woebin-python-0.1.0/target/release/woebin.dll` & `woebin-python-0.1.2/target/release/woebin.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180029e6c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Jul  3 08:38:42 2023
+Time/Date		Mon Jul  3 10:57:03 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	31
 SizeOfCode		000000000002ac00
 SizeOfInitializedData	000000000000c000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000029e6c
@@ -5604,15 +5604,15 @@
 	reloc    4 offset   a8 [360a8] DIR64
 	reloc    5 offset    0 [36000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1800321b0
 
 Type                Size     Rva      Offset
   2        CodeView 00000060 00032374 00031374
-(format RSDS signature 7ec4999bd7f141e1b2a36b01c1c003aa age 2 pdb C:\Users\alexander-o3\Development\woebin\target\release\deps\woebin.pdb)
+(format RSDS signature cdc6a3f8db8343a1b2e6da5dcfb407e4 age 1 pdb C:\Users\alexander-o3\Development\woebin\target\release\deps\woebin.pdb)
  12         Feature 00000014 000323d4 000313d4
  13         CoffGrp 00000318 000323e8 000313e8
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
   0 .text         0002aae7  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
@@ -63055,41 +63055,37 @@
    1800321a1:	ret    $0x8002
    1800321a4:	add    %eax,(%rax)
    1800321a6:	add    %al,(%rax)
    1800321a8:	push   $0x18002c2
    1800321ad:	add    %al,(%rax)
    1800321af:	add    %al,(%rax)
    1800321b1:	add    %al,(%rax)
-   1800321b3:	add    %dl,(%rdx)
-   1800321b5:	mov    %esp,0x64(%rdx)
-   1800321bb:	add    %al,(%rdx)
-   1800321bd:	add    %al,(%rax)
+   1800321b3:	add    %bh,-0x57(%rdi)
+   1800321b6:	movabs %al,0x20000000064
    1800321bf:	add    %ah,0x0(%rax)
    1800321c2:	add    %al,(%rax)
    1800321c4:	je     0x1800321e9
    1800321c6:	add    (%rax),%eax
    1800321c8:	je     0x1800321dd
    1800321ca:	add    (%rax),%eax
    1800321cc:	add    %al,(%rax)
    1800321ce:	add    %al,(%rax)
-   1800321d0:	adc    0x64a2(%rcx),%cl
-   1800321d6:	add    %al,(%rax)
-   1800321d8:	or     $0x0,%al
-   1800321da:	add    %al,(%rax)
-   1800321dc:	adc    $0x0,%al
+   1800321d0:	jg     0x18003217b
+   1800321d2:	movabs %al,0xc0000000064
+   1800321db:	add    %dl,(%rax,%rax,1)
    1800321de:	add    %al,(%rax)
    1800321e0:	(bad)
    1800321e1:	and    (%rbx),%eax
    1800321e3:	add    %dl,%ah
    1800321e5:	adc    (%rbx),%eax
    1800321e7:	add    %al,(%rax)
    1800321e9:	add    %al,(%rax)
-   1800321eb:	add    %dl,(%rdx)
-   1800321ed:	mov    %esp,0x64(%rdx)
-   1800321f3:	add    %cl,0x18000000(%rip)        # 0x1980321f9
+   1800321eb:	add    %bh,-0x57(%rdi)
+   1800321ee:	movabs %al,0xd0000000064
+   1800321f7:	add    %bl,(%rax)
    1800321f9:	add    (%rax),%eax
    1800321fb:	add    %ch,%al
    1800321fd:	and    (%rbx),%eax
    1800321ff:	add    %ch,%al
    180032201:	adc    (%rbx),%eax
 	...
    18003227f:	add    %ah,(%rax)
@@ -63174,27 +63170,25 @@
    18003236a:	add    %al,(%rax)
    18003236c:	push   %rbp
    18003236d:	mov    $0x920002,%edx
    180032372:	add    %al,(%rax)
    180032374:	push   %rdx
    180032375:	push   %rbx
    180032376:	rex.R push %rbx
-   180032378:	fwait
-   180032379:	cltd
-   18003237a:	(bad)
-   18003237b:	jle    0x18003236e
-   18003237d:	xlat   %ds:(%rbx)
-   18003237e:	loope  0x1800323c1
-   180032380:	mov    $0xa3,%dl
-   180032382:	imul   $0xffffffc1,(%rcx),%eax
-   180032385:	rolb   $0xaa,(%rbx)
-   180032388:	add    (%rax),%al
-   18003238a:	add    %al,(%rax)
-   18003238c:	cmp    0x73(%r13,%r10,2),%bl
-   180032391:	gs jb  0x180032407
+   180032378:	clc
+   180032379:	movabs %eax,0xe6b243a1db83cdc6
+   180032382:	ficompl -0x31(%rbp)
+   180032385:	mov    $0x7,%ah
+   180032387:	in     $0x1,%al
+   180032389:	add    %al,(%rax)
+   18003238b:	add    %al,0x3a(%rbx)
+   18003238e:	pop    %rsp
+   18003238f:	push   %rbp
+   180032390:	jae    0x1800323f7
+   180032392:	jb     0x180032407
    180032394:	pop    %rsp
    180032395:	(bad)
    180032396:	insb   (%dx),%es:(%rdi)
    180032397:	gs js  0x1800323fb
    18003239a:	outsb  %ds:(%rsi),(%dx)
    18003239b:	fs gs jb 0x1800323cc
    18003239f:	outsl  %ds:(%rsi),(%dx)
```

### Comparing `woebin-python-0.1.0/woebin/__init__.py` & `woebin-python-0.1.2/woebin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     def is_done(self):
         return dll.wbp_is_done(self.wbp)
 
     def process_categorial(self, series, target):
         assert len(series) == len(target)
         size = len(series)
 
+        series = map(hash, series)
+        target = map(bool, target)
+
         dll.wbp_process_categorial.argtypes = [
             ctypes.c_void_p, ctypes.c_uint64, 
             (ctypes.c_uint64 * size), (ctypes.c_bool * size)
         ]
         dll.wbp_process_categorial(
             ctypes.c_void_p(self.wbp),
             size,
@@ -44,14 +47,17 @@
             (ctypes.c_bool * size)(*target),
         )
 
     def process_numeric(self, series, target):
         assert len(series) == len(target)
         size = len(series)
 
+        series = map(strict_float_to_int, series)
+        target = map(bool, target)
+
         dll.wbp_process_numeric.argtypes = [
             ctypes.c_void_p, ctypes.c_uint64, 
             (ctypes.c_uint64 * size), (ctypes.c_bool * size)
         ]
         dll.wbp_process_numeric(
             ctypes.c_void_p(self.wbp),
             size,
@@ -102,14 +108,24 @@
     def get_iv_total(self):
         iv_total = 0.0
         for info in self.get_bins_info():
             iv_total += info['iv']
         return iv_total
 
 
+def strict_float_to_int(x):
+    if isinstance(x, float):
+        if float(x).is_integer():
+            return int(x)
+        else:
+            raise TypeError(x)
+    else:
+        return int(x)
+
+
 class BinInfo(ctypes.Structure):
     _fields_ = [
         ('woe', ctypes.c_double),
         ('iv', ctypes.c_double),
         ('size', ctypes.c_uint64),
     ]
```

