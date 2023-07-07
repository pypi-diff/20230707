# Comparing `tmp/kau3-tian2_iong7-ji7-2.2.0.tar.gz` & `tmp/kau3-tian2_iong7-ji7-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kau3-tian2_iong7-ji7-2.2.0.tar", last modified: Fri Jul 23 06:56:03 2021, max compression
+gzip compressed data, was "dist/kau3-tian2_iong7-ji7-3.0.5.tar", last modified: Fri Jul  7 08:10:52 2023, max compression
```

## Comparing `kau3-tian2_iong7-ji7-2.2.0.tar` & `kau3-tian2_iong7-ji7-3.0.5.tar`

### file list

```diff
@@ -1,21 +1,32 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-23 06:56:03.000000 kau3-tian2_iong7-ji7-2.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2021-07-23 06:56:03.000000 kau3-tian2_iong7-ji7-2.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3270 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1313 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/版本.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-23 06:56:03.000000 kau3-tian2_iong7-ji7-2.2.0/用字/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1230 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      551 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/apps.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-23 06:56:03.000000 kau3-tian2_iong7-ji7-2.2.0/用字/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      614 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/migrations/0002_用字管理表.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      395 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/migrations/0003_alter_用字表_分詞.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2023 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/公家變數.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   134316 2021-07-23 06:55:01.000000 kau3-tian2_iong7-ji7-2.2.0/用字/教典.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   274298 2021-07-23 06:55:03.000000 kau3-tian2_iong7-ji7-2.2.0/用字/教典名姓.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1202 2021-07-23 06:54:15.000000 kau3-tian2_iong7-ji7-2.2.0/用字/標點規範.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   238207 2021-07-23 06:55:05.000000 kau3-tian2_iong7-ji7-2.2.0/用字/甘字典.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       94 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3622 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/kau3_tian2_iong7_ji7.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-07-07 08:10:52.000000 kau3-tian2_iong7-ji7-3.0.5/kau3_tian2_iong7_ji7.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      692 2023-07-07 08:10:52.000000 kau3-tian2_iong7-ji7-3.0.5/kau3_tian2_iong7_ji7.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-07 08:10:52.000000 kau3-tian2_iong7-ji7-3.0.5/kau3_tian2_iong7_ji7.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-07-07 08:10:52.000000 kau3-tian2_iong7-ji7-3.0.5/kau3_tian2_iong7_ji7.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-07-07 08:10:52.000000 kau3-tian2_iong7-ji7-3.0.5/kau3_tian2_iong7_ji7.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/版本.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/用字/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      878 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      529 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/admin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/apps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/用字/management/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/用字/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/management/commands/用字表重正規化.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-07 08:10:52.624242 kau3-tian2_iong7-ji7-3.0.5/用字/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      614 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/migrations/0002_用字管理表.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      395 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/migrations/0003_alter_用字表_分詞.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      520 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/migrations/0004_remove_用字表_分詞_用字表_tuitsiau.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/公家變數.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   607590 2023-07-07 08:10:35.000000 kau3-tian2_iong7-ji7-3.0.5/用字/教典.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/書寫.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      792 2023-07-07 08:09:40.000000 kau3-tian2_iong7-ji7-3.0.5/用字/標點規範.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kau3-tian2_iong7-ji7-2.2.0/LICENSE` & `kau3-tian2_iong7-ji7-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kau3-tian2_iong7-ji7-2.2.0/setup.py` & `kau3-tian2_iong7-ji7-3.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     工具包 = []
     for 目錄, _, 檔案 in walk(頭):
         if '__init__.py' in 檔案:
             工具包.append(目錄.replace('/', '.'))
     return 工具包
 
 
-github網址 = 'https://github.com/i3thuan5/kau3-tian2_iong7-ji7'
+github網址 = 'https://github.com/i3thuan5/KauTian-IongJi/'
 
 
 setup(
     name='kau3-tian2_iong7-ji7',
     packages=揣工具包('用字'),
     version=版本,
     description='教典用字',
@@ -26,25 +26,25 @@
     url='https://ithuan.tw',
     download_url=github網址,
     keywords=[
         '語料庫',
         'Taiwan', 'Natural Language', 'Corpus',
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Operating System :: Unix',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Framework :: Django :: 4.2',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: Linguistic',
     ],
     install_requires=[
-        'tai5-uan5_gian5-gi2_kang1-ku7>=1.0.0',
+        'KeSi',
     ],
     package_data={
         '用字': [
             '教典.json',
-            '教典名姓.json',
-            '甘字典.json',
         ],
     }
 )
```

### Comparing `kau3-tian2_iong7-ji7-2.2.0/用字/admin.py` & `kau3-tian2_iong7-ji7-3.0.5/用字/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,14 @@
         proxy = True
         verbose_name = "用字表"
         verbose_name_plural = verbose_name
 
 
 class 用字表後台(admin.ModelAdmin):
     # change list
