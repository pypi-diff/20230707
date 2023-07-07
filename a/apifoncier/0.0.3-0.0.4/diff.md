# Comparing `tmp/apifoncier-0.0.3.tar.gz` & `tmp/apifoncier-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "apifoncier-0.0.4.tar", last modified: Fri Jul  7 13:10:51 2023, max compression
```

## Comparing `apifoncier-0.0.3.tar` & `apifoncier-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 apifoncier-0.0.3/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apifoncier-0.0.3/src/__init__.py
--rw-r--r--   0        0        0    11958 2020-02-02 00:00:00.000000 apifoncier-0.0.3/src/apifoncier.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 apifoncier-0.0.3/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 apifoncier-0.0.3/LICENSE
--rw-r--r--   0        0        0     9344 2020-02-02 00:00:00.000000 apifoncier-0.0.3/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 apifoncier-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     9683 2020-02-02 00:00:00.000000 apifoncier-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 13:10:51.176734 apifoncier-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-07 08:37:11.000000 apifoncier-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     9979 2023-07-07 13:10:51.175983 apifoncier-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.4/README.md
+-rw-rw-rw-   0        0        0      855 2023-07-07 13:08:52.000000 apifoncier-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:10:51.176734 apifoncier-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 13:10:51.160434 apifoncier-0.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-07-07 08:27:04.000000 apifoncier-0.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:10:51.172355 apifoncier-0.0.4/src/apifoncier.egg-info/
+-rw-rw-rw-   0        0        0     9979 2023-07-07 13:10:51.000000 apifoncier-0.0.4/src/apifoncier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-07 13:10:51.000000 apifoncier-0.0.4/src/apifoncier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:10:51.000000 apifoncier-0.0.4/src/apifoncier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-07 13:10:51.000000 apifoncier-0.0.4/src/apifoncier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 13:10:51.000000 apifoncier-0.0.4/src/apifoncier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11958 2023-07-07 11:40:21.000000 apifoncier-0.0.4/src/apifoncier.py
```

### Comparing `apifoncier-0.0.3/src/apifoncier.py` & `apifoncier-0.0.4/src/apifoncier.py`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.3/LICENSE` & `apifoncier-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.3/README.md` & `apifoncier-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.3/PKG-INFO` & `apifoncier-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,235 +1,236 @@
-Metadata-Version: 2.1
-Name: apifoncier
-Version: 0.0.3
-Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
-Project-URL: Homepage, https://github.com/rcadot/py.apifoncier
-Project-URL: Bug Tracker, https://github.com/rcadot/py.apifoncier/issues
-Author-email: Romain Cadot <romain.cadot@cerema.fr>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
- 
-
-> 🚧 Avertissement
->
-> Il s’agit d’une version de développement. Des modifications sur les
-> fonctions peuvent intervenir.
->
-> Consultez l’article
-> [Changements]()
-> pour plus d’informations.
-
-# Présentation du package
-
-Grâce au package `apifoncier`, vous pouvez interroger les
-différentes bases de données foncières produites par le Cerema et la
-DGALN directement depuis `python` ! *Une partie des données est interrogeable
-uniquement avec un accès restreint lié à vos droits. Pensez à vous
-rendre sur
-[ConsultDF](https://consultdf.cerema.fr/consultdf/services/apidf) pour
-obtenir un accès.*
-
-# Installation
-
-Vous pouvez installer `apifoncier` depuis
-[GitHub](https://github.com/) avec le code suivant :
-
-``` python
-pip install apifoncier
-```
-
-# Fonctions et données disponibles
-
-Vous trouverez ci-dessous l’ensemble des informations sur les jeux de
-données disponibles grâce à ce package. N’hésitez pas à parcourir
-l’ensemble des articles de la documentation ainsi que les pages dédiées
-à chaque fonction.
-
-Retrouvez également des fonctions de valorisation des données telles que
-des [graphiques](), [cartographies dynamiques]() ou encore [tableaux]().
-
-> ### À noter
->
-> À la différence de l’utilisation de l’API en directe, le package
-> permet d’obtenir les données pour le périmètre de votre choix. Vous
-> pouvez ainsi fournir une liste ou un vecteur de `code_insee`,
-> `code_epci`, etc. sans limite de volume.
-
-## Indicateurs de consommation d’espace (accès libre)
-
-> La lutte contre la consommation excessive d’espace est un objectif
-> prioritaire des dernières lois en matière d’urbanisme. Cependant, il
-> est difficile de définir comme « excessive » la consommation sans
-> disposer de moyens de mesure adaptés. Dans ce cadre, le Cerema produit
-> annuellement des données sur la consommation d’espaces à l’aide des
-> Fichiers fonciers.
->
-> *[Pour plus d’informations sur la consommation
-> d’espaces](https://artificialisation.developpement-durable.gouv.fr/suivi-consommation-espaces-naf)*
-
-Le package `{apifoncier}` permet d’interroger l’ensemble du territoire
-français afin d’obtenir les indicateurs de consommation d’espace pour la
-période comprise entre une deux années à l’échelle communale ou
-départementale.
-
-**Plus d’informations sur les fonctions disponibles en allant l’[article
-dédidé]()**
-
-## Indicateurs de prix (accès libre)
-
-> La base de données DV3F facilite l’observation des marchés et permet
-> de produire des indicateurs de prix et de volumes de transactions à
-> différentes échelles géographiques afin d’apprécier et d’étudier les
-> marchés fonciers et immobiliers d’un territoire.
->
-> Retrouvez l’ensemble de la documentation en suivant [ce
-> lien](https://doc-datafoncier.cerema.fr/dv3f/tuto/indicateurs_agreges).
-
-Les indicateurs de prix sont disponibles annuellement et de manière
-triennale à plusieurs échelles :
-
-- Régions ;
-- Départements ;
-- Aires d’attractivités des villes ;
-- EPCI ;
-- Communes.
-
-La période proposée court de 2010 à 2022 avec une exhaustivité moindre
-sur les derniers semestres.
-
-Les indicateurs proposés dans la version 2023-1 de DV3F utilisent les
-périmètres administratifs au 1er janvier 2022.
-
-**Plus d’informations sur les fonctions disponibles en allant sur
-l’[article dédié]().**
-
-## Cartofriches (accès libre)
-
-> Les travaux effectués par le Cerema pour constituer un premier
-> inventaire national ont permis de montrer la possibilité de
-> pré-identifier une partie des friches, mais ils montrent aussi les
-> limites de l’approche nationale. En effet, sur un sujet aussi complexe
-> que les friches, les bases nationales manquent d’exhaustivité et de
-> mise à jour. La comparaison de la base nationale avec des inventaires
-> locaux met en évidence l’absence de définition réglementaire d’une
-> friche, et le peu de mise à jour de certaines informations nationales.
->
-> Ainsi, si une base nationale permet d’avoir des informations homogènes
-> sur le territoire métropolitain, une base de données consolidées
-> nécessite la contribution large de nombreux acteurs proches du
-> terrain, et l’agglomération de données issues d’observatoires locaux,
-> en partageant un minimum de concepts.
->
-> [Plus d’informations sur
-> cartofriches](https://artificialisation.developpement-durable.gouv.fr/cartofriches/donnees-utilisees)
-
-**Plus d’informations sur les fonctions disponibles en allant sur
-l’[article dédié]()**
-
-## DVF+ (accès libre)
-
-> La DGALN et le Cerema propose “DVF+ open-data”, qui permet d’accéder
-> librement aux données DV3F sous la forme d’une base de données
-> géolocalisée aisément exploitable pour l’observation des marchés
-> fonciers et immobiliers.
->
-> La structuration de la donnée DVF proposée s’appuie sur le modèle de
-> données partagé dit “DVF+”, issu des travaux menés à l’initiative du
-> groupe national DVF et qui existe depuis 2013. Ce modèle, développé
-> pour faciliter les analyses, fournit notamment une table des mutations
-> dans laquelle chaque ligne correspond aux informations et à la
-> localisation d’une transaction.
->
-> La géolocalisation s’appuie sur les différents millésimes du Plan
-> cadastral informatisé également disponibles en open-data sur
-> data.gouv.fr.
->
-> Chacune des variables du modèle DVF+ est calculée uniquement à partir
-> des données brutes de DVF. Les variables calculées s’appliquent sur
-> l’ensemble du territoire et relèvent d’une méthodologie partagée. Il
-> n’y a pas de données exogènes à ce stade hormis les données de
-> géolocalisation issue du PCI Vecteur. A noter que le modèle DVF+
-> constitue également le socle pour la constitution de la base de
-> données DV3F.
->
-> [Pour en savoir plus sur DVF+](http://doc-datafoncier.cerema.fr/dv3f/tuto/objectif_tutoriel)
-
-**Plus d’informations sur les fonctions disponibles en allant sur
-l’[article dédié]()**
-
-## DV3F (accès restreint)
-
-> L’amélioration du fonctionnement des marchés fonciers et immobiliers
-> en France, la recherche d’une meilleure transparence sur les prix des
-> transactions, nécessite aujourd’hui l’accès à une donnée large et
-> aussi complète que possible sur les transactions, les biens et les
-> prix.
->
-> La Direction Générale des Finances Publiques (DGFiP) propose
-> gratuitement et en open-data le fichier “Demande de Valeurs Foncières”
-> (DVF) qui recense l’ensemble des mutations foncières à titre onéreux
-> publiées dans les services de la publicité foncière.
->
-> Cette donnée est riche et précise mais reste néanmoins difficilement
-> exploitable.
->
-> C’est pourquoi le Ministère du Logement a missionné le Cerema pour
-> travailler à une structuration de la donnée DVF en y associant des
-> données foncières complémentaires permettant des analyses plus fines.
->
-> Ces travaux ont conduit à la constitution de la base de données DV3F
-> ainsi qu’à des outils facilitant son exploitation.
->
-> Pour les acteurs ne pouvant bénéficier de DV3F, les données open-data
-> sont également disponibles librement sous un format “DVF+ - open-data”
-> structuré et géolocalisé.
->
-> [Plus d’informations sur DV3F](https://datafoncier.cerema.fr/dv3f)
-
-**Plus d’informations sur les fonctions disponibles en allant sur
-l’[article dédié]().**
-
-## Fichiers fonciers (accès restreint)
-
-> Depuis 2009, le Cerema retraite, géolocalise et enrichit les Fichiers
-> fonciers de la Direction Générale des Finances Publiques (DGFiP) pour
-> le compte du ministère en charge du Logement, des services de la
-> Direction Générale de l’Aménagement, du Logement et de la Nature
-> (DGALN), afin de permettre aux acteurs publics de réaliser facilement
-> des analyses fines et comparables sur leur territoire.
->
-> Les nouvelles politiques publiques et les stratégies d’aménagement
-> foncier amènent de nombreux acteurs publics à se saisir de cette base
-> de données nationale et complète.
->
-> Les Fichiers fonciers décrivent de manière détaillée le foncier, les
-> locaux ainsi que les différents droits de propriété qui leur sont
-> liés. Ils sont aujourd’hui devenus essentiels dans de nombreux
-> domaines tels que l’occupation du sol, l’aménagement, le logement, le
-> risque et l’énergie.
->
-> La base est disponible sous forme de millésimes via deux produits :
->
-> - les tables principales
-> - les tables agrégées (tables communales, carroyages, etc.).
->
-> [Plus d’informations sur les fichiers
-> fonciers](https://datafoncier.cerema.fr/fichiers-fonciers)
-
-**Plus d’informations sur les fonctions disponibles en allant sur
-l’[article dédié]().**
-
-# Ressources
-
-Pour retrouver toutes les informations sur les données foncières :
-[datafoncier.cerema.fr](datafoncier.cerema.fr)
-
-Dictionnaire et documentation sur toutes les variables :
-[doc-datafoncier.cerema.fr](doc-datafoncier.cerema.fr)
-
-[Pour en savoir plus sur l’API données foncières du
-cerema.](https://apidf-preprod.cerema.fr/swagger/)
+Metadata-Version: 2.1
+Name: apifoncier
+Version: 0.0.4
+Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
+Author-email: Romain Cadot <romain.cadot@cerema.fr>
+Project-URL: Homepage, https://github.com/rcadot/py.apifoncier
+Project-URL: Bug Tracker, https://github.com/rcadot/py.apifoncier/issues
+Keywords: api,foncier,cerema,dv3f,friches,artificialisation
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ 
+
+> 🚧 Avertissement
+>
+> Il s’agit d’une version de développement. Des modifications sur les
+> fonctions peuvent intervenir.
+>
+> Consultez l’article
+> [Changements]()
+> pour plus d’informations.
+
+# Présentation du package
+
+Grâce au package `apifoncier`, vous pouvez interroger les
+différentes bases de données foncières produites par le Cerema et la
+DGALN directement depuis `python` ! *Une partie des données est interrogeable
+uniquement avec un accès restreint lié à vos droits. Pensez à vous
+rendre sur
+[ConsultDF](https://consultdf.cerema.fr/consultdf/services/apidf) pour
+obtenir un accès.*
+
+# Installation
+
+Vous pouvez installer `apifoncier` depuis
+[GitHub](https://github.com/) avec le code suivant :
+
+``` python
+pip install apifoncier
+```
+
+# Fonctions et données disponibles
+
+Vous trouverez ci-dessous l’ensemble des informations sur les jeux de
+données disponibles grâce à ce package. N’hésitez pas à parcourir
+l’ensemble des articles de la documentation ainsi que les pages dédiées
+à chaque fonction.
+
+Retrouvez également des fonctions de valorisation des données telles que
+des [graphiques](), [cartographies dynamiques]() ou encore [tableaux]().
+
+> ### À noter
+>
+> À la différence de l’utilisation de l’API en directe, le package
+> permet d’obtenir les données pour le périmètre de votre choix. Vous
+> pouvez ainsi fournir une liste ou un vecteur de `code_insee`,
+> `code_epci`, etc. sans limite de volume.
+
+## Indicateurs de consommation d’espace (accès libre)
+
+> La lutte contre la consommation excessive d’espace est un objectif
+> prioritaire des dernières lois en matière d’urbanisme. Cependant, il
+> est difficile de définir comme « excessive » la consommation sans
+> disposer de moyens de mesure adaptés. Dans ce cadre, le Cerema produit
+> annuellement des données sur la consommation d’espaces à l’aide des
+> Fichiers fonciers.
+>
+> *[Pour plus d’informations sur la consommation
+> d’espaces](https://artificialisation.developpement-durable.gouv.fr/suivi-consommation-espaces-naf)*
+
+Le package `{apifoncier}` permet d’interroger l’ensemble du territoire
+français afin d’obtenir les indicateurs de consommation d’espace pour la
+période comprise entre une deux années à l’échelle communale ou
+départementale.
+
+**Plus d’informations sur les fonctions disponibles en allant l’[article
+dédidé]()**
+
+## Indicateurs de prix (accès libre)
+
+> La base de données DV3F facilite l’observation des marchés et permet
+> de produire des indicateurs de prix et de volumes de transactions à
+> différentes échelles géographiques afin d’apprécier et d’étudier les
+> marchés fonciers et immobiliers d’un territoire.
+>
+> Retrouvez l’ensemble de la documentation en suivant [ce
+> lien](https://doc-datafoncier.cerema.fr/dv3f/tuto/indicateurs_agreges).
+
+Les indicateurs de prix sont disponibles annuellement et de manière
+triennale à plusieurs échelles :
+
+- Régions ;
+- Départements ;
+- Aires d’attractivités des villes ;
+- EPCI ;
+- Communes.
+
+La période proposée court de 2010 à 2022 avec une exhaustivité moindre
+sur les derniers semestres.
+
+Les indicateurs proposés dans la version 2023-1 de DV3F utilisent les
+périmètres administratifs au 1er janvier 2022.
+
+**Plus d’informations sur les fonctions disponibles en allant sur
+l’[article dédié]().**
+
+## Cartofriches (accès libre)
+
+> Les travaux effectués par le Cerema pour constituer un premier
+> inventaire national ont permis de montrer la possibilité de
+> pré-identifier une partie des friches, mais ils montrent aussi les
+> limites de l’approche nationale. En effet, sur un sujet aussi complexe
+> que les friches, les bases nationales manquent d’exhaustivité et de
+> mise à jour. La comparaison de la base nationale avec des inventaires
+> locaux met en évidence l’absence de définition réglementaire d’une
+> friche, et le peu de mise à jour de certaines informations nationales.
+>
+> Ainsi, si une base nationale permet d’avoir des informations homogènes
+> sur le territoire métropolitain, une base de données consolidées
+> nécessite la contribution large de nombreux acteurs proches du
+> terrain, et l’agglomération de données issues d’observatoires locaux,
+> en partageant un minimum de concepts.
+>
+> [Plus d’informations sur
+> cartofriches](https://artificialisation.developpement-durable.gouv.fr/cartofriches/donnees-utilisees)
+
+**Plus d’informations sur les fonctions disponibles en allant sur
+l’[article dédié]()**
+
+## DVF+ (accès libre)
+
+> La DGALN et le Cerema propose “DVF+ open-data”, qui permet d’accéder
+> librement aux données DV3F sous la forme d’une base de données
+> géolocalisée aisément exploitable pour l’observation des marchés
+> fonciers et immobiliers.
+>
+> La structuration de la donnée DVF proposée s’appuie sur le modèle de
+> données partagé dit “DVF+”, issu des travaux menés à l’initiative du
+> groupe national DVF et qui existe depuis 2013. Ce modèle, développé
+> pour faciliter les analyses, fournit notamment une table des mutations
+> dans laquelle chaque ligne correspond aux informations et à la
+> localisation d’une transaction.
+>
+> La géolocalisation s’appuie sur les différents millésimes du Plan
+> cadastral informatisé également disponibles en open-data sur
+> data.gouv.fr.
+>
+> Chacune des variables du modèle DVF+ est calculée uniquement à partir
+> des données brutes de DVF. Les variables calculées s’appliquent sur
+> l’ensemble du territoire et relèvent d’une méthodologie partagée. Il
+> n’y a pas de données exogènes à ce stade hormis les données de
+> géolocalisation issue du PCI Vecteur. A noter que le modèle DVF+
+> constitue également le socle pour la constitution de la base de
+> données DV3F.
+>
+> [Pour en savoir plus sur DVF+](http://doc-datafoncier.cerema.fr/dv3f/tuto/objectif_tutoriel)
+
+**Plus d’informations sur les fonctions disponibles en allant sur
+l’[article dédié]()**
+
+## DV3F (accès restreint)
+
+> L’amélioration du fonctionnement des marchés fonciers et immobiliers
+> en France, la recherche d’une meilleure transparence sur les prix des
+> transactions, nécessite aujourd’hui l’accès à une donnée large et
+> aussi complète que possible sur les transactions, les biens et les
+> prix.
+>
+> La Direction Générale des Finances Publiques (DGFiP) propose
+> gratuitement et en open-data le fichier “Demande de Valeurs Foncières”
+> (DVF) qui recense l’ensemble des mutations foncières à titre onéreux
+> publiées dans les services de la publicité foncière.
+>
+> Cette donnée est riche et précise mais reste néanmoins difficilement
+> exploitable.
+>
+> C’est pourquoi le Ministère du Logement a missionné le Cerema pour
+> travailler à une structuration de la donnée DVF en y associant des
+> données foncières complémentaires permettant des analyses plus fines.
+>
+> Ces travaux ont conduit à la constitution de la base de données DV3F
+> ainsi qu’à des outils facilitant son exploitation.
+>
+> Pour les acteurs ne pouvant bénéficier de DV3F, les données open-data
+> sont également disponibles librement sous un format “DVF+ - open-data”
+> structuré et géolocalisé.
+>
+> [Plus d’informations sur DV3F](https://datafoncier.cerema.fr/dv3f)
+
+**Plus d’informations sur les fonctions disponibles en allant sur
+l’[article dédié]().**
+
+## Fichiers fonciers (accès restreint)
+
+> Depuis 2009, le Cerema retraite, géolocalise et enrichit les Fichiers
+> fonciers de la Direction Générale des Finances Publiques (DGFiP) pour
+> le compte du ministère en charge du Logement, des services de la
+> Direction Générale de l’Aménagement, du Logement et de la Nature
+> (DGALN), afin de permettre aux acteurs publics de réaliser facilement
+> des analyses fines et comparables sur leur territoire.
+>
+> Les nouvelles politiques publiques et les stratégies d’aménagement
+> foncier amènent de nombreux acteurs publics à se saisir de cette base
+> de données nationale et complète.
+>
+> Les Fichiers fonciers décrivent de manière détaillée le foncier, les
+> locaux ainsi que les différents droits de propriété qui leur sont
+> liés. Ils sont aujourd’hui devenus essentiels dans de nombreux
+> domaines tels que l’occupation du sol, l’aménagement, le logement, le
+> risque et l’énergie.
+>
+> La base est disponible sous forme de millésimes via deux produits :
+>
+> - les tables principales
+> - les tables agrégées (tables communales, carroyages, etc.).
+>
+> [Plus d’informations sur les fichiers
+> fonciers](https://datafoncier.cerema.fr/fichiers-fonciers)
+
+**Plus d’informations sur les fonctions disponibles en allant sur
+l’[article dédié]().**
+
+# Ressources
+
+Pour retrouver toutes les informations sur les données foncières :
+[datafoncier.cerema.fr](datafoncier.cerema.fr)
+
+Dictionnaire et documentation sur toutes les variables :
+[doc-datafoncier.cerema.fr](doc-datafoncier.cerema.fr)
+
+[Pour en savoir plus sur l’API données foncières du
+cerema.](https://apidf-preprod.cerema.fr/swagger/)
```

