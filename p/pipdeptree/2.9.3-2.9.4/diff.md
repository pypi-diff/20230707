# Comparing `tmp/pipdeptree-2.9.3.tar.gz` & `tmp/pipdeptree-2.9.4.tar.gz`

## Comparing `pipdeptree-2.9.3.tar` & `pipdeptree-2.9.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/tox.ini
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.github/dependabot.yml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.github/workflows/check.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.github/workflows/release.yml
--rw-r--r--   0        0        0    39278 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/src/pipdeptree/version.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    35359 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/LICENSE
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/README.md
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/pyproject.toml
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pipdeptree-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/CHANGES.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/tox.ini
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/workflows/check.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0    39608 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    41622 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/LICENSE
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/PKG-INFO
```

### Comparing `pipdeptree-2.9.3/.pre-commit-config.yaml` & `pipdeptree-2.9.4/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.272"
+    rev: "v0.0.277"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "1.3.0"
+    rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "0.11.2"
+    rev: "0.13.0"
     hooks:
       - id: pyproject-fmt
-        additional_dependencies: ["tox>=4.6"]
+        additional_dependencies: ["tox>=4.6.4"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         args: ["--print-width=120", "--prose-wrap=always"]
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
```

### Comparing `pipdeptree-2.9.3/CHANGES.md` & `pipdeptree-2.9.4/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.3/tox.ini` & `pipdeptree-2.9.4/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       tests}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
 skip_install = true
 deps =
-    pre-commit>=3.3.2
+    pre-commit>=3.3.3
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:readme]
 description = check that the long description is valid
 base_python = python3.10
 skip_install = true
```

### Comparing `pipdeptree-2.9.3/.github/workflows/check.yml` & `pipdeptree-2.9.4/.github/workflows/check.yml`

 * *Files 4% similar despite different names*

```diff
@@ -91,12 +91,12 @@
           python-version: "3.11"
       - name: install build
         run: python -m pip install build
       - uses: actions/checkout@v3
       - name: build package
         run: python -m build --sdist --wheel . -o dist
       - name: publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           skip_existing: true
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `pipdeptree-2.9.3/.github/workflows/release.yml` & `pipdeptree-2.9.4/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         run: python -m pip install build
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Build package
         run: pyproject-build -s -w . -o dist
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
```

### Comparing `pipdeptree-2.9.3/src/pipdeptree/__init__.py` & `pipdeptree-2.9.4/src/pipdeptree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         for k, vs in self._obj.items():
             for v in vs:
                 # if v is already added to the dict, then ensure that
                 # we are using the same object. This check is required
                 # as we're using array mutation
                 try:
                     node = [p for p in m if p.key == v.key][0]
-                except IndexError:
+                except IndexError:  # noqa: PERF203
                     node = v
                 m[node].append(k.as_parent_of(v))
             if k.key not in child_keys:
                 m[k.as_requirement()] = []
         return ReversedPackageDAG(dict(m))
 
     def sort(self):
@@ -452,23 +452,23 @@
         """
         m = defaultdict(list)
         child_keys = {r.key for r in chain.from_iterable(self._obj.values())}
         for k, vs in self._obj.items():
             for v in vs:
                 try:
                     node = [p for p in m if p.key == v.key][0]
-                except IndexError:
+                except IndexError:  # noqa: PERF203
                     node = v.as_parent_of(None)
                 m[node].append(k)
             if k.key not in child_keys:
                 m[k.dist] = []
         return PackageDAG(dict(m))
 
 
-def render_text(tree, max_depth, list_all=True, frozen=False):  # noqa: FBT002
+def render_text(tree, max_depth, encoding, list_all=True, frozen=False):  # noqa: FBT002
     """
     Print tree as text on console.
 
     :param dict tree: the package tree
     :param bool list_all: whether to list all the pgks at the root level or only those that are the sub-dependencies
     :param bool frozen: show the names of the pkgs in the output that's favourable to pip --freeze
     :returns: None
@@ -476,15 +476,15 @@
     tree = tree.sort()
     nodes = tree.keys()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
 
     if not list_all:
         nodes = [p for p in nodes if p.key not in branch_keys]
 
-    if sys.stdout.encoding.lower() in ("utf-8", "utf-16", "utf-32"):
+    if encoding in ("utf-8", "utf-16", "utf-32"):
         _render_text_with_unicode(tree, nodes, max_depth, frozen)
     else:
         _render_text_without_unicode(tree, nodes, max_depth, frozen)
 
 
 def _render_text_with_unicode(tree, nodes, max_depth, frozen):
     use_bullets = not frozen
@@ -824,29 +824,29 @@
     if hasattr(dump_output, "encode"):
         print(dump_output)  # noqa: T201
     else:
         with os.fdopen(sys.stdout.fileno(), "wb") as bytestream:
             bytestream.write(dump_output)
 
 
