# Comparing `tmp/ms_salesforce_api-1.1.2.tar.gz` & `tmp/ms_salesforce_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.1.2.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.2.0.tar", max compression
```

## Comparing `ms_salesforce_api-1.1.2.tar` & `ms_salesforce_api-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/LICENSE
--rw-r--r--   0        0        0     8325 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3541 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15342 2023-06-16 10:33:32.417963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     7675 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    20445 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    23968 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     9228 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    17755 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/helpers.py
--rw-r--r--   0        0        0     1055 2023-06-16 10:33:32.421963 ms_salesforce_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8325 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-07-07 09:29:17.021010 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3541 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15342 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     9513 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    24332 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    28267 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12570 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    17755 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-07-07 09:29:17.025011 ms_salesforce_api-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.2.0/PKG-INFO
```

### Comparing `ms_salesforce_api-1.1.2/LICENSE` & `ms_salesforce_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/README.md` & `ms_salesforce_api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     Operation_Coordinator__r.Controller__c,
     Operation_Coordinator_Sub__r.Controller_SUB__c,
     Profit_Center__c,
     Cost_Center__c,
     Opportunity__r.Probability,
     Opportunity__r.Tier_Short__c,
     Opportunity__r.JiraComponentURL__c,
-
     Project_Account__r.Id,
     Project_Account__r.Name,
     Project_Account__r.MS_Customer_Account_Assigment_Group__c,
     Project_Account__r.MS_Customer_Tax_Category__c,
     Project_Account__r.MS_Customer_Tax_Classification__c,
     Project_Account__r.TXT_SAPId__c,
     Project_Account__r.ms_Business_Function__c,
@@ -45,14 +44,26 @@
     Project_Account__r.BillingStreet,
     Project_Account__r.MS_Company_Invoicing__c,
     Project_Account__r.MS_Office__c,
     Project_Account__r.Payment_Terms__c,
     Project_Account__r.BillingStateCode,
     Project_Account__r.MAIL_Invoicing__c,
     Project_Account__r.Invoicing_Email__c,
