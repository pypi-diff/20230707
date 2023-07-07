# Comparing `tmp/chemistry_tools-0.5.1.tar.gz` & `tmp/chemistry_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemistry_tools-0.5.1.tar", last modified: Wed May  4 21:13:00 2022, max compression
+gzip compressed data, was "chemistry_tools-0.6.0.tar", last modified: Fri Jul  7 11:12:19 2023, max compression
```

## Comparing `chemistry_tools-0.5.1.tar` & `chemistry_tools-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0 runner    (1001) docker     (121)    11856 2022-05-04 21:13:00.102617 chemistry_tools-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-05-04 21:13:00.050617 chemistry_tools-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     6891 2022-05-04 21:13:00.050617 chemistry_tools-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-05-04 21:13:00.038617 chemistry_tools-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-05-04 21:13:00.050617 chemistry_tools-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2022-05-04 21:12:17.950181 chemistry_tools-0.5.1/chemistry_tools/spectrum_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/property_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     7922 2022-05-04 21:12:17.950181 chemistry_tools-0.5.1/chemistry_tools/units.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/_memoized_property.py
--rw-r--r--   0 runner    (1001) docker     (121)     7731 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8842 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/names.py
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2022-05-04 21:12:17.950181 chemistry_tools-0.5.1/chemistry_tools/toxnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/cas.py
--rw-r--r--   0 runner    (1001) docker     (121)     4375 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/_memoized_property.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14884 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/pug_rest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/atom.py
--rw-r--r--   0 runner    (1001) docker     (121)    20327 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/bond.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/synonyms.py
--rw-r--r--   0 runner    (1001) docker     (121)     5750 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/description.py
--rw-r--r--   0 runner    (1001) docker     (121)     4751 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/pubchem/full_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/composition.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/latex.py
--rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/_parser_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)    27073 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/formula.py
--rw-r--r--   0 runner    (1001) docker     (121)     6081 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/unicode.py
--rw-r--r--   0 runner    (1001) docker     (121)    10201 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/iso_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12437 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/formulae/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    14102 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/noble_gases.py
--rw-r--r--   0 runner    (1001) docker     (121)    33686 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/lanthanides.py
--rw-r--r--   0 runner    (1001) docker     (121)    12747 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/chalcogens.py
--rw-r--r--   0 runner    (1001) docker     (121)    12668 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/halogens.py
--rw-r--r--   0 runner    (1001) docker     (121)    14069 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/alkali_metals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12879 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/pnictogens.py
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/_isotope_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    13191 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/triels.py
--rw-r--r--   0 runner    (1001) docker     (121)    25825 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/actinides.py
--rw-r--r--   0 runner    (1001) docker     (121)    13576 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/alkaline_earth_metals.py
--rw-r--r--   0 runner    (1001) docker     (121)    19435 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7903 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12749 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/tetrels.py
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    64225 2022-05-04 21:12:17.946181 chemistry_tools-0.5.1/chemistry_tools/elements/transition_metals.py
--rw-r--r--   0 runner    (1001) docker     (121)     6594 2022-05-04 21:12:17.942181 chemistry_tools-0.5.1/chemistry_tools/elements/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-07-07 11:12:19.529570 chemistry_tools-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-07 11:12:19.529570 chemistry_tools-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-07-07 11:12:19.537571 chemistry_tools-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-07 11:12:19.521571 chemistry_tools-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6893 2023-07-07 11:12:19.529570 chemistry_tools-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/_memoized_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/toxnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/cas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11278 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/spectrum_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     7922 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/units.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/_memoized_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8842 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7731 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/property_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33686 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/lanthanides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/_isotope_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12747 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/chalcogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12879 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/pnictogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19500 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/alkaline_earth_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14102 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/noble_gases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/alkali_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64225 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/transition_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/halogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/triels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/tetrels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25825 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/actinides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10097 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10201 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/species.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12457 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/iso_dist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5771 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/latex.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/composition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9673 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/_parser_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27097 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/full_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3915 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5750 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4864 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/bond.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    14717 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5660 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/atom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/pug_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/synonyms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19223 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/properties.py
```

### Comparing `chemistry_tools-0.5.1/PKG-INFO` & `chemistry_tools-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: chemistry-tools
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python tools for analysis of chemical compounds.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: LGPL-3.0-or-later
 Keywords: chemistry,utility
 Home-page: https://github.com/domdfcoding/chemistry_tools
 Project-URL: Issue Tracker, https://github.com/domdfcoding/chemistry_tools/issues
 Project-URL: Source Code, https://github.com/domdfcoding/chemistry_tools
