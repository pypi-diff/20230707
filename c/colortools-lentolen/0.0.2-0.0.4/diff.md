# Comparing `tmp/colortools_lentolen-0.0.2.tar.gz` & `tmp/colortools_lentolen-0.0.4.tar.gz`

## Comparing `colortools_lentolen-0.0.2.tar` & `colortools_lentolen-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/__init__.py
--rw-r--r--   0        0        0    22280 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/color_utils.py
--rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/data/color-meanings.com.csv
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/data/html-ger.csv
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/data/html.csv
--rw-r--r--   0        0        0   658468 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/data/meodai.csv
--rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/src/colortools/data/x11.csv
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/README.md
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/__init__.py
+-rw-r--r--   0        0        0    26129 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/color_utils.py
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/color-meanings.com.csv
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/html-ger.csv
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/html.csv
+-rw-r--r--   0        0        0   658468 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/meodai.csv
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/src/colortools/data/x11.csv
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/README.md
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 colortools_lentolen-0.0.4/PKG-INFO
```

### Comparing `colortools_lentolen-0.0.2/src/colortools/color_utils.py` & `colortools_lentolen-0.0.4/src/colortools/color_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -152,14 +152,16 @@
     _validate_rgb(rgba)
 
     return (rgba[0], rgba[1], rgba[2])
 
 def _val_rgb(rgb):
     if len(rgb) > 3:
         return (rgb[0], rgb[1], rgb[2])
+    else:
+        return rgb
 
 def hex_to_hsl(hex: str) -> tuple:
     """
     Convert HEX values to HSL values.
 
     Args:
     - HEX Code (str).
@@ -181,15 +183,15 @@
     Returns:
     - tuple: A tuple containing the CMYK values
     """
     rgb = hex_to_rgb(hex)    
     rgb = _val_rgb(rgb)
     return rgb_to_cmyk(rgb)
 
-def hex_to_hsl(hex: str) -> tuple:
+def hex_to_hsv(hex: str) -> tuple:
     """
     Convert HEX values to HSV values.
 
     Args:
     - HEX (str)
 
     Returns:
@@ -209,15 +211,15 @@
     Returns:
     - tuple: A tuple containing the LAB values
     """
     rgb = hex_to_rgb(hex)    
     rgb = _val_rgb(rgb)
     return rgb_to_lab(rgb)
 
-def hex_to_lab(hex: str) -> tuple:
+def hex_to_xyz(hex: str) -> tuple:
     """
     Convert HEX values to XYZ values.
 
     Args:
     - HEX (str)
 
     Returns:
@@ -326,67 +328,81 @@
     # Convert RGB values to the range [0, 255]
     r = int((r + m) * 255)
     g = int((g + m) * 255)
     b = int((b + m) * 255)
 
     return r, g, b
 
+def hsl_to_hex(hsl: tuple) -> tuple:
+    """
+    Convert HSL values to hex.
+
+    Args:
+    - HSL (tuple)
+
+    Returns:
+    - str: Hexadecimal color code.
+    """
+    rgb = hsl_to_rgb(hsl)    
+    rgb = _val_rgb(rgb)
+    return rgb_to_hex(rgb)
+
 def hsl_to_cmyk(hsl: tuple) -> tuple:
     """
     Convert HSL values to CMYK values.
 
     Args:
     - HSL (tuple)
 
     Returns:
     - tuple: A tuple containing the CMYK values
     """
-    rgb = hsl_to_rgb(hex)    
+    rgb = hsl_to_rgb(hsl)    
     rgb = _val_rgb(rgb)
     return rgb_to_cmyk(rgb)
 
 def hsl_to_hsv(hsl: tuple) -> tuple:
     """
     Convert HSL values to HSV values.
 
     Args:
     - HSL (tuple)
 
     Returns:
     - tuple: A tuple containing the HSV values
     """
-    rgb = hsl_to_rgb(hex)    
+    rgb = hsl_to_rgb(hsl)    
     rgb = _val_rgb(rgb)
-    return rgb_to_hsl(rgb)
+    return rgb_to_hsv(rgb)
 
 def hsl_to_lab(hsl: tuple) -> tuple:
     """
     Convert HSL values to LAB values.
 
     Args:
     - HSL (tuple)
 
     Returns:
     - tuple: A tuple containing the LAB values
     """
-    rgb = hsl_to_rgb(hex)    
+    rgb = hsl_to_rgb(hsl)    
     rgb = _val_rgb(rgb)
     return rgb_to_lab(rgb)
 
 def hsl_to_xyz(hsl: tuple) -> tuple:
     """
     Convert HSL values to XYZ values.
 
     Args:
     - HSL (tuple)
 
     Returns:
     - tuple: A tuple containing the XYZ values
     """
-    rgb = hsl_to_rgb(hex)    
+    rgb = hsl_to_rgb(hsl)    
     rgb = _val_rgb(rgb)
     return rgb_to_xyz(rgb)
 
 def rgb_to_cmyk(rgb: tuple) -> tuple:
     """
     Converts an RGB tuple to CMYK tuple.
     
