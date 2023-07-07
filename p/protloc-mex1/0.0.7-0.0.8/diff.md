# Comparing `tmp/protloc_mex1-0.0.7.tar.gz` & `tmp/protloc_mex1-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex1-0.0.7.tar", last modified: Mon Jun 12 12:21:06 2023, max compression
+gzip compressed data, was "protloc_mex1-0.0.8.tar", last modified: Fri Jul  7 03:53:16 2023, max compression
```

## Comparing `protloc_mex1-0.0.7.tar` & `protloc_mex1-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:21:06.577835 protloc_mex1-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     7733 2023-06-12 12:21:06.572709 protloc_mex1-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 12:21:06.529862 protloc_mex1-0.0.7/protloc_mex1/
--rw-rw-rw-   0        0        0    19901 2023-06-12 12:12:22.000000 protloc_mex1-0.0.7/protloc_mex1/AA_count.py
--rw-rw-rw-   0        0        0     8014 2023-06-12 12:12:22.000000 protloc_mex1-0.0.7/protloc_mex1/GO_count.py
--rw-rw-rw-   0        0        0    10510 2023-06-12 12:12:22.000000 protloc_mex1-0.0.7/protloc_mex1/SHAP_conduct.py
--rw-rw-rw-   0        0        0    31630 2023-06-12 12:12:22.000000 protloc_mex1-0.0.7/protloc_mex1/SHAP_plus.py
--rw-rw-rw-   0        0        0       39 2023-06-12 12:12:22.000000 protloc_mex1-0.0.7/protloc_mex1/__init__.py
--rw-rw-rw-   0        0        0    11881 2023-06-12 12:12:22.000000 protloc_mex1-0.0.7/protloc_mex1/classifier_evalute.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:21:06.569563 protloc_mex1-0.0.7/protloc_mex1.egg-info/
--rw-rw-rw-   0        0        0     7733 2023-06-12 12:21:06.000000 protloc_mex1-0.0.7/protloc_mex1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-12 12:21:06.000000 protloc_mex1-0.0.7/protloc_mex1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:21:06.000000 protloc_mex1-0.0.7/protloc_mex1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-12 12:21:06.000000 protloc_mex1-0.0.7/protloc_mex1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 12:21:06.000000 protloc_mex1-0.0.7/protloc_mex1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      859 2023-06-12 12:14:21.000000 protloc_mex1-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 12:21:06.578349 protloc_mex1-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 03:53:16.362831 protloc_mex1-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     7733 2023-07-07 03:53:16.361831 protloc_mex1-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 03:53:16.327175 protloc_mex1-0.0.8/protloc_mex1/
+-rw-rw-rw-   0        0        0    19901 2023-06-12 12:11:40.000000 protloc_mex1-0.0.8/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.8/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.8/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    33141 2023-07-03 03:39:28.000000 protloc_mex1-0.0.8/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.8/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    14425 2023-06-22 02:36:30.000000 protloc_mex1-0.0.8/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:53:16.360330 protloc_mex1-0.0.8/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     7733 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      859 2023-07-07 03:47:35.000000 protloc_mex1-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 03:53:16.362831 protloc_mex1-0.0.8/setup.cfg
```

### Comparing `protloc_mex1-0.0.7/LICENSE.txt` & `protloc_mex1-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.7/PKG-INFO` & `protloc_mex1-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc_mex1
-Version: 0.0.7
+Version: 0.0.8
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.7/README.md` & `protloc_mex1-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.7/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.8/protloc_mex1/AA_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.7/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.8/protloc_mex1/GO_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.7/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.8/protloc_mex1/SHAP_conduct.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.7/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.8/protloc_mex1/SHAP_plus.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,31 +45,31 @@
         str_outcom=[]
         for i in input_names:
             if re.search(pattern,i):
                 str_outcom.append(i)
         return(str_outcom)
     
     @staticmethod
