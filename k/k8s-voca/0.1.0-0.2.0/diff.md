# Comparing `tmp/k8s_voca-0.1.0.tar.gz` & `tmp/k8s_voca-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8s_voca-0.1.0.tar", last modified: Thu Jul  6 12:38:38 2023, max compression
+gzip compressed data, was "k8s_voca-0.2.0.tar", last modified: Thu Jul  6 12:46:32 2023, max compression
```

## Comparing `k8s_voca-0.1.0.tar` & `k8s_voca-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:38:38.413059 k8s_voca-0.1.0/
--rw-r--r--   0 m2         (502) staff       (20)    35149 2023-07-06 11:56:11.000000 k8s_voca-0.1.0/LICENSE
--rw-r--r--   0 m2         (502) staff       (20)     1473 2023-07-06 12:38:38.413116 k8s_voca-0.1.0/PKG-INFO
--rw-r--r--   0 m2         (502) staff       (20)      908 2023-07-06 12:37:11.000000 k8s_voca-0.1.0/README.md
--rw-r--r--   0 m2         (502) staff       (20)      103 2023-07-06 11:56:11.000000 k8s_voca-0.1.0/pyproject.toml
--rw-r--r--   0 m2         (502) staff       (20)      755 2023-07-06 12:38:38.413408 k8s_voca-0.1.0/setup.cfg
-drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:38:38.411425 k8s_voca-0.1.0/src/
-drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:38:38.412255 k8s_voca-0.1.0/src/k8s_voca/
--rw-r--r--   0 m2         (502) staff       (20)      138 2023-07-06 11:56:11.000000 k8s_voca-0.1.0/src/k8s_voca/__init__.py
--rw-r--r--   0 m2         (502) staff       (20)     4678 2023-07-06 12:37:42.000000 k8s_voca-0.1.0/src/k8s_voca/k8s_voca.py
-drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:38:38.412934 k8s_voca-0.1.0/src/k8s_voca.egg-info/
--rw-r--r--   0 m2         (502) staff       (20)     1473 2023-07-06 12:38:38.000000 k8s_voca-0.1.0/src/k8s_voca.egg-info/PKG-INFO
--rw-r--r--   0 m2         (502) staff       (20)      275 2023-07-06 12:38:38.000000 k8s_voca-0.1.0/src/k8s_voca.egg-info/SOURCES.txt
--rw-r--r--   0 m2         (502) staff       (20)        1 2023-07-06 12:38:38.000000 k8s_voca-0.1.0/src/k8s_voca.egg-info/dependency_links.txt
--rw-r--r--   0 m2         (502) staff       (20)       37 2023-07-06 12:38:38.000000 k8s_voca-0.1.0/src/k8s_voca.egg-info/entry_points.txt
--rw-r--r--   0 m2         (502) staff       (20)        9 2023-07-06 12:38:38.000000 k8s_voca-0.1.0/src/k8s_voca.egg-info/top_level.txt
+drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:46:32.967768 k8s_voca-0.2.0/
+-rw-r--r--   0 m2         (502) staff       (20)    35149 2023-07-06 11:56:11.000000 k8s_voca-0.2.0/LICENSE
+-rw-r--r--   0 m2         (502) staff       (20)     1395 2023-07-06 12:46:32.967825 k8s_voca-0.2.0/PKG-INFO
+-rw-r--r--   0 m2         (502) staff       (20)      830 2023-07-06 12:43:22.000000 k8s_voca-0.2.0/README.md
+-rw-r--r--   0 m2         (502) staff       (20)      103 2023-07-06 11:56:11.000000 k8s_voca-0.2.0/pyproject.toml
+-rw-r--r--   0 m2         (502) staff       (20)      755 2023-07-06 12:46:32.968161 k8s_voca-0.2.0/setup.cfg
+drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:46:32.966040 k8s_voca-0.2.0/src/
+drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:46:32.966926 k8s_voca-0.2.0/src/k8s_voca/
+-rw-r--r--   0 m2         (502) staff       (20)      138 2023-07-06 11:56:11.000000 k8s_voca-0.2.0/src/k8s_voca/__init__.py
+-rw-r--r--   0 m2         (502) staff       (20)     4977 2023-07-06 12:45:19.000000 k8s_voca-0.2.0/src/k8s_voca/k8s_voca.py
+drwxr-xr-x   0 m2         (502) staff       (20)        0 2023-07-06 12:46:32.967659 k8s_voca-0.2.0/src/k8s_voca.egg-info/
+-rw-r--r--   0 m2         (502) staff       (20)     1395 2023-07-06 12:46:32.000000 k8s_voca-0.2.0/src/k8s_voca.egg-info/PKG-INFO
+-rw-r--r--   0 m2         (502) staff       (20)      275 2023-07-06 12:46:32.000000 k8s_voca-0.2.0/src/k8s_voca.egg-info/SOURCES.txt
+-rw-r--r--   0 m2         (502) staff       (20)        1 2023-07-06 12:46:32.000000 k8s_voca-0.2.0/src/k8s_voca.egg-info/dependency_links.txt
+-rw-r--r--   0 m2         (502) staff       (20)       37 2023-07-06 12:46:32.000000 k8s_voca-0.2.0/src/k8s_voca.egg-info/entry_points.txt
+-rw-r--r--   0 m2         (502) staff       (20)        9 2023-07-06 12:46:32.000000 k8s_voca-0.2.0/src/k8s_voca.egg-info/top_level.txt
```

### Comparing `k8s_voca-0.1.0/LICENSE` & `k8s_voca-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `k8s_voca-0.1.0/PKG-INFO` & `k8s_voca-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s_voca
-Version: 0.1.0
+Version: 0.2.0
 Summary: kubernetes vocabulary
 Home-page: https://dmario24.github.io/k8s-voca
 Author: dmario24
 Author-email: data.mario24@gmail.com
 License: GNU General Public License (GPL)
 Project-URL: Bug Tracker, https://github.com/dmario24/k8s-voca/issues
 Platform: macOS
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # k8s-voca
 
 ### kubernetes vocabulary
 
-<img src="https://github.com/dMario24/k8s-voca/assets/134017660/40d16add-96fa-4709-8f1e-f154c10f32af" width=200 />
+![LGTM](https://i.lgtm.fun/2i0x.png)
 
 - [https://pypi.org/project/k8s-voca](https://pypi.org/project/k8s-voca)
 
 ```
 .　/＼＿／ヽ
 ／ _ノ　ヽ_ ＼
 |　　━　 ━　i
