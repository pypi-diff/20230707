# Comparing `tmp/kk-0.9.4.tar.gz` & `tmp/kk-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-0.9.4.tar", last modified: Wed Jun 28 09:10:15 2023, max compression
+gzip compressed data, was "kk-0.9.5.tar", last modified: Fri Jul  7 06:45:37 2023, max compression
```

## Comparing `kk-0.9.4.tar` & `kk-0.9.5.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.965628 kk-0.9.4/
--rw-r--r--   0 root         (0) root         (0)      589 2023-06-28 09:10:15.965628 kk-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3203 2022-07-14 13:13:22.000000 kk-0.9.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.949629 kk-0.9.4/kk/
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-28 09:10:09.000000 kk-0.9.4/kk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36753 2023-06-28 09:09:06.000000 kk-0.9.4/kk/handler.py
--rwxr-xr-x   0 root         (0) root         (0)     4035 2022-07-14 13:13:22.000000 kk-0.9.4/kk/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.949629 kk-0.9.4/kk/static/
--rw-r--r--   0 root         (0) root         (0)     4286 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.953629 kk-0.9.4/kk/static/img/
--rw-rw-r--   0 root         (0) root         (0)     3397 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/apk.png
--rw-rw-r--   0 root         (0) root         (0)     3105 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/audio.png
--rw-rw-r--   0 root         (0) root         (0)     4154 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/c.png
--rw-rw-r--   0 root         (0) root         (0)     3638 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/cpp.png
--rw-rw-r--   0 root         (0) root         (0)     5479 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/css.png
--rw-rw-r--   0 root         (0) root         (0)     4934 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/database.png
--rw-rw-r--   0 root         (0) root         (0)     3229 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/dmg.png
--rw-rw-r--   0 root         (0) root         (0)     4321 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/docx.png
--rw-rw-r--   0 root         (0) root         (0)     4436 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/exe.png
--rw-rw-r--   0 root         (0) root         (0)     3409 2023-06-19 00:58:34.000000 kk-0.9.4/kk/static/img/file.png
--rw-rw-r--   0 root         (0) root         (0)     1595 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/folder.png
--rw-rw-r--   0 root         (0) root         (0)     6366 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/golang.png
--rw-rw-r--   0 root         (0) root         (0)     3457 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/html.png
--rw-rw-r--   0 root         (0) root         (0)     3494 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/image.png
--rw-rw-r--   0 root         (0) root         (0)     5324 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/ini.png
--rw-rw-r--   0 root         (0) root         (0)     5633 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/iso.png
--rw-rw-r--   0 root         (0) root         (0)     5994 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/java.png
--rw-rw-r--   0 root         (0) root         (0)     5472 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/javascript.png
--rw-rw-r--   0 root         (0) root         (0)     4946 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/json.png
--rw-rw-r--   0 root         (0) root         (0)    11198 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/kindle.png
--rw-rw-r--   0 root         (0) root         (0)     3968 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/markdown.png
--rw-rw-r--   0 root         (0) root         (0)     4285 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/pdf.png
--rw-rw-r--   0 root         (0) root         (0)     3158 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/pptx.png
--rw-rw-r--   0 root         (0) root         (0)     3859 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/python.png
--rw-rw-r--   0 root         (0) root         (0)     2114 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/rar.png
--rw-rw-r--   0 root         (0) root         (0)     1394 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/shell.png
--rw-rw-r--   0 root         (0) root         (0)     3806 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/txt.png
--rw-rw-r--   0 root         (0) root         (0)     2448 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/video.png
--rw-rw-r--   0 root         (0) root         (0)     3623 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/vue.png
--rw-rw-r--   0 root         (0) root         (0)     3406 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/xlsx.png
--rw-r--r--   0 root         (0) root         (0)     3446 2023-06-19 01:39:13.000000 kk-0.9.4/kk/static/img/xml.png
--rw-rw-r--   0 root         (0) root         (0)     4812 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/yaml.png
--rw-rw-r--   0 root         (0) root         (0)     1930 2023-06-19 00:48:55.000000 kk-0.9.4/kk/static/img/zip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.957629 kk-0.9.4/kk/static/img2/
--rw-r--r--   0 root         (0) root         (0)     5153 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/apk.png
--rw-r--r--   0 root         (0) root         (0)    17071 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/audio.png
--rw-r--r--   0 root         (0) root         (0)     6382 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/c.png
--rw-r--r--   0 root         (0) root         (0)     6673 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/cpp.png
--rw-r--r--   0 root         (0) root         (0)     5635 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/css.png
--rw-r--r--   0 root         (0) root         (0)    16755 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/database.png
--rw-r--r--   0 root         (0) root         (0)     4006 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/dmg.png
--rw-r--r--   0 root         (0) root         (0)     7904 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/docx.png
--rw-r--r--   0 root         (0) root         (0)     2245 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/exe.png
--rw-r--r--   0 root         (0) root         (0)     2822 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/file.png
--rw-r--r--   0 root         (0) root         (0)     3688 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/folder.png
--rw-r--r--   0 root         (0) root         (0)    12494 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/golang.png
--rw-r--r--   0 root         (0) root         (0)     8140 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/html.png
--rw-r--r--   0 root         (0) root         (0)     7301 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/image.png
--rw-r--r--   0 root         (0) root         (0)     8962 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/ini.png
--rw-r--r--   0 root         (0) root         (0)     7287 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/iso.png
--rw-r--r--   0 root         (0) root         (0)    15616 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/java.png
--rw-r--r--   0 root         (0) root         (0)    10518 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/javascript.png
--rw-r--r--   0 root         (0) root         (0)     3847 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/json.png
--rw-r--r--   0 root         (0) root         (0)     2997 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/kindle.png
--rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/markdown.png
--rw-r--r--   0 root         (0) root         (0)    12717 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/pdf.png
--rw-r--r--   0 root         (0) root         (0)    12577 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/php.png
--rw-r--r--   0 root         (0) root         (0)     3574 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/pptx.png
--rw-r--r--   0 root         (0) root         (0)     9024 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/python.png
--rw-r--r--   0 root         (0) root         (0)     7434 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/shell.png
--rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/txt.png
--rw-r--r--   0 root         (0) root         (0)    15897 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/video.png
--rw-r--r--   0 root         (0) root         (0)    13413 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/vue.png
--rw-r--r--   0 root         (0) root         (0)     8139 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/xlsx.png
--rw-r--r--   0 root         (0) root         (0)     3449 2023-06-19 02:22:37.000000 kk-0.9.4/kk/static/img2/xml.png
--rw-r--r--   0 root         (0) root         (0)    11355 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/yaml.png
--rw-r--r--   0 root         (0) root         (0)     3509 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/img2/zip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.945629 kk-0.9.4/kk/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.957629 kk-0.9.4/kk/static/src/css/
--rw-r--r--   0 root         (0) root         (0)    45250 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/DPlayer.min.css
--rw-r--r--   0 root         (0) root         (0)     5254 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/iconfont.css
--rw-r--r--   0 root         (0) root         (0)     5572 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/iconfont.eot
--rw-r--r--   0 root         (0) root         (0)    15798 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/iconfont.svg
--rw-r--r--   0 root         (0) root         (0)     5404 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/iconfont.ttf
--rw-r--r--   0 root         (0) root         (0)     3536 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/iconfont.woff
--rw-r--r--   0 root         (0) root         (0)     2904 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/iconfont.woff2
--rw-r--r--   0 root         (0) root         (0)     3584 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/markdown.css
--rw-r--r--   0 root         (0) root         (0)     2477 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/css/monokai_sublime.css
--rw-r--r--   0 root         (0) root         (0)     9750 2023-06-19 02:23:34.000000 kk-0.9.4/kk/static/src/css/style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.957629 kk-0.9.4/kk/static/src/js/
--rw-r--r--   0 root         (0) root         (0)   116781 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/DPlayer.min.js
--rw-r--r--   0 root         (0) root         (0)    10453 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/clipboard.min.js
--rw-r--r--   0 root         (0) root         (0)   173418 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/flv.min.js
--rw-r--r--   0 root         (0) root         (0)    80655 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/highcharts-more.js
--rw-r--r--   0 root         (0) root         (0)   254576 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/highcharts.js
--rw-r--r--   0 root         (0) root         (0)   749330 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/highlight.pack.min.js
--rw-r--r--   0 root         (0) root         (0)   231552 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/hls.min.js
--rw-r--r--   0 root         (0) root         (0)     5595 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/imagesloaded.pkgd.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    24104 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/masonry.pkgd.min.js
--rw-r--r--   0 root         (0) root         (0)    20032 2023-06-21 03:28:51.000000 kk-0.9.4/kk/static/src/js/page.js
--rw-r--r--   0 root         (0) root         (0)     2221 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/utils.js
--rw-r--r--   0 root         (0) root         (0)    70754 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/js/webuploader.nolog.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.957629 kk-0.9.4/kk/static/src/layui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.957629 kk-0.9.4/kk/static/src/layui/css/
--rw-r--r--   0 root         (0) root         (0)    74304 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/layui.css
--rw-r--r--   0 root         (0) root         (0)     9886 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/layui.mobile.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.961629 kk-0.9.4/kk/static/src/layui/css/modules/
--rw-r--r--   0 root         (0) root         (0)     1064 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/code.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.945629 kk-0.9.4/kk/static/src/layui/css/modules/laydate/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.961629 kk-0.9.4/kk/static/src/layui/css/modules/laydate/default/
--rw-r--r--   0 root         (0) root         (0)     7538 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/laydate/default/laydate.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.949629 kk-0.9.4/kk/static/src/layui/css/modules/layer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.961629 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/
--rw-r--r--   0 root         (0) root         (0)     5911 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/icon-ext.png
--rw-r--r--   0 root         (0) root         (0)    11493 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/icon.png
--rw-r--r--   0 root         (0) root         (0)    14426 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/layer.css
--rw-r--r--   0 root         (0) root         (0)     5793 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/loading-0.gif
--rw-r--r--   0 root         (0) root         (0)      701 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/loading-1.gif
--rw-r--r--   0 root         (0) root         (0)     1787 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/css/modules/layer/default/loading-2.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.961629 kk-0.9.4/kk/static/src/layui/font/
--rw-r--r--   0 root         (0) root         (0)    46684 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/font/iconfont.eot
--rw-r--r--   0 root         (0) root         (0)   305858 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/font/iconfont.svg
--rw-r--r--   0 root         (0) root         (0)    46508 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/font/iconfont.ttf
--rw-r--r--   0 root         (0) root         (0)    30628 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/font/iconfont.woff
--rw-r--r--   0 root         (0) root         (0)    25964 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/font/iconfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.949629 kk-0.9.4/kk/static/src/layui/lay/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.961629 kk-0.9.4/kk/static/src/layui/lay/modules/
--rw-r--r--   0 root         (0) root         (0)     3863 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/carousel.js
--rw-r--r--   0 root         (0) root         (0)     1178 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/code.js
--rw-r--r--   0 root         (0) root         (0)    11740 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/colorpicker.js
--rw-r--r--   0 root         (0) root         (0)     7265 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/element.js
--rw-r--r--   0 root         (0) root         (0)     2027 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/flow.js
--rw-r--r--   0 root         (0) root         (0)     9464 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/form.js
--rw-r--r--   0 root         (0) root         (0)    97649 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/jquery.js
--rw-r--r--   0 root         (0) root         (0)    27378 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/laydate.js
--rw-r--r--   0 root         (0) root         (0)    12636 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/layedit.js
--rw-r--r--   0 root         (0) root         (0)    22042 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/layer.js
--rw-r--r--   0 root         (0) root         (0)     4473 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/laypage.js
--rw-r--r--   0 root         (0) root         (0)     1837 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/laytpl.js
--rw-r--r--   0 root         (0) root         (0)    53632 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/mobile.js
--rw-r--r--   0 root         (0) root         (0)     2754 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/rate.js
--rw-r--r--   0 root         (0) root         (0)     7050 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/slider.js
--rw-r--r--   0 root         (0) root         (0)    31564 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/table.js
--rw-r--r--   0 root         (0) root         (0)     6325 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/transfer.js
--rw-r--r--   0 root         (0) root         (0)    11545 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/tree.js
--rw-r--r--   0 root         (0) root         (0)     7467 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/upload.js
--rw-r--r--   0 root         (0) root         (0)     3837 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/lay/modules/util.js
--rw-r--r--   0 root         (0) root         (0)   278423 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/layui.all.js
--rw-r--r--   0 root         (0) root         (0)     7348 2022-07-14 13:13:22.000000 kk-0.9.4/kk/static/src/layui/layui.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.965628 kk-0.9.4/kk/templates/
--rw-r--r--   0 root         (0) root         (0)     3760 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/admin.html
--rw-r--r--   0 root         (0) root         (0)     4262 2023-02-19 15:22:17.000000 kk-0.9.4/kk/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     4032 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/chart.html
--rw-r--r--   0 root         (0) root         (0)    13923 2023-06-21 03:24:29.000000 kk-0.9.4/kk/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1772 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/manage.html
--rw-r--r--   0 root         (0) root         (0)     1461 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/reset.html
--rw-r--r--   0 root         (0) root         (0)     2995 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     1052 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/signin.html
--rw-r--r--   0 root         (0) root         (0)     1849 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/signup.html
--rw-r--r--   0 root         (0) root         (0)     5965 2022-07-14 13:13:22.000000 kk-0.9.4/kk/templates/table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 09:10:15.949629 kk-0.9.4/kk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      589 2023-06-28 09:10:15.000000 kk-0.9.4/kk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-28 09:10:15.000000 kk-0.9.4/kk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 09:10:15.000000 kk-0.9.4/kk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-28 09:10:15.000000 kk-0.9.4/kk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-28 09:10:15.000000 kk-0.9.4/kk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2023-06-28 09:10:15.000000 kk-0.9.4/kk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 09:10:15.965628 kk-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1319 2023-01-10 04:30:46.000000 kk-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.408516 kk-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-07 06:45:37.408516 kk-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3203 2022-07-14 13:13:22.000000 kk-0.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-07 06:45:33.000000 kk-0.9.5/kk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36574 2023-07-01 05:36:48.000000 kk-0.9.5/kk/handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     4035 2022-07-14 13:13:22.000000 kk-0.9.5/kk/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk/static/
+-rw-r--r--   0 root         (0) root         (0)     4286 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.384516 kk-0.9.5/kk/static/img/
+-rw-rw-r--   0 root         (0) root         (0)     3397 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/apk.png
+-rw-rw-r--   0 root         (0) root         (0)     3105 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/audio.png
+-rw-rw-r--   0 root         (0) root         (0)     4154 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/c.png
+-rw-rw-r--   0 root         (0) root         (0)     3638 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/cpp.png
+-rw-rw-r--   0 root         (0) root         (0)     5479 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/css.png
+-rw-rw-r--   0 root         (0) root         (0)     4934 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/database.png
+-rw-rw-r--   0 root         (0) root         (0)     3229 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/dmg.png
+-rw-rw-r--   0 root         (0) root         (0)     4321 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/docx.png
+-rw-rw-r--   0 root         (0) root         (0)     4436 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/exe.png
+-rw-rw-r--   0 root         (0) root         (0)     3409 2023-06-19 00:58:34.000000 kk-0.9.5/kk/static/img/file.png
+-rw-rw-r--   0 root         (0) root         (0)     1595 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/folder.png
+-rw-rw-r--   0 root         (0) root         (0)     6366 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/golang.png
+-rw-rw-r--   0 root         (0) root         (0)     3457 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/html.png
+-rw-rw-r--   0 root         (0) root         (0)     3494 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/image.png
+-rw-rw-r--   0 root         (0) root         (0)     5324 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/ini.png
+-rw-rw-r--   0 root         (0) root         (0)     5633 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/iso.png
+-rw-rw-r--   0 root         (0) root         (0)     5994 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/java.png
+-rw-rw-r--   0 root         (0) root         (0)     5472 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/javascript.png
+-rw-rw-r--   0 root         (0) root         (0)     4946 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/json.png
+-rw-rw-r--   0 root         (0) root         (0)    11198 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/kindle.png
+-rw-rw-r--   0 root         (0) root         (0)     3968 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/markdown.png
+-rw-rw-r--   0 root         (0) root         (0)     4285 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/pdf.png
+-rw-rw-r--   0 root         (0) root         (0)     3158 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/pptx.png
+-rw-rw-r--   0 root         (0) root         (0)     3859 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/python.png
+-rw-rw-r--   0 root         (0) root         (0)     2114 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/rar.png
+-rw-rw-r--   0 root         (0) root         (0)     1394 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/shell.png
+-rw-rw-r--   0 root         (0) root         (0)     3806 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/txt.png
+-rw-rw-r--   0 root         (0) root         (0)     2448 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/video.png
+-rw-rw-r--   0 root         (0) root         (0)     3623 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/vue.png
+-rw-rw-r--   0 root         (0) root         (0)     3406 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/xlsx.png
+-rw-r--r--   0 root         (0) root         (0)     3446 2023-06-19 01:39:13.000000 kk-0.9.5/kk/static/img/xml.png
+-rw-rw-r--   0 root         (0) root         (0)     4812 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/yaml.png
+-rw-rw-r--   0 root         (0) root         (0)     1930 2023-06-19 00:48:55.000000 kk-0.9.5/kk/static/img/zip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.388516 kk-0.9.5/kk/static/img2/
+-rw-r--r--   0 root         (0) root         (0)     5153 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/apk.png
+-rw-r--r--   0 root         (0) root         (0)    17071 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/audio.png
+-rw-r--r--   0 root         (0) root         (0)     6382 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/c.png
+-rw-r--r--   0 root         (0) root         (0)     6673 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/cpp.png
+-rw-r--r--   0 root         (0) root         (0)     5635 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/css.png
+-rw-r--r--   0 root         (0) root         (0)    16755 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/database.png
+-rw-r--r--   0 root         (0) root         (0)     4006 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/dmg.png
+-rw-r--r--   0 root         (0) root         (0)     7904 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/docx.png
+-rw-r--r--   0 root         (0) root         (0)     2245 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/exe.png
+-rw-r--r--   0 root         (0) root         (0)     2822 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/file.png
+-rw-r--r--   0 root         (0) root         (0)     3688 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/folder.png
+-rw-r--r--   0 root         (0) root         (0)    12494 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/golang.png
+-rw-r--r--   0 root         (0) root         (0)     8140 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/html.png
+-rw-r--r--   0 root         (0) root         (0)     7301 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/image.png
+-rw-r--r--   0 root         (0) root         (0)     8962 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/ini.png
+-rw-r--r--   0 root         (0) root         (0)     7287 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/iso.png
+-rw-r--r--   0 root         (0) root         (0)    15616 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/java.png
+-rw-r--r--   0 root         (0) root         (0)    10518 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/javascript.png
+-rw-r--r--   0 root         (0) root         (0)     3847 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/json.png
+-rw-r--r--   0 root         (0) root         (0)     2997 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/kindle.png
+-rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/markdown.png
+-rw-r--r--   0 root         (0) root         (0)    12717 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/pdf.png
+-rw-r--r--   0 root         (0) root         (0)    12577 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/php.png
+-rw-r--r--   0 root         (0) root         (0)     3574 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/pptx.png
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/python.png
+-rw-r--r--   0 root         (0) root         (0)     7434 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/shell.png
+-rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/txt.png
+-rw-r--r--   0 root         (0) root         (0)    15897 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/video.png
+-rw-r--r--   0 root         (0) root         (0)    13413 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/vue.png
+-rw-r--r--   0 root         (0) root         (0)     8139 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/xlsx.png
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-06-19 02:22:37.000000 kk-0.9.5/kk/static/img2/xml.png
+-rw-r--r--   0 root         (0) root         (0)    11355 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/yaml.png
+-rw-r--r--   0 root         (0) root         (0)     3509 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/img2/zip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.388516 kk-0.9.5/kk/static/src/css/
+-rw-r--r--   0 root         (0) root         (0)    45250 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/DPlayer.min.css
+-rw-r--r--   0 root         (0) root         (0)     5254 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/iconfont.css
+-rw-r--r--   0 root         (0) root         (0)     5572 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/iconfont.eot
+-rw-r--r--   0 root         (0) root         (0)    15798 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/iconfont.svg
+-rw-r--r--   0 root         (0) root         (0)     5404 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/iconfont.ttf
+-rw-r--r--   0 root         (0) root         (0)     3536 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/iconfont.woff
+-rw-r--r--   0 root         (0) root         (0)     2904 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/iconfont.woff2
+-rw-r--r--   0 root         (0) root         (0)     3584 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/markdown.css
+-rw-r--r--   0 root         (0) root         (0)     2477 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/css/monokai_sublime.css
+-rw-r--r--   0 root         (0) root         (0)     9820 2023-07-01 04:40:40.000000 kk-0.9.5/kk/static/src/css/style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.396516 kk-0.9.5/kk/static/src/js/
+-rw-r--r--   0 root         (0) root         (0)   116781 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/DPlayer.min.js
+-rw-r--r--   0 root         (0) root         (0)    10453 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/clipboard.min.js
+-rw-r--r--   0 root         (0) root         (0)   173418 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/flv.min.js
+-rw-r--r--   0 root         (0) root         (0)    80655 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/highcharts-more.js
+-rw-r--r--   0 root         (0) root         (0)   254576 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/highcharts.js
+-rw-r--r--   0 root         (0) root         (0)   749330 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/highlight.pack.min.js
+-rw-r--r--   0 root         (0) root         (0)   231552 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/hls.min.js
+-rw-r--r--   0 root         (0) root         (0)     5595 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/imagesloaded.pkgd.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    24104 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/masonry.pkgd.min.js
+-rw-r--r--   0 root         (0) root         (0)    20285 2023-07-07 06:43:07.000000 kk-0.9.5/kk/static/src/js/page.js
+-rw-r--r--   0 root         (0) root         (0)     2221 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/utils.js
+-rw-r--r--   0 root         (0) root         (0)    70754 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/js/webuploader.nolog.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.396516 kk-0.9.5/kk/static/src/layui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.396516 kk-0.9.5/kk/static/src/layui/css/
+-rw-r--r--   0 root         (0) root         (0)    74304 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/layui.css
+-rw-r--r--   0 root         (0) root         (0)     9886 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/layui.mobile.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.396516 kk-0.9.5/kk/static/src/layui/css/modules/
+-rw-r--r--   0 root         (0) root         (0)     1064 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/code.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk/static/src/layui/css/modules/laydate/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.396516 kk-0.9.5/kk/static/src/layui/css/modules/laydate/default/
+-rw-r--r--   0 root         (0) root         (0)     7538 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/laydate/default/laydate.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk/static/src/layui/css/modules/layer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.396516 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/
+-rw-r--r--   0 root         (0) root         (0)     5911 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/icon-ext.png
+-rw-r--r--   0 root         (0) root         (0)    11493 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/icon.png
+-rw-r--r--   0 root         (0) root         (0)    14426 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/layer.css
+-rw-r--r--   0 root         (0) root         (0)     5793 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/loading-0.gif
+-rw-r--r--   0 root         (0) root         (0)      701 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/loading-1.gif
+-rw-r--r--   0 root         (0) root         (0)     1787 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/css/modules/layer/default/loading-2.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.400516 kk-0.9.5/kk/static/src/layui/font/
+-rw-r--r--   0 root         (0) root         (0)    46684 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/font/iconfont.eot
+-rw-r--r--   0 root         (0) root         (0)   305858 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/font/iconfont.svg
+-rw-r--r--   0 root         (0) root         (0)    46508 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/font/iconfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    30628 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/font/iconfont.woff
+-rw-r--r--   0 root         (0) root         (0)    25964 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/font/iconfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk/static/src/layui/lay/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.404516 kk-0.9.5/kk/static/src/layui/lay/modules/
+-rw-r--r--   0 root         (0) root         (0)     3863 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/carousel.js
+-rw-r--r--   0 root         (0) root         (0)     1178 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/code.js
+-rw-r--r--   0 root         (0) root         (0)    11740 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/colorpicker.js
+-rw-r--r--   0 root         (0) root         (0)     7265 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/element.js
+-rw-r--r--   0 root         (0) root         (0)     2027 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/flow.js
+-rw-r--r--   0 root         (0) root         (0)     9464 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/form.js
+-rw-r--r--   0 root         (0) root         (0)    97649 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/jquery.js
+-rw-r--r--   0 root         (0) root         (0)    27378 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/laydate.js
+-rw-r--r--   0 root         (0) root         (0)    12636 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/layedit.js
+-rw-r--r--   0 root         (0) root         (0)    22042 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/layer.js
+-rw-r--r--   0 root         (0) root         (0)     4473 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/laypage.js
+-rw-r--r--   0 root         (0) root         (0)     1837 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/laytpl.js
+-rw-r--r--   0 root         (0) root         (0)    53632 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/mobile.js
+-rw-r--r--   0 root         (0) root         (0)     2754 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/rate.js
+-rw-r--r--   0 root         (0) root         (0)     7050 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/slider.js
+-rw-r--r--   0 root         (0) root         (0)    31564 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/table.js
+-rw-r--r--   0 root         (0) root         (0)     6325 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/transfer.js
+-rw-r--r--   0 root         (0) root         (0)    11545 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/tree.js
+-rw-r--r--   0 root         (0) root         (0)     7467 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/upload.js
+-rw-r--r--   0 root         (0) root         (0)     3837 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/lay/modules/util.js
+-rw-r--r--   0 root         (0) root         (0)   278423 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/layui.all.js
+-rw-r--r--   0 root         (0) root         (0)     7348 2022-07-14 13:13:22.000000 kk-0.9.5/kk/static/src/layui/layui.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.404516 kk-0.9.5/kk/templates/
+-rw-r--r--   0 root         (0) root         (0)     3760 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/admin.html
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-07-07 06:45:21.000000 kk-0.9.5/kk/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     4032 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/chart.html
+-rw-r--r--   0 root         (0) root         (0)    13769 2023-07-07 06:41:43.000000 kk-0.9.5/kk/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/manage.html
+-rw-r--r--   0 root         (0) root         (0)     1461 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/reset.html
+-rw-r--r--   0 root         (0) root         (0)     2995 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     1052 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/signin.html
+-rw-r--r--   0 root         (0) root         (0)     1849 2022-07-14 13:13:22.000000 kk-0.9.5/kk/templates/signup.html
+-rw-r--r--   0 root         (0) root         (0)     5934 2023-07-01 05:40:18.000000 kk-0.9.5/kk/templates/table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:45:37.376516 kk-0.9.5/kk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-07 06:45:37.000000 kk-0.9.5/kk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-07 06:45:37.000000 kk-0.9.5/kk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 06:45:37.000000 kk-0.9.5/kk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-07 06:45:37.000000 kk-0.9.5/kk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-07 06:45:37.000000 kk-0.9.5/kk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        3 2023-07-07 06:45:37.000000 kk-0.9.5/kk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 06:45:37.408516 kk-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-01-10 04:30:46.000000 kk-0.9.5/setup.py
```

### Comparing `kk-0.9.4/README.md` & `kk-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/handler.py` & `kk-0.9.5/kk/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import urllib.parse
 import zipfile
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 import markdown
 import tornado.web
