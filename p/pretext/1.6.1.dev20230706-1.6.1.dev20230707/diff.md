# Comparing `tmp/pretext-1.6.1.dev20230706.tar.gz` & `tmp/pretext-1.6.1.dev20230707.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230706.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230707.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230706.tar` & `pretext-1.6.1.dev20230707.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/README.md
--rw-r--r--   0        0        0     1962 2023-07-06 06:15:51.809100 pretext-1.6.1.dev20230706/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/build.py
--rw-r--r--   0        0        0    25736 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/core/__init__.py
--rw-r--r--   0        0        0   172498 2023-07-06 06:15:56.773153 pretext-1.6.1.dev20230706/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/core/resources.py
--rw-r--r--   0        0        0  1044737 2023-07-06 06:15:56.773153 pretext-1.6.1.dev20230706/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/generate.py
--rw-r--r--   0        0        0    29108 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/project.py
--rw-r--r--   0        0        0      739 2023-07-06 06:15:20.609075 pretext-1.6.1.dev20230706/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-07-06 06:15:56.837153 pretext-1.6.1.dev20230706/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-07-06 06:15:56.837153 pretext-1.6.1.dev20230706/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-07-06 06:15:56.825153 pretext-1.6.1.dev20230706/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-07-06 06:15:56.813153 pretext-1.6.1.dev20230706/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-07-06 06:15:56.841153 pretext-1.6.1.dev20230706/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    25086 2023-07-06 06:15:20.613075 pretext-1.6.1.dev20230706/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-07-06 06:15:51.809100 pretext-1.6.1.dev20230706/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230706/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-07 06:14:50.977571 pretext-1.6.1.dev20230707/LICENSE
+-rw-r--r--   0        0        0     9757 2023-07-07 06:14:50.977571 pretext-1.6.1.dev20230707/README.md
+-rw-r--r--   0        0        0     1962 2023-07-07 06:15:22.329636 pretext-1.6.1.dev20230707/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-07 06:14:50.977571 pretext-1.6.1.dev20230707/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-07-07 06:14:50.977571 pretext-1.6.1.dev20230707/pretext/build.py
+-rw-r--r--   0        0        0    25736 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172498 2023-07-07 06:15:27.237635 pretext-1.6.1.dev20230707/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/core/resources.py
+-rw-r--r--   0        0        0  1044735 2023-07-07 06:15:27.233635 pretext-1.6.1.dev20230707/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/generate.py
+-rw-r--r--   0        0        0    29108 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-07 06:15:27.305635 pretext-1.6.1.dev20230707/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-07 06:15:27.305635 pretext-1.6.1.dev20230707/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-07-07 06:15:27.301635 pretext-1.6.1.dev20230707/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-07-07 06:15:27.289635 pretext-1.6.1.dev20230707/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-07-07 06:15:27.285635 pretext-1.6.1.dev20230707/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-07-07 06:15:27.305635 pretext-1.6.1.dev20230707/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-07-07 06:15:27.305635 pretext-1.6.1.dev20230707/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-07-07 06:15:27.305635 pretext-1.6.1.dev20230707/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-07-07 06:15:27.305635 pretext-1.6.1.dev20230707/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-07-07 06:15:27.289635 pretext-1.6.1.dev20230707/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    25086 2023-07-07 06:14:50.981571 pretext-1.6.1.dev20230707/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-07-07 06:15:22.329636 pretext-1.6.1.dev20230707/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230707/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230706/LICENSE` & `pretext-1.6.1.dev20230707/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/README.md` & `pretext-1.6.1.dev20230707/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/__init__.py` & `pretext-1.6.1.dev20230707/pretext/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'a6a25b78566917b63f84f1e6974d71105e7d5934'
+CORE_COMMIT = '9322c1f6305e13b4a55d81f9397b1c206ffc6485'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230706/pretext/build.py` & `pretext-1.6.1.dev20230707/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/cli.py` & `pretext-1.6.1.dev20230707/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/codechat.py` & `pretext-1.6.1.dev20230707/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230707/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/core/pretext.py` & `pretext-1.6.1.dev20230707/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/core/resources.py` & `pretext-1.6.1.dev20230707/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/core/resources.zip` & `pretext-1.6.1.dev20230707/pretext/core/resources.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1044737 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/utilities/
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-06 06:15 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-06 06:15 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-06 06:15 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-06 06:15 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-06 06:15 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-06 06:15 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-06 06:15 xsl/README.md
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-06 06:15 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-06 06:15 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-06 06:15 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-06 06:15 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-06 06:15 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-06 06:15 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-06 06:15 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Jul-06 06:15 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-06 06:15 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-06 06:15 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-06 06:15 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-06 06:15 xsl/entities.ent
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-06 06:15 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-06 06:15 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-06 06:15 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Jul-06 06:15 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-06 06:15 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-06 06:15 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   611681 b- defN 23-Jul-06 06:15 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-06 06:15 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-06 06:15 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-06 06:15 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-06 06:15 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-06 06:15 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-06 06:15 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jul-06 06:15 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-06 06:15 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-06 06:15 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx   113893 b- defN 23-Jul-06 06:15 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-06 06:15 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-06 06:15 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx   545213 b- defN 23-Jul-06 06:15 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-06 06:15 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-06 06:15 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-06 06:15 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-06 06:15 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-06 06:15 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-06 06:15 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-06 06:15 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-06 06:15 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-06 06:15 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-06 06:15 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-06 06:15 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-06 06:15 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-06 06:15 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-06 06:15 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-06 06:15 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-06 06:15 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-06 06:15 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-06 06:15 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-06 06:15 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-06 06:15 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-06 06:15 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-06 06:15 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-06 06:15 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-06 06:15 xsl/localizations/fi-FI.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-06 06:15 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-06 06:15 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-06 06:15 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-06 06:15 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-06 06:15 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-06 06:15 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-06 06:15 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-06 06:15 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-06 06:15 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-06 06:15 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-06 06:15 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-06 06:15 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-06 06:15 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-06 06:15 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-06 06:15 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 06:15 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-06 06:15 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-06 06:15 schema/README.md
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-06 06:15 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-06 06:15 schema/pretext-dev.rng
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-06 06:15 schema/xml.xsd
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-06 06:15 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-06 06:15 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-06 06:15 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-06 06:15 schema/build.sh
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-06 06:15 schema/pretext.rnc
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-06 06:15 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-06 06:15 schema/pretext.xsd
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-06 06:15 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 06:15 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-06 06:15 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-06 06:15 pretext/pretext
--rw-r--r--  2.0 unx    36045 b- defN 23-Jul-06 06:15 pretext/braille_format.py
--rw-r--r--  2.0 unx   172498 b- defN 23-Jul-06 06:15 pretext/pretext.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-06 06:15 pretext/pretext.cfg
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-06 06:15 css/colors_default.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-06 06:15 css/pretext_add_on.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-06 06:15 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-06 06:15 css/kindle.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-06 06:15 css/README.md
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-06 06:15 css/epub.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-06 06:15 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-06 06:15 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-06 06:15 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-06 06:15 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-06 06:15 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-06 06:15 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-06 06:15 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_orange_navy.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-06 06:15 css/mathbook-3.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-06 06:15 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-06 06:15 css/setcolors.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-06 06:15 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-06 06:15 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-06 06:15 css/update_css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-06 06:15 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-06 06:15 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-06 06:15 css/colors_red_blue.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-06 06:15 css/colors_maroon_grey.css
-142 files, 4848428 bytes uncompressed, 1027163 bytes compressed:  78.8%
+Zip file size: 1044735 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 xsl/
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jul-07 06:15 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jul-07 06:15 pretext/module-test.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-07 06:15 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172498 b- defN 23-Jul-07 06:15 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jul-07 06:15 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 06:15 pretext/__init__.py
+-rw-r--r--  2.0 unx    36045 b- defN 23-Jul-07 06:15 pretext/braille_format.py
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jul-07 06:15 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-Jul-07 06:15 schema/xml.xsd
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jul-07 06:15 schema/pretext.rnc
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jul-07 06:15 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jul-07 06:15 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jul-07 06:15 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jul-07 06:15 schema/README.md
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jul-07 06:15 schema/pretext.xml
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-07 06:15 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jul-07 06:15 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jul-07 06:15 schema/pretext.rng
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jul-07 06:15 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jul-07 06:15 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_blue_red.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jul-07 06:15 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jul-07 06:15 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jul-07 06:15 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jul-07 06:15 css/style_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jul-07 06:15 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-07 06:15 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-07 06:15 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jul-07 06:15 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jul-07 06:15 css/setcolors.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jul-07 06:15 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jul-07 06:15 css/README.md
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jul-07 06:15 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jul-07 06:15 css/pretext.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jul-07 06:15 css/mathbook-content.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jul-07 06:15 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jul-07 06:15 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jul-07 06:15 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-07 06:15 css/colors_green_blue.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jul-07 06:15 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jul-07 06:15 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jul-07 06:15 css/kindle.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jul-07 06:15 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jul-07 06:15 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jul-07 06:15 xsl/entities.ent
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jul-07 06:15 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-07 06:15 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jul-07 06:15 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jul-07 06:15 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jul-07 06:15 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jul-07 06:15 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   611681 b- defN 23-Jul-07 06:15 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jul-07 06:15 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jul-07 06:15 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jul-07 06:15 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jul-07 06:15 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jul-07 06:15 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Jul-07 06:15 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jul-07 06:15 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jul-07 06:15 xsl/README.md
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jul-07 06:15 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jul-07 06:15 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jul-07 06:15 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jul-07 06:15 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jul-07 06:15 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jul-07 06:15 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx   545237 b- defN 23-Jul-07 06:15 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jul-07 06:15 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Jul-07 06:15 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jul-07 06:15 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jul-07 06:15 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jul-07 06:15 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jul-07 06:15 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jul-07 06:15 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jul-07 06:15 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-07 06:15 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jul-07 06:15 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jul-07 06:15 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jul-07 06:15 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx   113873 b- defN 23-Jul-07 06:15 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jul-07 06:15 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jul-07 06:15 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jul-07 06:15 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jul-07 06:15 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jul-07 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jul-07 06:15 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Jul-07 06:15 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jul-07 06:15 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jul-07 06:15 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jul-07 06:15 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jul-07 06:15 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jul-07 06:15 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 xsl/support/play-button/
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-07 06:15 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jul-07 06:15 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-07 06:15 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jul-07 06:15 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jul-07 06:15 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jul-07 06:15 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jul-07 06:15 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jul-07 06:15 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jul-07 06:15 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-07 06:15 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx    16534 b- defN 23-Jul-07 06:15 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Jul-07 06:15 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    15866 b- defN 23-Jul-07 06:15 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Jul-07 06:15 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Jul-07 06:15 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Jul-07 06:15 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Jul-07 06:15 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Jul-07 06:15 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Jul-07 06:15 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jul-07 06:15 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jul-07 06:15 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    19326 b- defN 23-Jul-07 06:15 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    17231 b- defN 23-Jul-07 06:15 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Jul-07 06:15 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jul-07 06:15 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Jul-07 06:15 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Jul-07 06:15 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Jul-07 06:15 xsl/localizations/af-ZA.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jul-07 06:15 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jul-07 06:15 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 06:15 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-07 06:15 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jul-07 06:15 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jul-07 06:15 script/mjsre/mj-sre-page.js
+142 files, 4848432 bytes uncompressed, 1027161 bytes compressed:  78.8%
```

#### zipnote {}

```diff
@@ -9,419 +9,419 @@
 
 Filename: script/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: xsl/latex/
