# Comparing `tmp/vanna-0.0.4.tar.gz` & `tmp/vanna-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.4.tar", last modified: Sat Jul  1 01:49:17 2023, max compression
+gzip compressed data, was "vanna-0.0.5.tar", last modified: Fri Jul  7 04:08:18 2023, max compression
```

## Comparing `vanna-0.0.4.tar` & `vanna-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-01 01:49:05.000000 vanna-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-01 01:49:17.141005 vanna-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 01:49:05.000000 vanna-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-01 01:49:05.000000 vanna-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 01:49:17.141005 vanna-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-01 01:49:05.000000 vanna-0.0.4/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-01 01:49:05.000000 vanna-0.0.4/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 04:08:08.000000 vanna-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:08:18.743048 vanna-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 04:08:08.000000 vanna-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 04:08:08.000000 vanna-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:08:18.743048 vanna-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-07 04:08:08.000000 vanna-0.0.5/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 04:08:08.000000 vanna-0.0.5/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:08:18.743048 vanna-0.0.5/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 04:08:18.000000 vanna-0.0.5/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.4/LICENSE` & `vanna-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.4/pyproject.toml` & `vanna-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vanna"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vanna-0.0.4/src/vanna/__init__.py` & `vanna-0.0.5/src/vanna/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,64 +9,207 @@
 import requests
 import pandas as pd
 import json
 import dataclasses
 import plotly
 import plotly.express as px
 import plotly.graph_objects as go
-from .types import SQLAnswer, Explanation, QuestionSQLPair, Question, QuestionId, DataResult, PlotlyResult, Status, FullQuestionDocument, QuestionList, QuestionCategory, AccuracyStats
+from .types import SQLAnswer, Explanation, QuestionSQLPair, Question, QuestionId, DataResult, PlotlyResult, Status, FullQuestionDocument, QuestionList, QuestionCategory, AccuracyStats, UserEmail, UserOTP, ApiKey, OrganizationList, Organization, NewOrganization
 from typing import List, Dict, Any, Union, Optional
 
 """Set the API key for Vanna.AI."""
 api_key: Union[str, None] = None # API key for Vanna.AI
 
 __org: Union[str, None] = None # Organization name for Vanna.AI
 
 _endpoint = "https://ask.vanna.ai/rpc"
+_unauthenticated_endpoint = "https://ask.vanna.ai/unauthenticated_rpc"
+
+def __unauthenticated_rpc_call(method, params):
+    headers = {
+        'Content-Type': 'application/json',
+    }
+    data = {
+        "method": method,
+        "params": [__dataclass_to_dict(obj) for obj in params]
+    }
+
+    response = requests.post(_unauthenticated_endpoint, headers=headers, data=json.dumps(data))
+    return response.json()
 
 def __rpc_call(method, params):
     global api_key
     global __org
 
     if api_key is None:
         raise Exception("API key not set")
     
-    if __org is None:
+    if __org is None and method != "list_orgs":
         raise Exception("Organization name not set")
 
-    headers = {
-        'Content-Type': 'application/json',
-        'Vanna-Key': api_key,
-        'Vanna-Org': __org
-    }
+    if method != "list_orgs":
+        headers = {
+            'Content-Type': 'application/json',
+            'Vanna-Key': api_key,
+            'Vanna-Org': __org
+        }
+    else:
+        headers = {
+            'Content-Type': 'application/json',
+            'Vanna-Key': api_key,
+            'Vanna-Org': 'demo-sales'
+        }
+
     data = {
         "method": method,
         "params": [__dataclass_to_dict(obj) for obj in params]
     }
 
     response = requests.post(_endpoint, headers=headers, data=json.dumps(data))
     return response.json()
 
 def __dataclass_to_dict(obj):
     return dataclasses.asdict(obj)
 
