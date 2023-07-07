# Comparing `tmp/datawhispers-0.2.8.8.tar.gz` & `tmp/datawhispers-0.2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.8.8.tar", last modified: Thu Jul  6 08:53:23 2023, max compression
+gzip compressed data, was "datawhispers-0.2.8.9.tar", last modified: Thu Jul  6 09:34:03 2023, max compression
```

## Comparing `datawhispers-0.2.8.8.tar` & `datawhispers-0.2.8.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:53:23.592875 datawhispers-0.2.8.8/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.8/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:53:23.592761 datawhispers-0.2.8.8/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)     1218 2023-07-05 20:19:46.000000 datawhispers-0.2.8.8/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:53:23.591924 datawhispers-0.2.8.8/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.8/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)    11593 2023-07-05 19:23:07.000000 datawhispers-0.2.8.8/datawhispers/advancedProg.py
--rw-r--r--   0 german     (501) staff       (20)    17824 2023-07-05 13:05:34.000000 datawhispers-0.2.8.8/datawhispers/datavis.py
--rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.8/datawhispers/mathFuncs.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:53:23.592546 datawhispers-0.2.8.8/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      309 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:53:23.592917 datawhispers-0.2.8.8/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2297 2023-07-06 08:53:11.000000 datawhispers-0.2.8.8/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 09:34:03.460246 datawhispers-0.2.8.9/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.9/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 09:34:03.460133 datawhispers-0.2.8.9/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)     1218 2023-07-05 20:19:46.000000 datawhispers-0.2.8.9/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 09:34:03.459398 datawhispers-0.2.8.9/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.9/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)    11593 2023-07-05 19:23:07.000000 datawhispers-0.2.8.9/datawhispers/advancedProg.py
+-rw-r--r--   0 german     (501) staff       (20)    20368 2023-07-06 09:32:49.000000 datawhispers-0.2.8.9/datawhispers/datavis.py
+-rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.9/datawhispers/mathFuncs.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 09:34:03.459954 datawhispers-0.2.8.9/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 09:34:03.000000 datawhispers-0.2.8.9/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      309 2023-07-06 09:34:03.000000 datawhispers-0.2.8.9/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-06 09:34:03.000000 datawhispers-0.2.8.9/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 09:34:03.000000 datawhispers-0.2.8.9/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-06 09:34:03.000000 datawhispers-0.2.8.9/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 09:34:03.460288 datawhispers-0.2.8.9/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2297 2023-07-06 09:33:43.000000 datawhispers-0.2.8.9/setup.py
```

### Comparing `datawhispers-0.2.8.8/LICENSE` & `datawhispers-0.2.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.8/PKG-INFO` & `datawhispers-0.2.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.8
+Version: 0.2.8.9
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.8/README.md` & `datawhispers-0.2.8.9/README.md`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.8/datawhispers/advancedProg.py` & `datawhispers-0.2.8.9/datawhispers/advancedProg.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.8/datawhispers/datavis.py` & `datawhispers-0.2.8.9/datawhispers/datavis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,102 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 from IPython.display import HTML, display
 
 from scipy.stats import chi2_contingency, ttest_ind, pearsonr
 
-# Korrelationstabellenerstellung #
+def Datensatz_bereinigen(df:pd.DataFrame,kategorische_Spalten:list|tuple=[],numerische_Spalten:list|tuple=[]):
+    """
+    Wandelt 'Numerische Daten' in Kategorische und anders herum.
+    @return Bereinigter Datensatz als pd.DataFrame
+    """
+    for x in kategorische_Spalten:
+        df[x]=df[x].apply(str)
+    for x in numerische_Spalten:
+        df[x]=df[x].apply(eval)
+    return df
 
-def Correlation_table(df:pd.DataFrame, max:int=10):
+def T_Test_Rückgabe(df:pd.DataFrame, Zielvariable, Zielvariable_Wert_gut, Zielvariable_Wert_schlecht,Numerische_Grenze,Grafik=False):
     """
-    [numerisch] - [numerisch]\n
-    Stellt die stärksten Korrelationen zwischen intervallskalierten Variablen sortiert visuell dar.\n 
-    Größeres p --> Größere Abhängigkeit
-    @Variabel df: Zugehöriges DataFrame
-    @Variabel max: Maximale Anzahl der Korrelationen
-    """
-    print("--------------------------------------------------")
-    print("|               Korrelationstabelle              |")
-    print("--------------------------------------------------")
-    
+    [metrisch] - [kategorisch]\n
+    Stellt die unterschiedlichen stat. Abhängigkeiten mit Mittelwert und Standardabweichung visuell dar
+    @Zielvariable: Nur zwei Ausprägungen
+    @return [Variable,p-Wert,t-wert,mü-gut, sigma-gut, mü-schlecht, sigma-schlecht]
+    """
+    P_Wert = []
+    if df.dtypes[Zielvariable]=="int64" or df.dtypes[Zielvariable]=="float64":
+        if Numerische_Grenze==0:
+            Durchschnitt = df[Zielvariable].values.mean()
+        else:
+            Durchschnitt = Numerische_Grenze
+        subset_good=df[df[Zielvariable]>Durchschnitt]
+        subset_bad=df[df[Zielvariable]<Durchschnitt]
+        Zielvariable_Wert_gut=f">{round(Durchschnitt,2)}"
+        Zielvariable_Wert_schlecht=f"<{round(Durchschnitt,2)}"
+    else:
+        subset_good=df[df[Zielvariable]==Zielvariable_Wert_gut]
+        subset_bad=df[df[Zielvariable]==Zielvariable_Wert_schlecht]
+    for testvar in df.keys():
+        if df.dtypes[testvar]=="int64" or df.dtypes[testvar]=="float64":
+            tval,pval=ttest_ind(subset_good[testvar],subset_bad[testvar])
+            
+            heights=[subset_good[testvar].mean(),subset_bad[testvar].mean()]
+            stds=[[0,0],[subset_good[testvar].std(),subset_bad[testvar].std()]]
+            
+            P_Wert.append((testvar,pval,tval,heights[0],stds[1][0],heights[1],stds[1][1],"","T-Test"))
+    if Grafik:
+        figure,axis=plt.subplots()
+        print(Zielvariable_Wert_gut,": ",u"\u03bc \u2248 ",'{:.4f}'.format(heights[0]),",",u"\u03C3 \u2248 \u00B1",'{:.4f}'.format(stds[1][0]))
+        print(Zielvariable_Wert_schlecht,": ",u"\u03bc \u2248 ",'{:.4f}'.format(heights[1]),",",u"\u03C3 \u2248 \u00B1",'{:.4f}'.format(stds[1][1]))      
+        axis.bar(x=np.arange(len(heights)),height=heights,tick_label=[Zielvariable_Wert_gut, Zielvariable_Wert_schlecht],color="gray",yerr=stds,ecolor="gray",width=0.4,capsize=4)
+        axis.set_title(f"{testvar} vs. {Zielvariable}")
+        axis.set_ylabel(f"Durchschnitt {testvar}");
+        axis.set_xlabel(Zielvariable);
+        plt.tight_layout()
+        plt.show()
+    return P_Wert
+
+def chi_square_all_Rückgabe(df:pd.DataFrame, Zielvariable,Numerische_Grenze):
+    """
+    [kategorisch] - [kategorisch]\n
+    Erstellt alle möglichen chi2-Werte und p werte\n
+    p<0.05 und chi2 sehr groß --> Signifikant
+    """
+    Ergebnis = []
+    Tabelle = []
+    for var in df.dtypes.items():
+        if var[1].name=="object" and var[0]!=Zielvariable:
+            Teillösung,expectedFreq,contigenzTable = chi_square_einzeln_Rückgabe(df, var[0], Zielvariable,Numerische_Grenze=Numerische_Grenze)
+            Ergebnis.append(Teillösung)
+            Tabelle.append((contigenzTable,expectedFreq))
+    return Ergebnis,Tabelle
+
+def chi_square_einzeln_Rückgabe(df:pd.DataFrame, varname, Zielvariable,Numerische_Grenze=0):
+    """
+    [kategorisch] - [kategorisch]
+    """
+    if df.dtypes[Zielvariable]=="int64" or df.dtypes[Zielvariable]=="float64":
+        Tab = df[Zielvariable]
+        if Numerische_Grenze==0:
+            Durchschnitt = df[Zielvariable].values.mean()
+            Tab = Tab>=Durchschnitt
+        else:
+            Durchschnitt = Numerische_Grenze
+            Tab = Tab>=Durchschnitt        
+        contingencyTable=pd.crosstab(df[varname],Tab)
+        chi2,pval,dof,expectedFreq=chi2_contingency(contingencyTable)
+        P_Wert=(varname,pval,chi2,"","","","",dof,"X²-Test")
+    else:
+        contingencyTable=pd.crosstab(df[varname],df[Zielvariable])
+        chi2,pval,dof,expectedFreq=chi2_contingency(contingencyTable)
+        P_Wert=(varname,pval,chi2,"","","","",dof,"X²-Test")
+    return P_Wert,expectedFreq,contingencyTable
+
+def Cor_tab(df,max=10):
     correlations=[]
     for var in df.dtypes.items():
         if var[1].name=="int64" or var[1].name=="float64":
             
             for othervar in df.dtypes.items():
                 if (var[0]==othervar[0]):
                     break
@@ -36,138 +110,114 @@
         max=len(correlations)
     for i in range(max):
         correlation=correlations[i]
         heights.append(correlation[0])
         labels.append(correlation[2])
         
     figure,axis=plt.subplots()
+    plt.title("Korrelationstabelle")
     plt.xticks(rotation=90)
     axis.bar(x=np.arange(len(heights)),height=heights,tick_label=labels,color="gray")
     axis.set_ylabel("Pearson Correlation p");
     plt.show()
+            
+def Analyse_Tabelle(df:pd.DataFrame,Zielvariable:str,Anzahl_an_gewünschten_Variablen:int=None,Zielvariable_good="",Zielvariable_bad="",Zielvariable_Grenze:int|float=0,kategorische_Variablen=[],Numerische_Variablen=[]):
+    """
+    Gibt die Tabelle mit den abhängigsten Variablen aus.
+    @param df: Der DataFrame
+    @param Zielvariable: Zielvariable
+    @param Anzahl_an_gewünschten_Variablen (opt.)
+    @param Zielvariable_good: Nur bei KATEGORISCHER Zielvariable
+    @param Zielvariable_bad: Nur bei KATEGORISCHER Zielvariable
+    @param Zielvariable_Grenze: Nur bei NUMERISCHER Zielvariable ;Schwellwert ab wann Gut oder Schlecht sonst Durchschnitt
+    @param kategorische_Variablen: Eingeben einer Liste an kategorischen Variablen, die im Datensatz als numerisch gekennzeichnet sind (opt.) 
+    @param numerische_Variablen: Eingeben einer Liste an numerischen Variablen, die im Datensatz als kategorisch gekennzeichnet sind (opt.) 
+    @return Tabelle mit Variablen, Kennwerten, Testverfahren
+    """
+    ## Korregieren der Tabelle ##
+        
+    df = Datensatz_bereinigen(df,kategorische_Variablen,Numerische_Variablen)
     
+    ## Erstellen der Variablentabelle sortiert nach größter Abhängigkeit
     
-
-def Correlation_analysis_all(df:pd.DataFrame):
+    # Tests
     
-    print("--------------------------------------------------")
-    print("|               Korrelationsanalyse              |")
-    print("--------------------------------------------------")
+    T_Ergebnis = T_Test_Rückgabe(df,Zielvariable,Zielvariable_good,Zielvariable_bad,Zielvariable_Grenze)
+    X_Ergebnis,X_Tabelle = chi_square_all_Rückgabe(df,Zielvariable,Zielvariable_Grenze) 
     
-    for var in df.dtypes.items():
-        if var[1].name=="int64" or var[1].name=="float64":
-            
-            for othervar in df.dtypes.items():
-                if (var[0]==othervar[0]):
-                    break
-                if ((othervar[1].name=="int64" or othervar[1]=="float64")): 
-                    correlation=df[var[0]].corr(df[othervar[0]])
-                    print(u"Pearsons Rho \u03C1 = ",abs(correlation))
-                    if abs(correlation)>0.2:
-                        print("!!!!Statistische Abhängigkeit!!!!")
-                    else:
-                        print()
-                    figure, axis = plt.subplots()
-                    axis.scatter(df[var[0]],df[othervar[0]],s=3,color="gray")
-                    axis.set_title(f"{othervar[0]} vs. {var[0]}")
-                    axis.set_ylabel(othervar[0])
-                    axis.set_xlabel(var[0])
-                    plt.tight_layout()
-                    plt.show()
-# T-Test #
-
-def T_Test(df:pd.DataFrame, Zielvariable, Zielvariable_Wert_gut, Zielvariable_Wert_schlecht):
-    """
-    [metrisch] - [kategorisch]\n
-    Stellt die unterschiedlichen stat. Abhängigkeiten mit Mittelwert und Standardabweichung visuell dar
-    @Zielvariable: Nur zwei Ausprägungen
-    """
+    # Tabelle
     
-    print("--------------------------------------------------")
-    print("|                     T-Test                     |")
-    print("--------------------------------------------------")
+    Ergebnistabelle = T_Ergebnis + X_Ergebnis
+    Ergebnistabelle = sorted(Ergebnistabelle,key=lambda x: x[1])
+    pd.options.display.float_format = '{:,.2f}'.format
+    Tabelle = pd.DataFrame(Ergebnistabelle, columns=['Variable', 'p-Wert',"X²;T-Wert",u"\u03bc_größer_grenze",u"\u03C3_größer_grenze",u"\u03bc_kleiner_grenze",u"\u03C3_kleiner_grenze","  dof  ","Testverfahren"])
     
-    subset_good=df[df[Zielvariable]==Zielvariable_Wert_gut]
-    subset_bad=df[df[Zielvariable]==Zielvariable_Wert_schlecht]
-    for testvar in df.keys():
-        if df.dtypes[testvar]=="int64" or df.dtypes[testvar]=="float64":
-            tval,pval=ttest_ind(subset_good[testvar],subset_bad[testvar])
-            print(testvar,"-",Zielvariable,":","\nt =",'{:.1f}'.format(abs(tval)),"\np =",'{:.1f}'.format(pval),pval)
+    display(Tabelle)
+    
+    Cor_tab(df,max=10)
+    
+    # Ausgabe X²-Test
+    
+    if Zielvariable_bad=="":
+        if Zielvariable_Grenze==0:
+            Bad = "< "+ "{:.1f}".format(df[Zielvariable].values.mean())
+            Good = "> "+ "{:.1f}".format(df[Zielvariable].values.mean())
+        else:
+            Bad = "< "+ f"{Zielvariable_Grenze}"
+            Good = "> "+ f"{Zielvariable_Grenze}" 
+    else:
+        Bad = Zielvariable_bad
+        Good = Zielvariable_good  
+    
+    if Anzahl_an_gewünschten_Variablen==None:
+        Anzahl = Tabelle["Variable"].values
+    else:
+        Anzahl = Tabelle.iloc[0:Anzahl_an_gewünschten_Variablen]["Variable"].values
+    
+    
+    for i in range(len(X_Tabelle)):
+        if ((X_Tabelle[i][0]).index.name) in Anzahl:
+            a = pd.DataFrame(X_Tabelle[i][0]) 
+            b = pd.DataFrame(X_Tabelle[i][1])
+            b=b.set_index(a.index)
+            merge = pd.concat([a,b],axis=1)
+            merge.columns=[Good,Bad,f"{Good}_erwartet",f"{Bad}_erwartet"]
+            
+            merge[f"{Good}%"] = merge[Good].combine(merge[f"{Good}_erwartet"], min) / merge[Good].combine(merge[f"{Good}_erwartet"], max)*100#merge["True"]/merge["True_erwartet"]*100
+            merge[f"{Bad}%"] = merge[Bad].combine(merge[f"{Bad}_erwartet"], min) / merge[Bad].combine(merge[f"{Bad}_erwartet"], max)*100
+            # merge = merge[["True","True_erwartet","False","False_erwartet","True%","False%"]]
+            merge = merge.reindex(columns=merge.columns[[0,2,4,1,3,5]])
+            merge = merge.rename_axis(Zielvariable,axis="columns")
+            print(u"\u03c1 wert = {:.2f}".format(X_Ergebnis[i][1]),X_Ergebnis[i][1])
+            print(u"\u03c7² = {:.2f}".format(X_Ergebnis[i][2]))
+            print(f"dof = {X_Ergebnis[i][7]}")
             
+            display(merge)
+            print()
+    
+    for i in range(len(T_Ergebnis)):
+        if ((T_Ergebnis[i][0])) in Anzahl:
+            t=T_Ergebnis[i]
             figure,axis=plt.subplots()
-            heights=[subset_good[testvar].mean(),subset_bad[testvar].mean()]
-            stds=[[0,0],[subset_good[testvar].std(),subset_bad[testvar].std()]]
-            print(Zielvariable_Wert_gut,": ",u"\u03bc \u2248 ",'{:.4f}'.format(heights[0]),",",u"\u03C3 \u2248 \u00B1",'{:.4f}'.format(stds[1][0]))
-            print(Zielvariable_Wert_schlecht,": ",u"\u03bc \u2248 ",'{:.4f}'.format(heights[1]),",",u"\u03C3 \u2248 \u00B1",'{:.4f}'.format(stds[1][1]))      
-            axis.bar(x=np.arange(len(heights)),height=heights,tick_label=[Zielvariable_Wert_gut, Zielvariable_Wert_schlecht],color="gray",yerr=stds,ecolor="gray",width=0.4,capsize=4)
-            axis.set_title(f"{testvar} vs. {Zielvariable}")
-            axis.set_ylabel(f"Durchschnitt {testvar}");
+            
+            print(t[0],"-",Zielvariable,":","\nt =",'{:.1f}'.format(abs(t[2])),"\np =",'{:.1f}'.format(t[1]),t[1])
+            print(Good,": ",u"\u03bc \u2248 ",'{:.4f}'.format(t[3]),",",u"\u03C3 \u2248 \u00B1",'{:.4f}'.format(t[4]))
+            print(Bad,": ",u"\u03bc \u2248 ",'{:.4f}'.format(t[5]),",",u"\u03C3 \u2248 \u00B1",'{:.4f}'.format(t[6]))      
+            axis.bar(x=np.arange(2),height=[t[3],t[5]],tick_label=[Good, Bad],color="gray",yerr=[[0,0],[t[4],t[6]]],ecolor="gray",width=0.4,capsize=4)
+            axis.set_title(f"{t[0]} vs. {Zielvariable}")
+            axis.set_ylabel(f"Durchschnitt {t[0]}");
             axis.set_xlabel(Zielvariable);
             plt.tight_layout()
             plt.show()
-
-# chi2 - Test #
-
-def chi_square_einzeln(df:pd.DataFrame, varname, Zielvariable):
-    """
-    [kategorisch] - [kategorisch]
-    """
-    contingencyTable=pd.crosstab(df[varname],df[Zielvariable])
-    chi2,pval,dof,expectedFreq=chi2_contingency(contingencyTable)
-    if pval<0.05:
-        print(varname,"--",Zielvariable,":","chi2=",'{:.1f}'.format(chi2),"p=",'{:.5f}'.format(pval),"dof=",dof)#show pval in non-scienetific expression
-        #print("expected values\n",expectedFreq)
-        #print(contingencyTable)
-    else:
-        print(f"Es gibt keinen stat. Zusammenhang p>0.05 bei {varname} --> p={pval};chi2={chi2}")
-    return contingencyTable
-
-def chi_square_einzeln_mit_Erwartungswerten(df:pd.DataFrame, varname, Zielvariable):
-    """
-    [kategorisch] - [kategorisch]\n
-    Mit Tabelle
-    """
-    contingencyTable=pd.crosstab(df[varname],df[Zielvariable])
-    chi2,pval,dof,expectedFreq=chi2_contingency(contingencyTable)
-    if pval<0.05:
-        print(varname,"--",Zielvariable,":",u"\u03C7\u00B2=",'{:.1f}'.format(chi2),"p=",'{:.5f}'.format(pval),"dof=",dof)#show pval in non-scienetific expression
-        print("expected values\n",expectedFreq)
-        print(contingencyTable)
-    else:
-        print(f"Es gibt keinen stat. Zusammenhang p>0.05 bei {varname} --> p={pval} \u03C7\u00B2={chi2}")
-    return contingencyTable
-
-def chi_square_all(df:pd.DataFrame, Zielvariable):
-    """
-    [kategorisch] - [kategorisch]\n
-    Erstellt alle möglichen chi2-Werte und p werte\n
-    p<0.05 und chi2 sehr groß --> Signifikant
-    """
-    print("--------------------------------------------------")
-    print("|                   Chi² - Test                  |")
-    print("--------------------------------------------------")
-    for var in df.dtypes.items():
-        if var[1].name=="object" and var[0]!=Zielvariable:
-            chi_square_einzeln_mit_Erwartungswerten(df, var[0], Zielvariable)
-            print(30*"---")
-
-def Analyse(df:pd.DataFrame,Zielvariable:str ,Zielvariable_gut,Zielvariable_schlecht,max=20):
-    """
-    Eine rundumanalyse eines Datensatzes in statistischer Form\n
-    Beachte, dass die Zielvariable kategorisch sein sollte, wenn nicht benutzte .map um es einzufügen
-    """
-    print("                                   --------------------------------------------------")
-    print("                                   |                     Analyse                    |")
-    print("                                   --------------------------------------------------")
-    Correlation_table(df,max) # Numerische Korrelationen
-    #time.sleep(0.5)
-    Correlation_analysis_all(df) # Grafiken zu numerischen Korrelationen
-    T_Test(df,Zielvariable,Zielvariable_gut,Zielvariable_schlecht) # Numerisch - Kategorischen Korrelationen
-    chi_square_all(df,Zielvariable) # Kategorisch - Kategorisch Korrelationen
     
+    ## Ausgabe
+    if Anzahl_an_gewünschten_Variablen==None:
+        return Tabelle,X_Tabelle,T_Ergebnis
+    else:
+        return Tabelle.iloc[0:Anzahl_an_gewünschten_Variablen],X_Tabelle,T_Ergebnis
 def make_scatter_plot(x,y, width:int=8, height:int=6, xlabel:str="", ylabel:str="" ,title:str="", color="gray", filename:str="fig.png"):
     """Outputs a scatter plot
     
     Args:
         x: array with x-values
         y: array with y-values
         xticks (optional): list with values to use as x-ticks
```

### Comparing `datawhispers-0.2.8.8/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.8.9/datawhispers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.8
+Version: 0.2.8.9
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.8/setup.py` & `datawhispers-0.2.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = "0.2.8.8",      # Start with a small number and increase it with every change you make
+  version = "0.2.8.9",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

