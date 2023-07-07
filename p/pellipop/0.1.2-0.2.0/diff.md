# Comparing `tmp/pellipop-0.1.2.tar.gz` & `tmp/pellipop-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pellipop-0.1.2.tar", last modified: Thu Jul  6 16:43:36 2023, max compression
+gzip compressed data, was "pellipop-0.2.0.tar", last modified: Fri Jul  7 08:39:15 2023, max compression
```

## Comparing `pellipop-0.1.2.tar` & `pellipop-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:36.401914 pellipop-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:36.397915 pellipop-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:36.397915 pellipop-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-06 16:43:23.000000 pellipop-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-06 16:43:23.000000 pellipop-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 16:43:36.401914 pellipop-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-06 16:43:23.000000 pellipop-0.1.2/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-06 16:43:23.000000 pellipop-0.1.2/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:36.397915 pellipop-0.1.2/pellipop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:23.000000 pellipop-0.1.2/pellipop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-06 16:43:23.000000 pellipop-0.1.2/pellipop/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:36.401914 pellipop-0.1.2/pellipop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 16:43:36.000000 pellipop-0.1.2/pellipop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-06 16:43:36.000000 pellipop-0.1.2/pellipop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:43:36.000000 pellipop-0.1.2/pellipop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 16:43:36.000000 pellipop-0.1.2/pellipop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 16:43:36.000000 pellipop-0.1.2/pellipop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 16:43:36.000000 pellipop-0.1.2/pellipop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 16:43:23.000000 pellipop-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:43:36.401914 pellipop-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-06 16:43:23.000000 pellipop-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.252168 pellipop-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.248167 pellipop-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.248167 pellipop-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 08:39:04.000000 pellipop-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-07 08:39:04.000000 pellipop-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 08:39:15.252168 pellipop-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 08:39:04.000000 pellipop-0.2.0/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 08:39:04.000000 pellipop-0.2.0/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.248167 pellipop-0.2.0/pellipop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:04.000000 pellipop-0.2.0/pellipop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-07 08:39:04.000000 pellipop-0.2.0/pellipop/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:39:15.252168 pellipop-0.2.0/pellipop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 08:39:15.000000 pellipop-0.2.0/pellipop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 08:39:04.000000 pellipop-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:39:15.252168 pellipop-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-07 08:39:04.000000 pellipop-0.2.0/setup.py
```

### Comparing `pellipop-0.1.2/.github/workflows/python-publish.yml` & `pellipop-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pellipop-0.1.2/.gitignore` & `pellipop-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pellipop-0.1.2/PKG-INFO` & `pellipop-0.2.0/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: pellipop
-Version: 0.1.2
-License: MPL-2.0 license
-Description-Content-Type: text/markdown
-
 # Pellipop
 
 ## Installation
 
 `pip install pellipop`
 
 ## Usage
@@ -23,16 +17,16 @@
 - `".wmv"`
 - `".webm"`
 - `".mkv"`
 - `".svf"`
 
 Il se lance avec `pellipop` dans un terminal, par défaut les vidéos sont cherchées dans le dossier où la commande est lancée, et les images créées sont également stockées au même endroit. Les paramètres peuvent toutefois être changés:
 
-- `--input_folder` : pour spécifier le dossier d'entrée où chercher les vidéos
-- `--output_folder` : pour spécifier l'endroit où stocker les images en sortie
+- `--input` : pour spécifier le dossier d'entrée où chercher les vidéos
+- `--output` : pour spécifier l'endroit où stocker les images en sortie
 - `--frequency` : pour spécifier la fréquence temporelle de capture des images (en s)
 - `--remove_duplicates` : permet de supprimer les doublons d'images pour un même film, note: cela peut ralentir la conversion.
 
 Exemple d'usage:
-`pellipop --input_folder C:\Users\Utilisateur\Videos\Captures --output_folder D:\Users\Bureau\Output --frequency 1 --remove_duplicates True`
+`pellipop --input C:\Users\Utilisateur\Videos\Captures --output D:\Users\Bureau\Output --frequency 1 --remove_duplicates`
 
-> Note: Le temps de découpe de chaque vidéo dépend de la qualité de la vidéo découpée.
+> Note: Le temps de découpe de chaque vidéo dépend de la qualité de la vidéo découpée.
```

### Comparing `pellipop-0.1.2/Readme.md` & `pellipop-0.2.0/description.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 - `".wmv"`
 - `".webm"`
 - `".mkv"`
 - `".svf"`
 
 Il se lance avec `pellipop` dans un terminal, par défaut les vidéos sont cherchées dans le dossier où la commande est lancée, et les images créées sont également stockées au même endroit. Les paramètres peuvent toutefois être changés:
 
-- `--input_folder` : pour spécifier le dossier d'entrée où chercher les vidéos
-- `--output_folder` : pour spécifier l'endroit où stocker les images en sortie
+- `--input` : pour spécifier le dossier d'entrée où chercher les vidéos
+- `--output` : pour spécifier l'endroit où stocker les images en sortie
 - `--frequency` : pour spécifier la fréquence temporelle de capture des images (en s)
 - `--remove_duplicates` : permet de supprimer les doublons d'images pour un même film, note: cela peut ralentir la conversion.
 
 Exemple d'usage:
-`pellipop --input_folder C:\Users\Utilisateur\Videos\Captures --output_folder D:\Users\Bureau\Output --frequency 1 --remove_duplicates True`
+`pellipop --input C:\Users\Utilisateur\Videos\Captures --output D:\Users\Bureau\Output --frequency 1 --remove_duplicates`
 
 > Note: Le temps de découpe de chaque vidéo dépend de la qualité de la vidéo découpée.