+Filename: pretext/pretext
 Comment: 
 
-Filename: xsl/localizations/
+Filename: pretext/module-test.py
 Comment: 
 
-Filename: xsl/support/
+Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: xsl/utilities/
+Filename: pretext/pretext.py
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: pretext/README.md
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: pretext/__init__.py
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: xsl/pretext-jupyter.xsl
+Filename: schema/pretext.xsd
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: schema/xml.xsd
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: schema/pretext.rnc
 Comment: 
 
-Filename: xsl/README.md
+Filename: schema/pretext-dev.rnc
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
-Filename: xsl/xml-to-json.xsl
+Filename: schema/pretext-schematron.xsl
 Comment: 
 
-Filename: xsl/extract-mom.xsl
+Filename: schema/README.md
 Comment: 
 
-Filename: xsl/pretext-litprog.xsl
+Filename: schema/pretext.xml
 Comment: 
 
-Filename: xsl/extract-datafile.xsl
+Filename: schema/build.sh
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: schema/pretext-dev.rng
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: css/colors_maroon_grey.css
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: css/colors_default.css
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: xsl/pretext-numbers.xsl
+Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: xsl/pretext-runestone-static.xsl
+Filename: css/style_default.css
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: css/setcolors.css
 Comment: 
 
-Filename: xsl/publisher-variables.xsl
+Filename: css/update_css
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: css/README.md
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: css/colors_blue_green.css
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: css/pretext.css
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: css/mathbook-content.css
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: css/mathbook-3.css
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: css/epub.css
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: xsl/utilities/README.md
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: xsl/utilities/pretext-enhanced-source.xsl
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: xsl/utilities/author-report.xsl
+Filename: css/mathbook-add-on.css
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: css/kindle.css
 Comment: 
 