+
+    Project_Account__r.LKP_CustomerSubgroup__r.LKP_CustomerGroup__r.Name,
+    Project_Account__r.LKP_CustomerSubgroup__r.LKP_CustomerGroup__r.DT_Start__c,
+    Project_Account__r.LKP_CustomerSubgroup__r.LKP_CustomerGroup__r.DT_End__c,
+    Project_Account__r.LKP_CustomerSubgroup__r.LKP_CustomerGroup__r.TXT_BQId__c,
+    Project_Account__r.LKP_CustomerSubgroup__r.LKP_CustomerGroup__r.PCK_Type__c,
+
+    Project_Account__r.LKP_CustomerSubgroup__r.Id,
+    Project_Account__r.LKP_CustomerSubgroup__r.Name,
+    Project_Account__r.LKP_CustomerSubgroup__r.DT_Start__c,
+    Project_Account__r.LKP_CustomerSubgroup__r.DT_End__c,
+    Project_Account__r.LKP_CustomerSubgroup__r.TXT_BQId__c,
     (
         SELECT
             Id,
             CreatedDate,
             LastModifiedDate,
             Duration_months__c,
             ProductNew__r.Name,
@@ -205,18 +216,55 @@
     billing_state_code  VARCHAR(255) DEFAULT NULL,
     mail_invoicing  VARCHAR(255) DEFAULT NULL,
     invoicing_email  VARCHAR(500) DEFAULT NULL,
     FOREIGN KEY (project_id) REFERENCES Opportunities(project_id)
 );
 """
 
-DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP = {
-    "Opportunities": DEFAULT_OPPORTUNITIES_CREATE_TABLE_QUERY,
-    "ProjectLine": DEFAULT_PROJECTLINE_CREATE_TABLE_QUERY,
-    "BillingLines": DEFAULT_BILLINGLINES_CREATE_TABLE_QUERY,
-    "Accounts": DEFAULT_ACCOUNTS_CREATE_TABLE_QUERY,
-}
+DEFAULT_GROUPS_CREATE_TABLE_QUERY = """
+CREATE TABLE Groups (
+    id VARCHAR(255) PRIMARY KEY,
+    project_id VARCHAR(255) DEFAULT NULL,
+    name VARCHAR(255) DEFAULT NULL,
+    start_date VARCHAR(255) DEFAULT NULL,
+    end_date VARCHAR(255) DEFAULT NULL,
+    bqid VARCHAR(255) DEFAULT NULL,
+    pck_type VARCHAR(255) DEFAULT NULL,
+    FOREIGN KEY (project_id) REFERENCES Opportunities(project_id)
+);
+"""
+
+DEFAULT_SUBGROUPS_CREATE_TABLE_QUERY = """
+CREATE TABLE SubGroups (
+    group_id VARCHAR(255) DEFAULT NULL,
+    name VARCHAR(255) DEFAULT NULL,
+    start_date VARCHAR(255) DEFAULT NULL,
+    end_date VARCHAR(255) DEFAULT NULL,
+    bqid VARCHAR(255) DEFAULT NULL,
+    FOREIGN KEY (group_id) REFERENCES Groups(id)
+);
+"""
+
+DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP = [
+    {
+        "db_name": "Opportunities",
+        "query": DEFAULT_OPPORTUNITIES_CREATE_TABLE_QUERY,
+    },
+    {
+        "db_name": "ProjectLine",
+        "query": DEFAULT_PROJECTLINE_CREATE_TABLE_QUERY,
+    },
+    {
+        "db_name": "BillingLines",
+        "query": DEFAULT_BILLINGLINES_CREATE_TABLE_QUERY,
+    },
+    {"db_name": "Accounts", "query": DEFAULT_ACCOUNTS_CREATE_TABLE_QUERY},
+    {"db_name": "Groups", "query": DEFAULT_GROUPS_CREATE_TABLE_QUERY},
+    {"db_name": "SubGroups", "query": DEFAULT_SUBGROUPS_CREATE_TABLE_QUERY},
+]
 
 DEFAULT_DELETE_OPPORTUNITIES_TABLE = "DELETE FROM Opportunities WHERE true"
 DEFAULT_DELETE_PROJECTLINES_TABLE = "DELETE FROM ProjectLine WHERE true"
 DEFAULT_DELETE_BILLINGLINES_TABLE = "DELETE FROM BillingLines WHERE true"
 DEFAULT_DELETE_ACCOUNTS_TABLE = "DELETE FROM Accounts WHERE true"
+DEFAULT_DELETE_GROUPS_TABLE = "DELETE FROM Groups WHERE true"
+DEFAULT_DELETE_SUBGROUPS_TABLE = "DELETE FROM SubGroups WHERE true"
```

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,14 +52,24 @@
         account_billing_street,
         account_company_invoicing,
         account_office,
         account_payment_terms,
         account_billing_state_code,
         account_mail_invoicing,
         account_invoicing_email,
+        group_name,
+        group_id,
+        group_start_date,
+        group_end_date,
+        group_bqid,
+        group_pck_type,
+        subgroup_name,
+        subgroup_start_date,
+        subgroup_end_date,
+        subgroup_bqid,
         billing_lines=[],
         project_line_items=[],
     ):
         self.account_business_name = account_business_name
         self.account_name = account_name
         self.account_id = account_id
         self.currency = currency
@@ -106,14 +116,24 @@
         self.account_billing_street = account_billing_street
         self.account_company_invoicing = account_company_invoicing
         self.account_office = account_office
         self.account_payment_terms = account_payment_terms
         self.account_billing_state_code = account_billing_state_code
         self.account_mail_invoicing = account_mail_invoicing
         self.account_invoicing_email = account_invoicing_email
+        self.group_name = group_name
+        self.group_id = group_id
+        self.group_start_date = group_start_date
+        self.group_end_date = group_end_date
+        self.group_bqid = group_bqid
+        self.group_pck_type = group_pck_type
+        self.subgroup_name = subgroup_name
+        self.subgroup_start_date = subgroup_start_date
+        self.subgroup_end_date = subgroup_end_date
+        self.subgroup_bqid = subgroup_bqid
 
     @staticmethod
     def from_salesforce_record(record):
         def _get_account_business_name():
             try:
                 return normalize_value(
                     record["Project_Account__r"]["Business_Name__c"]
@@ -408,14 +428,86 @@
 
         def _get_opportunity_percentage():
             try:
                 return normalize_value(record["Opportunity__r"]["Probability"])
             except (TypeError, KeyError):
                 return ""
 
+        def _get_group_name():
+            try:
+                return record["LKP_CustomerSubgroup__r"][
+                    "LKP_CustomerGroup__r"
+                ]["Name"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_group_id():
+            try:
+                return record["LKP_CustomerSubgroup__r"][
+                    "LKP_CustomerGroup__r"
+                ]["Id"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_group_start():
+            try:
+                return record["LKP_CustomerSubgroup__r"][
+                    "LKP_CustomerGroup__r"
+                ]["DT_Start__c"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_group_end():
+            try:
+                return record["LKP_CustomerSubgroup__r"][
+                    "LKP_CustomerGroup__r"
+                ]["DT_End__c"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_group_bqid():
+            try:
+                return record["LKP_CustomerSubgroup__r"][
+                    "LKP_CustomerGroup__r"
+                ]["TXT_BQId__c"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_group_pck_type():
+            try:
+                return record["LKP_CustomerSubgroup__r"][
+                    "LKP_CustomerGroup__r"
+                ]["PCK_Type__c"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_subgroup_name():
+            try:
+                return record["LKP_CustomerSubgroup__r"]["Name"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_subgroup_start():
+            try:
+                return record["LKP_CustomerSubgroup__r"]["DT_Start__c"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_subgroup_end():
+            try:
+                return record["LKP_CustomerSubgroup__r"]["DT_End__c"]
+            except (TypeError, KeyError):
+                return ""
+
+        def _get_subgroup_bqid():
+            try:
+                return record["LKP_CustomerSubgroup__r"]["TXT_BQId__c"]
+            except (TypeError, KeyError):
+                return ""
+
         project_line_items = (
             [
                 ProjectLineItemDTO.from_salesforce_record(item)
                 for item in record.get("Project_Line_Items__r", {}).get(
                     "records", []
                 )
             ]
@@ -470,14 +562,24 @@
             account_billing_street=_get_account_billing_street(),
             account_company_invoicing=_get_account_company_invoicing(),
             account_office=_get_account_office(),
             account_payment_terms=_get_account_payment_terms(),
             account_billing_state_code=_get_account_billing_state_code(),
             account_mail_invoicing=_get_account_mail_invoicing(),
             account_invoicing_email=_get_account_invoicing_email(),
+            group_name=_get_group_name(),
+            group_id=_get_group_id(),
+            group_start_date=_get_group_start(),
+            group_end_date=_get_group_end(),
+            group_bqid=_get_group_bqid(),
+            group_pck_type=_get_group_pck_type(),
+            subgroup_name=_get_subgroup_name(),
+            subgroup_start_date=_get_subgroup_start(),
+            subgroup_end_date=_get_subgroup_end(),
+            subgroup_bqid=_get_subgroup_bqid(),
         )
 
     def add_billing_lines(self, billing_lines):
         self.billing_lines.extend(billing_lines)
 
     def to_dict(self):
         return {
@@ -529,8 +631,18 @@
             "account_billing_street": self.account_billing_street,
             "account_company_invoicing": self.account_company_invoicing,
             "account_office": self.account_office,
             "account_payment_terms": self.account_payment_terms,
             "account_billing_state_code": self.account_billing_state_code,
             "account_mail_invoicing": self.account_mail_invoicing,
             "account_invoicing_email": self.account_invoicing_email,
+            "group_name": self.group_name,
+            "group_id": self.group_id,
+            "group_start_date": self.group_start_date,
+            "group_end_date": self.group_end_date,
+            "group_bqid": self.group_bqid,
+            "group_pck_type": self.group_pck_type,
+            "subgroup_name": self.subgroup_name,
+            "subgroup_start_date": self.subgroup_start_date,
+            "subgroup_end_date": self.subgroup_end_date,
+            "subgroup_bqid": self.subgroup_bqid,
         }
```

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,14 +110,31 @@
                 "sap_id": "STRING",
                 "tax_category": "STRING",
                 "tax_classification": "STRING",
                 "tax_id_type": "STRING",
                 "tier": "STRING",
                 "website": "STRING",
             },
+            "groups": {
+                "project_id": "STRING",
+                "id": "STRING",
+                "name": "STRING",
+                "start_date": "STRING",
+                "end_date": "STRING",
+                "bqid": "STRING",
+                "pck_type": "STRING",
+            },
+            "subgroups": {
+                "project_id": "STRING",
+                "group_id": "STRING",
+                "name": "STRING",
+                "start_date": "STRING",
+                "end_date": "STRING",
+                "bqid": "STRING",
+            },
         }
 
         for table_name, table_schema in self.schemas.items():
             self.client.create_table_if_not_exists(table_name, table_schema)
 
     def _execute_query(self, query, log_id, default_error_value=None):
         custom_error_value = f"{log_id}_custom_error"
@@ -631,14 +648,139 @@
                 .replace("  ", "")
             )
 
             self._execute_query(
                 query=insert_accounts_query, log_id="INSERT_accounts"
             )
 
+    def _export_groups(self, opportunities):
+        group_values = []
+        for opp in opportunities:
+            group_id = f'"{opp["group_id"]}"' if opp["group_id"] else "NULL"
+            group_name = (
+                f'"{opp["group_name"]}"' if opp["group_name"] else "NULL"
+            )
+
+            group_start = (
+                f'"{opp["group_start_date"]}"'
+                if opp["group_start_date"]
+                else "NULL"
+            )
+
+            group_end = (
+                f'"{opp["group_end_date"]}"'
+                if opp["group_end_date"]
+                else "NULL"
+            )
+
+            group_bqid = (
+                f'"{opp["group_bqid"]}"' if opp["group_bqid"] else "NULL"
+            )
+
+            group_pck_type = (
+                f'"{opp["group_pck_type"]}"'
+                if opp["group_pck_type"]
+                else "NULL"
+            )
+
+            group_values.append(
+                f"""
+                (
+                    "{opp['project_id']}",
+                    {group_id},
+                    {group_name},
+                    {group_start},
+                    {group_end},
+                    {group_bqid},
+                    {group_pck_type}
+                )
+                """
+            )
+
+        if group_values:
+            insert_group_query = f"""
+                INSERT INTO `{self.project_id}.{self.dataset_id}.groups` (
+                    project_id,
+                    id,
+                    name,
+                    start_date,
+                    end_date,
+                    bqid,
+                    pck_type
+                ) VALUES {', '.join(group_values)};
+            """
+            insert_group_query = (
+                insert_group_query.replace("\n", "")
+                .replace("    ", "")
+                .replace("  ", "")
+            )
+
+            self._execute_query(
+                query=insert_group_query,
+                log_id="INSERT_accounts",
+            )
+
+    def _export_subgroups(self, opportunities):
+        group_values = []
+        for opp in opportunities:
+            group_id = f'"{opp["group_id"]}"' if opp["group_id"] else "NULL"
+            subgroup_name = (
+                f'"{opp["subgroup_name"]}"' if opp["subgroup_name"] else "NULL"
+            )
+
+            subgroup_start = (
+                f'"{opp["subgroup_start_date"]}"'
+                if opp["subgroup_start_date"]
+                else "NULL"
+            )
+
+            subgroup_end = (
+                f'"{opp["subgroup_end_date"]}"'
+                if opp["subgroup_end_date"]
+                else "NULL"
+            )
+
+            subgroup_bqid = (
+                f'"{opp["subgroup_bqid"]}"' if opp["subgroup_bqid"] else "NULL"
+            )
+
+            group_values.append(
+                f"""
+                (
+                    {group_id},
+                    {subgroup_name},
+                    {subgroup_start},
+                    {subgroup_end},
+                    {subgroup_bqid},
+                )
+                """
+            )
+
+        if group_values:
+            insert_group_query = f"""
+                INSERT INTO `{self.project_id}.{self.dataset_id}.subgroups` (
+                    group_id,
+                    name,
+                    start_date,
+                    end_date,
+                    bqid,
+                    pck_type
+                ) VALUES {', '.join(group_values)};
+            """
+            insert_group_query = (
+                insert_group_query.replace("\n", "")
+                .replace("    ", "")
+                .replace("  ", "")
+            )
+
+            self._execute_query(
+                query=insert_group_query,
+                log_id="INSERT_accounts",
+            )
+
     def export_data(self, opportunities):
         opportunities_batches = [
             opportunities[i : i + self.batch_size]  # noqa: E203
             for i in range(0, len(opportunities), self.batch_size)
         ]
         for batch in opportunities_batches:
             self._export_opportunities(batch)
```

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 import psycopg2
 from psycopg2 import sql
 
 from ms_salesforce_api.salesforce.project.constants import (
     DEFAULT_DELETE_ACCOUNTS_TABLE,
     DEFAULT_DELETE_BILLINGLINES_TABLE,
+    DEFAULT_DELETE_GROUPS_TABLE,
     DEFAULT_DELETE_OPPORTUNITIES_TABLE,
     DEFAULT_DELETE_PROJECTLINES_TABLE,
+    DEFAULT_DELETE_SUBGROUPS_TABLE,
     DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP,
 )
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
@@ -71,54 +73,56 @@
 
         cursor.close()
         conn.close()
 
     def check_and_create_tables(self):
         cursor = self.connection.cursor()
 
-        for (
-            table_name,
-            create_table_query,
-        ) in DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP.items():
+        for db_schema in DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP:
+            table_name = db_schema["db_name"]
             # Check if table exists
             check_table_query = f"SELECT EXISTS (SELECT 1 FROM information_schema.tables WHERE table_name = '{table_name.lower()}')"  # noqa: E501
 
             cursor.execute(check_table_query)
 
             result = cursor.fetchone()
 
             if not result[0]:
-                cursor.execute(create_table_query)
+                cursor.execute(db_schema["query"])
                 logging.info(f"Table '{table_name}' created.")
 
         self.connection.commit()
 
         cursor.close()
 
     def delete_all_rows(self):
         cursor = self.connection.cursor()
         logging.info("Deleting all tables...")
 
         cursor.execute(DEFAULT_DELETE_BILLINGLINES_TABLE)
         cursor.execute(DEFAULT_DELETE_PROJECTLINES_TABLE)
         cursor.execute(DEFAULT_DELETE_ACCOUNTS_TABLE)
+        cursor.execute(DEFAULT_DELETE_SUBGROUPS_TABLE)
+        cursor.execute(DEFAULT_DELETE_GROUPS_TABLE)
         cursor.execute(DEFAULT_DELETE_OPPORTUNITIES_TABLE)
 
         self.connection.commit()
 
         cursor.close()
 
     def export_data(self, opportunities):
         with self.connection.cursor() as cursor:
             opportunity_batches = self._create_batches(
                 opportunities, self.BATCH_SIZE
             )
             for opportunity_batch in opportunity_batches:
                 self._insert_opportunities_batch(cursor, opportunity_batch)
                 self._insert_accounts_batch(cursor, opportunity_batch)
+                self._insert_groups_batch(cursor, opportunity_batch)
+                self._insert_subgroups_batch(cursor, opportunity_batch)
 
                 billing_lines = []
                 project_lines = []
 
                 for opportunity in opportunity_batch:
                     billing_lines.extend(
                         self._create_billing_lines(
@@ -160,14 +164,16 @@
     def _insert_opportunities_batch(self, cursor, opportunities):
         opportunity_fixed = [
             {
                 key: (value if value != "" else None)
                 for key, value in opportunity.items()
                 if key not in ["billing_lines", "project_line_items"]
                 and "account_" not in key
+                and "group_" not in key
+                and "subgroup_" not in key
             }
             for opportunity in opportunities
         ]
 
         insert_query = sql.SQL(
             """
             INSERT INTO Opportunities ({})