+def login(email: str, otp_code: Union[str, None] = None) -> bool:
+    """
+    ## Example
+    ```python
+    vn.login(email="username@example.com")
+    ```
+
+    Login to the Vanna.AI API.
+
+    Args:
+        email (str): The email address to login with.
+        otp_code (Union[str, None]): The OTP code to login with. If None, an OTP code will be sent to the email address.
+
+    Returns:
+        bool: True if the login was successful, False otherwise.
+    """
+    global api_key
+
+    if otp_code is None:
+        params = [UserEmail(email=email)]
+
+        d = __unauthenticated_rpc_call(method="send_otp", params=params)
+
+        if 'result' not in d:
+            return False
+
+        status = Status(**d['result'])
+
+        if not status.success:
+            return False
+
+        otp = input("Enter OTP: ")
+
+    params = [UserOTP(email=email, otp=otp)]
+
+    d = __unauthenticated_rpc_call(method="verify_otp", params=params)
+
+    if 'result' not in d:
+        return False
+
+    key = ApiKey(**d['result'])
+
+    if key is None:
+        return False
+
+    api_key = key.key
+    print("Login successful. API key set. If you'd like to stay logged in, save your vn.api_key.")
+
+    return True
+
+def list_orgs() -> List[str]:
+    """
+    ## Example
+    ```python
+    orgs = vn.list_orgs()
+    ```
+
+    List the organizations that the user is a member of.
+
+    Returns:
+        List[str]: A list of organization names.
+    """
+    d = __rpc_call(method="list_orgs", params=[])
+
+    if 'result' not in d:
+        return []
+
+    orgs = OrganizationList(**d['result'])
+
+    return orgs.organizations
+
+def create_org(org: str, db_type: str) -> bool:
+    """
+    ## Example
+    ```python
+    vn.create_org(org="my-org", db_type="postgres")
+    ```
+
+    Create a new organization.
+
+    Args:
+        org (str): The name of the organization to create.
+        db_type (str): The type of database to use for the organization. This can be "Snowflake", "BigQuery", "Postgres", or anything else.
+
+    Returns:
+        bool: True if the organization was created successfully, False otherwise.
+    """
+    params = [NewOrganization(org_name=org, db_type=db_type)]
+
+    d = __rpc_call(method="create_org", params=params)
+
+    if 'result' not in d:
+        return False
+
+    status = Status(**d['result'])
+
+    return status.success
+
+
 def set_org(org: str) -> None:
     """
     ## Example
     ```python
     vn.set_org("my-org")
     ```
 
     Set the organization name for the Vanna.AI API.
 
     Args:
         org (str): The organization name.
     """
     global __org
-    __org = org
+
+    my_orgs = list_orgs()
+    if org not in my_orgs:
+        # Check if org exists
+        d = __unauthenticated_rpc_call(method="check_org_exists", params=[Organization(name=org, user=None, connection=None)])
+
+        if 'result' not in d:
+            raise Exception("Failed to check if organization exists")
+
+        status = Status(**d['result'])
+
+        if status.success:
+            raise Exception(f"An organization with the name {org} already exists")
+
+        create = input(f"Would you like to create organization '{org}'? (y/n): ")
+
+        if create.lower() == 'y':
+            db_type = input("What type of database would you like to use? (Snowflake, BigQuery, Postgres, etc.): ")
+            if create_org(org=org, db_type=db_type):
+                __org = org
+            else:
+                raise Exception("Failed to create organization")
+    else:
+        __org = org
 
 def store_sql(question: str, sql: str) -> bool:
     """
     ## Example
     ```python
     vn.store_sql(
         question="What is the average salary of employees?", 
@@ -90,14 +233,32 @@
     if 'result' not in d:
         return False
     
     status = Status(**d['result'])
 
     return status.success
 
+def train(question: str, sql: str) -> bool:
+    """
+    ## Example
+    ```python
+    vn.train(
+        question="What is the average salary of employees?", 
+        sql="SELECT AVG(salary) FROM employees"
+    )
+    ```
+
+    Train Vanna.AI on a question and its corresponding SQL query. This is equivalent to calling [`store_sql()`][vanna.store_sql].
+
+    Args:
+        question (str): The question to train on.
+        sql (str): The SQL query to train on.
+    """
+    return store_sql(question=question, sql=sql)
+
 def flag_sql_for_review(question: str, sql: Union[str, None] = None, error_msg: Union[str, None] = None) -> bool:
     """
     ## Example
     ```python
     vn.flag_sql_for_review(question="What is the average salary of employees?")
     ```
     Flag a question and its corresponding SQL query for review. You can later retrieve the flagged questions using [`get_flagged_questions()`][vanna.get_flagged_questions].
@@ -172,14 +333,32 @@
         return None
 
     # Load the result into a dataclass
     sql_answer = SQLAnswer(**d['result'])
 
     return sql_answer.sql
 
+def ask(question: str) -> str:
+    """
+    ## Example
+    ```python
+    vn.ask(question="What is the average salary of employees?")
+    # SELECT AVG(salary) FROM employees
+    ```
+
+    Ask a question using the Vanna.AI API. This is equivalent to calling [`generate_sql()`][vanna.generate_sql].
+
+    Args:
+        question (str): The question to ask.
+
+    Returns:
+        str or None: The SQL query, or None if an error occurred.
+    """
+    return generate_sql(question=question)
+
 def generate_plotly_code(question: Union[str, None], sql: Union[str, None], df: pd.DataFrame) -> str:
     """
     ## Example
     ```python
     vn.generate_plotly_code(
         question="What is the average salary of employees?",
         sql="SELECT AVG(salary) FROM employees",
```

### Comparing `vanna-0.0.4/src/vanna/types.py` & `vanna-0.0.5/src/vanna/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,36 @@
 @dataclass
 class Organization:
     name: str
     user: str | None
     connection: Connection | None
 
 @dataclass
+class OrganizationList:
+    organizations: List[str]
+
+@dataclass
+class UserEmail:
+    email: str
+
+@dataclass
+class NewOrganization:
+    org_name: str
+    db_type: str
+
+@dataclass
+class UserOTP:
+    email: str
+    otp: str
+
+@dataclass
+class ApiKey:
+    key: str
+
+@dataclass
 class QuestionId:
     id: str
 
 @dataclass
 class Question:
     question: str
```