-Project-URL: Documentation, https://chemistry_tools.readthedocs.io/en/latest
+Project-URL: Documentation, https://chemistry-tools.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -33,21 +33,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: apeye>=0.9.1
 Requires-Dist: cachecontrol[filecache]>=0.12.6
 Requires-Dist: domdf-python-tools>=1.1.0
 Requires-Dist: enum-tools>=0.1.3
-Requires-Dist: lockfile>=0.12.2
+Requires-Dist: filelock>=3.8.0; python_version >= "3.7"
+Requires-Dist: lockfile>=0.12.2; python_version < "3.7"
 Requires-Dist: memoized-property>=1.0.3
 Requires-Dist: numpy>=1.19.1; platform_system != "Windows"
 Requires-Dist: numpy!=1.19.4,>=1.19.3; platform_system == "Windows"
 Requires-Dist: pandas>=1.0.1
 Requires-Dist: quantities>=0.12.4
 Requires-Dist: requests>=2.24.0
+Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: cawdrey>=0.1.7; extra == 'pubchem'
 Requires-Dist: mathematical>=0.1.13; extra == 'pubchem'
 Requires-Dist: pillow>=7.0.0; (platform_python_implementation == "PyPy" and python_version >= "3.8" and platform_system == "Windows") and extra == 'pubchem'
 Requires-Dist: pillow>=7.0.0; (platform_python_implementation == "PyPy" and python_version >= "3.7" and platform_system != "Windows") and extra == 'pubchem'
 Requires-Dist: pillow>=7.0.0; (platform_python_implementation != "PyPy") and extra == 'pubchem'
 Requires-Dist: pillow<9.0.0,>=7.0.0; (platform_python_implementation == "PyPy" and python_version == "3.7" and platform_system == "Windows") and extra == 'pubchem'
 Requires-Dist: pillow<8.0.0,>=7.0.0; (platform_python_implementation == "PyPy" and python_version == "3.6") and extra == 'pubchem'
@@ -109,16 +111,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/chemistry_tools/latest?logo=read-the-docs
-	:target: https://chemistry_tools.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/chemistry-tools/latest?logo=read-the-docs
+	:target: https://chemistry-tools.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/chemistry_tools/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/chemistry_tools/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/chemistry_tools/workflows/Linux/badge.svg
@@ -137,16 +139,16 @@
 	:target: https://github.com/domdfcoding/chemistry_tools/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/chemistry_tools/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/chemistry_tools/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/chemistry_tools/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/chemistry_tools/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/chemistry_tools/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/chemistry_tools/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/chemistry_tools/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/chemistry_tools?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/chemistry_tools?logo=codefactor
@@ -180,23 +182,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v0.5.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v0.6.0
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/chemistry_tools
 	:target: https://pypi.org/project/chemistry_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `chemistry_tools-0.5.1/pyproject.toml` & `chemistry_tools-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "chemistry_tools"