@@ -197,15 +203,15 @@
             raise (e)
 
     def _insert_accounts_batch(self, cursor, opportunities):
         opportunity_fixed = [
             {
                 key.replace("account_", ""): (value if value != "" else None)
                 for key, value in opportunity.items()
-                if "account_" in key
+                if "account_" in key or "project_id" == key
             }
             for opportunity in opportunities
         ]
 
         insert_query = sql.SQL(
             """
             INSERT INTO Accounts ({})
@@ -219,18 +225,14 @@
                 map(sql.Placeholder, opportunity_fixed[0].keys())
             ),
         )
 
         try:
             cursor.executemany(insert_query, opportunity_fixed)
         except Exception as e:
-            from pprint import pprint
-
-            pprint(opportunity_fixed)
-
             if self.debug_mode:
                 insert_query_string = cursor.mogrify(
                     insert_query.as_string(cursor.connection),
                     opportunity_fixed,
                 ).decode("utf-8")
                 logging.info(insert_query_string)
             logging.error(f"[ERROR - _insert_accounts_batch (cloudsql)] - {e}")
@@ -279,7 +281,92 @@
                 insert_query_string = cursor.mogrify(
                     cursor.query, project_lines
                 ).decode("utf-8")
                 logging.info(insert_query_string)
             logging.error(
                 f"[ERROR - _insert_project_lines_batch (cloudsql)] - {e}"
             )
+
+    def _insert_groups_batch(self, cursor, opportunities):
+        opportunity_fixed = [
+            {
+                key.replace("group_", ""): (value if value != "" else None)
+                for key, value in opportunity.items()
+                if ("group_" in key and "subgroup_" not in key)
+                or "project_id" == key
+            }
+            for opportunity in opportunities
+            if opportunity.get("group_id") is not None
+            and opportunity.get("group_id") != ""
+        ]
+
+        if opportunity_fixed:
+            insert_query = sql.SQL(
+                """
+                INSERT INTO Groups ({})
+                VALUES ({})
+                """
+            ).format(
+                sql.SQL(", ").join(
+                    map(sql.Identifier, opportunity_fixed[0].keys())
+                ),
+                sql.SQL(", ").join(
+                    map(sql.Placeholder, opportunity_fixed[0].keys())
+                ),
+            )
+
+            try:
+                cursor.executemany(insert_query, opportunity_fixed)
+            except Exception as e:
+                if self.debug_mode:
+                    insert_query_string = cursor.mogrify(
+                        insert_query.as_string(cursor.connection),
+                        opportunity_fixed,
+                    ).decode("utf-8")
+                    logging.info(insert_query_string)
+                logging.error(
+                    f"[ERROR - _insert_groups_batch (cloudsql)] - {e}"
+                )
+
+                raise (e)
+
+    def _insert_subgroups_batch(self, cursor, opportunities):
+        opportunity_fixed = [
+            {
+                key.replace("subgroup_", ""): (value if value != "" else None)
+                for key, value in opportunity.items()
+                if "subgroup_" in key
+            }
+            for opportunity in opportunities
+            if opportunity.get("group_id") is not None
+            and opportunity.get("group_id") != ""
+        ]
+
+        if opportunity_fixed:
+            insert_query = sql.SQL(
+                """
+                INSERT INTO SubGroups ({})
+                VALUES ({})
+                """
+            ).format(
+                sql.SQL(", ").join(
+                    map(sql.Identifier, opportunity_fixed[0].keys())
+                ),
+                sql.SQL(", ").join(
+                    map(sql.Placeholder, opportunity_fixed[0].keys())
+                ),
+            )
+
+            try:
+                cursor.executemany(insert_query, opportunity_fixed)
+            except Exception as e:
+                if self.debug_mode:
+                    insert_query_string = cursor.mogrify(
+                        insert_query.as_string(cursor.connection),
+                        opportunity_fixed,
+                    ).decode("utf-8")
+                    logging.info(insert_query_string)
+                logging.error(
+                    f"[ERROR - _insert_subgroups_batch (cloudsql)] - {e}"
+                )
+
+                raise (e)
```

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.2.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.1.2/pyproject.toml` & `ms_salesforce_api-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.1.2"
+version = "1.2.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-1.1.2/PKG-INFO` & `ms_salesforce_api-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 1.1.2
+Version: 1.2.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