-Filename: xsl/utilities/deprecate-index.sed
+Filename: xsl/latex/
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
+Filename: xsl/localizations/
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: xsl/support/
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: xsl/utilities/
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/localizations/hu-HU.xml
+Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-FR.xml
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-BR.xml
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: xsl/localizations/bg-BG.xml
+Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: xsl/localizations/ku-CKB.xml
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/localizations/cs-CZ.xml
+Filename: xsl/extract-identity.xsl
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: xsl/localizations/fi-FI.xml
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: xsl/support/play-button/
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/support/README.md
+Filename: xsl/README.md
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: xsl/support/extract-math.xsl
+Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: xsl/support/package-math.xsl
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
-Filename: xsl/support/play-button/README.md
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.png
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.svg
+Filename: xsl/pretext-common.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-chaos.xsl
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-CLP.xsl
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: script/mjsre/
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: script/README.md
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: script/mbx
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: xsl/xml-to-json.xsl
 Comment: 
 
-Filename: schema/README.md
+Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
-Filename: schema/build.sh
+Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: schema/pretext.rnc
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
-Filename: schema/pretext.xsd
+Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: pretext/README.md
+Filename: xsl/support/play-button/
 Comment: 
 
-Filename: pretext/__init__.py
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: pretext/pretext
+Filename: xsl/support/README.md
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: pretext/pretext.py
+Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: pretext/pretext.cfg
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
-Filename: css/colors_default.css
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
-Filename: css/kindle.css
+Filename: xsl/support/play-button/README.md
 Comment: 
 
