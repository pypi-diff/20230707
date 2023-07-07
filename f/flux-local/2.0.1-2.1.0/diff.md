# Comparing `tmp/flux-local-2.0.1.tar.gz` & `tmp/flux-local-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-2.0.1.tar", last modified: Sat Jul  1 22:28:37 2023, max compression
+gzip compressed data, was "flux-local-2.1.0.tar", last modified: Thu Jul  6 19:54:21 2023, max compression
```

## Comparing `flux-local-2.0.1.tar` & `flux-local-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 22:28:23.000000 flux-local-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 22:28:37.262033 flux-local-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-01 22:28:23.000000 flux-local-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.258033 flux-local-2.0.1/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-01 22:28:37.262033 flux-local-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 22:28:23.000000 flux-local-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:54:21.959898 flux-local-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 19:54:08.000000 flux-local-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-06 19:54:21.959898 flux-local-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-06 19:54:08.000000 flux-local-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:54:21.955898 flux-local-2.1.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26495 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:54:21.959898 flux-local-2.1.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-06 19:54:08.000000 flux-local-2.1.0/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:54:21.955898 flux-local-2.1.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-06 19:54:21.000000 flux-local-2.1.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-06 19:54:21.000000 flux-local-2.1.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:54:21.000000 flux-local-2.1.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 19:54:21.000000 flux-local-2.1.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 19:54:21.000000 flux-local-2.1.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 19:54:21.000000 flux-local-2.1.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 19:54:21.959898 flux-local-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-06 19:54:08.000000 flux-local-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:54:21.959898 flux-local-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-06 19:54:08.000000 flux-local-2.1.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-07-06 19:54:08.000000 flux-local-2.1.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-06 19:54:08.000000 flux-local-2.1.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-06 19:54:08.000000 flux-local-2.1.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-06 19:54:08.000000 flux-local-2.1.0/tests/test_manifest.py
```

### Comparing `flux-local-2.0.1/LICENSE` & `flux-local-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/PKG-INFO` & `flux-local-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 2.0.1
+Version: 2.1.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-2.0.1/README.md` & `flux-local-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/command.py` & `flux-local-2.1.0/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/exceptions.py` & `flux-local-2.1.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/git_repo.py` & `flux-local-2.1.0/flux_local/git_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 KUSTOMIZE_KIND = "Kustomization"
 HELM_REPO_KIND = "HelmRepository"
 HELM_RELEASE_KIND = "HelmRelease"
 CLUSTER_POLICY_KIND = "ClusterPolicy"
 GIT_REPO_KIND = "GitRepository"
 OCI_REPO_KIND = "OCIRepository"
 DEFAULT_NAMESPACE = "flux-system"