-def conflicting_deps(tree):
+def conflicting_deps(tree: PackageDAG) -> dict[DistPackage, list[ReqPackage]]:
     """
     Returns dependencies which are not present or conflict with the requirements of other packages.
 
     e.g. will warn if pkg1 requires pkg2==2.0 and pkg2==1.0 is installed
 
     :param tree: the requirements tree (dict)
     :returns: dict of DistPackage -> list of unsatisfied/unknown ReqPackage
     :rtype: dict
     """
     conflicting = defaultdict(list)
-    for p, rs in tree.items():
-        for req in rs:
+    for package, requires in tree.items():
+        for req in requires:
             if req.is_conflicting():
-                conflicting[p].append(req)
+                conflicting[package].append(req)  # noqa: PERF401
     return conflicting
 
 
 def render_conflicts_text(conflicts):
     if conflicts:
         print("Warning!!! Possibly conflicting dependencies found:", file=sys.stderr)  # noqa: T201
         # Enforce alphabetical order when listing conflicts
@@ -993,14 +993,20 @@
         type=lambda x: int(x) if x.isdigit() and (int(x) >= 0) else parser.error("Depth must be a number that is >= 0"),
         default=float("inf"),
         help=(
             "Display dependency tree up to a depth >=0 using the default text display. All other display options"
             " ignore this argument."
         ),
     )
+    parser.add_argument(
+        "--encoding",
+        dest="encoding_type",
+        default=sys.stdout.encoding,
+        help="Display dependency tree as text using specified encoding",
+    )
     return parser
 
 
 def _get_args():
     parser = get_parser()
     return parser.parse_args()
 
@@ -1110,8 +1116,8 @@
         print(render_json_tree(tree, indent=4))  # noqa: T201
     elif args.mermaid:
         print(render_mermaid(tree))  # noqa: T201
     elif args.output_format:
         output = dump_graphviz(tree, output_format=args.output_format, is_reverse=args.reverse)
         print_graphviz(output)
     else:
-        render_text(tree, args.depth, args.all, args.freeze)
+        render_text(tree, args.depth, args.encoding_type, args.all, args.freeze)
```

### Comparing `pipdeptree-2.9.3/tests/test_pipdeptree.py` & `pipdeptree-2.9.4/tests/test_pipdeptree.py`

 * *Files 23% similar despite different names*

```diff
@@ -490,18 +490,17 @@
             ],
         ),
     ],
 )
 def test_render_text(capsys, list_all, reverse, unicode, expected_output):
     tree = t.reverse() if reverse else t
     encoding = "utf-8" if unicode else "ascii"
-    with mock.patch("sys.stdout", MockStdout(encoding)):
-        render_text(tree, float("inf"), list_all=list_all, frozen=False)
-        captured = capsys.readouterr()
-        assert "\n".join(expected_output).strip() == captured.out.strip()
+    render_text(tree, float("inf"), encoding, list_all=list_all, frozen=False)
+    captured = capsys.readouterr()
+    assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 @pytest.mark.parametrize(
     ("unicode", "level", "expected_output"),
     [
         (
             True,
@@ -586,19 +585,170 @@
                 "  - f [required: >=3.0.0, installed: 3.1]",
                 "    - b [required: >=2.1.0, installed: 2.3.1]",
             ],
         ),
     ],
 )
 def test_render_text_given_depth(capsys, unicode, level, expected_output):
