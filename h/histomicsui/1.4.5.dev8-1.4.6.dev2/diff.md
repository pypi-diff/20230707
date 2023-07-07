# Comparing `tmp/histomicsui-1.4.5.dev8.tar.gz` & `tmp/histomicsui-1.4.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicsui-1.4.5.dev8.tar", last modified: Thu Jun 29 14:27:16 2023, max compression
+gzip compressed data, was "histomicsui-1.4.6.dev2.tar", last modified: Fri Jul  7 19:25:52 2023, max compression
```

## Comparing `histomicsui-1.4.5.dev8.tar` & `histomicsui-1.4.6.dev2.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.059119 histomicsui-1.4.5.dev8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.035119 histomicsui-1.4.5.dev8/.circleci/
--rw-r--r--   0 root         (0) root         (0)     3884 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      532 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/.git-blame-ignore-revs
--rw-r--r--   0 root         (0) root         (0)      556 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/.gitignore
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/.travis.yml
--rw-r--r--   0 root         (0) root         (0)    10173 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      585 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7025 2023-06-29 14:27:16.059119 histomicsui-1.4.5.dev8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6076 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.039119 histomicsui-1.4.5.dev8/docs/
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/docs/config_options.rst
--rw-r--r--   0 root         (0) root         (0)     6059 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/docs/controls.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.039119 histomicsui-1.4.5.dev8/docs/images/
--rwxr-xr-x   0 root         (0) root         (0)   133796 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/docs/images/difference.gif
--rwxr-xr-x   0 root         (0) root         (0)   133603 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/docs/images/intersect.gif
--rwxr-xr-x   0 root         (0) root         (0)   154141 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/docs/images/union.gif
--rwxr-xr-x   0 root         (0) root         (0)   168255 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/docs/images/xor.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.039119 histomicsui-1.4.5.dev8/histomicsui/
--rw-r--r--   0 root         (0) root         (0)    17663 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/constants.py
--rw-r--r--   0 root         (0) root         (0)    10489 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.039119 histomicsui-1.4.5.dev8/histomicsui/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/aperio.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/case.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/cohort.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/image.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/meta.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/pathology.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/models/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.043119 histomicsui-1.4.5.dev8/histomicsui/rest/
--rw-r--r--   0 root         (0) root         (0)      512 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3728 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/rest/aperio.py
--rw-r--r--   0 root         (0) root         (0)     9313 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/rest/hui_resource.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/rest/image_browse_resource.py
--rw-r--r--   0 root         (0) root         (0)    15298 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/rest/system.py
--rw-r--r--   0 root         (0) root         (0)    28968 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/rest/tcga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.043119 histomicsui-1.4.5.dev8/histomicsui/web_client/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.043119 histomicsui-1.4.5.dev8/histomicsui/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/collections/StyleCollection.js
--rw-r--r--   0 root         (0) root         (0)      405 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/collections/UserCollection.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/collections/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.043119 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/
--rw-r--r--   0 root         (0) root         (0)     1326 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/confirmDialog.js
--rw-r--r--   0 root         (0) root         (0)     3936 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/editElement.js
--rw-r--r--   0 root         (0) root         (0)     6663 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js
--rw-r--r--   0 root         (0) root         (0)    11184 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/editStyleGroups.js
--rw-r--r--   0 root         (0) root         (0)      478 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/index.js
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/metadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     4936 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js
--rw-r--r--   0 root         (0) root         (0)     2588 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/openImage.js
--rw-r--r--   0 root         (0) root         (0)    22740 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/saveAnnotation.js
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.043119 histomicsui-1.4.5.dev8/histomicsui/web_client/models/
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/models/StyleModel.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     3689 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/
--rw-r--r--   0 root         (0) root         (0)    23413 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/AnnotationSelector.js
--rw-r--r--   0 root         (0) root         (0)    43398 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/DrawWidget.js
--rw-r--r--   0 root         (0) root         (0)     1943 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/FrameSelectorWidget.js
--rw-r--r--   0 root         (0) root         (0)    14204 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/MetadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     5170 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/MetadataWidget.js
--rw-r--r--   0 root         (0) root         (0)     8115 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/OverviewWidget.js
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/RegionSelector.js
--rw-r--r--   0 root         (0) root         (0)     9946 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/ZoomWidget.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/panels/index.js
--rw-r--r--   0 root         (0) root         (0)     1485 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/router.js
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/static/
--rwxr-xr-x   0 root         (0) root         (0)     5072 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/static/favicon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.035119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/body/
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/body/configView.styl
--rw-r--r--   0 root         (0) root         (0)     1258 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/body/image.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/dialogs/
--rw-r--r--   0 root         (0) root         (0)      195 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/
--rw-r--r--   0 root         (0) root         (0)      986 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/header.styl
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/headerImage.styl
--rw-r--r--   0 root         (0) root         (0)     1387 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/layout.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
--rw-r--r--   0 root         (0) root         (0)     2651 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
--rw-r--r--   0 root         (0) root         (0)      430 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
--rw-r--r--   0 root         (0) root         (0)      929 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/regionSelector.styl
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.047119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/popover/
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
--rw-r--r--   0 root         (0) root         (0)     1513 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.051119 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/views/
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/views/itemList.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.035119 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.051119 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/body/
--rw-r--r--   0 root         (0) root         (0)     5608 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/body/configView.pug
--rw-r--r--   0 root         (0) root         (0)      783 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/body/image.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.051119 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/confirmDialog.pug
--rw-r--r--   0 root         (0) root         (0)     2079 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/editElement.pug
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
--rw-r--r--   0 root         (0) root         (0)     1541 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      838 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
--rw-r--r--   0 root         (0) root         (0)      353 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/openImage.pug
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.051119 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/
--rw-r--r--   0 root         (0) root         (0)      925 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/header.pug
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug
--rw-r--r--   0 root         (0) root         (0)     1467 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/headerImage.pug
--rw-r--r--   0 root         (0) root         (0)      641 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/headerUser.pug
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/layout.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.051119 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/
--rw-r--r--   0 root         (0) root         (0)     3961 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug
--rw-r--r--   0 root         (0) root         (0)     5685 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/drawWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/metadataWidgetPanel.pug
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/overviewWidget.pug
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/panel.pug
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/regionSelector.pug
--rw-r--r--   0 root         (0) root         (0)     1281 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.055119 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/popover/
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug
--rw-r--r--   0 root         (0) root         (0)      204 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.055119 histomicsui-1.4.5.dev8/histomicsui/web_client/views/
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/HierarchyWidget.js
--rw-r--r--   0 root         (0) root         (0)     2263 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/View.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.055119 histomicsui-1.4.5.dev8/histomicsui/web_client/views/body/
--rw-r--r--   0 root         (0) root         (0)     7205 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/body/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)    68637 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/body/ImageView.js
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/body/index.js
--rw-r--r--   0 root         (0) root         (0)      190 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)     3436 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/itemList.js
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/itemPage.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.055119 histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js
--rw-r--r--   0 root         (0) root         (0)     2861 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderImageView.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderUserView.js
--rw-r--r--   0 root         (0) root         (0)     1621 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderView.js
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.055119 histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/
--rw-r--r--   0 root         (0) root         (0)     4506 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js
--rw-r--r--   0 root         (0) root         (0)    10799 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js
--rw-r--r--   0 root         (0) root         (0)     1231 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js
--rw-r--r--   0 root         (0) root         (0)      176 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/index.js
--rw-r--r--   0 root         (0) root         (0)     2847 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/views/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.035119 histomicsui-1.4.5.dev8/histomicsui/web_client/vue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.055119 histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/
--rw-r--r--   0 root         (0) root         (0)     2650 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue
--rw-r--r--   0 root         (0) root         (0)    12531 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
--rw-r--r--   0 root         (0) root         (0)      745 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/web_client/webpack.helper.js
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/histomicsui/webroot.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.039119 histomicsui-1.4.5.dev8/histomicsui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7025 2023-06-29 14:27:15.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7365 2023-06-29 14:27:16.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:27:15.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-29 14:27:15.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:26:29.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-29 14:27:15.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-29 14:27:15.000000 histomicsui-1.4.5.dev8/histomicsui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-29 14:27:16.059119 histomicsui-1.4.5.dev8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2339 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.059119 histomicsui-1.4.5.dev8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/girder_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.059119 histomicsui-1.4.5.dev8/tests/test_files/
--rw-r--r--   0 root         (0) root         (0)     1286 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_files/.histomicsui_config.yaml
--rw-r--r--   0 root         (0) root         (0)      424 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_files/sample.anot
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_files/sample.meta
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_files/sample_girder_id.anot
--rw-r--r--   0 root         (0) root         (0)     8928 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_files/test_analysis_detection.xml
--rw-r--r--   0 root         (0) root         (0)    12017 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_files/test_analysis_features.xml
--rw-r--r--   0 root         (0) root         (0)     5257 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_handlers.py
--rw-r--r--   0 root         (0) root         (0)    19443 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_hui_rest.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_image_browse_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)    32496 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_tcga.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:27:16.059119 histomicsui-1.4.5.dev8/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     6643 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/analysisSpec.js
--rw-r--r--   0 root         (0) root         (0)    81737 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/annotationSpec.js
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/girderUISpec.js
--rw-r--r--   0 root         (0) root         (0)     4036 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/huiSpec.js
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/huiTest.js
--rw-r--r--   0 root         (0) root         (0)     4393 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/itemSpec.js
--rw-r--r--   0 root         (0) root         (0)     4436 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/metadataPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     6855 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/metadataPlotSpec.js
--rw-r--r--   0 root         (0) root         (0)     6131 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/overviewPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     2996 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/panelLayoutSpec.js
--rw-r--r--   0 root         (0) root         (0)    13991 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tests/web_client_specs/pixelmapCategorySpec.js
--rw-r--r--   0 root         (0) root         (0)     2944 2023-06-29 14:26:17.000000 histomicsui-1.4.5.dev8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.769914 histomicsui-1.4.6.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.741913 histomicsui-1.4.6.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      532 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/.git-blame-ignore-revs
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)    10173 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-07-07 19:25:52.769914 histomicsui-1.4.6.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.745913 histomicsui-1.4.6.dev2/docs/
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/docs/config_options.rst
+-rw-r--r--   0 root         (0) root         (0)     6407 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/docs/controls.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.745913 histomicsui-1.4.6.dev2/docs/images/
+-rwxr-xr-x   0 root         (0) root         (0)   133796 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/docs/images/difference.gif
+-rwxr-xr-x   0 root         (0) root         (0)   133603 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/docs/images/intersect.gif
+-rwxr-xr-x   0 root         (0) root         (0)   154141 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/docs/images/union.gif
+-rwxr-xr-x   0 root         (0) root         (0)   168255 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/docs/images/xor.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.745913 histomicsui-1.4.6.dev2/histomicsui/
+-rw-r--r--   0 root         (0) root         (0)    17663 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.745913 histomicsui-1.4.6.dev2/histomicsui/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/case.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/cohort.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/image.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/meta.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/pathology.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/models/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.749913 histomicsui-1.4.6.dev2/histomicsui/rest/
+-rw-r--r--   0 root         (0) root         (0)      512 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/rest/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     9313 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/rest/hui_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/rest/image_browse_resource.py
+-rw-r--r--   0 root         (0) root         (0)    15298 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/rest/system.py
+-rw-r--r--   0 root         (0) root         (0)    28968 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/rest/tcga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.749913 histomicsui-1.4.6.dev2/histomicsui/web_client/
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.749913 histomicsui-1.4.6.dev2/histomicsui/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/collections/StyleCollection.js
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/collections/UserCollection.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/collections/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.749913 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/confirmDialog.js
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/editElement.js
+-rw-r--r--   0 root         (0) root         (0)     6663 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/editRegionOfInterest.js
+-rw-r--r--   0 root         (0) root         (0)    11184 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/editStyleGroups.js
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/index.js
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/metadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     4936 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/openAnnotatedImage.js
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/openImage.js
+-rw-r--r--   0 root         (0) root         (0)    22740 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/saveAnnotation.js
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.753913 histomicsui-1.4.6.dev2/histomicsui/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/models/StyleModel.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3689 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.753913 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/
+-rw-r--r--   0 root         (0) root         (0)    23881 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/AnnotationSelector.js
+-rw-r--r--   0 root         (0) root         (0)    43398 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/DrawWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/FrameSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)    14204 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/MetadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/MetadataWidget.js
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/OverviewWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/RegionSelector.js
+-rw-r--r--   0 root         (0) root         (0)     9946 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/ZoomWidget.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/panels/index.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/router.js
+-rw-r--r--   0 root         (0) root         (0)      292 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.753913 histomicsui-1.4.6.dev2/histomicsui/web_client/static/
+-rwxr-xr-x   0 root         (0) root         (0)     5072 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/static/favicon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.741913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.753913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/body/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/body/configView.styl
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/body/image.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.753913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.753913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/
+-rw-r--r--   0 root         (0) root         (0)      986 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/header.styl
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/headerImage.styl
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/layout.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.757913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/drawWidget.styl
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      430 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/regionSelector.styl
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.757913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/popover/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.757913 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/views/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/views/itemList.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.741913 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.757913 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/body/
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/body/configView.pug
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/body/image.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.757913 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/confirmDialog.pug
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/editElement.pug
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/openImage.pug
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.757913 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/header.pug
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/headerAnalyses.pug
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/headerImage.pug
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/headerUser.pug
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/layout.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.761913 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/annotationSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/drawWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/drawWidgetElement.pug
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/metadataWidgetPanel.pug
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/overviewWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/regionSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/zoomWidget.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.761913 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/popover/
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/popover/annotationContextMenu.pug
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/popover/annotationPopover.pug
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.761913 histomicsui-1.4.6.dev2/histomicsui/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/View.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.761913 histomicsui-1.4.6.dev2/histomicsui/web_client/views/body/
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/body/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    68637 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/body/ImageView.js
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/body/index.js
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)     3436 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/itemList.js
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/itemPage.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.761913 histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderAnalysesView.js
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderImageView.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderUserView.js
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderView.js
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.761913 histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/AnnotationContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)    10799 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/AnnotationPopover.js
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/PixelmapContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/index.js
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/views/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.741913 histomicsui-1.4.6.dev2/histomicsui/web_client/vue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.765913 histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/ColorPickerInput.vue
+-rw-r--r--   0 root         (0) root         (0)    12531 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/web_client/webpack.helper.js
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/histomicsui/webroot.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.745913 histomicsui-1.4.6.dev2/histomicsui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-07-07 19:25:52.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-07-07 19:25:52.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 19:25:52.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-07 19:25:52.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 19:24:57.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-07 19:25:52.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-07 19:25:52.000000 histomicsui-1.4.6.dev2/histomicsui.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-07 19:25:52.769914 histomicsui-1.4.6.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.765913 histomicsui-1.4.6.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/girder_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.765913 histomicsui-1.4.6.dev2/tests/test_files/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_files/.histomicsui_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_files/sample.anot
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_files/sample.meta
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_files/sample_girder_id.anot
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_files/test_analysis_detection.xml
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_files/test_analysis_features.xml
+-rw-r--r--   0 root         (0) root         (0)     5257 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_handlers.py
+-rw-r--r--   0 root         (0) root         (0)    19443 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_hui_rest.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_image_browse_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)    32496 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_tcga.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:25:52.769914 histomicsui-1.4.6.dev2/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/analysisSpec.js
+-rw-r--r--   0 root         (0) root         (0)    81737 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/annotationSpec.js
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/girderUISpec.js
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/huiSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/huiTest.js
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/itemSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/metadataPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/metadataPlotSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6131 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/overviewPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/panelLayoutSpec.js
+-rw-r--r--   0 root         (0) root         (0)    13991 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tests/web_client_specs/pixelmapCategorySpec.js
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-07-07 19:24:43.000000 histomicsui-1.4.6.dev2/tox.ini
```

### Comparing `histomicsui-1.4.5.dev8/.circleci/config.yml` & `histomicsui-1.4.6.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/.git-blame-ignore-revs` & `histomicsui-1.4.6.dev2/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/.gitignore` & `histomicsui-1.4.6.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/.travis.yml` & `histomicsui-1.4.6.dev2/.travis.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/LICENSE` & `histomicsui-1.4.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/NOTICE` & `histomicsui-1.4.6.dev2/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/PKG-INFO` & `histomicsui-1.4.6.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.5.dev8
+Version: 1.4.6.dev2
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.5.dev8/README.rst` & `histomicsui-1.4.6.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/docs/config_options.rst` & `histomicsui-1.4.6.dev2/docs/config_options.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/docs/controls.rst` & `histomicsui-1.4.6.dev2/docs/controls.rst`

 * *Files 10% similar despite different names*

```diff
@@ -164,7 +164,19 @@
     available options.
 
 - **Pixelmap controls**
 
   **Left-click** on a superpixel to change its category to the current style group.
   Holding **shift** and **left-drag** the mouse to change multiple superpixels as
   the mouse passed over them.