-Filename: css/README.md
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: css/epub.css
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: css/mathbook-content.css
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
-Filename: css/pretext.css
+Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: css/style_soundwriting.css
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
-Filename: css/mathbook-3.css
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: css/setcolors.css
+Filename: xsl/localizations/ku-CKB.xml
 Comment: 
 
-Filename: css/mathbook-add-on.css
+Filename: xsl/localizations/ca-ES.xml
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: script/mjsre/
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: script/README.md
 Comment: 
 
-Filename: css/update_css
+Filename: script/mbx
 Comment: 
 
-Filename: css/style_default.css
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: script/mjsre/README.md
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
 Zip file comment:
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -1126,15 +1126,15 @@
     <!-- specifications we want to treat them as duplicates.  And we do not        -->
     <!-- write them into the HTML either.  So we make a subset of *unique* blocks. -->
     <xsl:variable name="unique-blocks" select="blocks/block[not(@ref)]"/>
     <div class="ptx-runestone-container">
       <div class="runestone" style="max-width: none;">
         <div data-component="hparsons" class="hparsons_section">
           <xsl:apply-templates select="." mode="runestone-id-attribute"/>
-          <div class="hp_question col-md-12">
+          <div class="hp_question">
             <!-- the prompt -->
             <xsl:apply-templates select="statement"/>
           </div>
           <!-- empty div seems necessary? -->
           <div class="hparsons"/>
           <textarea style="visibility: hidden">
             <!-- A SQL database can be provided for automated  -->