@@ -438,81 +454,151 @@
     # Convert CMYK to RGB using the formula
     r = round((1 - c) * (1 - k) * 255)
     g = round((1 - m) * (1 - k) * 255)
     b = round((1 - y) * (1 - k) * 255)
     
     return r, g, b
 
+def cmyk_to_hex(cmyk: tuple) -> tuple:
+    """
+    Convert CMYK values to hex.
+
+    Args:
+    - CMYK (tuple)
+
+    Returns:
+    - str: Hexadecimal color code.
+    """
+    rgb = cmyk_to_rgb(cmyk)    
+    rgb = _val_rgb(rgb)
+    return rgb_to_hex(rgb)
+
 def cmyk_to_hsv(cmyk: tuple) -> tuple:
     """
     Convert CMYK values to HSV values.
 
     Args:
     - CMYK (tuple)
 
     Returns:
     - tuple: A tuple containing the HSV values
     """
-    rgb = cmyk_to_rgb(hex)    
+    rgb = cmyk_to_rgb(cmyk)    
     rgb = _val_rgb(rgb)
     return rgb_to_hsv(rgb)
 
+def cmyk_to_hsl(cmyk: tuple) -> tuple:
+    """
+    Convert CMYK values to HSL values.
+
+    Args:
+    - CMYK (tuple)
+
+    Returns:
+    - tuple: A tuple containing the HSL values
+    """
+    rgb = cmyk_to_rgb(cmyk)    
+    rgb = _val_rgb(rgb)
+    return rgb_to_hsl(rgb)
+
 def cmyk_to_lab(cmyk: tuple) -> tuple:
     """
     Convert CMYK values to LAB values.
 
     Args:
     - CMYK (tuple)
 
     Returns:
     - tuple: A tuple containing the LAB values
     """
-    rgb = cmyk_to_rgb(hex)    
+    rgb = cmyk_to_rgb(cmyk)    
     rgb = _val_rgb(rgb)
     return rgb_to_lab(rgb)
 
 def cmyk_to_xyz(cmyk: tuple) -> tuple:
     """
     Convert CMYK values to XYZ values.
 
     Args:
     - CMYK (tuple)
 
     Returns:
     - tuple: A tuple containing the XYZ values
     """
-    rgb = cmyk_to_rgb(hex)    
+    rgb = cmyk_to_rgb(cmyk)    
     rgb = _val_rgb(rgb)
     return rgb_to_xyz(rgb)
 
+def hsv_to_hsl(hsv: tuple) -> tuple:
+    """
+    Convert HSV values to HSL values.
+
+    Args:
+    - HSV (tuple)
+
+    Returns:
+    - tuple: A tuple containing the HSL values
+    """
+    rgb = hsv_to_rgb(hsv)    
+    rgb = _val_rgb(rgb)
+    return rgb_to_hsl(rgb)
+
+def hsv_to_cmyk(hsv: tuple) -> tuple:
+    """
+    Convert HSV values to CMYK values.
+
+    Args:
+    - HSV (tuple)
+
+    Returns:
+    - tuple: A tuple containing the CMYK values
+    """
+    rgb = hsv_to_rgb(hsv)    
+    rgb = _val_rgb(rgb)
+    return rgb_to_cmyk(rgb)
+
+def hsv_to_hex(hsv: tuple) -> tuple:
+    """
+    Convert HSV values to hex values.
+
+    Args:
+    - HSV (tuple)
+
+    Returns:
+    - str: Hexadecimal color code.
+    """
+    rgb = hsv_to_rgb(hsv)    
+    rgb = _val_rgb(rgb)
+    return rgb_to_hex(rgb)
+
 def hsv_to_lab(hsv: tuple) -> tuple:
     """
     Convert HSV values to LAB values.
 
     Args:
     - HSV (tuple)
 
     Returns:
     - tuple: A tuple containing the LAB values
     """
-    rgb = hsv_to_rgb(hex)    
+    rgb = hsv_to_rgb(hsv)    
     rgb = _val_rgb(rgb)
     return rgb_to_lab(rgb)
 
 def hsv_to_xyz(hsv: tuple) -> tuple:
     """
     Convert HSV values to XYZ values.
 
     Args:
     - HSV (tuple)
 
     Returns:
     - tuple: A tuple containing the XYZ values
     """