-import yaml
 from bson import ObjectId
 from tornado.concurrent import run_on_executor
 from tornado_utils import BaseHandler, Blueprint
 from utils import Dict
 
 bp = Blueprint(__name__)
 
@@ -489,29 +488,25 @@
                 self.preview_tar(path)
             elif re.match('(docx|doc|xlsx|xls|pptx|ppt)$', suffix):
                 self.preview_office()
             elif re.match('(mp4|mkv|flv|m3u8)$', suffix):
                 self.preview_video()
             elif re.match('(mp3|ogg|amr|wav)$', suffix):
                 self.preview_audio()
-            elif re.match('(yml|yaml)$', suffix):
-                self.finish(yaml.load(open(path), Loader=yaml.FullLoader))
-            elif suffix == 'json':
-                self.finish(json.load(open(path)))
             elif re.match('(md|markdown)$', suffix):
                 exts = ['markdown.extensions.extra', 'markdown.extensions.codehilite', 'markdown.extensions.tables', 'markdown.extensions.toc']
                 html = markdown.markdown(path.read_text(), extensions=exts)
                 self.preview_html(html, padding=20, background='#fff')
             elif suffix == 'ipynb':
                 with tempfile.NamedTemporaryFile('w+', suffix='.html', delete=True) as fp:
                     command = f'jupyter nbconvert --to html --template full --output {fp.name} {path}'
                     dl = await asyncio.create_subprocess_shell(command)
                     await dl.wait()
                     self.finish(fp.read().replace('<link rel="stylesheet" href="custom.css">', ''))