@@ -1751,15 +1751,15 @@
           <div class="runestone explainer ac_section ">
             <div data-component="activecode">
               <xsl:attribute name="id">
                 <xsl:value-of select="$hid"/>
               </xsl:attribute>
               <!-- add some lead-in text to the window -->
               <xsl:if test="$exercise-statement">
-                <div class="ac_question col-md-12">
+                <div class="ac_question">
                   <xsl:attribute name="id">
                     <xsl:value-of select="concat($hid, '_question')"/>
                   </xsl:attribute>
                   <xsl:apply-templates select="$exercise-statement"/>
                 </div>
               </xsl:if>
               <textarea data-lang="{$active-language}" data-timelimit="25000" data-audio="" data-coach="true" style="visibility: hidden;">
```

#### xsl/pretext-latex.xsl

##### xsl/pretext-latex.xsl

```diff
@@ -9973,15 +9973,15 @@
   <!-- inside a  biblio/note  was being caught here and        -->
   <!-- producing a \footnotemark{}.  However, there was no     -->
   <!-- matching  \footnotetext  since "biblio" is not yet a    -->
   <!-- tcolorbox and the "pop-footnote-text" template was not  -->
   <!-- present as part of processing  biblio/note.             -->
   <xsl:template match="fn">
     <xsl:choose>
-      <xsl:when test="ancestor::*[ or  or   or  or  or  or  or  or  or  or self::tabular or self::commentary or self::list or self::sidebyside or self::gi or self::colophon/parent::backmatter or self::assemblage or self::exercise or (self::li and parent::dl)] and not(ancestor::note/parent::biblio)">
+      <xsl:when test="ancestor::*[ or  or   or  or  or  or  or  or  or  or  or self::tabular or self::commentary or self::list or self::sidebyside or self::gi or self::colophon/parent::backmatter or self::assemblage or self::exercise or (self::li and parent::dl)] and not(ancestor::note/parent::biblio)">
         <!-- a footnote in the text of a caption will migrate to -->
         <!-- the auxiliary file for use in the "list of figures" -->
         <!-- and there is some confusion of braces and the use   -->
         <!-- of \footnote and \footnotemark, hence a \protect    -->
         <!-- https://tex.stackexchange.com/questions/10181       -->
         <xsl:if test="ancestor::*[]">
           <xsl:text>\protect</xsl:text>
```

### Comparing `pretext-1.6.1.dev20230706/pretext/generate.py` & `pretext-1.6.1.dev20230707/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/project.py` & `pretext-1.6.1.dev20230707/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230707/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230707/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230707/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-06 06:15 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-06 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-06 06:15 assets/frog.jpg
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-06 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-06 06:15 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-06 06:15 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-06 06:15 source/section-1.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-07 06:15 .gitignore
+-rw-r--r--  2.0 unx       86 b- defN 23-Jul-07 06:14 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-07 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-07 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-07 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-07 06:14 source/section-2.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-07 06:14 source/section-1.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-07 06:14 source/main.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-07 06:14 assets/frog.jpg
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-07 06:15 .devcontainer/devcontainer.json
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

#### zipnote {}

