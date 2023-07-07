# Comparing `tmp/airmailer-0.1.2.tar.gz` & `tmp/airmailer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airmailer-0.1.2.tar", last modified: Tue Apr 19 20:23:02 2022, max compression
+gzip compressed data, was "dist/airmailer-0.2.0.tar", last modified: Fri Jul  7 00:02:10 2023, max compression
```

## Comparing `airmailer-0.1.2.tar` & `airmailer-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,32 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.767799 airmailer-0.1.2/
--rw-rw-r--   0 cmalek     (501) admin       (80)      161 2021-11-30 23:45:18.000000 airmailer-0.1.2/AUTHORS.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)     3542 2021-12-02 17:36:04.000000 airmailer-0.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)       89 2021-11-30 23:45:18.000000 airmailer-0.1.2/HISTORY.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)      589 2021-11-30 23:45:18.000000 airmailer-0.1.2/LICENSE
--rw-rw-r--   0 cmalek     (501) admin       (80)      262 2021-11-30 23:45:18.000000 airmailer-0.1.2/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     5273 2022-04-19 20:23:02.767999 airmailer-0.1.2/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     3201 2021-12-02 20:14:44.000000 airmailer-0.1.2/README.rst
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.754841 airmailer-0.1.2/airmailer/
--rw-rw-r--   0 cmalek     (501) admin       (80)      132 2022-04-19 20:22:30.000000 airmailer-0.1.2/airmailer/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.759508 airmailer-0.1.2/airmailer/backend/
--rw-rw-r--   0 cmalek     (501) admin       (80)      150 2021-12-02 17:45:23.000000 airmailer-0.1.2/airmailer/backend/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8645 2022-04-19 20:22:27.000000 airmailer-0.1.2/airmailer/backend/aws.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2272 2021-12-02 19:52:52.000000 airmailer-0.1.2/airmailer/backend/base.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6573 2021-12-02 18:31:49.000000 airmailer-0.1.2/airmailer/backend/smtp.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.760444 airmailer-0.1.2/airmailer/cli/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-12-02 18:43:46.000000 airmailer-0.1.2/airmailer/cli/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      453 2021-12-02 18:45:58.000000 airmailer-0.1.2/airmailer/cli/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      405 2021-12-02 17:22:14.000000 airmailer-0.1.2/airmailer/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      103 2021-12-02 18:45:46.000000 airmailer-0.1.2/airmailer/logging.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      188 2021-12-02 19:36:23.000000 airmailer-0.1.2/airmailer/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    16566 2021-12-03 01:05:53.000000 airmailer-0.1.2/airmailer/message.py
--rw-rw-r--   0 cmalek     (501) admin       (80)       47 2021-12-02 19:47:53.000000 airmailer-0.1.2/airmailer/utils.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.757136 airmailer-0.1.2/airmailer.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     5273 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      801 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       50 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/not-zip-safe
--rw-rw-r--   0 cmalek     (501) admin       (80)       23 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       10 2022-04-19 20:23:02.000000 airmailer-0.1.2/airmailer.egg-info/top_level.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.766024 airmailer-0.1.2/docs/
--rw-rw-r--   0 cmalek     (501) admin       (80)      610 2021-12-02 17:32:00.000000 airmailer-0.1.2/docs/Makefile
--rw-rw-r--   0 cmalek     (501) admin       (80)       28 2021-11-30 23:45:18.000000 airmailer-0.1.2/docs/authors.rst
--rwxrwxr-x   0 cmalek     (501) admin       (80)     4819 2021-12-02 17:35:41.000000 airmailer-0.1.2/docs/conf.py
--rw-rw-r--   0 cmalek     (501) admin       (80)       33 2021-11-30 23:45:18.000000 airmailer-0.1.2/docs/contributing.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)       28 2021-11-30 23:45:18.000000 airmailer-0.1.2/docs/history.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)      306 2021-12-02 17:36:04.000000 airmailer-0.1.2/docs/index.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)     1122 2021-12-02 17:35:53.000000 airmailer-0.1.2/docs/installation.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)      807 2021-12-02 17:32:58.000000 airmailer-0.1.2/docs/make.bat
--rw-rw-r--   0 cmalek     (501) admin       (80)       27 2021-11-30 23:45:18.000000 airmailer-0.1.2/docs/readme.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)       73 2021-12-02 17:31:01.000000 airmailer-0.1.2/docs/usage.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)      620 2022-04-19 20:23:02.768605 airmailer-0.1.2/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1511 2022-04-19 20:22:30.000000 airmailer-0.1.2/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-04-19 20:23:02.767231 airmailer-0.1.2/tests/
--rw-rw-r--   0 cmalek     (501) admin       (80)       39 2021-12-02 17:25:27.000000 airmailer-0.1.2/tests/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      834 2021-12-02 17:32:51.000000 airmailer-0.1.2/tests/test_airmailer.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.664908 airmailer-0.2.0/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      161 2021-11-30 23:45:18.000000 airmailer-0.2.0/AUTHORS.rst
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3542 2021-12-02 17:36:04.000000 airmailer-0.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cmalek     (501) admin       (80)       89 2021-11-30 23:45:18.000000 airmailer-0.2.0/HISTORY.rst
+-rw-rw-r--   0 cmalek     (501) admin       (80)      589 2021-11-30 23:45:18.000000 airmailer-0.2.0/LICENSE
+-rw-rw-r--   0 cmalek     (501) admin       (80)      262 2021-11-30 23:45:18.000000 airmailer-0.2.0/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2017 2023-07-07 00:02:10.665173 airmailer-0.2.0/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      769 2023-07-06 17:48:03.000000 airmailer-0.2.0/README.rst
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.653265 airmailer-0.2.0/airmailer/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      132 2023-07-07 00:00:47.000000 airmailer-0.2.0/airmailer/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.662661 airmailer-0.2.0/airmailer/backend/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      150 2021-12-02 17:45:23.000000 airmailer-0.2.0/airmailer/backend/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8867 2023-07-06 17:35:36.000000 airmailer-0.2.0/airmailer/backend/aws.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2519 2023-07-06 23:55:46.000000 airmailer-0.2.0/airmailer/backend/base.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6573 2021-12-02 18:31:49.000000 airmailer-0.2.0/airmailer/backend/smtp.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.663940 airmailer-0.2.0/airmailer/cli/
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-12-02 18:43:46.000000 airmailer-0.2.0/airmailer/cli/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      453 2021-12-02 18:45:58.000000 airmailer-0.2.0/airmailer/cli/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      405 2021-12-02 17:22:14.000000 airmailer-0.2.0/airmailer/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      103 2021-12-02 18:45:46.000000 airmailer-0.2.0/airmailer/logging.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      187 2023-06-30 22:26:03.000000 airmailer-0.2.0/airmailer/main.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    22227 2023-07-06 23:54:10.000000 airmailer-0.2.0/airmailer/message.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.659079 airmailer-0.2.0/airmailer.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2017 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      575 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       50 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/not-zip-safe
+-rw-rw-r--   0 cmalek     (501) admin       (80)       23 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       10 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      734 2023-07-07 00:02:10.666366 airmailer-0.2.0/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1511 2023-07-07 00:00:47.000000 airmailer-0.2.0/setup.py
```

### Comparing `airmailer-0.1.2/CONTRIBUTING.rst` & `airmailer-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `airmailer-0.1.2/LICENSE` & `airmailer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airmailer-0.1.2/airmailer/backend/aws.py` & `airmailer-0.2.0/airmailer/backend/aws.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,80 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
+from typing import List, Dict, Any
 import boto3
 
+import botocore
 from botocore.vendored.requests.packages.urllib3.exceptions import ResponseError
 from botocore.exceptions import BotoCoreError, ClientError
 
 from ..logging import logger
-from ..message import sanitize_address
+from ..message import sanitize_address, EmailMessage
 from .base import BaseEmailBackend
 
 
 class SESEmailBackend(BaseEmailBackend):
     """
     Send mails using the AWS SES API.
     """
 
     def __init__(
         self,
-        fail_silently=False,
-        aws_access_key_id=None,
-        aws_secret_access_key=None,
-        aws_region_name=None,
-        configuration_set_name=None,
-        aws_region_endpoint=None,
+        fail_silently: bool = False,
+        aws_access_key_id: str = None,
+        aws_secret_access_key: str = None,
+        aws_region_name: str = None,
+        configuration_set_name: str = None,
+        aws_region_endpoint: str = None,
         aws_config=None,
-        ses_from_arn=None,
-        ses_source_arn=None,
-        ses_return_path_arn=None,
+        ses_from_arn: str = None,
+        ses_source_arn: str = None,
+        ses_return_path_arn: str = None,
+        ses_tags: Dict[str, str] = None,
         **kwargs
     ):
-        """Creates a client for the AWS SES API.
-
-        :param fail_silently: If `True`, don't raise execeptions on client errors, defaults to False
-        :type fail_silently: bool
-
-        :param aws_access_key_id: the ``AWS_ACCESS_KEY_ID``, defaults to read from environment
-        :type aws_access_key_id: str, optional
-
-        :param aws_secret_access_key: the ``AWS_SECRET_ACCESS_KEY``, defaults to read from environment
-        :type aws_secret_access_key: str, optional
-
-        :param aws_region_name: the name of the AWS region to use, defaults to read from environment
-        :type aws_region_name: str, optional
-
-        :param configuration_set_name: the name of the SES Configuration Set to use, defaults to None
-        :type configuration_set_name: str, optional
-
-        :param aws_region_endpoint: the URL for the SES endpoint for the region, defaults to None
-        :type aws_region_endpoint: str, optional
-
-        :param aws_config: a properly constructed botocore Config object
-        :type aws_config: class:`botocore.config.Config`, optional
-
-        :param ses_from_arn: the FromArn when using cross-account identities, defaults to None
-        :type ses_from_arn: str, optional
-
-        :param ses_source_arn: the SourceArn when using cross-account identities, defaults to None
-        :type ses_source_arn: str, optional
+        """
+        Creates a client for the AWS SES API.
 
-        :param ses_return_path_arn: the ReturnPathArn when using cross-account identities, defaults to None
-        :type ses_return_path_arn: str, optional
+        Keyword Arguments:
+            fail_silently: If ``True``, don't raise execeptions on client errors
+            aws_access_key_id: the ``AWS_ACCESS_KEY_ID``, defaults to read from environment
+            aws_secret_access_key: the ``AWS_SECRET_ACCESS_KEY``, defaults to read from environment
+            aws_region_name: the name of the AWS region to use, defaults to read from environment
+            configuration_set_name: the name of the SES Configuration Set to use
+            aws_region_endpoint: the URL for the SES endpoint for the region
+            aws_config: a properly constructed :py:class:`botocore.config.Config` object
+            ses_from_arn: the ``FromArn`` when using cross-account identities
+            ses_source_arn: the ``SourceArn`` when using cross-account identities
+            ses_return_path_arn: the ``ReturnPathArn`` when using cross-account identities
+            ses_tags: a dictionary of tags to apply set as ``X-SES-MESSAGE-TAGS`` on each
+                message sent
         """
         super().__init__(fail_silently=fail_silently)
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_region_name = aws_region_name
         self.aws_region_endpoint = aws_region_endpoint
-        self.aws_config = aws_config
+        self.aws_config: botocore.client.Config = aws_config
         self.ses_source_arn = ses_source_arn
         self.ses_from_arn = ses_from_arn
         self.ses_return_path_arn = ses_return_path_arn
         self.configuration_set_name = configuration_set_name
+        self.ses_tags = ses_tags
         self.connection = None
 
-    def open(self):
+    def open(self) -> bool:
+        """
+        Opens a connection to the AWS SES API.
+
+        Returns:
+            ``True`` if the connection was opened successfully, ``False`` otherwise.
+        """
         if self.connection:
             return False
 
         try:
             self.connection = boto3.client(
                 "ses",
                 aws_access_key_id=self.aws_access_key_id,
@@ -87,32 +82,36 @@
                 region_name=self.aws_region_name,
                 endpoint_url=self.aws_region_endpoint,
                 config=self.aws_config
             )
         except (ClientError, BotoCoreError):
             if not self.fail_silently:
                 raise
-            return None
+            return False
         return True
 
-    def close(self):
+    def close(self) -> None:
+        """
+        Close the connection to the AWS SES API.
+        """
         self.connection = None
 
-    def send_messages(self, email_messages):
+    def send_messages(self, email_messages: List[EmailMessage]) -> int:
         """
         Sends one or more messages returns the number of email messages sent.
 
-        :param email_messages: A list of emails to send
-        :type email_messages: List[airmailer.message.EmailMessage]
+        Args:
+            email_messages: A list of emails to send
 
-        :raises: class:`botocore.exceptions.ClientError`: AWS SES had an issue
-        :raises: class:`botocore.exceptions.BotoCoreError`: AWS SES had an issue
+        Raises:
+            botocore.exceptions.ClientError: AWS SES had an issue
+            botocore.exceptions.BotoCoreError: AWS SES had an issue
 
-        :return: count of messages sent
-        :rtype: int
+        Returns:
+            The number of messages sent
         """
         if not email_messages:
             return 0
 
         new_conn_created = self.open()
         if not self.connection:
             return 0
@@ -124,68 +123,72 @@
                 sent_message_count += 1
 
         if new_conn_created:
             self.close()
 
         return sent_message_count
 
-    def _send(self, email_message):
+    def _send(self, email_message: EmailMessage) -> bool:
         """
         Sends an individual message.
 
         If the message was submitted successfully to the AWS SES API, set
 
-        * `email_message.extra_headers['status']` to 200
-        * `email_message.extra_headers['message_id']` to the `MessageId`
-        * `email_message.extra_headers['request_id']` to the `RequestId` of the AWS API call response
+        * ``email_message.extra_headers['status']`` to 200
+        * ``email_message.extra_headers['message_id']`` to the ``MessageId``
+        * ``email_message.extra_headers['request_id']`` to the ``RequestId`` of the AWS API call response
 
         If the message was not submitted successfully to the AWS SES API, set
 
-        * `email_message.extra_headers['status']` to HTTP status of the response
-        * `email_message.extra_headers['reason']` to "Reason" given for the error in the response
-        * `email_message.extra_headers['error_code']` to error code of the response
-        * `email_message.extra_headers['error_message']` to error message from the response
-        * `email_message.extra_headers['body']` to body from the response
-        * `email_message.extra_headers['request_id']` to the `RequestId` of the AWS API call response
-
-        :param email_message: An email to send
-        :type email_message: class:`airmailer.message.EmailMessage`
-
-        :raises: class:`botocore.exceptions.ClientError`: AWS SES had an issue
-        :raises: class:`botocore.exceptions.BotoCoreError`: AWS SES had an issue
+        * ``email_message.extra_headers['status']`` to HTTP status of the response
+        * ``email_message.extra_headers['reason']`` to "Reason" given for the error in the response
+        * ``email_message.extra_headers['error_code']`` to error code of the response
+        * ``email_message.extra_headers['error_message']`` to error message from the response
+        * ``email_message.extra_headers['body']`` to body from the response
+        * ``email_message.extra_headers['request_id']`` to the ``RequestId`` of the AWS API call response
+
+        Args:
+            email_message: An email to send
+
+        Raises:
+            botocore.exceptions.ClientError: AWS SES had an issue
+            botocore.exceptions.BotoCoreError: AWS SES had an issue
 
-        :return: True if the message was sent, False otherwise
-        :rtype: bool
+        Returns:
+            ``True`` if the message was sent, ``False`` otherwise
         """
-
         if not email_message.recipients():
             return False
 
         encoding = email_message.encoding
         from_email = sanitize_address(email_message.from_email, email_message.encoding)
         recipients = [sanitize_address(addr, encoding) for addr in email_message.recipients()]
         message = email_message.message()
 
         try:
-            kwargs = {
+            kwargs: Dict[str, Any] = {
                 "Source": from_email,
                 "Destinations": recipients,
                 "RawMessage": {"Data": message.as_bytes(linesep="\r\n")},
             }
 
             if self.configuration_set_name is not None:
                 kwargs["ConfigurationSetName"] = self.configuration_set_name
             if self.ses_source_arn:
                 kwargs['SourceArn'] = self.ses_source_arn
             if self.ses_from_arn:
                 kwargs['FromArn'] = self.ses_from_arn
             if self.ses_return_path_arn:
                 kwargs['ReturnPathArn'] = self.ses_return_path_arn
-
-            response = self.connection.send_raw_email(**kwargs)
+            if self.ses_tags is not None:
+                kwargs["Tags"] = [
+                    {"Name": key, "Value": value}
+                    for key, value in self.ses_tags.items()
+                ]
+            response = self.connection.send_raw_email(**kwargs)  # type: ignore
         except ResponseError as err:
             # Store failure information so to post process it if required
             error_keys = ['status', 'reason', 'body', 'request_id',
                           'error_code', 'error_message']
             for key in error_keys:
                 email_message.extra_headers[key] = getattr(err, key, None)
             if not self.fail_silently:
```

