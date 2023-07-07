# Comparing `tmp/problem_bank_scripts-0.6.2.tar.gz` & `tmp/problem_bank_scripts-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.6.2.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.7.0.tar", max compression
```

## Comparing `problem_bank_scripts-0.6.2.tar` & `problem_bank_scripts-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.6.2/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.6.2/README.md
--rw-r--r--   0        0        0     1052 2023-06-16 02:56:32.963969 problem_bank_scripts-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-16 02:56:39.428442 problem_bank_scripts-0.6.2/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.6.2/src/problem_bank_scripts/attributions.json
--rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.6.2/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    42101 2023-06-16 02:55:43.161647 problem_bank_scripts-0.6.2/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.6.2/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.6.2/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2647 2023-06-16 02:56:59.648513 problem_bank_scripts-0.6.2/setup.py
--rw-r--r--   0        0        0     2679 2023-06-16 02:56:59.648759 problem_bank_scripts-0.6.2/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.7.0/README.md
+-rw-r--r--   0        0        0     1051 2023-07-07 00:05:52.988895 problem_bank_scripts-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-07 00:06:02.994431 problem_bank_scripts-0.7.0/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.7.0/src/problem_bank_scripts/attributions.json
+-rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.7.0/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    46545 2023-07-07 00:05:32.880433 problem_bank_scripts-0.7.0/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.7.0/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.7.0/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2643 2023-07-07 00:07:06.814077 problem_bank_scripts-0.7.0/setup.py
+-rw-r--r--   0        0        0     2625 2023-07-07 00:07:06.814296 problem_bank_scripts-0.7.0/PKG-INFO
```

### Comparing `problem_bank_scripts-0.6.2/README.md` & `problem_bank_scripts-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.2/pyproject.toml` & `problem_bank_scripts-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.6.2"
+version = "0.7.0"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^1.2.4"
+python = "^3.9"
+pandas = "^2.0"
 PyYAML = "^6.0"
 docopt = "^0.6.2"
 numpy = "^1.22"
 markdown-it-py = "^2.1.0"
 mdformat = "^0.7.14"
 sympy = "^1.8"
-problem-bank-helpers = "^0.1.12"
+problem-bank-helpers = "^0.1.14"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.4"
 nbsphinx = "^0.8.5"
 ipykernel = "^5.5.5"
 sphinx-autoapi = "^1.8.1"
 sphinx-rtd-theme = "^0.5.2"
@@ -32,8 +32,8 @@
 myst-parser = "^0.17"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-filterwarnings = ["ignore::DeprecationWarning"]
+filterwarnings = ["ignore::DeprecationWarning"]
```

### Comparing `problem_bank_scripts-0.6.2/src/problem_bank_scripts/attributions.json` & `problem_bank_scripts-0.7.0/src/problem_bank_scripts/attributions.json`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.2/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.7.0/src/problem_bank_scripts/prairielearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This file has been copied directly from the PL repo: https://github.com/PrairieLearn/PrairieLearn/blob/master/lib/python_helper_sympy.py
+# This has now been updated to: https://github.com/PrairieLearn/PrairieLearn/blob/master/apps/prairielearn/python/python_helper_sympy.py
 
 import sympy
 # import ast
 # import sys
 
 # import lxml.html
 # import html
@@ -345,8 +346,8 @@
             for j in range(0, num_cols):
                 row.append(str(v[i, j]))
             M.append(row)
         return {'_type': 'sympy_matrix', '_value': M, '_variables': s, '_shape': [num_rows, num_cols]}
     elif isinstance(v, pandas.DataFrame):
         return {'_type': 'dataframe', '_value': {'index': list(v.index), 'columns': list(v.columns), 'data': v.values.tolist()}}
     else:
-        return v
+        return v
```

### Comparing `problem_bank_scripts-0.6.2/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.7.0/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,19 +83,17 @@
         len(tokens[level2_headers[0] + 1].content) < 20
     ), "There is an (arbitrary/opinionated) restriction on the length of 20 chars for a a 'part' title."
 
     nested_dict[part]["title"] = tokens[level2_headers[0] + 1].content
 
     # Store the content of the level 2 header
     try:
