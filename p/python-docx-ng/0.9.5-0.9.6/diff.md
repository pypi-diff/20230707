# Comparing `tmp/python_docx_ng-0.9.5.tar.gz` & `tmp/python_docx_ng-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_docx_ng-0.9.5.tar", max compression
+gzip compressed data, was "python_docx_ng-0.9.6.tar", max compression
```

## Comparing `python_docx_ng-0.9.5.tar` & `python_docx_ng-0.9.6.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1150 2023-07-07 08:15:07.093121 python_docx_ng-0.9.5/LICENSE
--rw-r--r--   0        0        0     5089 2023-07-07 08:15:07.097121 python_docx_ng-0.9.5/README.md
--rw-r--r--   0        0        0     1945 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/__init__.py
--rw-r--r--   0        0        0     1754 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/api.py
--rw-r--r--   0        0        0     2959 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/blkcntnr.py
--rw-r--r--   0        0        0     1043 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/compat.py
--rw-r--r--   0        0        0        0 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/dml/__init__.py
--rw-r--r--   0        0        0     3978 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/dml/color.py
--rw-r--r--   0        0        0     8610 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/document.py
--rw-r--r--   0        0        0      343 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/enum/__init__.py
--rw-r--r--   0        0        0    11080 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/enum/base.py
--rw-r--r--   0        0        0     3533 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/enum/dml.py
--rw-r--r--   0        0        0     2666 2023-07-07 08:15:07.101121 python_docx_ng-0.9.5/docx/enum/section.py
--rw-r--r--   0        0        0      475 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/enum/shape.py
--rw-r--r--   0        0        0    12189 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/enum/style.py
--rw-r--r--   0        0        0     3929 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/enum/table.py
--rw-r--r--   0        0        0    10689 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/enum/text.py
--rw-r--r--   0        0        0      503 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/exceptions.py
--rw-r--r--   0        0        0     1002 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/bmp.py
--rw-r--r--   0        0        0     3541 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/constants.py
--rw-r--r--   0        0        0     2010 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/emf.py
--rw-r--r--   0        0        0      432 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/exceptions.py
--rw-r--r--   0        0        0     1260 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/gif.py
--rw-r--r--   0        0        0     3286 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/helpers.py
--rw-r--r--   0        0        0     8029 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/image.py
--rw-r--r--   0        0        0    16099 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/jpeg.py
--rw-r--r--   0        0        0     8789 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/png.py
--rw-r--r--   0        0        0     1296 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/svg.py
--rw-r--r--   0        0        0    11140 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/tiff.py
--rw-r--r--   0        0        0     1516 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/image/wmf.py
--rw-r--r--   0        0        0        0 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/compat.py
--rw-r--r--   0        0        0    20400 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/constants.py
--rw-r--r--   0        0        0     3246 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/coreprops.py
--rw-r--r--   0        0        0      302 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/exceptions.py
--rw-r--r--   0        0        0     2429 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/extendedprops.py
--rw-r--r--   0        0        0     8540 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/oxml.py
--rw-r--r--   0        0        0    10293 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/package.py
--rw-r--r--   0        0        0     3880 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/packuri.py
--rw-r--r--   0        0        0     8157 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/part.py
--rw-r--r--   0        0        0        0 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/parts/__init__.py
--rw-r--r--   0        0        0     1664 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/parts/coreprops.py
--rw-r--r--   0        0        0     1588 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/parts/extendedprops.py
--rw-r--r--   0        0        0     4452 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/phys_pkg.py
--rw-r--r--   0        0        0    10107 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/pkgreader.py
--rw-r--r--   0        0        0     4601 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/pkgwriter.py
--rw-r--r--   0        0        0     5415 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/rel.py
--rw-r--r--   0        0        0     1453 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/shared.py
--rw-r--r--   0        0        0      716 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/opc/spec.py
--rw-r--r--   0        0        0    13177 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/__init__.py
--rw-r--r--   0        0        0     3292 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/comment.py
--rw-r--r--   0        0        0    10278 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/coreprops.py
--rw-r--r--   0        0        0     2769 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/document.py
--rw-r--r--   0        0        0      290 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/exceptions.py
--rw-r--r--   0        0        0     5934 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/extendedprops.py
--rw-r--r--   0        0        0     2207 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/footnote.py
--rw-r--r--   0        0        0     4017 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/ns.py
--rw-r--r--   0        0        0     5181 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/numbering.py
--rw-r--r--   0        0        0    11114 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/section.py
--rw-r--r--   0        0        0     3491 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/settings.py
--rw-r--r--   0        0        0     9131 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/shape.py
--rw-r--r--   0        0        0     1623 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/shared.py
--rw-r--r--   0        0        0    14160 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/simpletypes.py
--rw-r--r--   0        0        0    11670 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/styles.py
--rw-r--r--   0        0        0    33584 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/table.py
--rw-r--r--   0        0        0        0 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/text/__init__.py
--rw-r--r--   0        0        0    12707 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/text/font.py
--rw-r--r--   0        0        0     2839 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/text/form.py
--rw-r--r--   0        0        0     3832 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/text/paragraph.py
--rw-r--r--   0        0        0    12405 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/text/parfmt.py
--rw-r--r--   0        0        0     7894 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/text/run.py
--rw-r--r--   0        0        0    24857 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/oxml/xmlchemy.py
--rw-r--r--   0        0        0     3868 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/package.py
--rw-r--r--   0        0        0        0 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/__init__.py
--rw-r--r--   0        0        0     1285 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/altchunk.py
--rw-r--r--   0        0        0      812 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/comment.py
--rw-r--r--   0        0        0     5646 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/document.py
--rw-r--r--   0        0        0      820 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/footnote.py
--rw-r--r--   0        0        0     1717 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/hdrftr.py
--rw-r--r--   0        0        0     2668 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/image.py
--rw-r--r--   0        0        0     1230 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/numbering.py
--rw-r--r--   0        0        0     1465 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/settings.py
--rw-r--r--   0        0        0     3282 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/story.py
--rw-r--r--   0        0        0     1428 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/parts/styles.py
--rw-r--r--   0        0        0    17290 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/section.py
--rw-r--r--   0        0        0      780 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/settings.py
--rw-r--r--   0        0        0     2811 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/shape.py
--rw-r--r--   0        0        0     6791 2023-07-07 08:15:07.105121 python_docx_ng-0.9.5/docx/shared.py
--rw-r--r--   0        0        0     1500 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/styles/__init__.py
--rw-r--r--   0        0        0     7549 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/styles/latent.py
--rw-r--r--   0        0        0     7987 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/styles/style.py
--rw-r--r--   0        0        0     5766 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/styles/styles.py
--rw-r--r--   0        0        0    21294 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/table.py
--rw-r--r--   0        0        0     1427 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-comments.xml
--rw-r--r--   0        0        0     1444 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/[Content_Types].xml
--rw-r--r--   0        0        0      589 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/_rels/.rels
--rw-r--r--   0        0        0      300 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
--rw-r--r--   0        0        0      262 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/customXml/item1.xml
--rw-r--r--   0        0        0      354 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/customXml/itemProps1.xml
--rw-r--r--   0        0        0      708 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/docProps/app.xml
--rw-r--r--   0        0        0      726 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/docProps/core.xml
--rw-r--r--   0        0        0     8324 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/docProps/thumbnail.jpeg
--rw-r--r--   0        0        0      949 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/_rels/document.xml.rels
--rw-r--r--   0        0        0     2869 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/document.xml
--rw-r--r--   0        0        0     2722 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/fontTable.xml
--rw-r--r--   0        0        0    15657 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/numbering.xml
--rw-r--r--   0        0        0     3667 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/settings.xml
--rw-r--r--   0        0        0    44248 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/styles.xml
--rw-r--r--   0        0        0   438131 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/stylesWithEffects.xml
--rw-r--r--   0        0        0     8392 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/theme/theme1.xml
--rw-r--r--   0        0        0      893 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-docx-template/word/webSettings.xml
--rw-r--r--   0        0        0     1395 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-footer.xml
--rw-r--r--   0        0        0     1905 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-footnotes.xml
--rw-r--r--   0        0        0     1395 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-header.xml
--rw-r--r--   0        0        0     1640 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-settings.xml
--rw-r--r--   0        0        0    32959 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default-styles.xml
--rw-r--r--   0        0        0    15636 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/templates/default.docx
--rw-r--r--   0        0        0        0 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/__init__.py
--rw-r--r--   0        0        0      527 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/comment.py
--rw-r--r--   0        0        0    13134 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/font.py
--rw-r--r--   0        0        0     7694 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/paragraph.py
--rw-r--r--   0        0        0    11643 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/parfmt.py
--rw-r--r--   0        0        0    10597 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/run.py
--rw-r--r--   0        0        0     4183 2023-07-07 08:15:07.109121 python_docx_ng-0.9.5/docx/text/tabstops.py
--rw-r--r--   0        0        0      730 2023-07-07 08:15:07.133122 python_docx_ng-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 python_docx_ng-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1150 2023-07-07 09:27:17.881949 python_docx_ng-0.9.6/LICENSE
+-rw-r--r--   0        0        0     5382 2023-07-07 09:27:17.881949 python_docx_ng-0.9.6/README.md
+-rw-r--r--   0        0        0     1946 2023-07-07 09:27:17.885949 python_docx_ng-0.9.6/docx/__init__.py
+-rw-r--r--   0        0        0     1754 2023-07-07 09:27:17.885949 python_docx_ng-0.9.6/docx/api.py
+-rw-r--r--   0        0        0     2959 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/blkcntnr.py
+-rw-r--r--   0        0        0     1043 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/compat.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/dml/__init__.py
+-rw-r--r--   0        0        0     3978 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/dml/color.py
+-rw-r--r--   0        0        0     8610 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/document.py
+-rw-r--r--   0        0        0      343 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/__init__.py
+-rw-r--r--   0        0        0    11080 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/base.py
+-rw-r--r--   0        0        0     3533 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/dml.py
+-rw-r--r--   0        0        0     2666 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/section.py
+-rw-r--r--   0        0        0      475 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/shape.py
+-rw-r--r--   0        0        0    12189 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/style.py
+-rw-r--r--   0        0        0     3929 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/table.py
+-rw-r--r--   0        0        0    10689 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/enum/text.py
+-rw-r--r--   0        0        0      503 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/exceptions.py
+-rw-r--r--   0        0        0     1002 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/__init__.py
+-rw-r--r--   0        0        0     1512 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/bmp.py
+-rw-r--r--   0        0        0     3541 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/constants.py
+-rw-r--r--   0        0        0     2010 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/emf.py
+-rw-r--r--   0        0        0      432 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/exceptions.py
+-rw-r--r--   0        0        0     1260 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/gif.py
+-rw-r--r--   0        0        0     3286 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/helpers.py
+-rw-r--r--   0        0        0     8029 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/image.py
+-rw-r--r--   0        0        0    16099 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/jpeg.py
+-rw-r--r--   0        0        0     8789 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/png.py
+-rw-r--r--   0        0        0     1296 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/svg.py
+-rw-r--r--   0        0        0    11140 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/tiff.py
+-rw-r--r--   0        0        0     1516 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/image/wmf.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/compat.py
+-rw-r--r--   0        0        0    20400 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/constants.py
+-rw-r--r--   0        0        0     3246 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/coreprops.py
+-rw-r--r--   0        0        0      302 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/exceptions.py
+-rw-r--r--   0        0        0     2429 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/extendedprops.py
+-rw-r--r--   0        0        0     8540 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/oxml.py
+-rw-r--r--   0        0        0    10293 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/package.py
+-rw-r--r--   0        0        0     3880 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/packuri.py
+-rw-r--r--   0        0        0     8157 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/part.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/parts/__init__.py
+-rw-r--r--   0        0        0     1664 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/parts/coreprops.py
+-rw-r--r--   0        0        0     1588 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/parts/extendedprops.py
+-rw-r--r--   0        0        0     4452 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/phys_pkg.py
+-rw-r--r--   0        0        0    10107 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/pkgreader.py
+-rw-r--r--   0        0        0     4601 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/pkgwriter.py
+-rw-r--r--   0        0        0     5415 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/rel.py
+-rw-r--r--   0        0        0     1453 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/shared.py
+-rw-r--r--   0        0        0      716 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/opc/spec.py
+-rw-r--r--   0        0        0    13177 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/__init__.py
+-rw-r--r--   0        0        0     3292 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/comment.py
+-rw-r--r--   0        0        0    10278 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/coreprops.py
+-rw-r--r--   0        0        0     2769 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/document.py
+-rw-r--r--   0        0        0      290 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/exceptions.py
+-rw-r--r--   0        0        0     5934 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/extendedprops.py
+-rw-r--r--   0        0        0     2207 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/footnote.py
+-rw-r--r--   0        0        0     4017 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/ns.py
+-rw-r--r--   0        0        0     5181 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/numbering.py
+-rw-r--r--   0        0        0    11114 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/section.py
+-rw-r--r--   0        0        0     3491 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/settings.py
+-rw-r--r--   0        0        0     9131 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/shape.py
+-rw-r--r--   0        0        0     1623 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/shared.py
+-rw-r--r--   0        0        0    14160 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/simpletypes.py
+-rw-r--r--   0        0        0    11670 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/styles.py
+-rw-r--r--   0        0        0    33584 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/table.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/text/__init__.py
+-rw-r--r--   0        0        0    12707 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/text/font.py
+-rw-r--r--   0        0        0     2839 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/text/form.py
+-rw-r--r--   0        0        0     3832 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/text/paragraph.py
+-rw-r--r--   0        0        0    12405 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/text/parfmt.py
+-rw-r--r--   0        0        0     7894 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/text/run.py
+-rw-r--r--   0        0        0    24857 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/oxml/xmlchemy.py
+-rw-r--r--   0        0        0     3868 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/package.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/parts/__init__.py
+-rw-r--r--   0        0        0     1285 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/parts/altchunk.py
+-rw-r--r--   0        0        0      812 2023-07-07 09:27:17.889948 python_docx_ng-0.9.6/docx/parts/comment.py
+-rw-r--r--   0        0        0     5646 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/document.py
+-rw-r--r--   0        0        0      820 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/footnote.py
+-rw-r--r--   0        0        0     1717 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/hdrftr.py
+-rw-r--r--   0        0        0     2668 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/image.py
+-rw-r--r--   0        0        0     1230 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/numbering.py
+-rw-r--r--   0        0        0     1465 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/settings.py
+-rw-r--r--   0        0        0     3282 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/story.py
+-rw-r--r--   0        0        0     1428 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/parts/styles.py
+-rw-r--r--   0        0        0    17290 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/section.py
+-rw-r--r--   0        0        0      780 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/settings.py
+-rw-r--r--   0        0        0     2811 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/shape.py
+-rw-r--r--   0        0        0     6791 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/shared.py
+-rw-r--r--   0        0        0     1500 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/styles/__init__.py
+-rw-r--r--   0        0        0     7549 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/styles/latent.py
+-rw-r--r--   0        0        0     7987 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/styles/style.py
+-rw-r--r--   0        0        0     5766 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/styles/styles.py
+-rw-r--r--   0        0        0    21294 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/table.py
+-rw-r--r--   0        0        0     1427 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-comments.xml
+-rw-r--r--   0        0        0     1444 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/[Content_Types].xml
+-rw-r--r--   0        0        0      589 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/_rels/.rels
+-rw-r--r--   0        0        0      300 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
+-rw-r--r--   0        0        0      262 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/customXml/item1.xml
+-rw-r--r--   0        0        0      354 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/customXml/itemProps1.xml
+-rw-r--r--   0        0        0      708 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/docProps/app.xml
+-rw-r--r--   0        0        0      726 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/docProps/core.xml
+-rw-r--r--   0        0        0     8324 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/docProps/thumbnail.jpeg
+-rw-r--r--   0        0        0      949 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/_rels/document.xml.rels
+-rw-r--r--   0        0        0     2869 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/document.xml
+-rw-r--r--   0        0        0     2722 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/fontTable.xml
+-rw-r--r--   0        0        0    15657 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/numbering.xml
+-rw-r--r--   0        0        0     3667 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/settings.xml
+-rw-r--r--   0        0        0    44248 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/styles.xml
+-rw-r--r--   0        0        0   438131 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/stylesWithEffects.xml
+-rw-r--r--   0        0        0     8392 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/theme/theme1.xml
+-rw-r--r--   0        0        0      893 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-docx-template/word/webSettings.xml
+-rw-r--r--   0        0        0     1395 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-footer.xml
+-rw-r--r--   0        0        0     1905 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-footnotes.xml
+-rw-r--r--   0        0        0     1395 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-header.xml
+-rw-r--r--   0        0        0     1640 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-settings.xml
+-rw-r--r--   0        0        0    32959 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default-styles.xml
+-rw-r--r--   0        0        0    15636 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/templates/default.docx
+-rw-r--r--   0        0        0        0 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/__init__.py
+-rw-r--r--   0        0        0      527 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/comment.py
+-rw-r--r--   0        0        0    13134 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/font.py
+-rw-r--r--   0        0        0     7694 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/paragraph.py
+-rw-r--r--   0        0        0    11643 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/parfmt.py
+-rw-r--r--   0        0        0    10715 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/run.py
+-rw-r--r--   0        0        0     4183 2023-07-07 09:27:17.893948 python_docx_ng-0.9.6/docx/text/tabstops.py
+-rw-r--r--   0        0        0      862 2023-07-07 09:27:17.921948 python_docx_ng-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     6018 1970-01-01 00:00:00.000000 python_docx_ng-0.9.6/PKG-INFO
```

### Comparing `python_docx_ng-0.9.5/LICENSE` & `python_docx_ng-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/README.md` & `python_docx_ng-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,41 @@
+Metadata-Version: 2.1
+Name: python-docx-ng
+Version: 0.9.6
+Summary: python-docx-ng is a Python library for creating and updating Microsoft Word (.docx) files.
+License: MIT
+Author: toxicphreAK
+Author-email: pentesting.laboratories@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: behave (>=1.2.6,<2.0.0)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Description-Content-Type: text/markdown
+
 # python-docx-ng
 
 [![Python Packaging](https://github.com/toxicphreAK/python-docx-ng/actions/workflows/python-publish.yml/badge.svg)](https://github.com/toxicphreAK/python-docx-ng/actions/workflows/python-publish.yml)
 
 *python-docx-ng* is a Python library for creating and updating Microsoft Word (.docx) files.
 It was originally designed and developed by [scanny](https://github.com/scanny) as [python-docx](https://github.com/python-openxml/python-docx).
 As he is not actively developing his repo and there are soo many useful pull requests, bringing together a more powerful tool.
 This repo should merge a lot of those things and create a more powerful version, hopefully bearing the original structure of scanny in mind.
 
-A new documentation section will be build up soon based on Markdown in the [docs](docs) section.
-Examples can be found here: [examples](docs/examples)
+A new documentation section will be build up soon based on Markdown in the [https://github.com/toxicphreAK/python-docx-ng/blob/master/docs](docs) section.
+Examples can be found here: [examples](https://github.com/toxicphreAK/python-docx-ng/blob/master/docs/examples)
 Older information is available in the [python-docx Documentation](https://python-docx.readthedocs.org/en/latest/).
 
+Repo: https://github.com/toxicphreAK/python-docx-ng/blob/master/
+Release: https://github.com/toxicphreAK/python-docx-ng/releases
+PyPi: https://pypi.org/project/python-docx-ng/
+
 ## Installation
 
 ```commandline
 pip install python-docx-ng
 ```
 
 > Hint: The library is called `docx` in python scripts, so use imports like `import docx`. 
@@ -59,7 +80,8 @@
       + [ ] specify table location (not at end of document) - https://github.com/python-openxml/python-docx/issues/1204
       + [ ] read information from activex elements - https://github.com/python-openxml/python-docx/issues/1197
       + [ ] begin new list numbering - https://github.com/python-openxml/python-docx/issues/1194
   + [ ] Search on stackoverflow and document solutions
 + [ ] Remove code references to original repo of python-docx
 + [ ] Setup new docs (markdown based)
 + [ ] Add missing tests
+
```

### Comparing `python_docx_ng-0.9.5/docx/__init__.py` & `python_docx_ng-0.9.6/docx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 
 from docx.api import Document  # noqa
 
-__version__ = "0.9.5"
+__version__ = "0.9.6s"
 
 
 # register custom Part classes with opc package reader
 
 from docx.opc.constants import CONTENT_TYPE as CT, RELATIONSHIP_TYPE as RT
 from docx.opc.part import PartFactory
 from docx.opc.parts.coreprops import CorePropertiesPart
```

### Comparing `python_docx_ng-0.9.5/docx/api.py` & `python_docx_ng-0.9.6/docx/api.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/blkcntnr.py` & `python_docx_ng-0.9.6/docx/blkcntnr.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/compat.py` & `python_docx_ng-0.9.6/docx/compat.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/dml/color.py` & `python_docx_ng-0.9.6/docx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/document.py` & `python_docx_ng-0.9.6/docx/document.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/enum/base.py` & `python_docx_ng-0.9.6/docx/enum/base.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/enum/dml.py` & `python_docx_ng-0.9.6/docx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/enum/section.py` & `python_docx_ng-0.9.6/docx/enum/section.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/enum/style.py` & `python_docx_ng-0.9.6/docx/enum/style.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/enum/table.py` & `python_docx_ng-0.9.6/docx/enum/table.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/enum/text.py` & `python_docx_ng-0.9.6/docx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/__init__.py` & `python_docx_ng-0.9.6/docx/image/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/bmp.py` & `python_docx_ng-0.9.6/docx/image/bmp.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/constants.py` & `python_docx_ng-0.9.6/docx/image/constants.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/emf.py` & `python_docx_ng-0.9.6/docx/image/emf.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/gif.py` & `python_docx_ng-0.9.6/docx/image/gif.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/helpers.py` & `python_docx_ng-0.9.6/docx/image/helpers.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/image.py` & `python_docx_ng-0.9.6/docx/image/image.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/jpeg.py` & `python_docx_ng-0.9.6/docx/image/jpeg.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/png.py` & `python_docx_ng-0.9.6/docx/image/png.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/svg.py` & `python_docx_ng-0.9.6/docx/image/svg.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/tiff.py` & `python_docx_ng-0.9.6/docx/image/tiff.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/image/wmf.py` & `python_docx_ng-0.9.6/docx/image/wmf.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/compat.py` & `python_docx_ng-0.9.6/docx/opc/compat.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/constants.py` & `python_docx_ng-0.9.6/docx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/coreprops.py` & `python_docx_ng-0.9.6/docx/opc/coreprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/extendedprops.py` & `python_docx_ng-0.9.6/docx/opc/extendedprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/oxml.py` & `python_docx_ng-0.9.6/docx/opc/oxml.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/package.py` & `python_docx_ng-0.9.6/docx/opc/package.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/packuri.py` & `python_docx_ng-0.9.6/docx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/part.py` & `python_docx_ng-0.9.6/docx/opc/part.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/parts/coreprops.py` & `python_docx_ng-0.9.6/docx/opc/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/parts/extendedprops.py` & `python_docx_ng-0.9.6/docx/opc/parts/extendedprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/phys_pkg.py` & `python_docx_ng-0.9.6/docx/opc/phys_pkg.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/pkgreader.py` & `python_docx_ng-0.9.6/docx/opc/pkgreader.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/pkgwriter.py` & `python_docx_ng-0.9.6/docx/opc/pkgwriter.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/rel.py` & `python_docx_ng-0.9.6/docx/opc/rel.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/shared.py` & `python_docx_ng-0.9.6/docx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/opc/spec.py` & `python_docx_ng-0.9.6/docx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/__init__.py` & `python_docx_ng-0.9.6/docx/oxml/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/comment.py` & `python_docx_ng-0.9.6/docx/oxml/comment.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/coreprops.py` & `python_docx_ng-0.9.6/docx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/document.py` & `python_docx_ng-0.9.6/docx/oxml/document.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/extendedprops.py` & `python_docx_ng-0.9.6/docx/oxml/extendedprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/footnote.py` & `python_docx_ng-0.9.6/docx/oxml/footnote.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/ns.py` & `python_docx_ng-0.9.6/docx/oxml/ns.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/numbering.py` & `python_docx_ng-0.9.6/docx/oxml/numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/section.py` & `python_docx_ng-0.9.6/docx/oxml/section.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/settings.py` & `python_docx_ng-0.9.6/docx/oxml/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/shape.py` & `python_docx_ng-0.9.6/docx/oxml/shape.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/shared.py` & `python_docx_ng-0.9.6/docx/oxml/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/simpletypes.py` & `python_docx_ng-0.9.6/docx/oxml/simpletypes.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/styles.py` & `python_docx_ng-0.9.6/docx/oxml/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/table.py` & `python_docx_ng-0.9.6/docx/oxml/table.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/text/font.py` & `python_docx_ng-0.9.6/docx/oxml/text/font.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/text/form.py` & `python_docx_ng-0.9.6/docx/oxml/text/form.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/text/paragraph.py` & `python_docx_ng-0.9.6/docx/oxml/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/text/parfmt.py` & `python_docx_ng-0.9.6/docx/oxml/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/text/run.py` & `python_docx_ng-0.9.6/docx/oxml/text/run.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/oxml/xmlchemy.py` & `python_docx_ng-0.9.6/docx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/package.py` & `python_docx_ng-0.9.6/docx/package.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/altchunk.py` & `python_docx_ng-0.9.6/docx/parts/altchunk.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/comment.py` & `python_docx_ng-0.9.6/docx/parts/comment.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/document.py` & `python_docx_ng-0.9.6/docx/parts/document.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/footnote.py` & `python_docx_ng-0.9.6/docx/parts/footnote.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/hdrftr.py` & `python_docx_ng-0.9.6/docx/parts/hdrftr.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/image.py` & `python_docx_ng-0.9.6/docx/parts/image.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/numbering.py` & `python_docx_ng-0.9.6/docx/parts/numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/settings.py` & `python_docx_ng-0.9.6/docx/parts/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/story.py` & `python_docx_ng-0.9.6/docx/parts/story.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/parts/styles.py` & `python_docx_ng-0.9.6/docx/parts/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/section.py` & `python_docx_ng-0.9.6/docx/section.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/settings.py` & `python_docx_ng-0.9.6/docx/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/shape.py` & `python_docx_ng-0.9.6/docx/shape.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/shared.py` & `python_docx_ng-0.9.6/docx/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/styles/__init__.py` & `python_docx_ng-0.9.6/docx/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/styles/latent.py` & `python_docx_ng-0.9.6/docx/styles/latent.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/styles/style.py` & `python_docx_ng-0.9.6/docx/styles/style.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/styles/styles.py` & `python_docx_ng-0.9.6/docx/styles/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/table.py` & `python_docx_ng-0.9.6/docx/table.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-comments.xml` & `python_docx_ng-0.9.6/docx/templates/default-comments.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/[Content_Types].xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/_rels/.rels` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/docProps/app.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/docProps/core.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/docProps/thumbnail.jpeg` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/_rels/document.xml.rels` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/document.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/document.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/fontTable.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/numbering.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/settings.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/styles.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/stylesWithEffects.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/theme/theme1.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-docx-template/word/webSettings.xml` & `python_docx_ng-0.9.6/docx/templates/default-docx-template/word/webSettings.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-footer.xml` & `python_docx_ng-0.9.6/docx/templates/default-footer.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-footnotes.xml` & `python_docx_ng-0.9.6/docx/templates/default-footnotes.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-header.xml` & `python_docx_ng-0.9.6/docx/templates/default-header.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-settings.xml` & `python_docx_ng-0.9.6/docx/templates/default-settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default-styles.xml` & `python_docx_ng-0.9.6/docx/templates/default-styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/templates/default.docx` & `python_docx_ng-0.9.6/docx/templates/default.docx`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/text/comment.py` & `python_docx_ng-0.9.6/docx/text/comment.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/text/font.py` & `python_docx_ng-0.9.6/docx/text/font.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/text/paragraph.py` & `python_docx_ng-0.9.6/docx/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/text/parfmt.py` & `python_docx_ng-0.9.6/docx/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/docx/text/run.py` & `python_docx_ng-0.9.6/docx/text/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 Run-related proxy objects for python-docx, Run in particular.
 """
 
 from __future__ import absolute_import, print_function, unicode_literals
 from datetime import datetime
 
 from docx.oxml.ns import qn
-from docx.opc.packuri import PackURI
-from docx.opc.part import Part
+# see TODO below
+#from docx.opc.packuri import PackURI
+#from docx.opc.part import Part
 
 from ..enum.style import WD_STYLE_TYPE
 from ..enum.text import WD_BREAK
 from .font import Font
 from ..shape import InlineShape
 from ..shared import Parented
 
@@ -241,14 +242,16 @@
     def comments(self):
         comment_part = self._parent._parent.part._comments_part.element
         comment_refs = self._element.findall(qn('w:commentReference'))
         ids = [int(ref.get(qn('w:id'))) for ref in comment_refs]
         coms = [com for com in comment_part if com._id in ids]
         return [Comment(com, comment_part) for com in coms]
 
+    # TODO: source out part components as it breaks flow and should not be here...
+    '''
     def add_ole_object_to_run(self, ole_object_path):
         """
         Add saved OLE Object in the disk to an run and retun the newly created relationship ID
         Note: OLE Objects must be stored in the disc as `.bin` file
         """
         reltype: str = "http://schemas.openxmlformats.org/officeDocument/2006/relationships/oleObject"
         pack_path: str = "/word/embeddings/" + ole_object_path.split("\\")[-1]
@@ -257,14 +260,15 @@
 
         with open(ole_object_path, "rb") as f:
             blob = f.read()
         target_part = Part(partname=partname, content_type=content_type, blob=blob)
         rel_id: str = self.part.rels._next_rId
         self.part.rels.add_relationship(reltype=reltype, target=target_part, rId=rel_id)
         return rel_id
+    '''
 
     def add_fldChar(self, fldCharType, fldLock: bool = False, dirty: bool = False):
 
         fldChar = self._r.add_fldChar(fldCharType, fldLock, dirty)
         return fldChar
 
     @property
```

### Comparing `python_docx_ng-0.9.5/docx/text/tabstops.py` & `python_docx_ng-0.9.6/docx/text/tabstops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.5/pyproject.toml` & `python_docx_ng-0.9.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "python-docx-ng"
-version = "0.9.5"
+version = "0.9.6"
 description = "python-docx-ng is a Python library for creating and updating Microsoft Word (.docx) files."
 authors = ["toxicphreAK <pentesting.laboratories@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "docx"}]
 
 [project.urls]
 homepage = "https://github.com/toxicphreAK/python-docx-ng"
 documentation = "https://github.com/toxicphreAK/python-docx-ng/tree/master/docs"
 changelog = "https://github.com/toxicphreAK/python-docx-ng"
+"Homepage" = "https://github.com/toxicphreAK/python-docx-ng"
+"Bug Tracker" = "https://github.com/toxicphreAK/python-docx-ng/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 behave = "^1.2.6"
 lxml = "^4.9.1"
```

### Comparing `python_docx_ng-0.9.5/PKG-INFO` & `python_docx_ng-0.9.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,24 @@
-Metadata-Version: 2.1
-Name: python-docx-ng
-Version: 0.9.5
-Summary: python-docx-ng is a Python library for creating and updating Microsoft Word (.docx) files.
-License: MIT
-Author: toxicphreAK
-Author-email: pentesting.laboratories@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: behave (>=1.2.6,<2.0.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Description-Content-Type: text/markdown
-
 # python-docx-ng
 
 [![Python Packaging](https://github.com/toxicphreAK/python-docx-ng/actions/workflows/python-publish.yml/badge.svg)](https://github.com/toxicphreAK/python-docx-ng/actions/workflows/python-publish.yml)
 
 *python-docx-ng* is a Python library for creating and updating Microsoft Word (.docx) files.
 It was originally designed and developed by [scanny](https://github.com/scanny) as [python-docx](https://github.com/python-openxml/python-docx).
 As he is not actively developing his repo and there are soo many useful pull requests, bringing together a more powerful tool.
 This repo should merge a lot of those things and create a more powerful version, hopefully bearing the original structure of scanny in mind.
 
-A new documentation section will be build up soon based on Markdown in the [docs](docs) section.
-Examples can be found here: [examples](docs/examples)
+A new documentation section will be build up soon based on Markdown in the [https://github.com/toxicphreAK/python-docx-ng/blob/master/docs](docs) section.
+Examples can be found here: [examples](https://github.com/toxicphreAK/python-docx-ng/blob/master/docs/examples)
 Older information is available in the [python-docx Documentation](https://python-docx.readthedocs.org/en/latest/).
 
+Repo: https://github.com/toxicphreAK/python-docx-ng/blob/master/
+Release: https://github.com/toxicphreAK/python-docx-ng/releases
+PyPi: https://pypi.org/project/python-docx-ng/
+
 ## Installation
 
 ```commandline
 pip install python-docx-ng
 ```
 
 > Hint: The library is called `docx` in python scripts, so use imports like `import docx`. 
@@ -76,8 +63,7 @@
       + [ ] specify table location (not at end of document) - https://github.com/python-openxml/python-docx/issues/1204
       + [ ] read information from activex elements - https://github.com/python-openxml/python-docx/issues/1197
       + [ ] begin new list numbering - https://github.com/python-openxml/python-docx/issues/1194
   + [ ] Search on stackoverflow and document solutions
 + [ ] Remove code references to original repo of python-docx
 + [ ] Setup new docs (markdown based)
 + [ ] Add missing tests
-
```