```diff
@@ -6,38 +6,38 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
-Comment: 
-
-Filename: assets/frog.jpg
+Filename: publication/publication.ptx
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/section-2.ptx
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: source/section-1.ptx
 Comment: 
 
-Filename: source/section-2.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: assets/frog.jpg
 Comment: 
 
-Filename: source/section-1.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230707/pretext/templates/resources/book.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-06 06:15 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-06 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-06 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-06 06:15 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-07 06:15 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-07 06:14 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-07 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-07 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jul-07 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jul-07 06:14 source/main.ptx
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-07 06:15 .devcontainer/devcontainer.json
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
-Comment: 
-
-Filename: .devcontainer/devcontainer.json
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230707/pretext/templates/resources/demo.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-06 06:15 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-06 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-06 06:15 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-06 06:15 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-06 06:15 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/images/
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-06 06:15 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-06 06:15 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-06 06:15 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-06 06:15 source/ch-empty.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-06 06:15 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-06 06:15 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-06 06:15 source/docinfo.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jul-06 06:15 source/main.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-06 06:15 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-06 06:15 source/frontmatter.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-06 06:15 source/ch-generate.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-06 06:15 source/ch-features.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-06 06:15 source/ex-first.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-06 06:15 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-06 06:15 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-06 06:15 source/sec-features.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-06 06:15 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-06 06:15 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-06 06:15 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 06:15 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-07 06:15 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-07 06:14 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-07 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-07 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jul-07 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jul-07 06:14 source/ex-first.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-07 06:14 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jul-07 06:14 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jul-07 06:14 source/sec-features.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-07 06:14 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jul-07 06:14 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-07 06:14 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jul-07 06:14 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jul-07 06:14 source/backmatter.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jul-07 06:14 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-07 06:14 source/ch-features.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jul-07 06:14 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jul-07 06:14 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jul-07 06:14 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-07 06:14 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jul-07 06:14 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-07 06:14 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-07 06:14 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-07 06:14 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jul-07 06:14 source/images/tikz.tex
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-07 06:14 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jul-07 06:14 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-07 06:15 .devcontainer/devcontainer.json
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

#### zipnote {}

```diff
@@ -6,98 +6,98 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
-Comment: 
-
-Filename: assets/jsxgraph/
+Filename: publication/publication.ptx
 Comment: 
 
-Filename: assets/frog.jpg
+Filename: source/images/
 Comment: 
 
-Filename: assets/jsxgraph/infinity.js
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/ch-generate.ptx
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
-Filename: source/images/
+Filename: source/sec-features.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/ch-empty.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/sec-first-intro.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/ch-empty.ptx
+Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/fig-tikz.ptx
+Filename: source/backmatter.ptx
 Comment: 
 
-Filename: source/fig-sage3d.ptx
+Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/docinfo.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
-Filename: source/fig-sage2d.ptx
+Filename: source/fig-tikz.ptx
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/ch-generate.ptx
+Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/ch-features.ptx
+Filename: source/docinfo.ptx
 Comment: 
 
-Filename: source/ex-first.ptx
+Filename: source/images/sageplot2d.sage
 Comment: 
 
-Filename: source/sec-first-examples.ptx
+Filename: source/images/cflag.asy
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/images/sageplot3d.sage
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/images/tikz.tex
 Comment: 
 
-Filename: source/images/cflag.asy
+Filename: assets/jsxgraph/
 Comment: 
 
-Filename: source/images/sageplot3d.sage
+Filename: assets/frog.jpg
 Comment: 
 
-Filename: source/images/tikz.tex
+Filename: assets/jsxgraph/infinity.js
 Comment: 
 
-Filename: source/images/sageplot2d.sage
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230707/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230707/pretext/templates/resources/hello.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-06 06:15 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-06 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-06 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-06 06:15 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-07 06:15 .gitignore
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-07 06:14 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jul-07 06:14 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-07 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-07 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-07 06:14 source/main.ptx
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-07 06:15 .devcontainer/devcontainer.json
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: README.md
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
-Comment: 
-
-Filename: .devcontainer/devcontainer.json
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230707/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230707/pretext/templates/resources/slideshow.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-06 06:15 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-06 06:15 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-06 06:15 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-06 06:15 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-06 06:15 xsl/slides.xsl
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-06 06:15 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-06 06:15 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-06 06:15 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 06:14 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-07 06:15 .gitignore
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-07 06:14 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-07 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jul-07 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jul-07 06:14 source/main.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-07 06:14 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-07 06:15 .devcontainer/devcontainer.json
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

#### zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: source/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: project.ptx
+Filename: .gitignore
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: xsl/slides.xsl
+Filename: publication/publication.ptx
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/main.ptx
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: xsl/slides.xsl
 Comment: 
 
-Filename: source/main.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230706/pretext/utils.py` & `pretext-1.6.1.dev20230707/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230706/pyproject.toml` & `pretext-1.6.1.dev20230707/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230706"
+version = "1.6.1.dev20230707"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230706/PKG-INFO` & `pretext-1.6.1.dev20230707/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230706
+Version: 1.6.1.dev20230707
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