### Comparing `airmailer-0.1.2/airmailer/backend/base.py` & `airmailer-0.2.0/airmailer/backend/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+from typing import Iterable
 
 from ..message import EmailMultiAlternatives
 
 
 class BaseEmailBackend:
     """
     Base class for email backend implementations.
 
-    Subclasses must at least overwrite send_messages().
+    Subclasses must at least overwrite :py:meth:`send_messages`
 
-    open() and close() can be called indirectly by using a backend object as a
-    context manager:
+    :py:meth:`open` and :py:meth:`close` can be called indirectly by using a
+    backend object as a context manager:
+
+    .. code-block:: python
 
        with backend as connection:
            # do something with connection
            pass
     """
     def __init__(self, fail_silently=False, **kwargs):
         self.fail_silently = fail_silently
@@ -26,18 +29,18 @@
 
         This method can be overwritten by backend implementations to
         open a network connection.
 
         It's up to the backend implementation to track the status of
         a network connection if it's needed by the backend.
 
-        This method can be called by applications to force a single
-        network connection to be used when sending mails. See the
-        send_messages() method of the SMTP backend for a reference
-        implementation.
+        This method can be called by applications to force a single network
+        connection to be used when sending mails. See the
+        :py:meth:`airmailer.backend.smtp.SMTPEmailBackend.send_messages` method
+        of the SMTP backend for a reference implementation.
 
         The default implementation does nothing.
         """
         pass
 
     def close(self):
         """Close a network connection."""
@@ -52,20 +55,27 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def send_messages(self, email_messages):
         """
