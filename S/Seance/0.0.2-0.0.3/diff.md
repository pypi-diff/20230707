# Comparing `tmp/Seance-0.0.2-py3-none-any.whl.zip` & `tmp/Seance-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15260 bytes, number of entries: 16
+Zip file size: 15469 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat     2360 b- defN 23-Jun-21 13:29 Seance/Explainer.py
--rw-rw-rw-  2.0 fat    11262 b- defN 23-Jun-22 19:52 Seance/Forecaster.py
--rw-rw-rw-  2.0 fat     9882 b- defN 23-Jun-22 19:52 Seance/Optimizer.py
+-rw-rw-rw-  2.0 fat    11991 b- defN 23-Jul-07 01:46 Seance/Forecaster.py
+-rw-rw-rw-  2.0 fat    10054 b- defN 23-Jul-06 14:42 Seance/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:41 Seance/__init__.py
 -rw-rw-rw-  2.0 fat     3358 b- defN 23-May-18 13:18 Seance/Builder/PanelAxis.py
--rw-rw-rw-  2.0 fat     3990 b- defN 23-May-18 13:16 Seance/Builder/PreProcess.py
+-rw-rw-rw-  2.0 fat     3916 b- defN 23-Jul-06 20:13 Seance/Builder/PreProcess.py
 -rw-rw-rw-  2.0 fat     6595 b- defN 23-May-31 15:17 Seance/Builder/Transformations.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:40 Seance/Builder/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Jun-03 01:07 Seance/basis_functions/__init__.py
--rw-rw-rw-  2.0 fat      865 b- defN 23-May-27 00:20 Seance/basis_functions/fourier_basis.py
+-rw-rw-rw-  2.0 fat      845 b- defN 23-Jul-06 19:45 Seance/basis_functions/fourier_basis.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-May-31 21:10 Seance/basis_functions/linear_basis.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2684 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1302 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/RECORD
-16 files, 46399 bytes uncompressed, 13112 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2684 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1303 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/RECORD
+16 files, 47207 bytes uncompressed, 13321 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: Seance/basis_functions/fourier_basis.py
 Comment: 
 
 Filename: Seance/basis_functions/linear_basis.py
 Comment: 
 
-Filename: Seance-0.0.2.dist-info/LICENSE
+Filename: Seance-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: Seance-0.0.2.dist-info/METADATA
+Filename: Seance-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: Seance-0.0.2.dist-info/WHEEL
+Filename: Seance-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: Seance-0.0.2.dist-info/top_level.txt
+Filename: Seance-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Seance-0.0.2.dist-info/RECORD
+Filename: Seance-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Seance/Forecaster.py