+ROOT_KUSTOMIZATION_NAME = "flux-system"
 
 
 @dataclass
 class Source:
     """A source is a named mapping from a k8s object name to a path in the git repo.
 
     This is needed to map the location within a reop if it's not the root. For example,
@@ -377,15 +378,16 @@
                 f"Try specifying another path within the git repo?"
             )
 
         # Source path is relative to the search path. Update to have the
         # full prefix relative to the root.
         for kustomization in docs:
             if not kustomization.path:
-                kustomization.path = str(root / path)
+                _LOGGER.debug("Assigning implicit path %s", path_selector.relative_path)
+                kustomization.path = str(path_selector.relative_path)
             if not kustomization.source_path:
                 continue
             kustomization.source_path = str(
                 ((root / path) / kustomization.source_path).relative_to(root)
             )
             _LOGGER.debug(
                 "Updated relative path: %s => %s",
@@ -463,14 +465,17 @@
     for ks in kustomizations:
         if not ks.source_path:
             raise InputException(
                 "Kustomization did not have source path; Old kustomize?"
             )
 
         graph.add_node(node_name(ks), ks=ks)
+        if ks.name == ROOT_KUSTOMIZATION_NAME and ks.namespace == DEFAULT_NAMESPACE:
+            # Do not attempt parent search below
+            continue
 
         # Find the parent Kustomization that produced this based on the
         # matching the kustomize source parent paths with a Kustomization
         # target path.
         source = Path(ks.source_path)
         _LOGGER.debug("--- Examining candidate Kustomization ---")
         _LOGGER.debug("Ks         : %s", ks.namespaced_name)
@@ -487,27 +492,33 @@
                 # the source path so within the same cluster.
                 if candidate.namespaced_name != ks.namespaced_name:
                     _LOGGER.debug(
                         "Found parent %s => %s",
                         ks.namespaced_name,
                         candidate.namespaced_name,
                     )
-                    graph.add_edge(node_name(candidate), node_name(ks))
+                    if graph.has_edge(node_name(ks), node_name(candidate)):
+                        _LOGGER.debug("Already has opposite edge; Skipping cycle")
+                    else:
+                        graph.add_edge(node_name(candidate), node_name(ks))
                 else:
                     _LOGGER.debug(
                         "Skipping candidate source %s", candidate.namespaced_name
                     )
         else:
             _LOGGER.debug("No parent for %s (source=%s)", node_name(ks), source)
 
     # Clusters are subgraphs within the graph that are connected, with the root
     # node being the cluster itself. All children Kustomizations are flattended.
     _LOGGER.debug("Creating clusters based on connectivity")
+    for node, degree in graph.in_degree():
+        _LOGGER.debug("Node: %s, degree: %s", node, degree)
     roots = [node for node, degree in graph.in_degree() if degree == 0]
     roots.sort()
+
     clusters: list[Cluster] = []
     _LOGGER.debug("roots=%s", roots)
     for root in roots:
         root_ks = graph.nodes[root]["ks"]
         nodes = [root] + list(networkx.descendants(graph, root))
         nodes.sort()
         kustomizations = [graph.nodes[node]["ks"] for node in nodes]
@@ -658,19 +669,23 @@
     clusters = await get_clusters(
         selector.path, selector.cluster, selector.kustomization
     )
     if not clusters and selector.path.path:
         _LOGGER.debug("No clusters found; Processing as a Kustomization: %s", selector)
         # The argument path may be a Kustomization inside a cluster. Create a synthetic
         # cluster with any found Kustomizations
-        cluster = Cluster(name="cluster", namespace="", path=str(selector.path.path))
+        cluster = Cluster(
+            name="cluster", namespace="", path=str(selector.path.relative_path)
+        )
         objects = await get_kustomizations(selector.path.path)
         if objects:
             cluster.kustomizations = [
-                Kustomization(name="kustomization", path=str(selector.path.path))
+                Kustomization(
+                    name="kustomization", path=str(selector.path.relative_path)
+                )
             ]
             clusters.append(cluster)
 
     async def update_kustomization(cluster: Cluster) -> None:
         build_tasks = []
         for kustomization in cluster.kustomizations:
             _LOGGER.debug(
```

### Comparing `flux-local-2.0.1/flux_local/helm.py` & `flux-local-2.1.0/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/kustomize.py` & `flux-local-2.1.0/flux_local/kustomize.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,19 @@
 ]
 
 KUSTOMIZE_BIN = "kustomize"
 KYVERNO_BIN = "kyverno"
 HELM_RELEASE_KIND = "HelmRelease"
 KUSTOMIZE_FILES = ["kustomization.yaml", "kustomization.yml", "Kustomization"]
 
+# Use the same behavior as flux to allow loading files outside the directory
+# containing kustomization.yaml
+# https://fluxcd.io/flux/faq/#what-is-the-behavior-of-kustomize-used-by-flux
+KUSTOMIZE_BUILD_FLAGS = ["--load-restrictor=LoadRestrictionsNone"]
+
 
 class Kustomize:
     """Library for issuing a kustomize command."""
 
     def __init__(self, cmds: list[Task]) -> None:
         """Initialize Kustomize, used internally for copying object."""
         self._cmds = cmds
@@ -186,15 +191,17 @@
 
 class Build(Task):
     """A task that issues a build command, handling implicit Kustomizations."""
 
     def __init__(self, path: Path, kustomize_flags: list[str] | None = None) -> None:
         """Initialize Build."""
         self._path = path
-        self._kustomize_flags = kustomize_flags or []
+        self._kustomize_flags = list(KUSTOMIZE_BUILD_FLAGS)
+        if kustomize_flags:
+            self._kustomize_flags.extend(kustomize_flags)
 
     async def run(self, stdin: bytes | None = None) -> bytes:
         """Run the task."""
         if stdin is not None:
             raise InputException("Invalid stdin cannot be passed to build command")
 
         if not await isdir(self._path):
```

### Comparing `flux-local-2.0.1/flux_local/manifest.py` & `flux-local-2.1.0/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/tool/build.py` & `flux-local-2.1.0/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/tool/diff.py` & `flux-local-2.1.0/flux_local/tool/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 ) -> Generator[git_repo.PathSelector, None, None]:
     """Create a context manager for the diff path.
 
     This will create a new worktree by default, or use the path in the flags
     which is useful when run from CI.
     """
     if path_orig := kwargs.get("path_orig"):
-        yield git_repo.PathSelector(path_orig)
+        yield git_repo.PathSelector(path_orig, sources=kwargs.get("sources"))
         return
 
     with git_repo.create_worktree(selector.repo) as worktree:
         yield git_repo.PathSelector(pathlib.Path(worktree) / selector.relative_path)
 
 
 class DiffKustomizationAction:
```

### Comparing `flux-local-2.0.1/flux_local/tool/flux_local.py` & `flux-local-2.1.0/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/tool/format.py` & `flux-local-2.1.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/tool/get.py` & `flux-local-2.1.0/flux_local/tool/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
             selector=query, options=selector.options(**kwargs)
         )
 
         results: list[dict[str, str]] = []
         cols = ["name", "path"]
         if output == "wide":
             cols.extend(["helmrepos", "releases"])
+        if query.kustomization.namespace is None:
+            cols.insert(0, "namespace")
         if len(manifest.clusters) > 1:
             cols.insert(0, "cluster")
         for cluster in manifest.clusters:
             for ks in cluster.kustomizations:
                 value = ks.dict(include=set(cols))
                 if output == "wide":
                     value["helmrepos"] = len(ks.helm_repos)
```

### Comparing `flux-local-2.0.1/flux_local/tool/selector.py` & `flux-local-2.1.0/flux_local/tool/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,17 +204,18 @@
 ) -> git_repo.ResourceSelector:
     """Build a selector object form the specified flags."""
     _LOGGER.debug("Building flux cluster Kustomization selector from args: %s", kwargs)
     selector = git_repo.ResourceSelector()
     selector.path = git_repo.PathSelector(
         kwargs.get("path"), sources=kwargs.get("sources")
     )
-    selector.cluster.namespace = kwargs.get("namespace")
+    selector.kustomization.namespace = kwargs.get("namespace")
     if kwargs.get("all_namespaces"):
         selector.cluster.namespace = None
+        selector.kustomization.namespace = None
     return selector
 
 
 def not_found(resource: str, mds: git_repo.MetadataSelector) -> str:
     """Return a not found error message for the given resource type and query."""
     if mds.name:
         return (
```

### Comparing `flux-local-2.0.1/flux_local/tool/test.py` & `flux-local-2.1.0/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/flux_local/tool/visitor.py` & `flux-local-2.1.0/flux_local/tool/visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,24 @@
 
     cluster_path: str
     kustomization_path: str
     kind: str
     namespace: str
     name: str
 
+    def __post_init__(self) -> None:
+        if self.cluster_path.startswith("/"):
+            raise AssertionError(
+                f"Expected cluster_path as relative: {self.cluster_path}"
+            )
+        if self.kustomization_path.startswith("/"):
+            raise AssertionError(
+                f"Expected kustomization_path as relative: {self.kustomization_path}"
+            )
+
     @property
     def label(self) -> str:
         parts = []
         # Either path is a unique identifier within the git repo so prefer the
         # most specific path first.
         if self.kustomization_path and self.kustomization_path != ".":
             parts.append(self.kustomization_path)
```

### Comparing `flux-local-2.0.1/flux_local.egg-info/PKG-INFO` & `flux-local-2.1.0/flux_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 2.0.1
+Version: 2.1.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-2.0.1/flux_local.egg-info/SOURCES.txt` & `flux-local-2.1.0/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/setup.cfg` & `flux-local-2.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 2.0.1
+version = 2.1.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-2.0.1/tests/test_command.py` & `flux-local-2.1.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/tests/test_git_repo.py` & `flux-local-2.1.0/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/tests/test_helm.py` & `flux-local-2.1.0/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.1/tests/test_kustomize.py` & `flux-local-2.1.0/tests/test_kustomize.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,7 +171,19 @@
 async def test_fluxtomize_ignores_empty_subdir(tmp_path: Path) -> None:
     """Test implicit kustomization."""
     subdir = tmp_path / "subdir"
     subdir.mkdir()
 
     content = await kustomize.fluxtomize(tmp_path)
     assert not content
+
+
+async def test_build_flags() -> None:
+    """Test a kustomize build command with extra flags."""
+    result = await kustomize.build(
+        TESTDATA_DIR / "repo",
+        # Duplicates existing flags, should be a no-op
+        kustomize_flags=["--load-restrictor=LoadRestrictionsNone"],
+    ).run()
+    assert "Secret" in result
+    assert "ConfigMap" in result
+    assert result == (TESTDATA_DIR / "repo/all.golden").read_text()
```

### Comparing `flux-local-2.0.1/tests/test_manifest.py` & `flux-local-2.1.0/tests/test_manifest.py`

 * *Files identical despite different names*