-            elif re.match('(py|sh|cu|h|hpp|c|cpp|vue|php|js|css|html|less|scss|pig|java|go|ini|conf|txt|cfg|log)$', suffix):
+            elif re.match('(py|sh|cu|h|hpp|c|cpp|vue|php|js|css|html|less|scss|pig|java|go|ini|conf|txt|cfg|log|json|yml|yaml)$', suffix):
                 code = {
                     'py': 'python',
                     'sh': 'bash',
                     'h': 'c',
                     'js': 'javascript',
                     'vue': 'javascript',
                     'conf': 'txt',
@@ -687,15 +682,15 @@
             await self.delete(name)
         else:
             await self.upload(path)
 
     @check_auth
     async def delete(self, name):
         if not self.app.options.delete:
-            raise tornado.web.HTTPError(403)
+            return self.finish({'err': 1, 'msg': '无权限删除文件'})
 
         path = self.root / name
         if not path.exists():
             return self.finish({'err': 1, 'msg': f'{name} 文件不存在'})
 
         if self.app.options.auth:
             await self.db.share.delete_many({'name': name})
```

### Comparing `kk-0.9.4/kk/index.py` & `kk-0.9.5/kk/index.py`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/favicon.ico` & `kk-0.9.5/kk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/apk.png` & `kk-0.9.5/kk/static/img/apk.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/audio.png` & `kk-0.9.5/kk/static/img/audio.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/c.png` & `kk-0.9.5/kk/static/img/c.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/cpp.png` & `kk-0.9.5/kk/static/img/cpp.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/css.png` & `kk-0.9.5/kk/static/img/css.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/database.png` & `kk-0.9.5/kk/static/img/database.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/dmg.png` & `kk-0.9.5/kk/static/img/dmg.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/docx.png` & `kk-0.9.5/kk/static/img/docx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/exe.png` & `kk-0.9.5/kk/static/img/exe.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/file.png` & `kk-0.9.5/kk/static/img/file.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/folder.png` & `kk-0.9.5/kk/static/img/folder.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/golang.png` & `kk-0.9.5/kk/static/img/golang.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/html.png` & `kk-0.9.5/kk/static/img/html.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/image.png` & `kk-0.9.5/kk/static/img/image.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/ini.png` & `kk-0.9.5/kk/static/img/ini.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/iso.png` & `kk-0.9.5/kk/static/img/iso.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/java.png` & `kk-0.9.5/kk/static/img/java.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/javascript.png` & `kk-0.9.5/kk/static/img/javascript.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/json.png` & `kk-0.9.5/kk/static/img/json.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/kindle.png` & `kk-0.9.5/kk/static/img/kindle.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/markdown.png` & `kk-0.9.5/kk/static/img/markdown.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/pdf.png` & `kk-0.9.5/kk/static/img/pdf.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/pptx.png` & `kk-0.9.5/kk/static/img/pptx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/python.png` & `kk-0.9.5/kk/static/img/python.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/rar.png` & `kk-0.9.5/kk/static/img/rar.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/shell.png` & `kk-0.9.5/kk/static/img/shell.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/txt.png` & `kk-0.9.5/kk/static/img/txt.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/video.png` & `kk-0.9.5/kk/static/img/video.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/vue.png` & `kk-0.9.5/kk/static/img/vue.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/xlsx.png` & `kk-0.9.5/kk/static/img/xlsx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/xml.png` & `kk-0.9.5/kk/static/img/xml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/yaml.png` & `kk-0.9.5/kk/static/img/yaml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img/zip.png` & `kk-0.9.5/kk/static/img/zip.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/apk.png` & `kk-0.9.5/kk/static/img2/apk.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/audio.png` & `kk-0.9.5/kk/static/img2/audio.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/c.png` & `kk-0.9.5/kk/static/img2/c.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/cpp.png` & `kk-0.9.5/kk/static/img2/cpp.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/css.png` & `kk-0.9.5/kk/static/img2/css.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/database.png` & `kk-0.9.5/kk/static/img2/database.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/dmg.png` & `kk-0.9.5/kk/static/img2/dmg.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/docx.png` & `kk-0.9.5/kk/static/img2/docx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/exe.png` & `kk-0.9.5/kk/static/img2/exe.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/file.png` & `kk-0.9.5/kk/static/img2/file.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/folder.png` & `kk-0.9.5/kk/static/img2/folder.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/golang.png` & `kk-0.9.5/kk/static/img2/golang.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/html.png` & `kk-0.9.5/kk/static/img2/html.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/image.png` & `kk-0.9.5/kk/static/img2/image.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/ini.png` & `kk-0.9.5/kk/static/img2/ini.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/iso.png` & `kk-0.9.5/kk/static/img2/iso.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/java.png` & `kk-0.9.5/kk/static/img2/java.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/javascript.png` & `kk-0.9.5/kk/static/img2/javascript.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/json.png` & `kk-0.9.5/kk/static/img2/json.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/kindle.png` & `kk-0.9.5/kk/static/img2/kindle.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/markdown.png` & `kk-0.9.5/kk/static/img2/markdown.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/pdf.png` & `kk-0.9.5/kk/static/img2/pdf.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/php.png` & `kk-0.9.5/kk/static/img2/php.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/pptx.png` & `kk-0.9.5/kk/static/img2/pptx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/python.png` & `kk-0.9.5/kk/static/img2/python.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/shell.png` & `kk-0.9.5/kk/static/img2/shell.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/txt.png` & `kk-0.9.5/kk/static/img2/txt.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/video.png` & `kk-0.9.5/kk/static/img2/video.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/vue.png` & `kk-0.9.5/kk/static/img2/vue.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/xlsx.png` & `kk-0.9.5/kk/static/img2/xlsx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/xml.png` & `kk-0.9.5/kk/static/img2/xml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/yaml.png` & `kk-0.9.5/kk/static/img2/yaml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/img2/zip.png` & `kk-0.9.5/kk/static/img2/zip.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/DPlayer.min.css` & `kk-0.9.5/kk/static/src/css/DPlayer.min.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/iconfont.css` & `kk-0.9.5/kk/static/src/css/iconfont.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/iconfont.eot` & `kk-0.9.5/kk/static/src/css/iconfont.eot`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/iconfont.svg` & `kk-0.9.5/kk/static/src/css/iconfont.svg`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/iconfont.ttf` & `kk-0.9.5/kk/static/src/css/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/iconfont.woff` & `kk-0.9.5/kk/static/src/css/iconfont.woff`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/iconfont.woff2` & `kk-0.9.5/kk/static/src/css/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/markdown.css` & `kk-0.9.5/kk/static/src/css/markdown.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/monokai_sublime.css` & `kk-0.9.5/kk/static/src/css/monokai_sublime.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/css/style.css` & `kk-0.9.5/kk/static/src/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,18 @@
 .layui-icon:hover {
     color: #63ab5e;
 }
 .layui-card {
   background-color: #f9f9f9;
   text-align: center;
 }
+.layui-card-body:hover {
+  transform: scale(1.05);
+  z-index: 1000;
+}
 .list-name {
   white-space: pre-wrap;
   word-wrap: break-word;
 }
 .table-name {
   white-space: pre-wrap;
   word-wrap: break-word;
```

### Comparing `kk-0.9.4/kk/static/src/js/DPlayer.min.js` & `kk-0.9.5/kk/static/src/js/DPlayer.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/clipboard.min.js` & `kk-0.9.5/kk/static/src/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/flv.min.js` & `kk-0.9.5/kk/static/src/js/flv.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/highcharts-more.js` & `kk-0.9.5/kk/static/src/js/highcharts-more.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/highcharts.js` & `kk-0.9.5/kk/static/src/js/highcharts.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/highlight.pack.min.js` & `kk-0.9.5/kk/static/src/js/highlight.pack.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/hls.min.js` & `kk-0.9.5/kk/static/src/js/hls.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/imagesloaded.pkgd.min.js` & `kk-0.9.5/kk/static/src/js/imagesloaded.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/jquery.min.js` & `kk-0.9.5/kk/static/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/masonry.pkgd.min.js` & `kk-0.9.5/kk/static/src/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/page.js` & `kk-0.9.5/kk/static/src/js/page.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -384,29 +384,33 @@
             })
         })
 
         $(document).on('click', '.btn-select', function() {
             $(this).parents('tr').toggleClass('selected')
         })
 