```diff
@@ -134,14 +134,16 @@
                                           linear_test_window=linear_test_window,
                                           seasonal_period=max_period,
                                           outlier_cap=outlier_cap,
                                           run_dict=self.run_dict)
         self.processed_df = self.processor.process(df)
         self.processed_df = self.processed_df.sort_values(['Seance ID', date_column])
         self.processed_df[date_column] = self.processed_df[date_column].dt.tz_localize(None)
+        self.last_dates = self.processed_df[['Seance ID', date_column]].sort_values([date_column]).groupby('Seance ID').tail(1)
+        self.last_dates = self.last_dates.sort_values('Seance ID')
         if self.n_basis is not None and self.n_basis:
             self.basis_list = []
             basis = self.processed_df.groupby('Seance ID')[target_column].apply(self.linear_basis)
             self.processed_df = pd.concat([self.processed_df, basis], axis=1)
         if self.seasonal_period is not None:
             self.processed_df = self.processed_df.merge(seasonal_df, on=date_column)
         self.processed_df['cat_id_col'] = self.processed_df['Seance ID'].copy()
@@ -188,42 +190,51 @@
         unscaled = self.processor._transformers[seance_id](df['LGBMRegressor'].values)
         unscaled = np.array(unscaled).reshape(-1)
         df['LGBMRegressor'] = unscaled
         return df
 
     def predict(self, forecast_horizon):
         self.forecast_horizon = forecast_horizon
-        dates = pd.date_range(start=self.time_periods.iloc[-1],
-                              freq=self.freq,
-                              periods=forecast_horizon + 1)[1:]
-        dates = dates.tz_localize(None)
-        future_dates = pd.DataFrame(dates,
-                                    columns=[self.date_column])
+        future_dates = pd.date_range(start=self.time_periods.iloc[-1],
+                                     freq=self.freq,
+                                     periods=forecast_horizon + 1)[1:]
+        full_dates = pd.concat([self.time_periods, pd.Series(future_dates)])
         id_df = self.run_dict['global']['ID Mapping']
-        pred_X = pd.merge(id_df, future_dates, how='cross')
+        uids = pd.Series(np.repeat(id_df['Seance ID'].values, forecast_horizon),
+                         name='Seance ID',
+                         dtype='category')
+        pred_dates = []
+        for date in self.last_dates[self.date_column]:
+            pred_dates += list(pd.date_range(start=date,
+                              freq=self.freq,
+                              periods=forecast_horizon + 1)[1:])
+        pred_X = pd.DataFrame(uids, columns=['Seance ID'])
+        pred_X[self.date_column] = pred_dates
+        pred_X[self.date_column] = pred_X[self.date_column].dt.tz_localize(None)
         if self.seasonal_period is not None:
             seasonal_df = []
             for i in self.seasonal_period:
                 fourier_basis = get_future_fourier(forecast_horizon=forecast_horizon,
                                                    length=len(self.time_periods),
                                                    seasonal_period=i,
                                                    fourier_order=self.fourier_order)
                 column_names = [f'{i}_fourier_{j+1}' for j in range(2 * self.fourier_order)]
                 fourier_basis = pd.DataFrame(fourier_basis, columns=column_names).astype(float)
                 seasonal_df.append(fourier_basis)
             seasonal_df = pd.concat(seasonal_df)
-            seasonal_df[self.date_column] = future_dates
+            seasonal_df[self.date_column] = full_dates.values
             pred_X = pred_X.merge(seasonal_df, on=self.date_column)
         if self.n_basis is not None and self.n_basis:
             basis = pred_X.groupby('Seance ID').apply(self.future_linear_basis)
             pred_X = pd.concat([pred_X, basis], axis=1)
         if self.seasonal_period is not None or (self.n_basis is not None and self.n_basis):
             self.dynamic_dfs = [pred_X]
         else:
             self.dynamic_dfs = None
+        self.pred_X = pred_X
         predicted = self.mlforecast.predict(horizon=forecast_horizon,
                                             dynamic_dfs=self.dynamic_dfs)
         predicted = predicted.merge(self.run_dict['global']['ID Mapping'],
                                     on='Seance ID')
         if self.scale:
             predicted = predicted.groupby('Seance ID').apply(self.inverse_transform)
         predicted['LGBMRegressor'] = predicted['LGBMRegressor'].clip(lower=self.floor)
@@ -233,8 +244,9 @@
         return predicted
 
     def plot_importance(self, max_num_features=20):
         lgb.plot_importance(self.mlforecast.models_['LGBMRegressor'],
                             max_num_features=max_num_features)
         return
 
-    
+
+
```

## Seance/Optimizer.py