```

### Comparing `k8s_voca-0.1.0/README.md` & `k8s_voca-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # k8s-voca
 
 ### kubernetes vocabulary
 
-<img src="https://github.com/dMario24/k8s-voca/assets/134017660/40d16add-96fa-4709-8f1e-f154c10f32af" width=200 />
+![LGTM](https://i.lgtm.fun/2i0x.png)
 
 - [https://pypi.org/project/k8s-voca](https://pypi.org/project/k8s-voca)
 
 ```
 .　/＼＿／ヽ
 ／ _ノ　ヽ_ ＼
 |　　━　 ━　i
```

### Comparing `k8s_voca-0.1.0/setup.cfg` & `k8s_voca-0.2.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = k8s_voca
-version = 0.1.0
+version = 0.2.0
 author = dmario24
 author_email = data.mario24@gmail.com
 description = kubernetes vocabulary
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://dmario24.github.io/k8s-voca
 project_urls =
```

### Comparing `k8s_voca-0.1.0/src/k8s_voca/k8s_voca.py` & `k8s_voca-0.2.0/src/k8s_voca/k8s_voca.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,19 @@
     "Job": "단 한번만 실행 완료 후 중단되는 작업을 정의",
     "CronJob": "스케줄에 따라 반복되고 실행 완료 후 중단되는 작업을 정의",
     "Static Pod": "스태틱 파드는API 서버없이 특정 노드에 있는 kubelet 데몬에 의해 직접 관리된다. 컨트롤 플레인에 의해 관리되는 파드(예를 들어디플로이먼트(Deployment))와는 달리, kubelet 이 각각의 스태틱 파드를 감시한다. (만약 실패할 경우 다시 구동한다.)",
 
     "노드": "쿠버네티스는 컨테이너를 파드내에 배치하고 노드 에서 실행함으로 워크로드를 구동한다. 노드는 클러스터에 따라 가상(EC2) 또는 물리적 머신일 수 있다.",
     "node": "쿠버네티스는 컨테이너를 파드내에 배치하고 노드 에서 실행함으로 워크로드를 구동한다. 노드는 클러스터에 따라 가상(EC2) 또는 물리적 머신일 수 있다.",
 
-    "컨트롤 플레인(마스터 노드)": "컨트롤 플레인은 워커 노드와 클러스터 내 파드를 관리한다.",
+    "Control Plane": "컨트롤 플레인은 워커 노드와 클러스터 내 파드를 관리한다.",
+    "컨트롤 플레인": "컨트롤 플레인은 워커 노드와 클러스터 내 파드를 관리한다.",
+    "마스터 노드": "컨트롤 플레인은 워커 노드와 클러스터 내 파드를 관리한다.",
+
+    "Data Plane": "워커 노드는 애플리케이션의 구성요소인 파드를 호스트한다.",
     "데이타 플레인(워커 노드)": "워커 노드는 애플리케이션의 구성요소인 파드를 호스트한다.",
 
     "ConfigMap": "컨피그맵은 키-값 쌍으로 기밀이 아닌 데이터를 저장",
 
     "Secret": "암호, 토큰 또는 키와 같은 소량의 중요한 데이터를 포함하는 오브젝트",
 
     "서비스": "파드 집합에서 실행중인 애플리케이션을 네트워크 서비스로 노출하는 추상화 방법",
```

### Comparing `k8s_voca-0.1.0/src/k8s_voca.egg-info/PKG-INFO` & `k8s_voca-0.2.0/src/k8s_voca.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-voca
-Version: 0.1.0
+Version: 0.2.0
 Summary: kubernetes vocabulary
 Home-page: https://dmario24.github.io/k8s-voca
 Author: dmario24
 Author-email: data.mario24@gmail.com
 License: GNU General Public License (GPL)
 Project-URL: Bug Tracker, https://github.com/dmario24/k8s-voca/issues
 Platform: macOS
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # k8s-voca
 
 ### kubernetes vocabulary
 
-<img src="https://github.com/dMario24/k8s-voca/assets/134017660/40d16add-96fa-4709-8f1e-f154c10f32af" width=200 />
+![LGTM](https://i.lgtm.fun/2i0x.png)
 
 - [https://pypi.org/project/k8s-voca](https://pypi.org/project/k8s-voca)
 
 ```
 .　/＼＿／ヽ
 ／ _ノ　ヽ_ ＼
 |　　━　 ━　i
```