-    def feature_shap_statistic(type_data_all,depleted_ID_len=0):
-        type_data_all_feature_shap=list(map(lambda x:type_data_all[x].iloc[:,:len(type_data_all[x].columns)-depleted_ID_len],type_data_all.keys()))
-        type_data_all_feature_shap=dict(zip(list(type_data_all.keys()),type_data_all_feature_shap))
-        for i,value in enumerate(type_data_all_feature_shap):
-            feature_inner_name=type_data_all_feature_shap[value].columns
-            type_data_all_feature_shap[value]=list(map(lambda x:pd.DataFrame(type_data_all_feature_shap[value][x]),type_data_all_feature_shap[value].columns))
-            type_data_all_feature_shap[value]=dict(zip(list(feature_inner_name),type_data_all_feature_shap[value]))
-            for i_1,value_1 in enumerate(type_data_all_feature_shap[value]):
-                type_data_all_feature_shap[value][value_1].columns=[value]
-        type_data_all_feature_shap_outcome=dict()
+    def feature_shap_statistic(SHAP_data_all,depleted_ID_len=0):
+        SHAP_data_all_feature_shap=list(map(lambda x:SHAP_data_all[x].iloc[:,:len(SHAP_data_all[x].columns)-depleted_ID_len],SHAP_data_all.keys()))
+        SHAP_data_all_feature_shap=dict(zip(list(SHAP_data_all.keys()),SHAP_data_all_feature_shap))
+        for i,value in enumerate(SHAP_data_all_feature_shap):
+            feature_inner_name=SHAP_data_all_feature_shap[value].columns
+            SHAP_data_all_feature_shap[value]=list(map(lambda x:pd.DataFrame(SHAP_data_all_feature_shap[value][x]),SHAP_data_all_feature_shap[value].columns))
+            SHAP_data_all_feature_shap[value]=dict(zip(list(feature_inner_name),SHAP_data_all_feature_shap[value]))
+            for i_1,value_1 in enumerate(SHAP_data_all_feature_shap[value]):
+                SHAP_data_all_feature_shap[value][value_1].columns=[value]
+        SHAP_data_all_feature_shap_outcome=dict()
         
         for i in list(feature_inner_name):
-            type_data_all_feature_shap_outcome[i]=list(map(lambda x: type_data_all_feature_shap[x][i],type_data_all_feature_shap.keys()))   
+            SHAP_data_all_feature_shap_outcome[i]=list(map(lambda x: SHAP_data_all_feature_shap[x][i],SHAP_data_all_feature_shap.keys()))   
               
-            type_data_all_feature_shap_outcome[i]=reduce(lambda x,y: pd.concat([x,y],axis=1),type_data_all_feature_shap_outcome[i])       
+            SHAP_data_all_feature_shap_outcome[i]=reduce(lambda x,y: pd.concat([x,y],axis=1),SHAP_data_all_feature_shap_outcome[i])       
             
-        return(type_data_all_feature_shap_outcome)
+        return(SHAP_data_all_feature_shap_outcome)
     
     # def SHAP_importance_sum_claulate_process(self,depleted_ID_len=0,file_name='human_'):
     #     scale=MinMaxScaler()
     #     self.type_data_shap_sum_all=dict()
     #     self.type_data_shap_sum_all_outcome=dict()
     #     self.shap_feature_importance=dict()
     #     self.shap_feature_importance_T=None
@@ -133,14 +133,47 @@
         self.shap_feature_importance.columns = [re.compile('('+file_name+')|(_shap_value)').sub('', name) for name in self.shap_feature_importance.columns]
         # shap_feature_importance转置
         self.shap_feature_importance_T = self.shap_feature_importance.T
         return {'type_data_shap_sum_all_outcome': self.type_data_shap_sum_all_outcome,
                 'shap_feature_importance': self.shap_feature_importance,
                 'shap_feature_importance_T': self.shap_feature_importance_T}
     