```diff
@@ -21,20 +21,26 @@
     def __init__(self,
                  df,
                  target_column,
                  date_column,
                  id_column,
                  freq,
                  test_size,
+                 categorical_columns=None,
                  metric='mse',
                  seasonal_period=0,
                  n_folds=1, #TODO
                  n_trials=100,
                  max_n_estimators=500,
                  ar_lags=None,
+                 scale_types=['log','standard','minmax','robust_boxcox','none'],
+                 min_bagging_pct=.1,
+                 max_bagging_pct=1.0,
+                 min_feature_fraction=.1,
+                 max_n_basis=25,
                  timeout=None):
         self.df = df.sort_values([id_column, date_column])
         if isinstance(seasonal_period, list):
             self.max_pulse = max(seasonal_period)
         else:
             self.max_pulse = seasonal_period
         self.seasonal_period = seasonal_period
@@ -49,14 +55,20 @@
         self.max_n_estimators = max_n_estimators
         # if ar_lags is None and seasonal_period is not None:
         #     ar_lags = list(np.arange(1, self.max_pulse + 1))
         # if ar_lags is None and seasonal_period is None:
         #     ar_lags = list(np.arange(1, 13))
         self.ar_lags = ar_lags
         self.metric= metric
+        self.scale_types = scale_types
+        self.min_bagging_pct = min_bagging_pct
+        self.max_bagging_pct = max_bagging_pct
+        self.min_feature_fraction = min_feature_fraction
+        self.max_n_basis = max_n_basis
+        self.categorical_columns = categorical_columns
 
     # def logic_layer(self):
     #     n_samples = len(y)
     #     test_size = n_samples//(self.n_folds + 1)
     #     if n_samples - test_size < self.max_pulse:
     #         self.seasonal_period = 0
 
@@ -67,73 +79,68 @@
         self.train_df = df[df['test_split'] == False]
         # self.train_df[self.date_column] = pd.to_datetime(self.train_df[self.date_column]).dt.
         self.test_df = df[df['test_split'] == True]
 
     def scorer(self, params, metric):
         scores = []
         # for train_index, test_index in cv_splits:
-        try:
-            model_obj = Forecaster()
-            model_obj.fit(self.train_df,
-                          target_column=self.target_column,
-                          date_column=self.date_column,
-                          id_column=self.id_column,
-                          freq=self.freq,
-                          **params)
-            predicted = model_obj.predict(self.test_size)
-            self.predicted = predicted
-            if len(predicted) != len(self.test_df):
-                print('Predicted not the same size as test set')
-    
-            if any(np.isnan(predicted['LGBMRegressor'])):
-                scores.append(np.inf)
-            else:
-                # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
-                self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
-                self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
-                if metric == 'mse':
-                    scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df['LGBMRegressor'].values))
-                elif metric == 'smape':
-                    scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column))
-        except Exception as e:
-                scores.append(np.inf)
-                print(f'ERROR WHILE TUNING: {e}')
+        # try:
+        print(params)
+        model_obj = Forecaster()
+        model_obj.fit(self.train_df,
+                      target_column=self.target_column,
+                      date_column=self.date_column,
+                      id_column=self.id_column,
+                      freq=self.freq,
+                      categorical_columns=self.categorical_columns,
+                      **params)
+        predicted = model_obj.predict(self.test_size)
+        self.predicted = predicted
+        if len(predicted) != len(self.test_df):
+            print('Predicted not the same size as test set')
+
+        if any(np.isnan(predicted['LGBMRegressor'])):
+            scores.append(np.inf)
+        else:
+            # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
+            self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
+            self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
+            if metric == 'mse':
+                scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df['LGBMRegressor'].values))
+            elif metric == 'smape':
+                scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column))
+        # except Exception as e:
+        #         scores.append(np.inf)
+        #         print(f'ERROR WHILE TUNING: {e}')
         return np.mean(scores)
 
 
     def objective(self, trial):
         params = {
             "n_estimators": trial.suggest_int(name="n_estimators", low=50, high=self.max_n_estimators),
             'lambda_l1': trial.suggest_float('lambda_l1', 1e-8, 10.0),
             'lambda_l2': trial.suggest_float('lambda_l2', 1e-8, 10.0),
             'num_leaves': trial.suggest_int('num_leaves', 2, 512),
-            'feature_fraction': trial.suggest_float('feature_fraction', 0.1, 1.0),
-            'bagging_fraction': trial.suggest_float('bagging_fraction', 0.1, 1.0),
+            'feature_fraction': trial.suggest_float('feature_fraction', self.min_feature_fraction, 1.0),
+            'bagging_fraction': trial.suggest_float('bagging_fraction', self.min_bagging_pct, self.max_bagging_pct),
             'bagging_freq': trial.suggest_int('bagging_freq', 0, 15),
             'min_child_samples': trial.suggest_int('min_child_samples', 1, 100),
             "use_id": trial.suggest_categorical("use_id", [True, False]),
             "objective": trial.suggest_categorical("objective", ['regression', 'regression_l1']),
-            "n_basis": trial.suggest_int("n_basis", 0, 25),
+            "n_basis": trial.suggest_int("n_basis", 0, self.max_n_basis),
             "differences": trial.suggest_categorical("differences", [None, 1]),
             "decay": trial.suggest_categorical("decay", [-1,
                                                          .05,
                                                          .1,
                                                          .25,
                                                          .5,
                                                          .75,
                                                          .9,
                                                          .99]),
-            "scale_type": trial.suggest_categorical("scale_type", ['log',
-                                                                   'standard',
-                                                                    'minmax',
-                                                                   # 'maxabs',
-                                                                   # 'robust',
-                                                                   # 'boxcox',
-                                                                   'robust_boxcox',
-                                                                   'none']),
+            "scale_type": trial.suggest_categorical("scale_type", self.scale_types),
         }
         if self.seasonal_period:
             params.update({'seasonal_period': trial.suggest_categorical("seasonal_period", [None, self.seasonal_period])})
         if self.ar_lags is not None:
             params.update({'lags': trial.suggest_categorical("lags", self.ar_lags)})
         else:
             if self.seasonal_period:
@@ -148,14 +155,16 @@
     def fit(self, seed):
         self.get_splits(self.df, self.id_column)
         study = optuna.create_study(direction="minimize", sampler=optuna.samplers.TPESampler(seed=seed))
         study.optimize(self.objective, n_trials=self.n_trials)
         best_params = study.best_params
         if best_params['lags'] == 1:
             best_params.update({'lags': [study.best_params['lags']]})
+        elif isinstance(best_params['lags'], list):
+            pass
         else:
             best_params.update({'lags': list(range(1, best_params['lags']))})
         return best_params, study
 
 #%%
 if __name__ == '__main__':
     import matplotlib.pyplot as plt
```