+
+Frame Selector Controls
+-----------------------
+
+- **Channel/band controls**:
+
+  When compositing channels or bands, the visibility of individual channels or
+  bands can be toggled.
+
+  - **ctrl+<number>** toggles the visibility of channels / bands 1 through 10.
+
+  - **alt+ctrl+<number>** toggles the visibility of channels / bands 11 through 20.
```

### Comparing `histomicsui-1.4.5.dev8/docs/images/difference.gif` & `histomicsui-1.4.6.dev2/docs/images/difference.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/docs/images/intersect.gif` & `histomicsui-1.4.6.dev2/docs/images/intersect.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/docs/images/union.gif` & `histomicsui-1.4.6.dev2/docs/images/union.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/docs/images/xor.gif` & `histomicsui-1.4.6.dev2/docs/images/xor.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/__init__.py` & `histomicsui-1.4.6.dev2/histomicsui/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/constants.py` & `histomicsui-1.4.6.dev2/histomicsui/constants.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/handlers.py` & `histomicsui-1.4.6.dev2/histomicsui/handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/aperio.py` & `histomicsui-1.4.6.dev2/histomicsui/models/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/case.py` & `histomicsui-1.4.6.dev2/histomicsui/models/case.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/cohort.py` & `histomicsui-1.4.6.dev2/histomicsui/models/cohort.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/image.py` & `histomicsui-1.4.6.dev2/histomicsui/models/image.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/meta.py` & `histomicsui-1.4.6.dev2/histomicsui/models/meta.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/pathology.py` & `histomicsui-1.4.6.dev2/histomicsui/models/pathology.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/models/slide.py` & `histomicsui-1.4.6.dev2/histomicsui/models/slide.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/rest/__init__.py` & `histomicsui-1.4.6.dev2/histomicsui/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/rest/aperio.py` & `histomicsui-1.4.6.dev2/histomicsui/rest/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/rest/hui_resource.py` & `histomicsui-1.4.6.dev2/histomicsui/rest/hui_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/rest/image_browse_resource.py` & `histomicsui-1.4.6.dev2/histomicsui/rest/image_browse_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/rest/system.py` & `histomicsui-1.4.6.dev2/histomicsui/rest/system.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/rest/tcga.py` & `histomicsui-1.4.6.dev2/histomicsui/rest/tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/app.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/app.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/confirmDialog.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/confirmDialog.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/editElement.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/editElement.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/editRegionOfInterest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/editStyleGroups.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/editStyleGroups.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/metadataPlot.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/metadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/openAnnotatedImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/openImage.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/openImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/dialogs/saveAnnotation.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/dialogs/saveAnnotation.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/main.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/main.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/package.json` & `histomicsui-1.4.6.dev2/histomicsui/web_client/package.json`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/AnnotationSelector.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/AnnotationSelector.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -64,14 +64,16 @@
         this._opacity = settings.opacity || 0.9;
         this._fillOpacity = settings.fillOpacity || 1.0;
         this._showAllAnnotationsState = false;
         this.listenTo(this.collection, 'sync remove update reset change:displayed change:loading', this._debounceRender);
         this.listenTo(this.collection, 'change:highlight', this._changeAnnotationHighlight);
         this.listenTo(eventStream, 'g:event.job_status', _.debounce(this._onJobUpdate, 500));
         this.listenTo(eventStream, 'g:eventStream.start', this._refreshAnnotations);
+        this.listenTo(eventStream, 'g:event.large_image_annotation.create', this._refreshAnnotations);
+        this.listenTo(eventStream, 'g:event.large_image_annotation.remove', this._refreshAnnotations);
         this.listenTo(this.collection, 'change:annotation change:groups', this._saveAnnotation);
         this.listenTo(girderEvents, 'g:login', () => {
             this.collection.reset();
             this._parentId = undefined;
         });
     },
 
@@ -251,14 +253,18 @@
     _onJobUpdate(evt) {
         if (this.parentItem && evt.data.status > 2) {
             this._refreshAnnotations();
         }
     },
 
     _refreshAnnotations() {
+        if (this._norefresh) {
+            delete this._norefresh;
+            return;
+        }
         if (!this.parentItem || !this.parentItem.id || !this.viewer) {
             return;
         }
         // if any annotations are saving, defer this
         if (!this.viewer._saving) {
             this.viewer._saving = {};
         }
@@ -303,14 +309,17 @@
             }
             // remove annotations that are displayed but have been deleted
             Object.keys(models).forEach((id) => {
                 if (!this.collection.get(id) && models[id].get('displayed')) {
                     this._deselectAnnotationElements(models[id]);
                     this.viewer.removeAnnotation(models[id]);
                 }
+                if (activeId === id) {
+                    this.trigger('h:deleteAnnotation', models[id]);
+                }
             });
             return null;
         });
     },
 
     toggleLabels(evt) {
         this._showLabels = !this._showLabels;
@@ -404,14 +413,15 @@
         });
         this.listenToOnce(
             showSaveAnnotationDialog(model, {
                 title: 'Create annotation'
             }),
             'g:submit',
             () => {
+                this._norefresh = true;
                 model.save().done(() => {
                     model.set('displayed', true);
                     this.collection.add(model);
                     this.trigger('h:editAnnotation', model);
                     this._activeAnnotation = model;
                 });
             }
```

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/DrawWidget.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/DrawWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/FrameSelectorWidget.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/FrameSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/MetadataPlot.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/MetadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/MetadataWidget.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/OverviewWidget.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/OverviewWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/RegionSelector.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/RegionSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/panels/ZoomWidget.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/panels/ZoomWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/router.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/router.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/static/favicon.png` & `histomicsui-1.4.6.dev2/histomicsui/web_client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/body/image.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/body/image.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/header.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/header.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/layout/layout.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/annotationSelector.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/drawWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
       display flex
       flex-direction column
       padding 0
 
       &.invisible
         display none
 