-        Send one or more EmailMessage objects and return the number of email
-        messages sent.
+        Send one or more :py:class:`airmailer.message.EmailMessage` objects and
+        return the number of email messages sent.
         """
         raise NotImplementedError('subclasses of BaseEmailBackend must override send_messages() method')
 
-    def send_mail(self, subject, message, from_email, recipient_list, html_message=None):
+    def send_mail(
+        self,
+        subject: str,
+        message,
+        from_email: str,
+        recipient_list: Iterable[str],
+        html_message: str = None
+    ):
         """
         Easy wrapper for sending a single message to a recipient list. All members
         of the recipient list will see the other recipients in the 'To' field.
         """
         mail = EmailMultiAlternatives(subject, message, from_email, recipient_list)
         if html_message:
             mail.attach_alternative(html_message, 'text/html')
```

### Comparing `airmailer-0.1.2/airmailer/backend/smtp.py` & `airmailer-0.2.0/airmailer/backend/smtp.py`

 * *Files identical despite different names*

### Comparing `airmailer-0.1.2/airmailer/message.py` & `airmailer-0.2.0/airmailer/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,121 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 Adapted shamelessly from Django 3.2.9.
 """
 
+from typing import Dict, Set, Optional, Union, Tuple, List, Iterable, cast
+
 import mimetypes
 from email import (
     charset as Charset, encoders as Encoders, generator, message_from_string,
 )
 from email.errors import HeaderParseError
 from email.header import Header