-        content = codecs.unicode_escape_decode(
-            mdformat.renderer.MDRenderer().render(
+        content = mdformat.renderer.MDRenderer().render(
                 tokens[3 : get_next_headerloc(3, tokens, 3)], mdit.options, env
             )  # Note the 3 is there to exclude header start,header content,header end tokens
-        )[0]
         nested_dict[part]["content"] = content
     except IndexError:
         print("It looks like there is an empty section of header level 2 in your md file.")
         raise
 
     # Get all Level 3 headers
     level3_headers = [i for i, j in enumerate(tokens) if j.tag == "h3" if j.nesting == 1]
@@ -330,17 +328,15 @@
     body_parts = {}
     parts_dict = {}
 
     part_counter = 0
 
     for k, v in blocks.items():
 
-        rendered_part = codecs.unicode_escape_decode(
-            mdformat.renderer.MDRenderer().render(tokens[v[0] : v[1]], mdit.options, env)
-        )[0]
+        rendered_part = mdformat.renderer.MDRenderer().render(tokens[v[0] : v[1]], mdit.options, env)
 
         if k == "title":
             body_parts["title"] = rendered_part
 
         elif k == "preamble":
             body_parts["preamble"] = rendered_part
 
@@ -435,15 +431,16 @@
         q_types.append(parsed_question["header"][part]["type"])
 
     auto_tags = []
     if len(q_types) > 1:
         auto_tags.append("multi_part")
     auto_tags.extend(list(set(q_types)))
 
-    auto_tags.extend(parsed_question["header"]["tags"])
+    # tags is technically an optional key for a question author to specify
+    auto_tags.extend(parsed_question["header"].get("tags", []))
     auto_tags = [v for v in auto_tags if v != "unknown"]
 
     info_json = {
         "uuid": str(uuid.uuid3(uuid.NAMESPACE_DNS, str(output_path))),
         "title": parsed_question["header"]["title"],
         "topic": parsed_question["header"]["topic"],
         "tags": auto_tags,
@@ -503,14 +500,23 @@
     output_path = pathlib.Path(output_path)
 
     server_file = assemble_server_py(parsed_question, "prairielearn")
 
     # Deal with path differences when using PL
     server_file = server_file.replace('read_csv("', 'read_csv(data["options"]["client_files_course_path"]+"/')
 
+    server_file = re.sub(
+        r"(data2?\[(?P<Quote1>\"|\')params(?P=Quote1)\]\[(?P<Quote2>\"|\')part\d+(?P=Quote2)\]"
+        + r"\[(?P<Quote3>\"|\')ans\d+(?P=Quote3)\]\[(?P<Quote4>\"|\')value(?P=Quote4)\] ?= "
+        + r"?f?(?P<Opening>\"{3}|\'{3}|\"|\'|).*?(?P=Opening)$)",
+        lambda match: backticks_to_code_tags(match.expand(r"\1")),
+        server_file,
+        flags=re.MULTILINE | re.DOTALL,
+    )
+
     # Write server.py
     (output_path / "server.py").write_text(server_file, encoding="utf8")
 
 
 def process_multiple_choice(part_name, parsed_question, data_dict):
     """Processes markdown format multiple-choice questions and returns PL HTML
     Args:
@@ -543,15 +549,15 @@
         if "ans" in a:
             if data_dict["params"][f"{part_name}"][f"{a}"]["feedback"]:
                 feedback = f"|@ params.{part_name}.{a}.feedback @|"
             else:
                 feedback = f"Feedback for this choice is not available yet."
 
             correctness = f"|@ params.{part_name}.{a}.correct @|"
-            value = f"|@ params.{part_name}.{a}.value @|"
+            value = f"|@|@ params.{part_name}.{a}.value @|@|"
 
             ## Hack to remove feedback for Dropdown questions
             if parsed_question["header"][part_name]['type'] == 'dropdown':
                 html += f"\t<pl-answer correct= {correctness} > {value} {units} </pl-answer>\n"
             else:
                 html += f"\t<pl-answer correct= {correctness} feedback = '{feedback}' > {value} {units} </pl-answer>\n"
 
@@ -652,14 +658,57 @@
     html = f"""<pl-question-panel>\n<markdown>{parsed_question['body_parts_split'][part_name]['content']}</markdown>\n</pl-question-panel>\n\n"""
 
     html += f"""<pl-rich-text-editor { pl_customizations } > </pl-rich-text-editor>"""
 
     return replace_tags(html)
 
 
+def process_matching(part_name, parsed_question, data_dict):
+    """Processes markdown format matching questions and returns PL HTML
+    Args:
+        output_path (Path): [description]
+        parsed_question (dict): [description]
+        data_dict (dict)
+
+    Returns:
+        str: Matching question is returned as a string with PL-compliant syntax.
+    """
+    print("Processing matching question...")
+
+    html = f"""<pl-question-panel>\n<markdown>{parsed_question['body_parts_split'][part_name]['content']}</markdown>\n</pl-question-panel>\n\n"""
+
+    pl_customizations = " ".join(
+        [f'{k} = "{v}"' for k, v in parsed_question["header"][part_name]["pl-customizations"].items()]
+    )  # PL-customizations
+    html += f"""<pl-matching answers-name="{part_name}_matching" {pl_customizations} >\n"""
+
+    options = ''
+    statements = ''
+    ## Note: `|@`` gets converted into `{{` and `@|`` gets converted to `}}` by `replace_tags()`
+    for a in data_dict["params"][f"{part_name}"].keys():
+
+        if "option" in a:
+            value = f"|@ params.{part_name}.{a}.value @|"
+
+            options += f"\t<pl-option name= '{a}' > {value} </pl-option>\n"
+
+        if "statement" in a:
+            matches_with = f"|@ params.{part_name}.{a}.matches @|"
+            value = f"|@ params.{part_name}.{a}.value @|"
+
+            statements += f"\t<pl-statement match= '{matches_with}' > {value} </pl-statement>\n"
+
+    html += statements
+    html += options
+
+    html += "</pl-matching>\n"
+
+    return replace_tags(html)
+
+
 def process_file_upload(part_name, parsed_question, data_dict):
     """Processes markdown format of file-upload questions and returns PL HTML
     Args:
         part_name (string): Name of the question part being processed (e.g., part1, part2, etc...)
         parsed_question (dict): Dictionary of the MD-parsed question (output of `read_md_problem`)
         data_dict (dict): Dictionary of the `data` dict created after running server.py using `exec()`
 
@@ -702,14 +751,33 @@
 
     html = f"""<pl-question-panel>\n<markdown>{parsed_question['body_parts_split'][part_name]['content']}</markdown>\n</pl-question-panel>\n\n"""
 
     html += f"""<pl-file-editor { pl_customizations } > </pl-file-editor>"""
 
     return replace_tags(html)
 
+def process_string_input(part_name, parsed_question, data_dict):
+    """Processes markdown format of string-input questions and returns PL HTML
+    Args:
+        part_name (string): Name of the question part being processed (e.g., part1, part2, etc...)
+        parsed_question (dict): Dictionary of the MD-parsed question (output of `read_md_problem`)
+        data_dict (dict): Dictionary of the `data` dict created after running server.py using `exec()`
+
+    Returns:
+        html: A string of HTML that is part of the final PL question.html file.
+    """
+    pl_customizations = " ".join(
+        [f'{k} = "{v}"' for k, v in parsed_question["header"][part_name]["pl-customizations"].items()]
+    )  # PL-customizations
+
+    html = f"""<pl-question-panel>\n<markdown>{parsed_question['body_parts_split'][part_name]['content']}</markdown>\n</pl-question-panel>\n\n"""
+
+    html += f"""<pl-string-input { pl_customizations } ></pl-string-input>"""
+
+    return replace_tags(html)
 
 def replace_tags(string):
     """Takes in a string with tags: |@ and @| and returns {{ and }} respectively. This is because Python strings can't have double curly braces.
 
     Args:
         string (str): String to be processed, can be multi-line.
 
@@ -865,15 +933,15 @@
 
         # Write the YAML to a file
         output_path.parent.mkdir(parents=True, exist_ok=True)
         output_path.write_text(
             "---\n"
             + header_yml
             + "---\n"
-            + text
+            + text.replace(r"\\", "\\")
             + "\n## Attribution\n\n"
             + process_attribution(header.get("attribution")),
             encoding="utf8",
         )
 
         ####################################################
         #### End Temporary Fix for issue of myst no longer permitting nested dicts
@@ -921,27 +989,34 @@
         output_path.parent.mkdir(parents=True, exist_ok=True)
         output_path.write_text(
             "---\n"
             + header_yml
             + "\n---\n"
             + dict_to_md(
                 body_parts,
-            )
+            ).replace(r"\\", "\\")
             + "\n## Attribution\n\n"
             + process_attribution(header.get("attribution")),
             encoding="utf8",
         )
 
     # Move image assets
     files_to_copy = header.get("assets")
     if files_to_copy:
         [copy2(pathlib.Path(source_filepath).parent / fl, output_path.parent) for fl in files_to_copy]
 
+    # Move autograde py test files
+    files_to_copy = header.get("autogradeTestFiles")
+    if files_to_copy:
+        pl_path = output_path.parent / "tests"
+        pl_path.mkdir(parents=True, exist_ok=True)
+        [copy2(pathlib.Path(source_filepath).parent / "tests" / fl, pl_path / fl) for fl in files_to_copy if (instructor or fl=="starter_code.py")]
+
 
-def process_question_pl(source_filepath, output_path=None):
+def process_question_pl(source_filepath, output_path=None, dev=False):
 
     try:
         pathlib.Path(source_filepath)
     except:
         print(f"{source_filepath} - File does not exist.")
         raise
 
@@ -972,14 +1047,19 @@
     exec(server_py, server.__dict__)
 
     data2 = pbh.create_data2()
 
     server.generate(data2)
     #################################################################################
 
+    if dev:
+        tags = parsed_q["header"].get("tags", [])
+        tags.append("DEV")
+        parsed_q["header"]["tags"] = tags
+
     # Write info.json file
     write_info_json(output_path, parsed_q)
 
     # Question Preamble
     preamble = parsed_q["body_parts"].get("preamble", None)
     #TODO: Remove Debugging print statement
     #print(f"premable: {preamble}")
@@ -1032,14 +1112,18 @@
             question_html += process_dropdown(part, parsed_q, data2)
         elif "longtext" in q_type:
             question_html += process_longtext(part, parsed_q, data2)
         elif "file-upload" in q_type:
             question_html += process_file_upload(part, parsed_q, data2)
         elif "file-editor" in q_type:
             question_html += process_file_editor(part, parsed_q, data2)
+        elif "string-input" in q_type:
+            question_html += process_string_input(part, parsed_q, data2)
+        elif "matching" in q_type:
+            question_html += process_matching(part, parsed_q, data2)
         else:
             raise NotImplementedError(f"This question type ({q_type}) is not yet implemented.")
 
         if parsed_q["num_parts"] > 1:
             question_html += "</div>\n</div>\n"
 
         # Add pl-submission-panel and pl-answer-panel (if they exist)
@@ -1119,7 +1203,30 @@
     res = re.subn(
         r"src[\s,=]*\"(?!http)(.*\.jpg)",
         'src="{{options.client_files_question_url}}/\\1',
         res[0],
     )  # works
 
     return res[0]
+
+def backticks_to_code_tags(html):
+    """
+    Converts backticks to <code> tags, and code fences to <pl-code> tags.
+
+    Args:
+        html (str): The HTML to convert.
+
+    """
+    html = re.sub(
+        r"```(?P<language>\w+)?(?(language)(\{(?P<highlighting>[\d,-]*)\})?|)(?P<Code>[^`]+)```",
+        r'<pl-code language="\g<language>" highlight-lines="\g<highlighting>">\g<Code></pl-code>',
+        html,
+        flags=re.MULTILINE,
+    )
+    html = html.replace(' language=""', "")  # Remove empty language attributes
+    html = html.replace(
+        ' highlight-lines=""', ""
+    )  # Remove empty highlight-lines attributes
+    html = re.sub(r"(?<!\\)`(?P<Code>[^`]+)`", r"<code>\g<Code></code>", html)
+    html = html.replace("\\`", "`")  # Replace escaped backticks
+    return html
+
```

### Comparing `problem_bank_scripts-0.6.2/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.7.0/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.2/setup.py` & `problem_bank_scripts-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'docopt>=0.6.2,<0.7.0',
  'markdown-it-py>=2.1.0,<3.0.0',
  'mdformat>=0.7.14,<0.8.0',
  'numpy>=1.22,<2.0',
- 'pandas>=1.2.4,<2.0.0',
- 'problem-bank-helpers>=0.1.12,<0.2.0',
+ 'pandas>=2.0,<3.0',
+ 'problem-bank-helpers>=0.1.14,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.6.2',
+    'version': '0.7.0',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `problem_bank_scripts-0.6.2/PKG-INFO` & `problem_bank_scripts-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.6.2
+Version: 0.7.0
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: markdown-it-py (>=2.1.0,<3.0.0)
 Requires-Dist: mdformat (>=0.7.14,<0.8.0)
 Requires-Dist: numpy (>=1.22,<2.0)
-Requires-Dist: pandas (>=1.2.4,<2.0.0)
-Requires-Dist: problem-bank-helpers (>=0.1.12,<0.2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: problem-bank-helpers (>=0.1.14,<0.2.0)
 Requires-Dist: sympy (>=1.8,<2.0)
 Project-URL: Documentation, https://problem_bank_scripts.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/open-resources/problem_bank_scripts
 Description-Content-Type: text/markdown
 
 # Problem Bank Scripts
```