-    rgb = hsv_to_rgb(hex)    
+    rgb = hsv_to_rgb(hsv)    
     rgb = _val_rgb(rgb)
     return rgb_to_xyz(rgb)
 
 
 def rgb_to_hsv(rgb: tuple) -> tuple:
     """
     Convert RGB values to HSV values.
@@ -849,15 +935,15 @@
     return cie94(lab1, lab2)
 
 
 # colorname
 
 def hex_to_colorname(hex_color, naming_standard="html"):
     """
-    Find the closest matching color name for a given hex color in a color name system.
+    Find the closest matching color name for a given hex color in a color name system using the CIEDE2000 formula.
     
     Args:
         hex_color (str): Hex color code.
         naming_standard (str): html, html-ger, x11, color-meanings.com, meodai(color-name Github Project with over 30.000 colors).
 
     Returns:
         str: Closest matching color name.
@@ -882,8 +968,75 @@
             return color_name
         rgb_code = hex_to_rgb(hex_code)
         diff = ciede2000_rgb(rgb_color, rgb_code)
         if diff < min_diff:
             min_diff = diff
             closest_color = color_name
 
-    return closest_color
+    return closest_color
+
+def colorname_to_hex(colorname: str, naming_standard="html"):
+    """
+    Get the hex code of a colorname if it exists in the specified colorname system. Else returns None.  
+
+    Args:
+        colorname (string): colorname.
+        naming_standard (str): html, html-ger, x11, color-meanings.com, meodai(color-name Github Project with over 30.000 colors).
+
+    Returns:
+        str: matching hex code or None.
+    """
+    if naming_standard not in ["html", "html-ger", "x11", "color-meanings.com", "meodai"]:
+        raise ValueError("naming_standard input is not a valid option")
+    
+    # Read data from CSV file
+    color_dict = {}
+    with open(files("colortools") / "data" / f"{naming_standard}.csv", mode='r') as file:
+        reader = csv.reader(file)
+        for row in reader:
+            color_name = row[0]
+            hex_code = row[1]
+            color_dict[color_name] = hex_code
+    
+    for color_name, hex_code in color_dict.items():
+        if colorname.lower == color_name.lower():
+            return hex_code
+        
+    return None
+
+def rgb_to_colorname(rgb: tuple, naming_standard="html"):
+    """
+    Find the closest matching color name for a given rgb color tuple in a color name system.
+    
+    Args:
+        rgb (tuple): rgb tuple.
+        naming_standard (str): html, html-ger, x11, color-meanings.com, meodai(color-name Github Project with over 30.000 colors).
+
+    Returns:
+        str: Closest matching color name.
+    """
+    # validate input
+    _validate_rgb(rgb)
+    if len(rgb) == 4:
+        rgb = (rgb[0], rgb[1], rgb[2])
+        
+    hexc = rgb_to_hex(rgb)
+
+    # conversion
+    colorname = hex_to_colorname(hexc, naming_standard)
+    return colorname
+
+def colorname_to_rgb(colorname: str, naming_standard="html"):
+    """
+    Get the rgb tuple of a colorname if it exists in the specified colorname system. Else returns None.  
+
+    Args:
+        colorname (string): colorname.
+        naming_standard (str): html, html-ger, x11, color-meanings.com, meodai(color-name Github Project with over 30.000 colors).
+
+    Returns:
+        str: matching rgb tuple or None.
+    """
+    hexc = colorname_to_hex(colorname, naming_standard)
+    if hexc is not None:
+        return hex_to_rgb(hexc)
+    return hexc
```

### Comparing `colortools_lentolen-0.0.2/src/colortools/data/color-meanings.com.csv` & `colortools_lentolen-0.0.4/src/colortools/data/color-meanings.com.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/src/colortools/data/html-ger.csv` & `colortools_lentolen-0.0.4/src/colortools/data/html-ger.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/src/colortools/data/html.csv` & `colortools_lentolen-0.0.4/src/colortools/data/html.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/src/colortools/data/meodai.csv` & `colortools_lentolen-0.0.4/src/colortools/data/meodai.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/src/colortools/data/x11.csv` & `colortools_lentolen-0.0.4/src/colortools/data/x11.csv`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/LICENSE.txt` & `colortools_lentolen-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/README.md` & `colortools_lentolen-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - [Documentation](#documentation)
 - [License](#license)
 
 ## Description
 Python package for conversions between common color representations like RGB and HEX and color comparisons using CIE formulas.
 
 ## Features
-### Conversion between common color represantations
+### Conversion between common color representations
 - RGB
 - HEX
 - CMYK
 - HSL
 - HSV
 - LAB
 - XYZ
@@ -31,38 +31,38 @@
 > measure of the perceptual difference between two colors
 - Delta E (ΔE) CIE76 Formula
 - Delta E (ΔE) CIE94 Formula
 - Delta E (ΔE) CIEDE2000 Formula
 
 ## Quickstart
 ### Installation 
-To install from test PyPI with pip:
+To install from PyPI with pip:
 
 ```console
 $ python -m pip install colortools-lentolen
 ```
 
 ### Example usage: 
-Using colortools in a Python script to calculate the CIEDE200 difference between to hex colors.
+Using colortools in a Python script to calculate the CIEDE200 difference between two hex colors.
 ```python
 from colortools import color_utils
 color1 = color_utils.hex_to_rgb("#ddf4ee")