+    def calculate_feature_shap_bins(self, keys, feature, bins_num=10, q_num=10):
+        result = pd.DataFrame()
+        for key in keys:
+            data = self.shapley_data_all[key]
+            feature_data = data[feature]
+            # 先按分位数分箱
+            quantiles = pd.qcut(feature_data, q=q_num, duplicates='drop')
+            # 记录全局箱子编号
+            global_bins = 0
+            bins_list = []
+            # 在每个分位数区间内按等距分箱
+            for _, group in feature_data.groupby(quantiles):
+                # 由于group的index是feature_data的index，所以可以通过这个index从feature_data中取到对应的值
+                group_values = feature_data[group.index]
+                bins = pd.cut(group_values, bins=bins_num, include_lowest=True)
+                # 获取箱子编号，并加上全局箱子编号
+                bins_codes = bins.cat.codes + global_bins
+                bins_list.append(bins_codes)
+                # 更新全局箱子编号
+                global_bins = bins_codes.max() + 1
+            # 拼接所有的箱子编号
+            bins_codes = pd.concat(bins_list)
+            temp_df = pd.DataFrame({
+                f'shap_values_{key}': feature_data,
+                f'bins_{key}': bins_codes
+            })
+            if result.empty:
+                result = temp_df
+            else:
+                result = result.join(temp_df, how='outer')
+        return result
+    
+
 
     
 
 class FeaturePlotSource:
     def __init__(self, X_data, shapley_data_all):
         self.X_data = X_data
         self.shapley_data_all = shapley_data_all
```

### Comparing `protloc_mex1-0.0.7/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.8/protloc_mex1/classifier_evalute.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 import matplotlib.pyplot as plt
 
 from functools import reduce
 import logging
 
 from packaging import version
 import warnings
-
+import seaborn as sns
 try:
     import sklearn
     if version.parse(sklearn.__version__) < version.parse('1.0.2'):
         warnings.warn("Your sklearn version is older than 1.0.2 and may not operate correctly.")
     from sklearn.metrics import roc_curve, auc, confusion_matrix
     from sklearn.metrics import classification_report, accuracy_score, roc_auc_score
     from sklearn.metrics import matthews_corrcoef
 except ImportError:
     warnings.warn("Sklearn not found. Some functions will not be available.")
 