-    list_display = ['id', '漢字', '羅馬字', '分詞', ]
-    search_fields = ['id', '漢字', '羅馬字', '分詞', ]
+    list_display = ['id', '漢字', '羅馬字',]
+    search_fields = ['id', '漢字', '羅馬字',]
     # change view
     fields = ('漢字', '羅馬字',)
 
 
 admin.site.register(用字管理表, 用字表後台)
```

### Comparing `kau3-tian2_iong7-ji7-2.2.0/用字/migrations/0001_initial.py` & `kau3-tian2_iong7-ji7-3.0.5/用字/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kau3-tian2_iong7-ji7-2.2.0/用字/migrations/0002_用字管理表.py` & `kau3-tian2_iong7-ji7-3.0.5/用字/migrations/0002_用字管理表.py`

 * *Files identical despite different names*

### Comparing `kau3-tian2_iong7-ji7-2.2.0/用字/models.py` & `kau3-tian2_iong7-ji7-3.0.5/用字/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-from 臺灣言語工具.解析整理.解析錯誤 import 解析錯誤
-from 臺灣言語工具.音標系統.閩南語.臺灣閩南語羅馬字拼音 import 臺灣閩南語羅馬字拼音
+from kesi import Ku
+from 用字.書寫 import tsingkuihua
 from django.db import models
 from django.core.exceptions import ValidationError
-from 臺灣言語工具.解析整理.拆文分析器 import 拆文分析器
 from 用字 import 字典
 from 用字 import 建議
 
 
 class 用字表(models.Model):
     漢字 = models.CharField(max_length=5)
     羅馬字 = models.CharField(max_length=15)
-    分詞 = models.CharField(max_length=20, blank=True)
-    _用字ê範圍 = 建議.全部分詞()
+    _用字ê範圍 = 建議.全部對照()
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(fields=['漢字', '羅馬字'], name='tuitsiau'),
+        ]
 
     @classmethod
     def 有這个字無(cls, 字物件):
-        字臺羅物件 = 字物件.轉音(臺灣閩南語羅馬字拼音)
-        字臺羅物件.型 = 字臺羅物件.型.lstrip('-')
-        字臺羅物件.音 = 字臺羅物件.音.lstrip('0').lstrip('-')
-        字臺羅物件.輕聲標記 = False
-        字分詞 = 字臺羅物件.看分詞()
-        if 字分詞 in cls._用字ê範圍:
+        return cls.有這對應無(字物件.型, 字物件.音)
+
+    @classmethod
+    def 有這對應無(cls, han, lo):
+        han, lo = tsingkuihua(han, lo)
+        if (han, lo) in cls._用字ê範圍:
             return True
-        return cls.objects.filter(分詞=字分詞).exists()
+        return cls.objects.filter(漢字=han, 羅馬字=lo).exists()
 
     def clean(self):
-        # 提掉舊的輕聲規範
-        羅馬字 = self.羅馬字.lstrip('0').lstrip('-')
-        漢字 = self.漢字.lstrip('-')
-        try:
-            詞物件 = 拆文分析器.對齊詞物件(漢字, 羅馬字)
-        except 解析錯誤:
-            raise ValidationError('漢羅ài攏是一ê字')
-        if len(詞物件.篩出字物件()) > 1:
-            raise ValidationError('漢羅ài攏是一ê字')
-        字臺羅物件 = (
-            詞物件.篩出字物件()[0]
-            .轉音(臺灣閩南語羅馬字拼音)
-        )
-        字臺羅物件.輕聲標記 = False
-        self.分詞 = 字臺羅物件.看分詞()
+        hantng = len(list(Ku(self.漢字).thianji()))
+        lotng = len(list(Ku(self.羅馬字).thianji()))
+        if hantng != 1 or lotng != 1:
+            raise ValidationError('漢羅攏ài拄好一ê字，漢字有{}字，羅馬字有{}字'.format(
+                hantng, lotng
+            ))
+        self.漢字, self.羅馬字 = tsingkuihua(self.漢字, self.羅馬字)
         super().clean()
 
     @classmethod
     def 這馬(cls):
-        return 字典(cls.全部分詞())
+        return 字典(cls.全部對照())
 
     @classmethod
-    def 全部分詞(cls):
-        return cls._用字ê範圍 | set(cls.objects.values_list('分詞', flat=True))
+    def 全部對照(cls):
+        tsuanpoo = set(cls._用字ê範圍)
+        for ji in cls.objects.values_list('漢字', '羅馬字'):
+            tsuanpoo.add(tuple(ji))
+        return tsuanpoo
```