```

### Comparing `pellipop-0.1.2/description.md` & `pellipop-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: pellipop
+Version: 0.2.0
+License: MPL-2.0 license
+Description-Content-Type: text/markdown
+
 # Pellipop
 
 ## Installation
 
 `pip install pellipop`
 
 ## Usage
@@ -17,16 +23,16 @@
 - `".wmv"`
 - `".webm"`
 - `".mkv"`
 - `".svf"`
 
 Il se lance avec `pellipop` dans un terminal, par défaut les vidéos sont cherchées dans le dossier où la commande est lancée, et les images créées sont également stockées au même endroit. Les paramètres peuvent toutefois être changés:
 
-- `--input_folder` : pour spécifier le dossier d'entrée où chercher les vidéos
-- `--output_folder` : pour spécifier l'endroit où stocker les images en sortie
+- `--input` : pour spécifier le dossier d'entrée où chercher les vidéos
+- `--output` : pour spécifier l'endroit où stocker les images en sortie
 - `--frequency` : pour spécifier la fréquence temporelle de capture des images (en s)
 - `--remove_duplicates` : permet de supprimer les doublons d'images pour un même film, note: cela peut ralentir la conversion.
 
 Exemple d'usage:
-`pellipop --input_folder C:\Users\Utilisateur\Videos\Captures --output_folder D:\Users\Bureau\Output --frequency 1 --remove_duplicates True`
+`pellipop --input C:\Users\Utilisateur\Videos\Captures --output D:\Users\Bureau\Output --frequency 1 --remove_duplicates`
 
-> Note: Le temps de découpe de chaque vidéo dépend de la qualité de la vidéo découpée.
+> Note: Le temps de découpe de chaque vidéo dépend de la qualité de la vidéo découpée.
```

### Comparing `pellipop-0.1.2/pellipop/main.py` & `pellipop-0.2.0/pellipop/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     #Note : la valeur 500 (minutes)*60 (pour passer en secondes) est une valeur aléatoire, l'idée est juste de donnée une longueur max de film au-delà de laquelle on ne regarde pas. Mais si le film est plus court ça ne semble pas poser de soucis.
 
     print("Travail terminé !")
 
 def start():
     #Possibilité de paramétrage dans le terminal/l'invite de commandes
     parser = argparse.ArgumentParser()
-    parser.add_argument("--input_folder", type=str, help="Dossier racine contenant les vidéos", nargs='?', const=os.getcwd())
-    parser.add_argument("--frequency", type=int, help="Définition de l'intervalle de temps (en secondes) à laquelle réaliser des captures d'écran. Il faut simplement indiqué une valeur numérique.", nargs='?', const=5)
-    parser.add_argument("--output_folder", type=str, help="Dossier de sortie pour les images extraites", nargs='?', const=os.getcwd())
-    parser.add_argument("--remove_duplicates", type=bool, help="Permet de supprimer les doublons d'images pour un même film en utilisant l'algorithme average hash", nargs='?', const=False)
+    parser.add_argument("--input", type=str, help="Dossier racine contenant les vidéos", default=os.getcwd())
+    parser.add_argument("--frequency", type=int, help="Définition de l'intervalle de temps (en secondes) à laquelle réaliser des captures d'écran. Il faut simplement indiqué une valeur numérique.", default=5)
+    parser.add_argument("--output", type=str, help="Dossier de sortie pour les images extraites", default=os.getcwd())
+    parser.add_argument("--remove_duplicates", type=bool, help="Permet de supprimer les doublons d'images pour un même film en utilisant l'algorithme average hash", default=False, nargs='?', const=True)
     args = parser.parse_args()
 
-    main(input_folder=args.input_folder, intervalle_de_temps=args.frequency, output_folder=args.output_folder, remove_duplicates=args.remove_duplicates)
+    main(input_folder=args.input, intervalle_de_temps=args.frequency, output_folder=args.output, remove_duplicates=args.remove_duplicates)
 
 if __name__ == "__main__":
     start()
```

### Comparing `pellipop-0.1.2/pellipop.egg-info/PKG-INFO` & `pellipop-0.2.0/pellipop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pellipop
-Version: 0.1.2
+Version: 0.2.0
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Pellipop
 
 ## Installation
 
@@ -23,16 +23,16 @@
 - `".wmv"`
 - `".webm"`
 - `".mkv"`
 - `".svf"`
 
 Il se lance avec `pellipop` dans un terminal, par défaut les vidéos sont cherchées dans le dossier où la commande est lancée, et les images créées sont également stockées au même endroit. Les paramètres peuvent toutefois être changés:
 
-- `--input_folder` : pour spécifier le dossier d'entrée où chercher les vidéos
-- `--output_folder` : pour spécifier l'endroit où stocker les images en sortie
+- `--input` : pour spécifier le dossier d'entrée où chercher les vidéos
+- `--output` : pour spécifier l'endroit où stocker les images en sortie
 - `--frequency` : pour spécifier la fréquence temporelle de capture des images (en s)
 - `--remove_duplicates` : permet de supprimer les doublons d'images pour un même film, note: cela peut ralentir la conversion.
 
 Exemple d'usage:
-`pellipop --input_folder C:\Users\Utilisateur\Videos\Captures --output_folder D:\Users\Bureau\Output --frequency 1 --remove_duplicates True`
+`pellipop --input C:\Users\Utilisateur\Videos\Captures --output D:\Users\Bureau\Output --frequency 1 --remove_duplicates`
 
 > Note: Le temps de découpe de chaque vidéo dépend de la qualité de la vidéo découpée.
```

### Comparing `pellipop-0.1.2/setup.py` & `pellipop-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "pellipop"
-VERSION = "0.1.2"
+VERSION = "0.2.0"
 
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
```