-from email.headerregistry import Address, parser
+from email.headerregistry import Address, parser  # type: ignore
 from email.message import Message
 from email.mime.base import MIMEBase
 from email.mime.message import MIMEMessage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formataddr, formatdate, getaddresses, make_msgid
 from io import BytesIO, StringIO
 from pathlib import Path
 import socket
 
-# Don't BASE64-encode UTF-8 messages so that we avoid unwanted attention from
-# some spam filters.
+EmailPayload = Union[List[Message], str, bytes, bytearray]
+EmailContent = Union[MIMEBase, str, bytes, bytearray]
+EmailAttachment = Union[EmailContent, Tuple[str, bytes, str]]
+
+#: Our ``utf-8`` charset definition.  This differs from the default in that we
+#: configure it to not BASE64-encode UTF-8 messages so that we avoid unwanted
+#: attention from : some spam filters.
 utf8_charset = Charset.Charset('utf-8')
-utf8_charset.body_encoding = None  # Python defaults to BASE64
+utf8_charset.body_encoding = None  # type: ignore
+#: A specific ``utf-8`` charset definition that we use when one or more of the
+#: lines in our message headers or body is longer than
+#: :py:data:`RFC5322_EMAIL_LINE_LENGTH_LIMIT` : This sets the body encoding to
+#: :py:data:`Charset.QP` (quoted-printable) to ensure that the message is still
+#: delivered.  Quoted-printable encoding has the side effect of shortening the
+#: long lines.
 utf8_charset_qp = Charset.Charset('utf-8')
 utf8_charset_qp.body_encoding = Charset.QP
 