+    .icon-keyboard
+      display none
+
   .image-frame-simple-control
     padding 0
 
   label[for="mode"]
     display none
 
   table
```

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/panels/zoomWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl` & `histomicsui-1.4.6.dev2/histomicsui/web_client/stylesheets/popover/annotationPopover.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/body/configView.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/body/configView.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/body/image.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/body/image.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/editElement.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/editElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/editStyleGroups.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/metadataPlot.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/dialogs/saveAnnotation.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/header.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/header.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/headerAnalyses.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/headerImage.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/headerImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/layout/headerUser.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/layout/headerUser.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/annotationSelector.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/drawWidget.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/drawWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/drawWidgetElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/panels/zoomWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/popover/annotationContextMenu.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug` & `histomicsui-1.4.6.dev2/histomicsui/web_client/templates/popover/annotationPopover.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/HierarchyWidget.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/View.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/View.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/body/ConfigView.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/body/ConfigView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/body/ImageView.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/body/ImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/itemList.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/itemList.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/itemPage.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/itemPage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderAnalysesView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderImageView.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/layout/HeaderView.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/AnnotationContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/AnnotationPopover.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/popover/PixelmapContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/views/utils.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue` & `histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/ColorPickerInput.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue` & `histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue` & `histomicsui-1.4.6.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/web_client/webpack.helper.js` & `histomicsui-1.4.6.dev2/histomicsui/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui/webroot.mako` & `histomicsui-1.4.6.dev2/histomicsui/webroot.mako`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/histomicsui.egg-info/PKG-INFO` & `histomicsui-1.4.6.dev2/histomicsui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.5.dev8
+Version: 1.4.6.dev2
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.5.dev8/histomicsui.egg-info/SOURCES.txt` & `histomicsui-1.4.6.dev2/histomicsui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/setup.py` & `histomicsui-1.4.6.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/datastore.py` & `histomicsui-1.4.6.dev2/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/girder_utilities.py` & `histomicsui-1.4.6.dev2/tests/girder_utilities.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_files/.histomicsui_config.yaml` & `histomicsui-1.4.6.dev2/tests/test_files/.histomicsui_config.yaml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_files/test_analysis_detection.xml` & `histomicsui-1.4.6.dev2/tests/test_files/test_analysis_detection.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_files/test_analysis_features.xml` & `histomicsui-1.4.6.dev2/tests/test_files/test_analysis_features.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_handlers.py` & `histomicsui-1.4.6.dev2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_hui_rest.py` & `histomicsui-1.4.6.dev2/tests/test_hui_rest.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_image_browse_endpoints.py` & `histomicsui-1.4.6.dev2/tests/test_image_browse_endpoints.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_tcga.py` & `histomicsui-1.4.6.dev2/tests/test_tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/test_web_client.py` & `histomicsui-1.4.6.dev2/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/analysisSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/analysisSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/annotationSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/annotationSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/girderUISpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/girderUISpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/huiSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/huiSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/huiTest.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/huiTest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/itemSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/itemSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/metadataPanelSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/metadataPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/metadataPlotSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/metadataPlotSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/overviewPanelSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/overviewPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/panelLayoutSpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/panelLayoutSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tests/web_client_specs/pixelmapCategorySpec.js` & `histomicsui-1.4.6.dev2/tests/web_client_specs/pixelmapCategorySpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.5.dev8/tox.ini` & `histomicsui-1.4.6.dev2/tox.ini`

 * *Files identical despite different names*

