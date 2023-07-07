# Comparing `tmp/vlite-0.1.4.tar.gz` & `tmp/vlite-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.1.4.tar", last modified: Tue Jul  4 15:15:50 2023, max compression
+gzip compressed data, was "vlite-0.1.7.tar", last modified: Fri Jul  7 06:27:15 2023, max compression
```

## Comparing `vlite-0.1.4.tar` & `vlite-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 15:15:50.779893 vlite-0.1.4/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 15:15:50.779743 vlite-0.1.4/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.4/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 15:15:50.779951 vlite-0.1.4/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-04 15:15:30.000000 vlite-0.1.4/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 15:15:50.778784 vlite-0.1.4/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       23 2023-07-04 08:27:33.000000 vlite-0.1.4/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     2626 2023-07-04 15:11:01.000000 vlite-0.1.4/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     2611 2023-07-04 15:11:23.000000 vlite-0.1.4/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     3041 2023-07-04 15:13:56.000000 vlite-0.1.4/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 15:15:50.779545 vlite-0.1.4/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      224 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-07 06:27:15.765326 vlite-0.1.7/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-07 06:27:15.765175 vlite-0.1.7/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     1547 2023-07-04 23:54:37.000000 vlite-0.1.7/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-07 06:27:15.765383 vlite-0.1.7/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-07 06:23:53.000000 vlite-0.1.7/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-07 06:27:15.764253 vlite-0.1.7/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       23 2023-07-04 08:27:33.000000 vlite-0.1.7/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     2626 2023-07-04 15:11:01.000000 vlite-0.1.7/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     3278 2023-07-06 23:49:16.000000 vlite-0.1.7/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     3041 2023-07-04 15:13:56.000000 vlite-0.1.7/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-07 06:27:15.764963 vlite-0.1.7/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      224 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/top_level.txt
```

### Comparing `vlite-0.1.4/vlite/main.py` & `vlite-0.1.7/vlite/main.py`

 * *Files identical despite different names*

### Comparing `vlite-0.1.4/vlite/model.py` & `vlite-0.1.7/vlite/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,20 +25,36 @@
 
         print("Tokenizer:", self.tokenizer)
         # print("Dimension:", self.dimension)
         # print("Max sequence length:", self.max_seq_length)
 
     def embed(self, texts, max_seq_length=256, device="mps"):
 
-        device = torch.device(device)  # Create a torch.device object
+        if(torch.backends.mps.is_available()):
+            print("MPS is available")
+            dev = torch.device("mps")
+        else:
+            print("MPS is not available")
+            dev = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+        device = torch.device(dev)  # Create a torch.device object
+        print("Device:", device)
         self.model.to(device)  # Move the model to the specified device
 
         encoded_input = self.tokenizer(texts, padding=True, truncation=True, return_tensors='pt', max_length=max_seq_length)
+        print("Encoded input done",encoded_input['input_ids'].shape)
+        
+        if encoded_input['input_ids'].shape[0] > 1300:
+            print("Encoded input too large, defaulting to CPU")
+            device = torch.device("cpu")
+            self.model.to(device)  # Move the model to the specified device
+        
         encoded_input = {name: tensor.to(device) for name, tensor in encoded_input.items()}  # Move all input tensors to the specified device
-
+        print("Encoded input moved to device")
+        
         with torch.no_grad():
             model_output = self.model(**encoded_input)
 
         embeddings = mean_pooling(model_output, encoded_input['attention_mask'], device=device)
         tensor_embeddings = torch.nn.functional.normalize(embeddings, p=2, dim=1)
         np_embeddings = tensor_embeddings.cpu().numpy()  # Move tensor to CPU before converting to numpy
```

### Comparing `vlite-0.1.4/vlite/utils.py` & `vlite-0.1.7/vlite/utils.py`

 * *Files identical despite different names*