-# Default MIME type to use on attachments (if it is not explicitly given
-# and cannot be guessed).
-DEFAULT_ATTACHMENT_MIME_TYPE = 'application/octet-stream'
+#: Default MIME type to use on attachments (if it is not explicitly given
+#: and cannot be guessed).
+DEFAULT_ATTACHMENT_MIME_TYPE: str = 'application/octet-stream'
 
-RFC5322_EMAIL_LINE_LENGTH_LIMIT = 998
+#: The maximum number of bytes allowed in a single header line, as per RFC 5322
+RFC5322_EMAIL_LINE_LENGTH_LIMIT: int = 998
 
 
 class BadHeaderError(ValueError):
     pass
 
 
-# Header names that contain structured address data (RFC #5322)
-ADDRESS_HEADERS = {
+#: Header names that contain structured address data (RFC #5322)
+ADDRESS_HEADERS: Set[str] = {
     'from',
     'sender',
     'reply-to',
     'to',
     'cc',
     'bcc',
     'resent-from',
     'resent-sender',
     'resent-to',
     'resent-cc',
     'resent-bcc',
 }
 
 
-def force_str(s, encoding='utf-8', errors='strict'):
+def force_str(s: Union[str, bytes], encoding: str = 'utf-8', errors: str = 'strict') -> str:
+    """
+    Given a string-like object, return the string version of it, encoded as
+    specified in ``encoding``.
+
+    Args:
+        s: the string-like object
+        encoding: the encoding to use to decode the bytestring, if s is a bytestring
+        errors: how to handle errors in decoding the bytestring
+
+    Returns:
+        The decoded string.
+    """
     if isinstance(s, bytes):
         s = str(s, encoding, errors)
     else:
         s = str(s)
     return s
 
 
-def forbid_multi_line_headers(name, val, encoding):
-    """Forbid multi-line headers to prevent header injection."""
+def forbid_multi_line_headers(name: str, val: str, encoding: Optional[str]) -> Tuple[str, str]:
+    """
+    Forbid multi-line headers to prevent header injection.
+
+    If ``name`` is in :data:`ADDRESS_HEADERS`, each address in ``val`` is run
+    through :py:func:`sanitize_address`.
+
+    Given a header name and header value, check if there are any newline
+    characters in it. If there are, raise a ``BadHeaderError`` exception.
+
+    Args:
+        name: the header name
+        val: the header value
+        encoding: the encoding to use to decode ``val``, if 'ascii' encoding
+            fails
+
+    Raises:
+        BadHeaderError: if there are any newline characters in the header value
+
+    Returns:
+        Sanitized header name and value.
+    """
     encoding = encoding or 'utf-8'
     if '\n' in val or '\r' in val:
         raise BadHeaderError("Header values can't contain newlines (got %r for header %r)" % (val, name))
     try:
         val.encode('ascii')
     except UnicodeEncodeError:
         if name.lower() in ADDRESS_HEADERS:
@@ -78,17 +124,28 @@
             val = Header(val, encoding).encode()
     else:
         if name.lower() == 'subject':
             val = Header(val).encode()
     return name, val
 
 
-def sanitize_address(addr, encoding):
+def sanitize_address(addr: Union[str, Tuple[str, str]], encoding: str) -> str:
     """
     Format a pair of (name, address) or an email address string.
+
+    Args:
+        addr: the address to sanitize
+        encoding: the encoding to use re-encode the address if 'ascii' is not
+            sufficient
+
+    Raises:
+        ValueError: if the address is not a valid email address
+
+    Returns:
+        A santiized email address.
     """
     address = None
     if not isinstance(addr, tuple):
         addr = force_str(addr)
         try:
             token, rest = parser.get_mailbox(addr)
         except (HeaderParseError, ValueError, IndexError):
@@ -124,91 +181,165 @@
     domain = domain.encode('idna').decode('ascii')
 
     parsed_address = Address(username=localpart, domain=domain)
     return formataddr((nm, parsed_address.addr_spec))
 
 
 class MIMEMixin:
-    def as_string(self, unixfrom=False, linesep='\n'):
-        """Return the entire formatted message as a string.
-        Optional `unixfrom' when True, means include the Unix From_ envelope
-        header.
+    """
+    A mixin for :py:class:`Message` that provides methods for converting the
+    message to string or bytes in ways the rest of the code expects.
+    """
 
-        This overrides the default as_string() implementation to not mangle
-        lines that begin with 'From '. See bug #13433 for details.
+    def as_string(self, unixfrom: bool = False, linesep: str = '\n') -> str:
+        """
+        Return the entire formatted message as a string.
+
+        Keyword Args:
+            unixfrom: if ``True,`` include the Unix ``From_`` envelope header
+            linesep: the line separator to use in the returned string
+
+        Returns:
+            The entire formatted message as a string.
         """
         fp = StringIO()
         g = generator.Generator(fp, mangle_from_=False)
-        g.flatten(self, unixfrom=unixfrom, linesep=linesep)
+        g.flatten(cast(Message, self), unixfrom=unixfrom, linesep=linesep)
         return fp.getvalue()
 
-    def as_bytes(self, unixfrom=False, linesep='\n'):
-        """Return the entire formatted message as bytes.
-        Optional `unixfrom' when True, means include the Unix From_ envelope
-        header.
+    def as_bytes(self, unixfrom: bool = False, linesep: str = '\n') -> bytes:
+        """
+        Return the entire formatted message as bytes.
+
+        Keyword Args:
+            unixfrom: if ``True,`` include the Unix ``From_`` envelope header
+            linesep: the line separator to use in the returned string
 
-        This overrides the default as_bytes() implementation to not mangle
-        lines that begin with 'From '. See bug #13433 for details.
+        Returns:
+            The entire formatted message as a string.
         """
         fp = BytesIO()
         g = generator.BytesGenerator(fp, mangle_from_=False)
-        g.flatten(self, unixfrom=unixfrom, linesep=linesep)
+        g.flatten(cast(Message, self), unixfrom=unixfrom, linesep=linesep)
         return fp.getvalue()
 
 
 class SafeMIMEMessage(MIMEMixin, MIMEMessage):
+    """
+    A :py:class:`email.message.Message` subclass that sanitizes any headers
+    before they are added to the message.
+    """
+
+    def __setitem__(self, name: str, val: str) -> None:
+        """
+        Add a header to the message, sanitizing the header name and value.
 
-    def __setitem__(self, name, val):
+        Args:
+            name: the header name
+            val: the header value
+        """
         # message/rfc822 attachments must be ASCII
         name, val = forbid_multi_line_headers(name, val, 'ascii')
         MIMEMessage.__setitem__(self, name, val)
 
 
 class SafeMIMEText(MIMEMixin, MIMEText):
+    """
+    A :py:class:`email.mime.text.MIMEText` subclass doe some payload
+    sanitization.
 
-    def __init__(self, _text, _subtype='plain', _charset=None):
+    * If the payload contains any lines longer than :py:data:`RFC5322_EMAIL_LINE_LENGTH_LIMIT`,
+      use quoted-printable encoding for the body.
+    * Sanitize any headers before they are added to the message.
+    """
+
+    def __init__(self, _text: str, _subtype='plain', _charset=None):
         self.encoding = _charset
         MIMEText.__init__(self, _text, _subtype=_subtype, _charset=_charset)
 
-    def __setitem__(self, name, val):
+    def __setitem__(self, name: str, val: str) -> None:
+        """
+        Add a header to the message, sanitizing the header name and value.
+
+        Args:
+            name: the header name
+            val: the header value
+        """
         name, val = forbid_multi_line_headers(name, val, self.encoding)
         MIMEText.__setitem__(self, name, val)
 
-    def set_payload(self, payload, charset=None):
+    def set_payload(self, payload: str, charset: Union[str, Charset.Charset] = None):
+        """
+        If the payload contains any lines longer than
+        :py:data:`RFC5322_EMAIL_LINE_LENGTH_LIMIT`, the payload will be encoded
+        using quoted-printable encoding.
+
+        Args:
+            payload: the payload to set
+            charset: the charset to use to encode the payload
+        """
         if charset == 'utf-8' and not isinstance(charset, Charset.Charset):
             has_long_lines = any(
                 len(line.encode()) > RFC5322_EMAIL_LINE_LENGTH_LIMIT
                 for line in payload.splitlines()
             )
             # Quoted-Printable encoding has the side effect of shortening long
             # lines, if any (#22561).
             charset = utf8_charset_qp if has_long_lines else utf8_charset
         MIMEText.set_payload(self, payload, charset=charset)
 
 
 class SafeMIMEMultipart(MIMEMixin, MIMEMultipart):
+    """
+    A mulitpart MIME message that sanitizes any headers before they are added.
+    """
 
-    def __init__(self, _subtype='mixed', boundary=None, _subparts=None, encoding=None, **_params):
+    def __init__(
+        self,
+        _subtype: str = 'mixed',
+        boundary: str = None,
+        _subparts=None,
+        encoding: str = None,
+        **_params
+    ):
         self.encoding = encoding
         MIMEMultipart.__init__(self, _subtype, boundary, _subparts, **_params)
 
-    def __setitem__(self, name, val):
+    def __setitem__(self, name: str, val: str) -> None:
         name, val = forbid_multi_line_headers(name, val, self.encoding)
         MIMEMultipart.__setitem__(self, name, val)
 
 
 class EmailMessage:
-    """A container for email information."""
-    content_subtype = 'plain'
-    mixed_subtype = 'mixed'
-    encoding = 'utf-8'
-
-    def __init__(self, subject='', body='', from_email=None, to=None, bcc=None,
-                 attachments=None, headers=None, cc=None,
-                 reply_to=None):
+    """
+    A container class for email information.  We use this instead of
+    :py:class:`email.message.Message` directly so that we can send the same
+    message to multiple recipients and to ease the construction of the
+    complicated ``Message`` object.
+    """
+    #: When constructing the mimetype for the message body, use this subtype of
+    #: "text".  Default is "plain", which means that the message body
+    #: will be specified as "text/plain".
+    content_subtype: str = 'plain'
+    mixed_subtype: str = 'mixed'
+    #: Use this as the default encoding for our message body.
+    encoding: str = 'utf-8'
+
+    def __init__(
+        self,
+        subject: str = '',
+        body: str = '',
+        from_email: str = None,
+        to: Iterable[str] = None,
+        bcc: Iterable[str] = None,
+        attachments: List[EmailAttachment] = None,
+        headers: Dict[str, str] = None,
+        cc: Iterable[str] = None,
+        reply_to: Iterable[str] = None
+    ):
         """
         Initialize a single email message (which can be sent to multiple
         recipients).
         """
         if to:
             if isinstance(to, str):
                 raise TypeError('"to" argument must be a list or tuple')
@@ -274,125 +405,150 @@
     def recipients(self):
         """
         Return a list of all recipients of the email (includes direct
         addressees as well as Cc and Bcc entries).
         """
         return [email for email in (self.to + self.cc + self.bcc) if email]
 
-    def attach(self, filename=None, content=None, mimetype=None):
+    def attach(
+        self,
+        filename: Union[Path, str] = None,
+        content: EmailContent = None,
+        mimetype: str = None
+    ):
         """
         Attach a file with the given filename and content. The filename can
         be omitted and the mimetype is guessed, if not provided.
 
-        If the first parameter is a MIMEBase subclass, insert it directly
-        into the resulting message attachments.
+        If the first parameter is a :py:class:`email.mime.base.MIMEBase`
+        subclass, insert it directly into the resulting message attachments.
 
-        For a text/* mimetype (guessed or specified), when a bytes object is
+        For a ``text/*`` mimetype (guessed or specified), when a bytes object is
         specified as content, decode it as UTF-8. If that fails, set the
-        mimetype to DEFAULT_ATTACHMENT_MIME_TYPE and don't decode the content.
+        mimetype to :py:data:`DEFAULT_ATTACHMENT_MIME_TYPE` and don't decode the
+        content.
         """
         if isinstance(filename, MIMEBase):
             if content is not None or mimetype is not None:
                 raise ValueError(
                     'content and mimetype must not be given when a MIMEBase '
                     'instance is provided.'
                 )
             self.attachments.append(filename)
         elif content is None:
             raise ValueError('content must be provided.')
         else:
             mimetype = mimetype or mimetypes.guess_type(filename)[0] or DEFAULT_ATTACHMENT_MIME_TYPE
-            basetype, subtype = mimetype.split('/', 1)
+            basetype, _ = mimetype.split('/', 1)
 
             if basetype == 'text':
                 if isinstance(content, bytes):
                     try:
                         content = content.decode()
                     except UnicodeDecodeError:
                         # If mimetype suggests the file is text but it's
                         # actually binary, read() raises a UnicodeDecodeError.
                         mimetype = DEFAULT_ATTACHMENT_MIME_TYPE
 
             self.attachments.append((filename, content, mimetype))
 
-    def attach_file(self, path, mimetype=None):
+    def attach_file(self, path: Union[Path, str], mimetype: str = None):
         """
         Attach a file from the filesystem.
 
-        Set the mimetype to DEFAULT_ATTACHMENT_MIME_TYPE if it isn't specified
-        and cannot be guessed.
+        Set the mimetype to :py:data:`DEFAULT_ATTACHMENT_MIME_TYPE` if it isn't
+        specified and cannot be guessed.
 
-        For a text/* mimetype (guessed or specified), decode the file's content
-        as UTF-8. If that fails, set the mimetype to
-        DEFAULT_ATTACHMENT_MIME_TYPE and don't decode the content.
+        For a ``text/*`` mimetype (guessed or specified), decode the file's
+        content as UTF-8. If that fails, set the mimetype to
+        :py:data:`DEFAULT_ATTACHMENT_MIME_TYPE` and don't decode the content.
         """
         path = Path(path)
         with path.open('rb') as file:
             content = file.read()
             self.attach(path.name, content, mimetype)
 
-    def _create_message(self, msg):
+    def _create_message(self, msg: MIMEBase):
         return self._create_attachments(msg)
 
-    def _create_attachments(self, msg):
+    def _create_attachments(self, msg: MIMEBase):
         if self.attachments:
             encoding = self.encoding or 'utf-8'
             body_msg = msg
             msg = SafeMIMEMultipart(_subtype=self.mixed_subtype, encoding=encoding)
             if self.body or body_msg.is_multipart():
                 msg.attach(body_msg)
             for attachment in self.attachments:
                 if isinstance(attachment, MIMEBase):
                     msg.attach(attachment)
                 else:
                     msg.attach(self._create_attachment(*attachment))
         return msg
 
-    def _create_mime_attachment(self, content, mimetype):
+    def _create_mime_attachment(
+        self,
+        content: "Union[Message, EmailMessage, str]",
+        mimetype: str
+    ) -> Union[MIMEBase, SafeMIMEText, SafeMIMEMessage]:
         """
         Convert the content, mimetype pair into a MIME attachment object.
 
-        If the mimetype is message/rfc822, content may be an
-        email.Message or EmailMessage object, as well as a str.
+        If the mimetype is ``message/rfc822``, content may be an
+        :py:class:`email.message.Message` or :py:class:`EmailMessage` object, as
+        well as a str.
+
+        Args:
+            content: The content of the attachment.
+            mimetype: The mimetype of the attachment.
+
+        Returns:
+            A MIME attachment object.
         """
+        attachment: Union[MIMEBase, SafeMIMEText, SafeMIMEMessage]
         basetype, subtype = mimetype.split('/', 1)
         if basetype == 'text':
             encoding = self.encoding or 'utf-8'
-            attachment = SafeMIMEText(content, subtype, encoding)
+            attachment = SafeMIMEText(cast(str, content), subtype, encoding)
         elif basetype == 'message' and subtype == 'rfc822':
             # Bug #18967: per RFC2046 s5.2.1, message/rfc822 attachments
             # must not be base64 encoded.
             if isinstance(content, EmailMessage):
                 # convert content into an email.Message first
                 content = content.message()
             elif not isinstance(content, Message):
                 # For compatibility with existing code, parse the message
                 # into an email.Message object if it is not one already.
                 content = message_from_string(force_str(content))
 
-            attachment = SafeMIMEMessage(content, subtype)
+            attachment = SafeMIMEMessage(cast(Message, content), subtype)
         else:
             # Encode non-text attachments with base64.
             attachment = MIMEBase(basetype, subtype)
             attachment.set_payload(content)
             Encoders.encode_base64(attachment)
         return attachment
 
-    def _create_attachment(self, filename, content, mimetype=None):
+    def _create_attachment(self, filename: str, content, mimetype: str = None):
         """
         Convert the filename, content, mimetype triple into a MIME attachment
         object.
+
+        Args:
+            filename: The filename to attach the content as.
+            content: The content to attach.
+            mimetype: The mimetype of the content, if not specified, guess
         """
         attachment = self._create_mime_attachment(content, mimetype)
-        if filename:
+        _filename: Union[str, Tuple[str, str, str]] = filename
+        if _filename:
             try:
-                filename.encode('ascii')
+                cast(str, _filename).encode('ascii')
             except UnicodeEncodeError:
-                filename = ('utf-8', '', filename)
-            attachment.add_header('Content-Disposition', 'attachment', filename=filename)
+                _filename = ('utf-8', '', filename)
+            attachment.add_header('Content-Disposition', 'attachment', filename=_filename)
         return attachment
 
     def _set_list_header_if_not_empty(self, msg, header, values):
         """
         Set msg's header, either from self.extra_headers, if present, or from
         the values argument.
         """
@@ -402,23 +558,33 @@
             except KeyError:
                 value = ', '.join(str(v) for v in values)
             msg[header] = value
 
 
 class EmailMultiAlternatives(EmailMessage):
     """
-    A version of EmailMessage that makes it easy to send multipart/alternative
-    messages. For example, including text and HTML versions of the text is
-    made easier.
-    """
-    alternative_subtype = 'alternative'
-
-    def __init__(self, subject='', body='', from_email=None, to=None, bcc=None,
-                 attachments=None, headers=None, alternatives=None,
-                 cc=None, reply_to=None):
+    A version of :py:class:`EmailMessage` that makes it easy to send
+    multipart/alternative messages. For example, including text and HTML
+    versions of the text is made easier.
+    """
+    alternative_subtype: str = 'alternative'
+
+    def __init__(
+        self,
+        subject: str = '',
+        body: str = '',
+        from_email: str = None,
+        to: Iterable[str] = None,
+        bcc: Iterable[str] = None,
+        attachments: List[EmailAttachment] = None,
+        headers: Dict[str, str] = None,
+        alternatives=None,
+        cc: Iterable[str] = None,
+        reply_to: Iterable[str] = None
+    ):
         """
         Initialize a single email message (which can be sent to multiple
         recipients).
         """
         super().__init__(
             subject, body, from_email, to, bcc, attachments,
             headers, cc, reply_to,
```

### Comparing `airmailer-0.1.2/setup.cfg` & `airmailer-0.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
 [bumpversion:file:airmailer/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
+[bumpversion:file:doc/source/conf.py]
+
 [bdist_wheel]
 universal = 1
 
 [flake8]
 max-line-length = 120
 filename = *.py
 exclude = *.cfg, *.js, *.json, *.bak, *.md, *.sql, *.sh, *.txt, *.yml, simple_test_db, Makefile, Dockerfile, MANIFEST.in, docs
 ignore = E221,E241,E265,E266,E401,W504
 
 [mypy]
 python_executable = ~/.pyenv/shims/python
+implicit_optional = True
+exclude = (^build/.*$|^docs/.*\.py$|test_.*\.py$)
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `airmailer-0.1.2/setup.py` & `airmailer-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords=['aws', 'email'],
     name='airmailer',
     packages=find_packages(include=['airmailer', 'airmailer.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/cmalek/airmailer',
-    version='0.1.2',
+    version='0.2.0',
     zip_safe=False,
 )
```