-color2 = color_converter.hex_to_rgb("#88bfb1")
+color2 = color_utils.hex_to_rgb("#88bfb1")
 deltaE = color_utils.ciede2000_rgb(color1, color2)
 ```
 
 ## Documentation
 all color models are represented as tuples except hex codes: e.g: (255,255,255)
 ### color conversion:
 syntax example: 
 ```python
 colortools.color_utils.hex_to_rgb(hex)
 ```
 supported color models: rgb, hex, cmyk, hsl, hsv, lab, xyz, colorname
-> only hex codes can directly be converted to colornames. there are multiple color naming standards availabe: html (standard), html-ger, meodai, x11, [color-meanings.com](https://color-meanings.com).
+> There are multiple color naming standards availabe: html (standard), html-ger, meodai, x11, [color-meanings.com](https://color-meanings.com).
 
 This is how you can for example use the [meodai](https://github.com/meodai/color-names) GitHub color name collection:
 ```python
 colortools.color_utils.hex_to_colorname("#ffffff", "meodai")
 ```
 
 ### color difference:
```

### Comparing `colortools_lentolen-0.0.2/pyproject.toml` & `colortools_lentolen-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colortools_lentolen-0.0.2/PKG-INFO` & `colortools_lentolen-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortools_lentolen
-Version: 0.0.2
+Version: 0.0.4
 Summary: A package to do color conversions and comparisons
 Project-URL: Documentation, https://github.com/LentoLen/colortools#readme
 Project-URL: Issues, https://github.com/LentoLen/colortools/issues
 Project-URL: Source, https://github.com/LentoLen/colortools
 Author-email: LentoLen <len.vnn@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -36,15 +36,15 @@
 - [Documentation](#documentation)
 - [License](#license)
 
 ## Description
 Python package for conversions between common color representations like RGB and HEX and color comparisons using CIE formulas.
 
 ## Features
-### Conversion between common color represantations
+### Conversion between common color representations
 - RGB
 - HEX
 - CMYK
 - HSL
 - HSV
 - LAB
 - XYZ
@@ -53,38 +53,38 @@
 > measure of the perceptual difference between two colors
 - Delta E (ΔE) CIE76 Formula
 - Delta E (ΔE) CIE94 Formula
 - Delta E (ΔE) CIEDE2000 Formula
 
 ## Quickstart
 ### Installation 
-To install from test PyPI with pip:
+To install from PyPI with pip:
 
 ```console
 $ python -m pip install colortools-lentolen
 ```
 
 ### Example usage: 
-Using colortools in a Python script to calculate the CIEDE200 difference between to hex colors.
+Using colortools in a Python script to calculate the CIEDE200 difference between two hex colors.
 ```python
 from colortools import color_utils
 color1 = color_utils.hex_to_rgb("#ddf4ee")
-color2 = color_converter.hex_to_rgb("#88bfb1")
+color2 = color_utils.hex_to_rgb("#88bfb1")
 deltaE = color_utils.ciede2000_rgb(color1, color2)
 ```
 
 ## Documentation
 all color models are represented as tuples except hex codes: e.g: (255,255,255)
 ### color conversion:
 syntax example: 
 ```python
 colortools.color_utils.hex_to_rgb(hex)
 ```
 supported color models: rgb, hex, cmyk, hsl, hsv, lab, xyz, colorname
-> only hex codes can directly be converted to colornames. there are multiple color naming standards availabe: html (standard), html-ger, meodai, x11, [color-meanings.com](https://color-meanings.com).
+> There are multiple color naming standards availabe: html (standard), html-ger, meodai, x11, [color-meanings.com](https://color-meanings.com).
 
 This is how you can for example use the [meodai](https://github.com/meodai/color-names) GitHub color name collection:
 ```python
 colortools.color_utils.hex_to_colorname("#ffffff", "meodai")
 ```
 
 ### color difference:
```

