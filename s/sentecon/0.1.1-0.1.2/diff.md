# Comparing `tmp/sentecon-0.1.1-py3-none-any.whl.zip` & `tmp/sentecon-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2928 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-07 02:08 sentecon/__init__.py
--rw-rw-r--  2.0 unx     4839 b- defN 23-Jul-07 03:10 sentecon/core.py
--rw-rw-r--  2.0 unx      411 b- defN 23-Jul-07 03:12 sentecon-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 03:12 sentecon-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-07 03:12 sentecon-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      448 b- defN 23-Jul-07 03:12 sentecon-0.1.1.dist-info/RECORD
-6 files, 5825 bytes uncompressed, 2114 bytes compressed:  63.7%
+Zip file size: 2966 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-07 03:28 sentecon/__init__.py
+-rw-rw-r--  2.0 unx     4937 b- defN 23-Jul-07 03:49 sentecon/core.py
+-rw-rw-r--  2.0 unx      411 b- defN 23-Jul-07 03:50 sentecon-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 03:50 sentecon-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-07 03:50 sentecon-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      448 b- defN 23-Jul-07 03:50 sentecon-0.1.2.dist-info/RECORD
+6 files, 5923 bytes uncompressed, 2152 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sentecon/__init__.py
 Comment: 
 
 Filename: sentecon/core.py
 Comment: 
 
-Filename: sentecon-0.1.1.dist-info/METADATA
+Filename: sentecon-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: sentecon-0.1.1.dist-info/WHEEL
+Filename: sentecon-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: sentecon-0.1.1.dist-info/top_level.txt
+Filename: sentecon-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sentecon-0.1.1.dist-info/RECORD
+Filename: sentecon-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sentecon/core.py

```diff
@@ -11,27 +11,30 @@
 import torch
 import warnings
 warnings.filterwarnings("ignore")
 
 tqdm.pandas()
 
 class SenteCon:
-    def __init__(self, lexicon, lm, lm_library, data_dir, liwc_path, num_centroids=1, seed=230706):
+    def __init__(self, lexicon, lm, lm_library, data_dir, liwc_path=None, num_centroids=1, seed=230706):
         self.device = 'cuda' if cuda.is_available() else 'cpu'
         
-        self.data_dir = data_dir
+        self.data_dir = 'data'
         self.lexicon = lexicon
         self.lm = lm
         self.lm_library = lm_library
         self.num_centroids = num_centroids
 
         if self.lexicon == 'Empath':
             lexicon = Empath()
             self.category_names = list(lexicon.cats.keys())
         elif self.lexicon == 'LIWC':
+            if liwc_path == None:
+                print('No LIWC path provided')
+                exit()
             parse, category_names = liwc.load_token_parser(liwc_path)
             self.category_names = category_names[21:]
 
         if self.num_centroids > 1:
             self.category_headers = []
             for cluster in range(self.num_centroids):
                 self.category_headers += ['{}_c{}'.format(category, cluster) for category in category_names]
@@ -59,15 +62,15 @@
                 centroids[category] = cat_embeds.mean(axis=0)
             else:
                 cluster_model = KMeans(n_clusters=self.num_centroids, random_state=seed)
                 try:
                     cluster_model.fit(cat_embeds)
                 except:
                     print('Empty centroids')
-                    pdb.set_trace()
+                    exit()
                 clusters = cluster_model.predict(cat_embeds)
                 for cluster in set(clusters):
                     centroids['{}_c{}'.format(category, cluster)] = cat_embeds[clusters == cluster].mean(axis=0)  
 
             centroids = pd.DataFrame.from_dict(centroids)
 
         return centroids
```