-    encoding = "utf-8" if unicode else "ascii"
-    with mock.patch("sys.stdout", MockStdout(encoding)):
-        render_text(t, level)
-        captured = capsys.readouterr()
-        assert "\n".join(expected_output).strip() == captured.out.strip()
+    render_text(t, level, encoding="utf-8" if unicode else "ascii")
+    captured = capsys.readouterr()
+    assert "\n".join(expected_output).strip() == captured.out.strip()
+
+
+@pytest.mark.parametrize(
+    ("level", "encoding", "expected_output"),
+    [
+        (
+            0,
+            "utf-8",
+            [
+                "a==3.4.0",
+                "b==2.3.1",
+                "c==5.10.0",
+                "d==2.35",
+                "e==0.12.1",
+                "f==3.1",
+                "g==6.8.3rc1",
+            ],
+        ),
+        (
+            0,
+            "utf-8",
+            [
+                "a==3.4.0",
+                "b==2.3.1",
+                "c==5.10.0",
+                "d==2.35",
+                "e==0.12.1",
+                "f==3.1",
+                "g==6.8.3rc1",
+            ],
+        ),
+        (
+            2,
+            "utf-8",
+            [
+                "a==3.4.0",
+                "├── b [required: >=2.0.0, installed: 2.3.1]",
+                "│   └── d [required: >=2.30,<2.42, installed: 2.35]",
+                "└── c [required: >=5.7.1, installed: 5.10.0]",
+                "    ├── d [required: >=2.30, installed: 2.35]",
+                "    └── e [required: >=0.12.1, installed: 0.12.1]",
+                "b==2.3.1",
+                "└── d [required: >=2.30,<2.42, installed: 2.35]",
+                "    └── e [required: >=0.9.0, installed: 0.12.1]",
+                "c==5.10.0",
+                "├── d [required: >=2.30, installed: 2.35]",
+                "│   └── e [required: >=0.9.0, installed: 0.12.1]",
+                "└── e [required: >=0.12.1, installed: 0.12.1]",
+                "d==2.35",
+                "└── e [required: >=0.9.0, installed: 0.12.1]",
+                "e==0.12.1",
+                "f==3.1",
+                "└── b [required: >=2.1.0, installed: 2.3.1]",
+                "    └── d [required: >=2.30,<2.42, installed: 2.35]",
+                "g==6.8.3rc1",
+                "├── e [required: >=0.9.0, installed: 0.12.1]",
+                "└── f [required: >=3.0.0, installed: 3.1]",
+                "    └── b [required: >=2.1.0, installed: 2.3.1]",
+            ],
+        ),
+        (
+            2,
+            "ascii",
+            [
+                "a==3.4.0",
+                "  - b [required: >=2.0.0, installed: 2.3.1]",
+                "    - d [required: >=2.30,<2.42, installed: 2.35]",
+                "  - c [required: >=5.7.1, installed: 5.10.0]",
+                "    - d [required: >=2.30, installed: 2.35]",
+                "    - e [required: >=0.12.1, installed: 0.12.1]",
+                "b==2.3.1",
+                "  - d [required: >=2.30,<2.42, installed: 2.35]",
+                "    - e [required: >=0.9.0, installed: 0.12.1]",
+                "c==5.10.0",
+                "  - d [required: >=2.30, installed: 2.35]",
+                "    - e [required: >=0.9.0, installed: 0.12.1]",
+                "  - e [required: >=0.12.1, installed: 0.12.1]",
+                "d==2.35",
+                "  - e [required: >=0.9.0, installed: 0.12.1]",
+                "e==0.12.1",
+                "f==3.1",
+                "  - b [required: >=2.1.0, installed: 2.3.1]",
+                "    - d [required: >=2.30,<2.42, installed: 2.35]",
+                "g==6.8.3rc1",
+                "  - e [required: >=0.9.0, installed: 0.12.1]",
+                "  - f [required: >=3.0.0, installed: 3.1]",
+                "    - b [required: >=2.1.0, installed: 2.3.1]",
+            ],
+        ),
+        (
+            2,
+            "utf-8",
+            [
+                "a==3.4.0",
+                "├── b [required: >=2.0.0, installed: 2.3.1]",
+                "│   └── d [required: >=2.30,<2.42, installed: 2.35]",
+                "└── c [required: >=5.7.1, installed: 5.10.0]",
+                "    ├── d [required: >=2.30, installed: 2.35]",
+                "    └── e [required: >=0.12.1, installed: 0.12.1]",
+                "b==2.3.1",
+                "└── d [required: >=2.30,<2.42, installed: 2.35]",
+                "    └── e [required: >=0.9.0, installed: 0.12.1]",
+                "c==5.10.0",
+                "├── d [required: >=2.30, installed: 2.35]",
+                "│   └── e [required: >=0.9.0, installed: 0.12.1]",
+                "└── e [required: >=0.12.1, installed: 0.12.1]",
+                "d==2.35",
+                "└── e [required: >=0.9.0, installed: 0.12.1]",
+                "e==0.12.1",
+                "f==3.1",
+                "└── b [required: >=2.1.0, installed: 2.3.1]",
+                "    └── d [required: >=2.30,<2.42, installed: 2.35]",
+                "g==6.8.3rc1",
+                "├── e [required: >=0.9.0, installed: 0.12.1]",
+                "└── f [required: >=3.0.0, installed: 3.1]",
+                "    └── b [required: >=2.1.0, installed: 2.3.1]",
+            ],
+        ),
+        (
+            2,
+            "ascii",
+            [
+                "a==3.4.0",
+                "  - b [required: >=2.0.0, installed: 2.3.1]",
+                "    - d [required: >=2.30,<2.42, installed: 2.35]",
+                "  - c [required: >=5.7.1, installed: 5.10.0]",
+                "    - d [required: >=2.30, installed: 2.35]",
+                "    - e [required: >=0.12.1, installed: 0.12.1]",
+                "b==2.3.1",
+                "  - d [required: >=2.30,<2.42, installed: 2.35]",
+                "    - e [required: >=0.9.0, installed: 0.12.1]",
+                "c==5.10.0",
+                "  - d [required: >=2.30, installed: 2.35]",
+                "    - e [required: >=0.9.0, installed: 0.12.1]",
+                "  - e [required: >=0.12.1, installed: 0.12.1]",
+                "d==2.35",
+                "  - e [required: >=0.9.0, installed: 0.12.1]",
+                "e==0.12.1",
+                "f==3.1",
+                "  - b [required: >=2.1.0, installed: 2.3.1]",
+                "    - d [required: >=2.30,<2.42, installed: 2.35]",
+                "g==6.8.3rc1",
+                "  - e [required: >=0.9.0, installed: 0.12.1]",
+                "  - f [required: >=3.0.0, installed: 3.1]",
+                "    - b [required: >=2.1.0, installed: 2.3.1]",
+            ],
+        ),
+    ],
+)
+def test_render_text_encoding(capsys, level, encoding, expected_output):
+    render_text(t, level, encoding, True, False)
+    captured = capsys.readouterr()
+    assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 # Tests for graph outputs
 
 
 def randomized_dag_copy(t):
     """Returns a copy of the package tree fixture with dependencies in randomized order."""