-version = "0.5.1"
+version = "0.6.0"
 description = "Python tools for analysis of chemical compounds."
 readme = "README.rst"
 keywords = [ "chemistry", "utility",]
 dynamic = []
 dependencies = [
     "apeye>=0.9.1",
     "cachecontrol[filecache]>=0.12.6",
     "domdf-python-tools>=1.1.0",
     "enum-tools>=0.1.3",
-    "lockfile>=0.12.2",
+    'filelock>=3.8.0; python_version >= "3.7"',
+    'lockfile>=0.12.2; python_version < "3.7"',
     "memoized-property>=1.0.3",
     'numpy>=1.19.1; platform_system != "Windows"',
     'numpy!=1.19.4,>=1.19.3; platform_system == "Windows"',
     "pandas>=1.0.1",
     "quantities>=0.12.4",
     "requests>=2.24.0",
+    "typing-extensions>=4.0.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
@@ -54,15 +56,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/domdfcoding/chemistry_tools"
 "Issue Tracker" = "https://github.com/domdfcoding/chemistry_tools/issues"
 "Source Code" = "https://github.com/domdfcoding/chemistry_tools"
-Documentation = "https://chemistry_tools.readthedocs.io/en/latest"
+Documentation = "https://chemistry-tools.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
 pubchem = [
     "cawdrey>=0.1.7",
     "mathematical>=0.1.13",
     'pillow>=7.0.0; platform_python_implementation == "PyPy" and python_version >= "3.8" and platform_system == "Windows"',
     'pillow>=7.0.0; platform_python_implementation == "PyPy" and python_version >= "3.7" and platform_system != "Windows"',
@@ -133,34 +135,33 @@
 package_root = "chemistry_tools"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "enum_tools.autoenum",
     "_internal_extension",
-    "sphinx_toolbox_experimental.needspace",
-    "sphinx_toolbox_experimental.autosummary_widths",
-    "sphinx_toolbox_experimental.succinct_seealso",
+    "sphinx_toolbox.more_autosummary.column_widths",
+    "sphinx_toolbox.latex.succinct_seealso",
     "sphinx_toolbox_experimental.missing_xref",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
@@ -205,26 +206,26 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.7"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
 [tool.dep_checker]
-allowed_unused = [ "cachecontrol", "lockfile",]
+allowed_unused = [ "cachecontrol", "lockfile", "filelock",]
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
```

### Comparing `chemistry_tools-0.5.1/README.rst` & `chemistry_tools-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/chemistry_tools/latest?logo=read-the-docs
-	:target: https://chemistry_tools.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/chemistry-tools/latest?logo=read-the-docs
+	:target: https://chemistry-tools.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/chemistry_tools/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/chemistry_tools/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/chemistry_tools/workflows/Linux/badge.svg
@@ -53,16 +53,16 @@
 	:target: https://github.com/domdfcoding/chemistry_tools/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/chemistry_tools/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/chemistry_tools/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/chemistry_tools/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/chemistry_tools/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/chemistry_tools/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/chemistry_tools/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/chemistry_tools/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/chemistry_tools?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/chemistry_tools?logo=codefactor
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v0.5.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v0.6.0
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/chemistry_tools
 	:target: https://pypi.org/project/chemistry_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `chemistry_tools-0.5.1/LICENSE` & `chemistry_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/spectrum_similarity.py` & `chemistry_tools-0.6.0/chemistry_tools/spectrum_similarity.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,23 +46,56 @@
 #  |  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 #  |  ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  |  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 #  |  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
-from typing import Mapping, Optional, Sequence, Tuple, Union
+from typing import Mapping, Optional, Sequence, Tuple, Union, overload
 
 # 3rd party
 import numpy
 import pandas  # type: ignore
+from typing_extensions import Literal
 
 __all__ = ["spectrum_similarity", "normalize", "create_array"]
 
 
+@overload
+def spectrum_similarity(
+		spec_top: numpy.ndarray,
+		spec_bottom: numpy.ndarray,
+		t: float = ...,
+		b: float = ...,
+		top_label: Optional[str] = ...,
+		bottom_label: Optional[str] = ...,
+		xlim: Tuple[int, int] = ...,
+		x_threshold: float = ...,
+		print_alignment: bool = ...,
+		print_graphic: bool = ...,
+		output_list: Literal[True] = True,
+		) -> Tuple[float, float, pandas.DataFrame]: ...
+
+
+@overload
+def spectrum_similarity(
+		spec_top: numpy.ndarray,
+		spec_bottom: numpy.ndarray,
+		t: float,
+		b: float,
+		top_label: Optional[str],
+		bottom_label: Optional[str],
+		xlim: Tuple[int, int],
+		x_threshold: float,
+		print_alignment: bool,
+		print_graphic: bool,
+		output_list: Literal[False],
+		) -> Tuple[float, float]: ...
+
+
 def spectrum_similarity(
 		spec_top: numpy.ndarray,
 		spec_bottom: numpy.ndarray,
 		t: float = 0.25,
 		b: float = 10,
 		top_label: Optional[str] = None,
 		bottom_label: Optional[str] = None,
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/property_format.py` & `chemistry_tools-0.6.0/chemistry_tools/property_format.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/units.py` & `chemistry_tools-0.6.0/chemistry_tools/units.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/constants.py` & `chemistry_tools-0.6.0/chemistry_tools/constants.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/names.py` & `chemistry_tools-0.6.0/chemistry_tools/names.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/toxnet.py` & `chemistry_tools-0.6.0/chemistry_tools/toxnet.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/cas.py` & `chemistry_tools-0.6.0/chemistry_tools/cas.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/__init__.py` & `chemistry_tools-0.6.0/chemistry_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/cache.py` & `chemistry_tools-0.6.0/chemistry_tools/cache.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/enums.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/enums.pyi` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.pyi`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/compound.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/compound.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,29 @@
 from chemistry_tools.formulae import Formula
 from chemistry_tools.pubchem.atom import Atom, parse_atoms
 from chemistry_tools.pubchem.bond import Bond, parse_bonds
 from chemistry_tools.pubchem.enums import CoordinateType
 from chemistry_tools.pubchem.full_record import parse_full_record, rest_get_full_record
 from chemistry_tools.pubchem.properties import (
 		force_valid_properties,
-		insert_valid_properties_table,
 		parse_properties,
 		rest_get_properties_json,
 		valid_properties
 		)
 from chemistry_tools.pubchem.synonyms import get_synonyms
 
 __all__ = ["Compound", "compounds_to_frame", 'C']
 
 C = TypeVar('C', bound="Compound")
 
 
 @prettify_docstrings
 class Compound(Dictable):
 	"""
-	Corresponds to a single record from the PubChem Compound database.
+	Represents a single record from the PubChem Compound database.
 
 	The PubChem Compound database is constructed from the Substance database
 	using a standardization and deduplication process.
 	Each Compound is uniquely identified by a CID.
 
 	:param title: The title of the compound record (usually the name of the compound)
 	:param CID:
@@ -261,23 +260,21 @@
 	def elements(self) -> List[str]:
 		"""
 		List of element symbols for atoms in this Compound.
 		"""
 
 		return [a.element for a in self.atoms]
 
-	@insert_valid_properties_table()
 	def get_properties(self, properties: Union[Sequence[str], str]) -> Dict[str, Any]:
 		"""
 		Returns the requested properties for the Compound.
 
-		:param properties: The properties to retrieve for the compound. See the table below.
+		:param properties: The properties to retrieve for the compound.
 			Can be either a comma-separated string or a list.
-
-		:: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::
+			See :ref:`the table at the start of this chapter <properties table>` for a list of valid properties.
 
 		:return: Dictionary mapping the property names to their values
 		"""
 
 		if isinstance(properties, str) and properties.lower() == "all":
 			properties = list(valid_properties.keys())
 
@@ -305,23 +302,21 @@
 
 		for prop in cached_properties:
 			# print("Getting from cache")
 			output[prop] = self._properties[prop]
 
 		return output
 
-	@insert_valid_properties_table()
 	def get_property(self, prop: str) -> Any:
 		"""
 		Get a single property for the compound.
 
-		:param prop: The property to retrieve for the compound. See the table below.
-
-		:: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::
-		"""  # noqa: RST218
+		:param prop: The property to retrieve for the compound.
+			See :ref:`the table at the start of this chapter <properties table>` for a list of valid properties.
+		"""
 
 		prop = str(prop)
 
 		if prop not in self._properties:
 			raise ValueError(f"Unknown property '{prop}'")
 
 		if self._properties[prop] is not None:
@@ -518,15 +513,15 @@
 # cid
 # counts
 
 
 # TODO:
 def compounds_to_frame(compounds: Union[Compound, List[Compound]]) -> DataFrame:
 	"""
-	Construct a :class:`pandas.DataFrame` from a list of
+	Construct a :class:`~.pandas.DataFrame` from a list of
 	:class:`~chemistry_tools.pubchem.compound.Compound` objects.
 
 	:param compounds:
 	"""  # noqa: D400
 
 	if isinstance(compounds, Compound):
 		compounds = [compounds]
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/images.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/images.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/pug_rest.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/pug_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from typing import Dict, Iterable, Iterator, List, Optional, Sequence, Union
 from urllib.parse import quote
 
 # 3rd party
 import requests
 
 # this package
-from chemistry_tools import cached_requests
 from chemistry_tools.pubchem import API_BASE
 from chemistry_tools.pubchem.enums import PubChemFormats, PubChemNamespace
 from chemistry_tools.pubchem.errors import HTTP_ERROR_CODES, PubChemHTTPError
 from chemistry_tools.pubchem.utils import _force_sequence_or_csv, _make_base_url
 
 __all__ = ["get_full_json", "async_get", "request", "do_rest_get"]
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/atom.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/atom.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,14 @@
 
 	:param aid: The Atom ID within the owning Compound.
 	:param number: The Atomic number for this atom.
 	:param x: The x coordinate for this atom.
 	:param y: The y coordinate for this atom.
 	:param z: The z coordinate for this atom. Will be :py:obj:`None` in 2D Compound records.
 	:param charge: Formal charge on atom.
-
-	.. latex:clearpage::
 	"""
 
 	def __init__(
 			self,
 			aid: int,
 			number: int,
 			x: Optional[float] = None,
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/properties.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,43 +43,38 @@
 #  |  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  |  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 #  |  THE SOFTWARE.
 #
 
 # stdlib
 import warnings
-from textwrap import dedent
 from typing import Any, Callable, Dict, Iterable, List, NamedTuple, Sequence, Union
 
 # 3rd party
 from pandas import DataFrame  # type: ignore
-from tabulate import tabulate  # nodep
 
 # this package
 from chemistry_tools.formulae import Formula
 
 # this package
 from .enums import PubChemFormats, PubChemNamespace
 from .pug_rest import do_rest_get
 from .utils import _force_sequence_or_csv
 
 __all__ = [
 		"PropData",
-		"valid_property_descriptions",
 		"valid_properties",
 		"PROPERTY_MAP",
-		"insert_valid_properties_table",
 		"rest_get_properties_json",
 		"rest_get_properties",
 		"force_valid_properties",
 		"get_properties",
 		"get_property",
 		"parse_properties",
 		"PubChemProperty",
-		"string_list",
 		]
 
 
 class PropData(NamedTuple):
 	"""
 	Metadata about a property.
 	"""
@@ -303,71 +298,37 @@
 				"Fingerprint2D",
 				"Base64-encoded PubChem Substructure Fingerprint of a molecule.",
 				str,
 				"fingerprint_2d"
 				),
 		]
 
-#: Table giving descriptions of valid properties.
-valid_property_descriptions: str = tabulate(
-		[(prop.name, prop.description) for prop in _properties],
-		headers=["Property", "Description"],
-		tablefmt="rst",
-		)
-
 #: Properties for PubChem REST API
 valid_properties: Dict[str, Callable] = {prop.name: prop.type for prop in _properties}
 
 #: Allows properties to optionally be specified as underscore_separated, consistent with Compound attributes
 PROPERTY_MAP: Dict[str, str] = {prop.attr_name: prop.name for prop in _properties}
 
 
-def insert_valid_properties_table() -> Callable:
-	"""
-	Decorator to insert table of valid properties into the docstring of the decorated function.
-	"""
-
-	def wrapper(target: Callable) -> Callable:
-		target_doc = target.__doc__
-
-		if not target_doc:
-			return target
-
-		deindented_doc = dedent(target_doc)
-
-		replaced_doc = deindented_doc.replace(
-				":: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::",
-				valid_property_descriptions
-				)
-
-		target.__doc__ = replaced_doc
-
-		return target
-
-	return wrapper
-
-
-@insert_valid_properties_table()
 def rest_get_properties_json(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
 		namespace=PubChemNamespace.name,
 		properties: Union[Sequence[str], str] = '',
 		**kwargs
 		) -> Dict:
 	"""
 	Returns the properties for the compound with the given identifier as a dictionary.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
 		When using the CID namespace data for multiple compounds can be retrieved at once by
 		supplying either a comma-separated string or a list.
 	:param namespace: The type of identifier to look up. Valid values are in :class:`~.PubChemNamespace`.
-	:param properties: The properties to retrieve for the compound. See the table below. Can be either a
-		comma-separated string or a list.
-
-	:: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::
+	:param properties: The properties to retrieve for the compound.
+		Can be either a comma-separated string or a list.
+		See :ref:`the table at the start of this chapter <properties table>` for a list of valid properties.
 
 	:param kwargs: Optional arguments that ``json.loads`` takes.
 
 	:raises ValueError: If the response body does not contain valid JSON.
 
 	:return: Parsed JSON data
 	"""
@@ -377,32 +338,30 @@
 	for prop in properties:
 		if prop not in valid_properties:
 			raise ValueError(f"Unknown property '{prop}'")
 
 	return do_rest_get(namespace, identifier, domain=f"property/{','.join(properties)}").json(**kwargs)
 
 
-@insert_valid_properties_table()
 def rest_get_properties(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
 		namespace=PubChemNamespace.name,
 		properties: Union[Sequence[str], str] = '',
 		format_: Union[PubChemFormats, str] = PubChemFormats.CSV,
 		):
 	r"""
 	Returns the properties for the compound with the given identifier in the desired format.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
 		When using the CID namespace data for multiple compounds can be retrieved at once by
 		supplying either a comma-separated string or a list.
 	:param namespace: The type of identifier to look up. Valid values are in :class:`~.PubChemNamespace`
-	:param properties: The properties to retrieve for the compound. See the table below. Can be either a
-		comma-separated string or a list.
-
-	:: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::
+	:param properties: The properties to retrieve for the compound.
+		Can be either a comma-separated string or a list.
+		See :ref:`the table at the start of this chapter <properties table>` for a list of valid properties.
 
 	:param format\_: The format to obtain the data in
 	"""
 
 	properties = force_valid_properties(properties)
 
 	for prop in properties:
@@ -434,33 +393,31 @@
 
 	if not ordered_properties:
 		raise ValueError(f"Please supply one or more properties")
 
 	return ordered_properties
 
 
-@insert_valid_properties_table()
 def get_properties(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
 		properties: Union[Sequence[str], str] = '',
 		namespace: Union[PubChemNamespace, str] = PubChemNamespace.name,
 		as_dataframe: bool = False,
 		) -> Union[List[Dict[str, Any]], DataFrame]:
 	"""
 	Returns the requested properties for the compound with the given identifier.
 	As more than one compound may be identified the results are returned in a list.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
 		When using the CID namespace data for multiple compounds can be retrieved at once by
 		supplying either a comma-separated string or a list.
 
-	:param properties: The properties to retrieve for the compound. See the table below. Can be either a
-		comma-separated string or a list.
-
-	:: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::
+	:param properties: The properties to retrieve for the compound.
+		Can be either a comma-separated string or a list.
+		See :ref:`the table at the start of this chapter <properties table>` for a list of valid properties.
 
 	:param namespace: The type of identifier to look up. Valid values are in :class:`~.PubChemNamespace`.
 	:param as_dataframe: Automatically extract the properties into a pandas :class:`~pandas.DataFrame`.
 
 	:raises ValueError: If the response body does not contain valid JSON.
 	:raises NotFoundError: If the compound with the requested identifier was not found in PubChem.
 
@@ -486,15 +443,14 @@
 
 	if as_dataframe:
 		return DataFrame.from_records(results, index="CID")
 
 	return results
 
 
-@insert_valid_properties_table()
 def get_property(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
 		property: str = '',  # noqa: A002  # pylint: disable=redefined-builtin
 		namespace: Union[PubChemNamespace, str] = PubChemNamespace.name
 		) -> Any:
 	"""
 	Returns the requested property for the compound with the given identifier.
@@ -502,24 +458,26 @@
 	This convenience function only allows for a single property to be accessed at once,
 	and for only a single compound. if you require multiple properties and/or properties for
 	multiple compounds use :class:`chemistry_tools.pubchem.properties.get_properties`, which helps
 	reduce the burden on the PubChem servers.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
 
-	:param property: The property to retrieve for the compound. See the table below.
-
-	:: See chemistry_tools.pubchem.properties.valid_property_descriptions for a list of valid properties ::
+	:param properties: The properties to retrieve for the compound.
+		Can be either a comma-separated string or a list.
+		See :ref:`the table at the start of this chapter <properties table>` for a list of valid properties.
 
 	:param namespace: The type of identifier to look up. Valid values are in :class:`~.PubChemNamespace`.
 
 	:raises ValueError: If the response body does not contain valid JSON.
 	:raises NotFoundError: If the compound with the requested identifier was not found in PubChem.
 
-	:return: The requested property. Type depends on the property requested
+	:return: The requested property. Type depends on the property requested.
+
+	.. latex:clearpage::
 	"""
 
 	property_ = force_valid_properties(property)[0]
 
 	data = rest_get_properties_json(identifier, namespace, [property_])
 
 	return parse_properties(data)[0][property_]
@@ -528,16 +486,14 @@
 def parse_properties(property_data: Dict) -> List[Dict]:
 	"""
 	Parse raw data from the ``property`` endpoint of the REST API.
 
 	:param property_data:
 
 	:return: A list of dictionaries mapping the properties to values for each compound
-
-	.. latex:clearpage::
 	"""
 
 	compounds = {}
 	fields = valid_properties
 
 	for entry in property_data["PropertyTable"]["Properties"]:
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/bond.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/bond.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,19 @@
 			and self.aid2 == other.aid2
 			and self.order == other.order
 			and self.style == other.style
 			)  # yapf: disable
 
 	def to_dict(self) -> Dict[str, Any]:
 		"""
-		Return a dictionary containing Bond data.
+		Return a dictionary containing bond data.
+
+		:rtype:
+
+		.. latex:clearpage::
 		"""
 
 		data = {"aid1": self.aid1, "aid2": self.aid2, "order": self.order}
 
 		if self.style is not None:
 			data["style"] = self.style
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/lookup.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/lookup.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/synonyms.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/synonyms.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/errors.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/errors.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/description.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/description.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/utils.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/__init__.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 #  !/usr/bin/env python
 #
 #  __init__.py
-"""
+r"""
 This module provides a wrapper around the PubChem PUG_REST API.
 
-Data for compounds can be accessed using the :func:`chemistry_tools.pubchem.lookup.get_compounds` function.
+Data for compounds can be accessed using the
+:func:`pubchem.lookup.get_compounds <chemistry_tools.pubchem.lookup.get_compounds>` function.
+
+.. _properties table:
+
+The following table lists the various properties that can be obtained from the PubChem API:
+
+.. tabularcolumns:: |l|>{\raggedright\arraybackslash}p{10cm}|
+
+.. collapse:: Click to expand
+
+	.. properties-table::
+
 """
 #
 #  Copyright (c) 2019-2021 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as
 #  published by the Free Software Foundation; either version 3 of the
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/requirements.txt` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/requirements.txt`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/pubchem/full_record.py` & `chemistry_tools-0.6.0/chemistry_tools/pubchem/full_record.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/composition.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/composition.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/dataarray.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/dataarray.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/latex.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/latex.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/_parser_core.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/_parser_core.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/compound.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/compound.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/formula.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,14 +578,16 @@
 			Otherwise, only compositions are yielded.
 		:param elements_with_isotopes: A set of elements to be considered in isotopic distributions
 			(by default, every element has an isotopic distribution).
 		:param isotope_threshold: The threshold abundance of a specific isotope to be considered.
 		:param overall_threshold: The threshold abundance of the calculated isotopic composition.
 
 		:return: Iterator over possible isotopic compositions.
+
+		.. latex:clearpage::
 		"""
 
 		dict_elem_isotopes = {}
 		for element in self:
 			if elements_with_isotopes is None or element in elements_with_isotopes:
 				element_name, isotope_num = split_isotope(element)
 				isotopes = {
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/unicode.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/unicode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 #
 #  unicode.py
 """
 Functions and constants for converting formulae to unicode.
+
+.. latex:vspace:: -10px
 """
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/species.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/species.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 #  |  INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 #  |  CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 #  |  ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 #  |  POSSIBILITY OF SUCH DAMAGE.
 #  |
 
 # stdlib
-from typing import cast, Dict, List, Optional, Type, TypeVar
+from typing import Dict, List, Optional, Type, TypeVar, cast
 
 # 3rd party
 from cawdrey import frozendict  # nodep
 from typing_extensions import Literal  # nodep
 
 # this package
 from chemistry_tools.formulae.formula import Formula
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/iso_dist.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/iso_dist.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/utils.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/html.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/html.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/__init__.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/formulae/parser.py` & `chemistry_tools-0.6.0/chemistry_tools/formulae/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 #
 #  parser.py
 """
-Functions and constants for parsing formulae.
+Functions and parsing formulae.
+
+.. latex:vspace:: -10px
 """
 #
 #  Copyright (c) 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
@@ -280,14 +282,16 @@
 		>>> string_to_composition('NH4+') == {0: 1, "H": 4, "N": 1}
 		True
 		>>> string_to_composition('.NHO-(aq)') == {0: -1, "H": 1, "N": 1, "O": 1}
 		True
 		>>> string_to_composition('Na2CO3.7H2O') == {"Na": 2, "C": 1, "O": 10, "H": 14}
 		True
 
+	.. latex:vspace:: -10px
+
 	:param formula: Chemical formula, e.g. ``'H2O'``, ``'Fe+3'``, ``'Cl-'``
 	:param prefixes: Prefixes to ignore, e.g. ``('.', 'alpha-')``
 	:param suffixes: Suffixes to ignore.
 
 	:return: The composition, as a dictionary mapping atomic number -> multiplicity.
 		"Atomic number" 0 represents net charge.
 	"""
@@ -334,27 +338,25 @@
 	"""
 	Calculates molecular mass, in atomic mass units, from atomic weights.
 
 	.. latex:vspace:: -5px
 
 	.. note:: Atomic number 0 denotes charge or "net electron defficiency"
 
-	.. latex:vspace:: -5px
-
-	:param composition: Dictionary mapping :class:`str` or :class:`int` (element symbol or atomic number) to int (coefficient)
-	:param charge: The charge of the composition.
-
-	:rtype:
+	.. latex:vspace:: -15px
 
 	:bold-title:`Example:`
 
 	.. code-block:: python
 
 		>>> f'{mass_from_composition({0: -1, "H": 1, 8: 1}):.2f}'
 		'17.01'
+
+	:param composition: Mapping of :class:`str` or :class:`int` (element symbol or atomic number) to int (coefficient)
+	:param charge: The charge of the composition.
 	"""
 
 	if charge and 0 in composition:
 		if charge != composition[0]:
 			raise ValueError(
 					"'charge' can only be specified once, "
 					"either as a keyword argument or as the '0' key of 'composition'"
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/noble_gases.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/noble_gases.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/lanthanides.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/lanthanides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/chalcogens.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/chalcogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/halogens.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/halogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/alkali_metals.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/alkali_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/pnictogens.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/pnictogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/_isotope_data.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/_isotope_data.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/triels.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/triels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/actinides.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/actinides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/alkaline_earth_metals.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/alkaline_earth_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/classes.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 #  |  ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 #  |  POSSIBILITY OF SUCH DAMAGE.
 #  |
 #
 
 # stdlib
 import functools
-from functools import lru_cache
 from typing import Dict, Iterable, Iterator, List, Optional, Tuple, Union, overload
 
 # 3rd party
 from domdf_python_tools import doctools
 from domdf_python_tools.bases import Dictable
 from domdf_python_tools.doctools import prettify_docstrings
 
@@ -280,14 +279,18 @@
 
 	molecular_weight = mass
 
 	@memoized_property
 	def eleneg(self) -> float:
 		"""
 		The Electronegativity (Pauling scale).
+
+		:rtype:
+
+		.. latex:clearpage::
 		"""
 
 		return self._eleneg
 
 	@memoized_property
 	def eleaffin(self) -> float:
 		"""
@@ -369,16 +372,18 @@
 		return self._ionenergy
 
 	@memoized_property
 	def isotopes(self) -> Dict[int, "Isotope"]:
 		"""
 		The Isotopic composition.
 
-		| **keys**: isotope mass number
-		| **values**: Isotope(relative atomic mass, abundance)
+		* **keys**: isotope mass number
+		* **values**: Isotope(relative atomic mass, abundance)
+
+		.. latex:vspace:: -10px
 		"""
 
 		return self._isotopes
 
 	@memoized_property
 	def description(self) -> str:
 		"""
@@ -604,14 +609,15 @@
 class Elements(Iterable[Element]):
 	r"""
 	Ordered dict of Elements with lookup by number, symbol, and name.
 
 	:param \*elements: The elements to add to the dictionary.
 
 	.. autosummary-widths:: 1/2
+	.. latex:vspace:: -10px
 	"""
 
 	def __init__(self, *elements: Element):
 		self._list: List[Element] = []
 		self._dict: Dict[Union[str, int], Element] = {}
 
 		for element in elements:
@@ -684,15 +690,15 @@
 		else:
 			try:
 				symbol, isotope = self.split_isotope(key)
 				return self._dict[symbol.capitalize()]
 			except (ValueError, KeyError):
 				raise KeyError(f"Unknown key: '{key}'")
 
-	@lru_cache()
+	@functools.lru_cache()
 	def split_isotope(self, string: str) -> Tuple[str, int]:
 		"""
 		Returns the symbol and mass number for the isotope represented by ``string``.
 
 		Valid isotopes include ``'[C12]'``, ``'C[12]'`` and ``'[12C]'``.
 
 		:param string:
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/__init__.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  __init__.py
 """
 Properties of the chemical elements.
 
 Each chemical element is represented as an object instance. Physicochemical
 and descriptive properties of the elements are stored as instance attributes.
 
-Originally created by Christoph Gohlke <https://www.lfd.uci.edu/~gohlke/>`_
+Originally created by `Christoph Gohlke <https://www.lfd.uci.edu/~gohlke/>`_.
 Licensed under the BSD 3-Clause license
 
 
 References
 ----------
 1. https://www.nist.gov/pml/atomic-weights-and-isotopic-compositions-relative-atomic-masses
 2. https://en.wikipedia.org/wiki/{element.name}
@@ -118,21 +118,21 @@
 #  |  DOI: `10.1021/acs.jproteome.8b00717 <http://dx.doi.org/10.1021/acs.jproteome.8b00717>`_
 #
 #  Isotope data from http://www.nist.gov/pml/data/comp.cfm
 #
 
 # this package
 from ._elements import ELEMENTS, D, H, T
-from ._isotope_data import isotope_data  # , undefined_isotopes
+from ._isotope_data import isotope_data  # , undefined_isotopes  # noqa: F401
 from ._table import BLOCKS, GROUPS, PERIODS, SERIES
 from .actinides import Ac, Am, Bk, Cf, Cm, Es, Fm, Lr, Md, No, Np, Pa, Pu, Th, U
 from .alkali_metals import Cs, Fr, K, Li, Na, Rb
 from .alkaline_earth_metals import Ba, Be, Ca, Mg, Ra, Sr
 from .chalcogens import Lv, O, Po, S, Se, Te
-from .classes import Element, Elements, Isotope
+from .classes import Element, Elements, Isotope  # noqa: F401
 from .halogens import At, Br, Cl, F, I, Ts
 from .lanthanides import Ce, Dy, Er, Eu, Gd, Ho, La, Lu, Nd, Pm, Pr, Sm, Tb, Tm, Yb
 from .noble_gases import Ar, He, Kr, Ne, Og, Rn, Xe
 from .pnictogens import As, Bi, Mc, N, P, Sb
 from .tetrels import C, Fl, Ge, Pb, Si, Sn
 from .transition_metals import (
 		Ag,
```

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/tetrels.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/tetrels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/_table.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/_table.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/transition_metals.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/transition_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.5.1/chemistry_tools/elements/_elements.py` & `chemistry_tools-0.6.0/chemistry_tools/elements/_elements.py`

 * *Files identical despite different names*