## Seance/Builder/PreProcess.py

```diff
@@ -76,17 +76,17 @@
         return df
 
     def process(self, df):
         df = self.create_seance_id(df)
         if self.scale:
             df = df.groupby('Seance ID').apply(self.trans)
         if self.outlier_cap is not None:
-            df[self.target_column] = df.groupby('Seance ID')[self.target_column].transform(cap_outliers,
-                                                                              outlier_cap=self.outlier_cap,
-                                                                            )
+            df[self.target_column] = df.groupby('Seance ID')[self.target_column]\
+                                        .transform(cap_outliers,
+                                        outlier_cap=self.outlier_cap)
         return df
 
 
 
 #%%
 
 if __name__=='__main__':
```

## Seance/basis_functions/fourier_basis.py

```diff
@@ -14,13 +14,13 @@
 
 @njit
 def get_future_fourier(length, forecast_horizon, seasonal_period, fourier_order):
     x = 2 * np.pi * np.arange(1, fourier_order + 1) / seasonal_period
     t = np.arange(1, length + 1 + forecast_horizon).reshape(-1, 1)
     x = x * t
     fourier_series = np.concatenate((np.cos(x), np.sin(x)), axis=1)
-    return fourier_series[-forecast_horizon:]
+    return fourier_series
 
 #%%
 if __name__ == '__main__':
     f = get_fourier_series(300, 12, 10)
     ff = get_future_fourier(len(f), 50, 12, 10)
```

## Comparing `Seance-0.0.2.dist-info/LICENSE` & `Seance-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Seance-0.0.2.dist-info/METADATA` & `Seance-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Seance
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Wrapper around MLForecast.
 Home-page: https://github.com/tblume1992/Seance
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm,mlforecast
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `Seance-0.0.2.dist-info/RECORD` & `Seance-0.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Seance/Explainer.py,sha256=ViUQvXZhsyrKjAscA88NOmBZEXwBl6pldjKe8IJ_fT0,2360
-Seance/Forecaster.py,sha256=csW12Sytquao5R2InOa5q8DASG-bCGiZjOsftVrO2uQ,11262
-Seance/Optimizer.py,sha256=McIC6ZUCAJlSFTk0LRxQ_RneOLg2VFiflr67wBXqyqs,9882
+Seance/Forecaster.py,sha256=mjbPTFddHdjKe2TKlzO_Ak-0hnvPPrv5gWntMUs3_kQ,11991
+Seance/Optimizer.py,sha256=vRqi42lO7ry4OkWBKnuZ7yqGfgOy_YWc3XiC4S9a82I,10054
 Seance/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/Builder/PanelAxis.py,sha256=w5YYnDXgprHWUzCWcqqBEkV1xJ_6qLabzW_PIbQF9ZQ,3358
-Seance/Builder/PreProcess.py,sha256=i4IWwm12welXyK1b90CbHJyQi02vjtTHcaEacjLsm-A,3990
+Seance/Builder/PreProcess.py,sha256=lXDwzPEYw_01pDEB9533v60uqYJEQE7Jb12vjIxmWhA,3916
 Seance/Builder/Transformations.py,sha256=JY27tWWvxha2JXhVgOALQFJUhV-N2Hcmg2u9hhBSeaA,6595
 Seance/Builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
-Seance/basis_functions/fourier_basis.py,sha256=SNOuujoYtcofte1z9BoBDR7kCBdvWaCONrjeSWvesow,865
+Seance/basis_functions/fourier_basis.py,sha256=8KePMSK7FGqu9t_mkir101B2OvJGZ-FY9kqepiJSCyw,845
 Seance/basis_functions/linear_basis.py,sha256=1RHj--VkbA4heV8QwzNE7a9O0-aPu3Br3EqLlcuUHWU,2834
-Seance-0.0.2.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
-Seance-0.0.2.dist-info/METADATA,sha256=ZiE_6C29mUulcd1vyFYneyQmRLt2b2iKs7R-BJeH7Ls,2684
-Seance-0.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Seance-0.0.2.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
-Seance-0.0.2.dist-info/RECORD,,
+Seance-0.0.3.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
+Seance-0.0.3.dist-info/METADATA,sha256=hrQO8PZ1drDxFK646muHOtoLwU10_4uBi_BNUqoqQjg,2684
+Seance-0.0.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Seance-0.0.3.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
+Seance-0.0.3.dist-info/RECORD,,
```