```

### Comparing `pipdeptree-2.9.3/LICENSE` & `pipdeptree-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.3/README.md` & `pipdeptree-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.3/pyproject.toml` & `pipdeptree-2.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,20 @@
   "version",
 ]
 optional-dependencies.graphviz = [
   "graphviz>=0.20.1",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
-  "diff-cover>=7.5",
+  "diff-cover>=7.6",
   "pip>=23.1.2",
-  "pytest>=7.3.1",
+  "pytest>=7.4",
   "pytest-cov>=4.1",
-  "pytest-mock>=3.10",
-  "virtualenv<21,>=20.23",
+  "pytest-mock>=3.11.1",
+  "virtualenv<21,>=20.23.1",
 ]
 urls.Changelog = "https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md"
 urls.Documentation = "https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree"
 urls.Homepage = "https://github.com/tox-dev/pipdeptree"
 urls.Source = "https://github.com/tox-dev/pipdeptree"
 urls.Tracker = "https://github.com/tox-dev/pipdeptree/issues"
 scripts.pipdeptree = "pipdeptree:main"
@@ -62,21 +62,14 @@
 [tool.hatch]
 build.hooks.vcs.version-file = "src/pipdeptree/version.py"
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
-[tool.coverage]
-html.show_contexts = true
-html.skip_covered = false
-paths.source = ["src", ".tox/*/lib/python*/site-packages", "*/src"]
-run.parallel = true
-run.plugins = ["covdefaults"]
-
 [tool.ruff]
 select = ["ALL"]
 line-length = 120
 target-version = "py37"
 isort = {known-first-party = ["pipdeptree"], required-imports = ["from __future__ import annotations"]}
 ignore = [
   "INP001", # no implicit namespace
@@ -90,7 +83,14 @@
 "tests/**/*.py" = [
   "S101",  # asserts allowed in tests...
   "FBT",  # don"t care about booleans as positional arguments in tests
   "D",  # don"t care about documentation in tests
   "S603",  # `subprocess` call: check for execution of untrusted input
   "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
 ]
+
+[tool.coverage]
+html.show_contexts = true
+html.skip_covered = false
+paths.source = ["src", ".tox/*/lib/python*/site-packages", "*/src"]
+run.parallel = true
+run.plugins = ["covdefaults"]
```

### Comparing `pipdeptree-2.9.3/PKG-INFO` & `pipdeptree-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.9.3
+Version: 2.9.4
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
@@ -44,20 +44,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Provides-Extra: graphviz
 Requires-Dist: graphviz>=0.20.1; extra == 'graphviz'
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
-Requires-Dist: diff-cover>=7.5; extra == 'test'
+Requires-Dist: diff-cover>=7.6; extra == 'test'
 Requires-Dist: pip>=23.1.2; extra == 'test'
 Requires-Dist: pytest-cov>=4.1; extra == 'test'
-Requires-Dist: pytest-mock>=3.10; extra == 'test'
-Requires-Dist: pytest>=7.3.1; extra == 'test'
-Requires-Dist: virtualenv<21,>=20.23; extra == 'test'
+Requires-Dist: pytest-mock>=3.11.1; extra == 'test'
+Requires-Dist: pytest>=7.4; extra == 'test'
+Requires-Dist: virtualenv<21,>=20.23.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pipdeptree
 
 [![check](https://github.com/tox-dev/pipdeptree/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pipdeptree/actions/workflows/check.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tox-dev/pipdeptree/main.svg)](https://results.pre-commit.ci/latest/github/tox-dev/pipdeptree/main)
```