+        $(document).on('click', '.btn-enter', function() {
+            var link = $(this).parents('tr').find('.file-link').length > 0 ? $(this).parents('tr').find('.file-link') : $(this).parents('.layui-card-body').find('.file-link');
+            location.href = link.attr('href');
+        })
+
         $(document).on("click", ".btn-preview", function() {
             var link = $(this).parents('tr').find('.file-link').length > 0 ? $(this).parents('tr').find('.file-link') : $(this).parents('.layui-card-body').find('.file-link');
             var url = link.attr('href');
             if (url.indexOf('?') >= 0) url += '&f=preview';
             else url += '?f=preview';
             var name = $.trim(link.text());
             layer.open({
                 type: 2,
                 title: name,
                 content: url,
                 shadeClose: true,
                 area: ['1000px', '700px'],
                 success: function(layero, index) {
                     var css = {
-                        "display": "block",
                         "max-width": "100%",
                         "max-height": "100%",
                         "margin": "0 auto"
                     };
                     $($("iframe").contents().find("body")).children("img:first").css(css);
                 }
             })
```

### Comparing `kk-0.9.4/kk/static/src/js/utils.js` & `kk-0.9.5/kk/static/src/js/utils.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/js/webuploader.nolog.min.js` & `kk-0.9.5/kk/static/src/js/webuploader.nolog.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/layui.css` & `kk-0.9.5/kk/static/src/layui/css/layui.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/layui.mobile.css` & `kk-0.9.5/kk/static/src/layui/css/layui.mobile.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/code.css` & `kk-0.9.5/kk/static/src/layui/css/modules/code.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/laydate/default/laydate.css` & `kk-0.9.5/kk/static/src/layui/css/modules/laydate/default/laydate.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/layer/default/icon-ext.png` & `kk-0.9.5/kk/static/src/layui/css/modules/layer/default/icon-ext.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/layer/default/icon.png` & `kk-0.9.5/kk/static/src/layui/css/modules/layer/default/icon.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/layer/default/layer.css` & `kk-0.9.5/kk/static/src/layui/css/modules/layer/default/layer.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/layer/default/loading-0.gif` & `kk-0.9.5/kk/static/src/layui/css/modules/layer/default/loading-0.gif`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/layer/default/loading-1.gif` & `kk-0.9.5/kk/static/src/layui/css/modules/layer/default/loading-1.gif`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/css/modules/layer/default/loading-2.gif` & `kk-0.9.5/kk/static/src/layui/css/modules/layer/default/loading-2.gif`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/font/iconfont.eot` & `kk-0.9.5/kk/static/src/layui/font/iconfont.eot`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/font/iconfont.svg` & `kk-0.9.5/kk/static/src/layui/font/iconfont.svg`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/font/iconfont.ttf` & `kk-0.9.5/kk/static/src/layui/font/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/font/iconfont.woff` & `kk-0.9.5/kk/static/src/layui/font/iconfont.woff`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/font/iconfont.woff2` & `kk-0.9.5/kk/static/src/layui/font/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/carousel.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/carousel.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/code.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/code.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/colorpicker.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/colorpicker.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/element.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/element.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/flow.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/flow.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/form.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/form.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/jquery.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/jquery.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/laydate.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/laydate.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/layedit.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/layedit.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/layer.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/layer.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/laypage.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/laypage.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/laytpl.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/laytpl.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/mobile.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/mobile.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/rate.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/rate.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/slider.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/slider.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/table.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/table.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/transfer.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/transfer.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/tree.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/tree.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/upload.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/upload.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/lay/modules/util.js` & `kk-0.9.5/kk/static/src/layui/lay/modules/util.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/layui.all.js` & `kk-0.9.5/kk/static/src/layui/layui.all.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/static/src/layui/layui.js` & `kk-0.9.5/kk/static/src/layui/layui.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/admin.html` & `kk-0.9.5/kk/templates/admin.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/base.html` & `kk-0.9.5/kk/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         var params = parseUrl().params;
         layui.laypage.render({
           elem: 'pagination',
           limit: {{ handler.args.size }},
           count: {{ handler.args.total }},
           curr: {{ handler.args.page }},
           limits: [50, 100, 200, 300, 500],
-          layout: ['page', 'size', 'limit'],
+          layout: ['page', 'size', 'limit', 'count'],
           jump: function(obj, first){
             if(!first){
               params.page = obj.curr;
               params.size = obj.limit;
               location.href = location.pathname + '?' + layui.$.param(params);
             }
           }
```

### Comparing `kk-0.9.4/kk/templates/chart.html` & `kk-0.9.5/kk/templates/chart.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/index.html` & `kk-0.9.5/kk/templates/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -67,28 +67,28 @@
 <div class="layui-row">
   <div class="layui-col-md2" style="min-height:0.1px;">
     <ul id="tree" {% if not handler.get_cookie('tree') %}class="layui-hide"{% end %}></ul>
   </div>
   <div class="tree-table layui-col-md{{ 10 if handler.get_cookie('tree') else 12 }}">
     {% if handler.get_cookie('table') %}
     <div id="masonry" class="layui-row layui-col-space15">
-			{% set col = 3 if not handler.get_cookie('preview') and any([doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] for doc in entries]) else 2 %}
+			{% set col = 2 %}
       {% for doc in entries %}
       <div class="grid-item layui-col-md{{ col }}">
         <div class="layui-card">
           <div class="layui-card-body">
             {% set icon = 'folder.png' if doc.is_dir else handler.icon.get(doc.path.suffix.lower(), 'file.png') %}
             <a class="file-link" href="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}">
               {% if not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.webp'] %}
               <img style="display:block" src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}" {% if handler.args.w %}width="{{ int(handler.args.w) }}"{% end %} {% if handler.args.h %}height="{{ int(handler.args.h) }}"{% end %}>
               {% elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}
               <audio style="display:block" controls="controls"><source src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"></audio>
               {% else %}
               {% set icon = 'folder.png' if doc.is_dir else handler.icon.get(doc.path.suffix.lower(), 'file.png') %}
-              <img width=80 height=80 style="margin-bottom:3px" src="{{ static_url(f'img/{icon}') }}">
+              <img style="margin-bottom:3px" src="{{ static_url(f'img/{icon}') }}">
               {% end %}
               <span class="table-name">{{ doc.path.name }}</span>
             </a>
             <div class="action layui-hide">
               <button class="layui-btn layui-btn-radius layui-btn-primary layui-btn-xs btn-preview">
                 <i class="icon iconfont icon-yulan- layui-tips" tips="预览"></i>
               </button>
@@ -122,15 +122,15 @@
           <th class="pc" style="width:120px"><a href="{{ handler.add_args(sort='time', order=((0 - handler.args.order) if handler.args.sort == 'time' and handler.args.order else -1)) }}"><span>修改时间</span>{% if handler.args.sort == 'time' and handler.args.order == 1 %}<span class="arrow-down arrow-up"></span>{% elif handler.args.sort == 'time' and handler.args.order == - 1 %}<span class="arrow-down"></span>{% end %}</a></th>
           <th class="pc" style="width:60px"><a href="{{ handler.add_args(sort='size', order=((0 - handler.args.order) if handler.args.sort == 'size' and handler.args.order else -1)) }}"><span>文件大小</span>{% if handler.args.sort == 'size' and handler.args.order == 1 %}<span class="arrow-down arrow-up"></span>{% elif handler.args.sort == 'size' and handler.args.order == - 1 %}<span class="arrow-down"></span>{% end %}</a></th>
         </tr>
       </thead>
       <tbody>
         {% for doc in entries %}
         <tr>
-          <td class="btn-select" style="text-align:left !important">
+          <td class="btn-enter" style="text-align:left !important">
             {% if not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.webp'] %}
             <a href="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"><img style="display:block" src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}" {% if handler.args.w %}width="{{ int(handler.args.w) }}"{% end %} {% if handler.args.h %}height="{{ int(handler.args.h) }}"{% end %}></a>
             {% elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}
             <audio style="display:block" controls="controls" ><source src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"></audio>
             {% elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp4', 'mkv'] %}
             <video style="display:block" controls="controls"><source src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"></video>
             {% else %}
```

#### html2text {}

```diff
@@ -12,17 +12,15 @@
 else 1) %}
 {%_if_(i_==_2_and_handler.app.options.auth)_or_i_==_1_%}{%_else_%}{
 {_urllib.parse.unquote(path)_}}{%_end_%}
  {% end %} {% end %}
 {% end %}
 % if not handler.get_cookie('tree') %}class="layui-hide"{% end %}>
 {% if handler.get_cookie('table') %}
-{% set col = 3 if not handler.get_cookie('preview') and any(
-[doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] for doc in
-entries]) else 2 %} {% for doc in entries %}
+{% set col = 2 %} {% for doc in entries %}
 {% set icon = 'folder.png' if doc.is_dir else handler.icon.get
 (doc.path.suffix.lower(), 'file.png') %} {%_if_not_handler.get_cookie
 ('preview')_and_doc.path.suffix.lower()_in_['.jpg',_'.jpeg',_'.png',_'.bmp',
 '.gif',_'.webp']_%}_%_if_handler.args.w_%}width="{{_int(handler.args.w)_}}"{%
 end_%}_{%_if_handler.args.h_%}height="{{_int(handler.args.h)_}}"{%_end_%}>_{%
 elif_not_handler.get_cookie('preview')_and_doc.path.suffix.lower()_in_['.mp3',
 '.amr',_'.ogg',_'.wav']_%}__{%_else_%}_{%_set_icon_=_'folder.png'_if_doc.is_dir
```

### Comparing `kk-0.9.4/kk/templates/manage.html` & `kk-0.9.5/kk/templates/manage.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/reset.html` & `kk-0.9.5/kk/templates/reset.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/search.html` & `kk-0.9.5/kk/templates/search.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/signin.html` & `kk-0.9.5/kk/templates/signin.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/signup.html` & `kk-0.9.5/kk/templates/signup.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/kk/templates/table.html` & `kk-0.9.5/kk/templates/table.html`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,20 @@
             <td>顺序还是倒叙，默认为倒叙</td>
           </tr>
           <tr>
             <td>page</td>
             <td>当前页数，默认为1</td>
           </tr>
           <tr>
-            <td>count</td>
+            <td>size</td>
             <td>每一页显示多少项，默认为20</td>
           </tr>
           <tr>
             <td>f</td>
-            <td>当f=json时，返回json格式数据，可用于获取标注结果</td>
+            <td>当f=json时，返回json格式数据</td>
           </tr>
           <tr>
             <td rowspan=5>POST</td>
             <td rowspan=5>/table/name</td>
             <td rowspan=5>新增名为name的表<br>body为json格式，其字段类型描述如右所述</td>
           </tr>
           <tr>
```

### Comparing `kk-0.9.4/kk.egg-info/SOURCES.txt` & `kk-0.9.5/kk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kk-0.9.4/setup.py` & `kk-0.9.5/setup.py`

 * *Files identical despite different names*