-try:
-    import mglearn
-except ImportError:
-    warnings.warn("Mglearn not found. Some functions will not be available.")
+# try:
+#     import mglearn
+# except ImportError:
+#     warnings.warn("Mglearn not found. Some functions will not be available.")
 
     
 class ClassifierEvaluator:
     """
     A class for evaluating the performance of a classifier model.
     
     Attributes:
@@ -195,45 +195,95 @@
             plt.xlim([0.0, 1.0])
             plt.ylim([0.0, 1.05])
             plt.xlabel('False Positive Rate')
             plt.ylabel('True Positive Rate')
             plt.title('ROC Curve')
             plt.legend(loc="lower right")
             
-        def confusion_matrix_plot(self,figsize):
+        # def confusion_matrix_plot(self,figsize):
             
+        #     # create confusion matrix
+        #     matrix = confusion_matrix(self.self_obj.y_data, self.self_obj.X_hat_data["predict"].to_numpy())
+        #     plt.figure(figsize=figsize)
+        #     mglearn.tools.heatmap(matrix, xlabel='Predicted label', ylabel='True label',
+        #                           xticklabels=np.array(pd.Series(self.self_obj.type_class).str.slice(0,2)),
+        #                           yticklabels=self.self_obj.type_class, cmap=plt.cm.viridis_r, fmt="%d")
+        #     plt.gca().invert_yaxis()
+        def confusion_matrix_plot(self, figsize):
             # create confusion matrix
             matrix = confusion_matrix(self.self_obj.y_data, self.self_obj.X_hat_data["predict"].to_numpy())
+            
+            # Assuming type_class and x and y labels
+            xticklabels = np.array(pd.Series(self.self_obj.type_class).str.slice(0,2))
+            yticklabels = self.self_obj.type_class
+
+            # Set figure size
             plt.figure(figsize=figsize)
-            mglearn.tools.heatmap(matrix, xlabel='Predicted label', ylabel='True label',
-                                  xticklabels=np.array(pd.Series(self.self_obj.type_class).str.slice(0,2)),
-                                  yticklabels=self.self_obj.type_class, cmap=plt.cm.viridis_r, fmt="%d")
+
+            # Use seaborn
+            sns.heatmap(matrix, annot=True, cmap='viridis_r', fmt='d', xticklabels=xticklabels, yticklabels=yticklabels)
+
+            # Configure the plot details
             plt.gca().invert_yaxis()
+            plt.xlabel('Predicted label')
+            plt.ylabel('True label')
+    
+        def confusion_matrix_plot_percentage(self, figsize):
+            # create confusion matrix
+            matrix = confusion_matrix(self.self_obj.y_data, self.self_obj.X_hat_data["predict"].to_numpy())
             
+            # Convert to percentage
+            matrix = matrix.astype('float') / matrix.sum(axis=1)[:, np.newaxis]
+
+            # Assuming type_class and x and y labels
+            xticklabels = np.array(pd.Series(self.self_obj.type_class).str.slice(0,2))
+            yticklabels = self.self_obj.type_class
+
+            # Set figure size
+            plt.figure(figsize=figsize)
+
+            # Use seaborn
+            sns.heatmap(matrix, annot=True, cmap='viridis_r', fmt='.2%', xticklabels=xticklabels, yticklabels=yticklabels)
+
+            # Configure the plot details
+            plt.gca().invert_yaxis()
+            plt.xlabel('Predicted label')
+            plt.ylabel('True label')
+    
+
         def plot(self,save_path,file_name,figsize):
             
             if len(pd.unique(self.self_obj.y_data)) <= 2:
                 self.two_features_roc()
                 plt.title(file_name+'ROC curve')
                 plt.savefig(save_path+file_name+'_roc.png',dpi=1000,bbox_inches="tight")
                 plt.savefig(save_path+file_name+'_roc.pdf',dpi=1000,bbox_inches="tight")
                 plt.close()
                 self.confusion_matrix_plot(figsize)
                 plt.title(file_name+'Confusion matrix')
                 plt.savefig(save_path+file_name+'_confusion_matrix.png',dpi=1000,bbox_inches="tight")
                 plt.savefig(save_path+file_name+'_confusion_matrix.pdf',dpi=1000,bbox_inches="tight")
                 plt.close()
+                self.confusion_matrix_plot_percentage(figsize)
+                plt.title(file_name+'Confusion matrix percentage')
+                plt.savefig(save_path+file_name+'_confusion_matrix_percentage.png',dpi=1000,bbox_inches="tight")
+                plt.savefig(save_path+file_name+'_confusion_matrix_percentage.pdf',dpi=1000,bbox_inches="tight")
+                plt.close()
                 
             else:
                 self.confusion_matrix_plot(figsize)
                 plt.title(file_name+'Confusion matrix')
                 plt.savefig(save_path+file_name+'_confusion_matrix.png',dpi=1000,bbox_inches="tight")
                 plt.savefig(save_path+file_name+'_confusion_matrix.pdf',dpi=1000,bbox_inches="tight")
                 plt.close()
-
+                self.confusion_matrix_plot_percentage(figsize)
+                plt.title(file_name+'Confusion matrix percentage')
+                plt.savefig(save_path+file_name+'_confusion_matrix_percentage.png',dpi=1000,bbox_inches="tight")
+                plt.savefig(save_path+file_name+'_confusion_matrix_percentage.pdf',dpi=1000,bbox_inches="tight")
+                plt.close()
     @ClassificationEvaluatePlot
     def classification_evaluate_plot(self,save_path,file_name,figsize, *args, **kwargs):
         """
         Parameters
         ----------
         save_path : str
             input is file or plot save path way with no contain file name.
```

### Comparing `protloc_mex1-0.0.7/protloc_mex1.egg-info/PKG-INFO` & `protloc_mex1-0.0.8/protloc_mex1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex1
-Version: 0.0.7
+Version: 0.0.8
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.7/pyproject.toml` & `protloc_mex1-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

