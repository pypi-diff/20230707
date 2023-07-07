# Comparing `tmp/roboto_sdk-0.1.5.tar.gz` & `tmp/roboto_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.5.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.6.tar", max compression
```

## Comparing `roboto_sdk-0.1.5.tar` & `roboto_sdk-0.1.6.tar`

### file list

```diff
@@ -1,149 +1,169 @@
--rw-r--r--   0        0        0       22 2023-07-04 01:18:05.605793 roboto_sdk-0.1.5/README.md
--rw-r--r--   0        0        0      948 2023-07-04 01:19:42.474094 roboto_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-04 01:18:05.609793 roboto_sdk-0.1.5/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-07-04 01:18:05.609793 roboto_sdk-0.1.5/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0      322 2023-07-04 01:19:08.421988 roboto_sdk-0.1.5/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3811 2023-07-04 01:19:08.421988 roboto_sdk-0.1.5/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
--rw-r--r--   0        0        0     4037 2023-07-04 01:18:05.609793 roboto_sdk-0.1.5/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2058 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      822 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6774 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3659 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     4074 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0      120 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0      398 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1849 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc
--rw-r--r--   0        0        0     1641 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     1510 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6438 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0     3737 2023-07-04 01:19:08.457988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5170 2023-07-04 01:19:08.469988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1383 2023-07-04 01:19:08.469988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1124 2023-07-04 01:19:08.457988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
--rw-r--r--   0        0        0      636 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
--rw-r--r--   0        0        0     4784 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
--rw-r--r--   0        0        0     2321 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     4685 2023-07-04 01:19:08.473988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1310 2023-07-04 01:19:08.473988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2340 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
--rw-r--r--   0        0        0     7427 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     3015 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5168 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      640 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      808 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4499 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1726 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4768 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      566 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1652 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0      735 2023-07-04 01:19:08.477988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7400 2023-07-04 01:19:08.477988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0     3184 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5064 2023-07-04 01:19:08.489988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      867 2023-07-04 01:19:08.489988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1263 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     9836 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2215 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4911 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      867 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0      712 2023-07-04 01:19:08.481988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-07-04 01:19:08.481988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1536 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
--rw-r--r--   0        0        0     2835 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      723 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0      696 2023-07-04 01:19:08.481988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     3232 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1181 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      802 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2166 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      382 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2358 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0     1974 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/http_delegates.py
--rw-r--r--   0        0        0      728 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0      896 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2758 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5097 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1012 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2574 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc
--rw-r--r--   0        0        0     2178 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc
--rw-r--r--   0        0        0     2413 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc
--rw-r--r--   0        0        0     1709 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     2052 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     4674 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     1815 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1680 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_invite.py
--rw-r--r--   0        0        0     1432 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      722 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      640 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2697 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      685 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1003 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     2542 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc
--rw-r--r--   0        0        0      888 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     2038 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      216 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      455 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1832 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0      642 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2758 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      657 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2388 2023-07-04 01:19:08.513988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc
--rw-r--r--   0        0        0     1488 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      617 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
--rw-r--r--   0        0        0     2280 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2683 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      882 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0      554 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1617 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1940 2023-07-04 01:19:08.497988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1172 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      658 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc
--rw-r--r--   0        0        0     1051 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1213 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      485 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      194 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      841 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      500 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     9636 2023-07-04 01:19:08.073987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
--rw-r--r--   0        0        0     3963 2023-07-04 01:19:08.109987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
--rw-r--r--   0        0        0     1666 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
--rw-r--r--   0        0        0      216 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     9060 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3161 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0     1004 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      224 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0      428 2023-07-04 01:19:08.449988 roboto_sdk-0.1.5/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2991 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
--rw-r--r--   0        0        0     2977 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0     1250 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-07 04:18:57.189444 roboto_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0      948 2023-07-07 04:20:43.065351 roboto_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-07 04:18:57.193444 roboto_sdk-0.1.6/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-07 04:18:57.193444 roboto_sdk-0.1.6/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-07 04:20:01.901387 roboto_sdk-0.1.6/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3811 2023-07-07 04:20:01.901387 roboto_sdk-0.1.6/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
+-rw-r--r--   0        0        0     4037 2023-07-07 04:18:57.193444 roboto_sdk-0.1.6/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/commands.py
+-rw-r--r--   0        0        0     4678 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/create.py
+-rw-r--r--   0        0        0     1437 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/docker_login.py
+-rw-r--r--   0        0        0     3187 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/invoke.py
+-rw-r--r--   0        0        0     1174 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/list_invocations.py
+-rw-r--r--   0        0        0     1827 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/search.py
+-rw-r--r--   0        0        0     6397 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/shared.py
+-rw-r--r--   0        0        0      960 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/show.py
+-rw-r--r--   0        0        0     4945 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/update.py
+-rw-r--r--   0        0        0      334 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1471 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2286 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      891 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6741 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     4025 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      322 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/invocations/__init__.py
+-rw-r--r--   0        0        0     1967 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/invocations/status.py
+-rw-r--r--   0        0        0      110 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     8083 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3291 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2876 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0      120 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-07 04:20:01.541387 roboto_sdk-0.1.6/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2023-07-07 04:20:01.541387 roboto_sdk-0.1.6/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     1682 2023-07-07 04:20:01.937387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7230 2023-07-07 04:20:01.937387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     3263 2023-07-07 04:20:01.941387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_container_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     3263 2023-07-07 04:20:01.945387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5468 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1583 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1336 2023-07-07 04:20:01.945387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2023-07-07 04:20:01.961387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     5231 2023-07-07 04:20:01.949386 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
+-rw-r--r--   0        0        0     2517 2023-07-07 04:20:01.949386 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4924 2023-07-07 04:20:01.961387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1484 2023-07-07 04:20:01.961387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2519 2023-07-07 04:20:01.949386 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
+-rw-r--r--   0        0        0     8680 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     2685 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_container_resources.py
+-rw-r--r--   0        0        0     2875 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5629 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      860 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      988 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4836 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1939 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     5108 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      752 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1839 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-07 04:20:01.965386 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7622 2023-07-07 04:20:01.965386 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     3184 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5064 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2023-07-07 04:20:01.977387 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0    10221 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2215 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4911 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      867 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0      712 2023-07-07 04:20:01.969386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-07-07 04:20:01.969386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1536 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
+-rw-r--r--   0        0        0     2835 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      696 2023-07-07 04:20:01.969386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3232 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1181 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      802 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2166 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      382 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2358 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0     1974 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/http_delegates.py
+-rw-r--r--   0        0        0      852 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3586 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     6907 2023-07-07 04:20:01.989386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-07-07 04:20:01.989386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     4106 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc
+-rw-r--r--   0        0        0     2331 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc
+-rw-r--r--   0        0        0     2671 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc
+-rw-r--r--   0        0        0     1709 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2856 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     6889 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      540 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     3344 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1768 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1751 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      726 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      640 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2697 2023-07-07 04:20:01.997387 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      685 2023-07-07 04:20:01.997387 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1003 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2528 2023-07-07 04:20:01.997387 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc
+-rw-r--r--   0        0        0      888 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2038 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      216 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1826 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2758 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      657 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2392 2023-07-07 04:20:02.005386 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc
+-rw-r--r--   0        0        0     1488 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      617 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
+-rw-r--r--   0        0        0     2280 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2685 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      882 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1617 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2213 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1172 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc
+-rw-r--r--   0        0        0     1051 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1408 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      485 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      257 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      285 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2105 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__pycache__/domain.cpython-310.pyc
+-rw-r--r--   0        0        0     1266 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/domain.py
+-rw-r--r--   0        0        0      782 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-07 04:20:01.541387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2023-07-07 04:20:01.545387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0      688 2023-07-07 04:20:01.545387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0     9636 2023-07-07 04:20:01.545387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     3963 2023-07-07 04:20:01.585387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     1666 2023-07-07 04:20:01.937387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0      443 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/headers.py
+-rw-r--r--   0        0        0     9060 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3161 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0     1004 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      224 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0      428 2023-07-07 04:20:01.933386 roboto_sdk-0.1.6/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2991 2023-07-07 04:20:01.933386 roboto_sdk-0.1.6/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     2977 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.6/PKG-INFO
```

### Comparing `roboto_sdk-0.1.5/pyproject.toml` & `roboto_sdk-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.5"
+version = "0.1.6"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 4037 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 c50f 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 c50f 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6403  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6508 8300 5a0b 6401 5a0c  m.Z...e...Z.d.Z.
@@ -26,16 +26,16 @@
 00000190: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
 000001a0: 005a 0264 0153 0029 02da 1652 656a 6563  .Z.d.S.)...Rejec
 000001b0: 7465 6454 6f6b 656e 4578 6365 7074 696f  tedTokenExceptio
 000001c0: 6e4e 2903 da08 5f5f 6e61 6d65 5f5f da0a  nN)...__name__..
 000001d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000001e0: 616c 6e61 6d65 5f5f a900 720b 0000 0072  alname__..r....r
 000001f0: 0b00 0000 fae0 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000200: 2f6f 7574 7075 742f 7372 6333 3439 3732  /output/src34972
-00000210: 3638 3637 302f 7372 632f 636f 6465 7374  68670/src/codest
+00000200: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
+00000210: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
 00000220: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000230: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000240: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000250: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000260: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000270: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000280: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.6/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/command/args.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import argparse
 import json
 import os
 import pathlib
+import typing
 
 
 def JsonFileOrStrType(arg):
     arg_type = "string"
 
     if os.path.isfile(arg):
         arg_type = "file"
@@ -21,24 +22,30 @@
     except ValueError:
         raise argparse.ArgumentTypeError(
             "Could not interpret payload {} '{}' as JSON".format(arg_type, arg)
         )
 
 
 class KeyValuePairsAction(argparse.Action):
-    value_dict: dict[str, str] = {}
+    value_dict: dict[str, typing.Any] = {}
 
     def __call__(self, parser, namespace, values, option_string):
         for pair in values:
             key, value = pair.split("=")
             if key in self.value_dict:
                 raise parser.error(
                     f"Key '{key}' was defined multiple times for '{self.dest}'"
                 )
-            self.value_dict[key] = value
+            # Attempt to parse the value to better handle numbers, booleans, etc
+            parsed_value = value
+            try:
+                parsed_value = json.loads(value)
+            except json.decoder.JSONDecodeError:
+                pass  # swallow
+            self.value_dict[key] = parsed_value
 
         setattr(namespace, self.dest, self.value_dict)
 
 
 def ExistingPathlibPath(arg):
     path = pathlib.Path(arg)
     if not path.exists():
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/command/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
+import sys
 from typing import Any, Callable, Optional
 
+from ...exceptions import RobotoDomainException
 from ..context import CLIContext
 
 
 class RobotoCommand(object):
     _name: str
     _logic: Callable[
         [Any, CLIContext, argparse.ArgumentParser], None
@@ -33,15 +35,19 @@
     def command_kwargs(self):
         if self._command_kwargs is not None:
             return self._command_kwargs
         return {}
 
     def setup_parser(self, parser, context):
         def context_aware_logic(args):
-            return self._logic(args, context, parser)
+            try:
+                return self._logic(args, context, parser)
+            except RobotoDomainException as rde:
+                sys.stderr.write(f"{rde.__class__.__name__}: {rde}\n")
+                sys.exit(1)
 
         parser.set_defaults(func=context_aware_logic)
         if self._inner_setup_parser is not None:
             self._inner_setup_parser(parser)
 
 
 class RobotoCommandSet(object):
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 from typing import Optional
 
-from ..domain.actions import ActionDelegate
+from ..domain.actions import (
+    ActionDelegate,
+    InvocationDelegate,
+)
 from ..domain.datasets import DatasetDelegate
 from ..domain.orgs import OrgDelegate
 from ..domain.tokens import TokenDelegate
 from ..domain.triggers import TriggerDelegate
 from ..http import HttpClient
 
 
 class CLIContext:
     _http: Optional[HttpClient]
+    actions: ActionDelegate
     datasets: DatasetDelegate
+    invocations: InvocationDelegate
     orgs: OrgDelegate
     tokens: TokenDelegate
     triggers: TriggerDelegate
-    actions: ActionDelegate
 
     @property
     def http(self) -> HttpClient:
         # Necessary since http is lazy set after parsing args
         if self._http is None:
             raise ValueError("Unset HTTP client!")
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/datasets/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,10 +234,10 @@
     list_files_command,
     upload_files_command,
     download_files_command,
 ]
 
 command_set = RobotoCommandSet(
     name="datasets",
-    help="Commands for managing triggers which automatically invoke actions on datasets when certain criteria are met",
+    help="Get, create, update, and query datasets. Upload to and download from them.",
     commands=commands,
 )
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,53 @@
 
 import argparse
 import logging
 import pathlib
 import sys
 from typing import Any
 
-from ..domain.actions import ActionHttpDelegate
+from ..domain.actions import (
+    ActionHttpDelegate,
+    InvocationHttpDelegate,
+)
 from ..domain.datasets import DatasetHttpDelegate
 from ..domain.orgs import OrgHttpDelegate
 from ..domain.tokens import TokenHttpDelegate
 from ..domain.triggers import TriggerHttpDelegate
 from ..http import (
     HttpClient,
     LocalAuthDecorator,
     PATAuthDecorator,
 )
 from ..profile import RobotoProfile
+from .actions import (
+    command_set as actions_command_set,
+)
 from .context import CLIContext
 from .datasets import (
     command_set as datasets_command_set,
 )
+from .invocations import (
+    command_set as invocations_command_set,
+)
 from .orgs import command_set as orgs_command_set
 from .tokens import (
     command_set as tokens_command_set,
 )
 from .triggers import (
     command_set as triggers_command_set,
 )
 from .users import (
     command_set as users_command_set,
 )
 
 COMMAND_SETS = [
+    actions_command_set,
     datasets_command_set,
+    invocations_command_set,
     orgs_command_set,
     users_command_set,
     tokens_command_set,
     triggers_command_set,
 ]
 
 BETA_USER_POOL_CLIENT_ID = "7p2e45lijin58tuaairtflf3m8"
@@ -70,14 +81,17 @@
 
     context.actions = ActionHttpDelegate(
         http_client=http, roboto_service_base_url=profile_entry.default_endpoint
     )
     context.datasets = DatasetHttpDelegate(
         http_client=http, roboto_service_base_url=profile_entry.default_endpoint
     )
+    context.invocations = InvocationHttpDelegate(
+        http_client=http, roboto_service_base_url=profile_entry.default_endpoint
+    )
     context.orgs = OrgHttpDelegate(http_client=http)
     context.triggers = TriggerHttpDelegate(http_client=http)
     context.http = http
     context.tokens = TokenHttpDelegate(http_client=http)
 
 
 def entry():
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/tokens/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,35 +52,35 @@
         choices=[30, 60, 90],
         default=30,
         help="The number of days this token will be valid for.",
     )
 
 
 def list(args, context: CLIContext, parser: argparse.ArgumentParser):
-    tokens = Token.by_user_id(user_id=None, token_delegate=context.tokens)
+    tokens = Token.for_user(user_id=None, token_delegate=context.tokens)
     for token in tokens:
         sys.stdout.write(json.dumps(token.to_dict()) + "\n")
 
 
 def get(args, context: CLIContext, parser: argparse.ArgumentParser):
-    token = Token.by_token_id(token_id=args.token_id, token_delegate=context.tokens)
+    token = Token.from_id(token_id=args.token_id, token_delegate=context.tokens)
     sys.stdout.write(json.dumps(token.to_dict()) + "\n")
 
 
 def get_setup_parser(parser):
     parser.add_argument(
         "--token-id",
         type=str,
         required=True,
         help="The token_id for a token to look up.",
     )
 
 
 def delete(args, context: CLIContext, parser: argparse.ArgumentParser):
-    Token.by_token_id(token_id=args.token_id, token_delegate=context.tokens).delete()
+    Token.from_id(token_id=args.token_id, token_delegate=context.tokens).delete()
     sys.stdout.write("Successfully deleted!\n")
 
 
 def delete_setup_parser(parser):
     parser.add_argument(
         "--token-id",
         type=str,
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/triggers/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     parser.add_argument(
         "--action-name", type=str, required=True, help=ACTION_NAME_PARAM_HELP
     )
     parser.add_argument("--org", type=str, help=ORG_ARG_HELP)
 
 
 def get(args, context: CLIContext, parser: argparse.ArgumentParser):
-    record = Trigger.by_name(
+    record = Trigger.from_name(
         name=args.name,
         org_id=args.org,
         action_delegate=context.actions,
         trigger_delegate=context.triggers,
     )
     sys.stdout.write(json.dumps(record.to_dict()) + "\n")
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.6/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1974 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 b607 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 b607 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 6405 6409 6c0d  d.l.m.Z...d.d.l.
@@ -66,16 +66,16 @@
 00000410: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 00000420: 0000 0072 0f00 0000 290c 7218 0000 0072  ...r....).r....r
 00000430: 1900 0000 da05 656e 7472 795a 0461 7574  ......entryZ.aut
 00000440: 68da 0468 7474 7072 1000 0000 7211 0000  h..httpr....r...
 00000450: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
 00000460: 7215 0000 0072 1600 0000 a900 721e 0000  r....r......r...
 00000470: 00fa ed2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000480: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
-00000490: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
+00000480: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
+00000490: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
 000004a0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000004b0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000004c0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000004d0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000004e0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000004f0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000500: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 from .action import Action
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerCredentials,
+    ContainerParameters,
+    RepositoryPurpose,
+    RepositoryTag,
+)
 from .action_delegate import (
     ActionDelegate,
-    ContainerCredentials,
     UpdateCondition,
 )
 from .action_http_delegate import (
     ActionHttpDelegate,
 )
 from .action_http_resources import (
     ContainerUploadCredentials,
@@ -44,25 +50,29 @@
     "Action",
     "ActionDelegate",
     "ActionHttpDelegate",
     "ActionRecord",
     "ActionUpdateConditionCheckFailure",
     "ContainerCredentials",
     "ContainerUploadCredentials",
+    "ComputeRequirements",
+    "ContainerParameters",
     "CreateActionRequest",
     "CreateInvocationRequest",
     "Invocation",
     "InvocationDataSource",
     "InvocationDataSourceType",
     "InvocationDelegate",
     "InvocationError",
     "InvocationHttpDelegate",
     "InvocationProvenance",
     "InvocationRecord",
     "InvocationSource",
     "InvocationStatus",
     "InvocationStatusRecord",
+    "RepositoryPurpose",
+    "RepositoryTag",
     "SetLogsLocationRequest",
     "UpdateActionRequest",
     "UpdateCondition",
     "UpdateInvocationStatus",
 )
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1641 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,106 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 6906 0000  o.......Ms.di...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 5507 0000  o.......1..dU...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
-00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
-00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6407 6c11  m.Z.m.Z...d.d.l.
-00000090: 6d12 5a12 0100 6400 6408 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 6409 6c15 6d16 5a16 0100 6400  ..d.d.l.m.Z...d.
-000000b0: 640a 6c17 6d18 5a18 6d19 5a19 6d1a 5a1a  d.l.m.Z.m.Z.m.Z.
-000000c0: 0100 6400 640b 6c1b 6d1c 5a1c 6d1d 5a1d  ..d.d.l.m.Z.m.Z.
-000000d0: 6d1e 5a1e 6d1f 5a1f 6d20 5a20 6d21 5a21  m.Z.m.Z.m Z m!Z!
-000000e0: 6d22 5a22 0100 640c 5a23 640d 5300 290e  m"Z"..d.Z#d.S.).
-000000f0: e901 0000 0029 01da 0641 6374 696f 6e29  .....)...Action)
-00000100: 03da 0e41 6374 696f 6e44 656c 6567 6174  ...ActionDelegat
-00000110: 65da 1443 6f6e 7461 696e 6572 4372 6564  e..ContainerCred
-00000120: 656e 7469 616c 73da 0f55 7064 6174 6543  entials..UpdateC
-00000130: 6f6e 6469 7469 6f6e 2901 da12 4163 7469  ondition)...Acti
-00000140: 6f6e 4874 7470 4465 6c65 6761 7465 2903  onHttpDelegate).
-00000150: da1a 436f 6e74 6169 6e65 7255 706c 6f61  ..ContainerUploa
-00000160: 6443 7265 6465 6e74 6961 6c73 da13 4372  dCredentials..Cr
-00000170: 6561 7465 4163 7469 6f6e 5265 7175 6573  eateActionReques
-00000180: 74da 1355 7064 6174 6541 6374 696f 6e52  t..UpdateActionR
-00000190: 6571 7565 7374 2901 da0c 4163 7469 6f6e  equest)...Action
-000001a0: 5265 636f 7264 2902 da21 4163 7469 6f6e  Record)..!Action
-000001b0: 5570 6461 7465 436f 6e64 6974 696f 6e43  UpdateConditionC
-000001c0: 6865 636b 4661 696c 7572 65da 0f49 6e76  heckFailure..Inv
-000001d0: 6f63 6174 696f 6e45 7272 6f72 2901 da0a  ocationError)...
-000001e0: 496e 766f 6361 7469 6f6e 2901 da12 496e  Invocation)...In
-000001f0: 766f 6361 7469 6f6e 4465 6c65 6761 7465  vocationDelegate
-00000200: 2901 da16 496e 766f 6361 7469 6f6e 4874  )...InvocationHt
-00000210: 7470 4465 6c65 6761 7465 2903 da17 4372  tpDelegate)...Cr
-00000220: 6561 7465 496e 766f 6361 7469 6f6e 5265  eateInvocationRe
-00000230: 7175 6573 74da 1653 6574 4c6f 6773 4c6f  quest..SetLogsLo
-00000240: 6361 7469 6f6e 5265 7175 6573 74da 1655  cationRequest..U
-00000250: 7064 6174 6549 6e76 6f63 6174 696f 6e53  pdateInvocationS
-00000260: 7461 7475 7329 07da 1449 6e76 6f63 6174  tatus)...Invocat
-00000270: 696f 6e44 6174 6153 6f75 7263 65da 1849  ionDataSource..I
-00000280: 6e76 6f63 6174 696f 6e44 6174 6153 6f75  nvocationDataSou
-00000290: 7263 6554 7970 65da 1449 6e76 6f63 6174  rceType..Invocat
-000002a0: 696f 6e50 726f 7665 6e61 6e63 65da 1049  ionProvenance..I
-000002b0: 6e76 6f63 6174 696f 6e52 6563 6f72 64da  nvocationRecord.
-000002c0: 1049 6e76 6f63 6174 696f 6e53 6f75 7263  .InvocationSourc
-000002d0: 65da 1049 6e76 6f63 6174 696f 6e53 7461  e..InvocationSta
-000002e0: 7475 73da 1649 6e76 6f63 6174 696f 6e53  tus..InvocationS
-000002f0: 7461 7475 7352 6563 6f72 6429 1872 0200  tatusRecord).r..
-00000300: 0000 7203 0000 0072 0600 0000 720a 0000  ..r....r....r...
-00000310: 0072 0b00 0000 7204 0000 0072 0700 0000  .r....r....r....
-00000320: 7208 0000 0072 1000 0000 720d 0000 0072  r....r....r....r
-00000330: 1300 0000 7214 0000 0072 0e00 0000 720c  ....r....r....r.
-00000340: 0000 0072 0f00 0000 7215 0000 0072 1600  ...r....r....r..
-00000350: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000360: 0072 1100 0000 7209 0000 0072 0500 0000  .r....r....r....
-00000370: 7212 0000 004e 2924 da06 6163 7469 6f6e  r....N)$..action
-00000380: 7202 0000 005a 0f61 6374 696f 6e5f 6465  r....Z.action_de
-00000390: 6c65 6761 7465 7203 0000 0072 0400 0000  legater....r....
-000003a0: 7205 0000 005a 1461 6374 696f 6e5f 6874  r....Z.action_ht
-000003b0: 7470 5f64 656c 6567 6174 6572 0600 0000  tp_delegater....
-000003c0: 5a15 6163 7469 6f6e 5f68 7474 705f 7265  Z.action_http_re
-000003d0: 736f 7572 6365 7372 0700 0000 7208 0000  sourcesr....r...
-000003e0: 0072 0900 0000 5a0d 6163 7469 6f6e 5f72  .r....Z.action_r
-000003f0: 6563 6f72 6472 0a00 0000 da05 6572 726f  ecordr......erro
-00000400: 7272 0b00 0000 720c 0000 005a 0a69 6e76  rr....r....Z.inv
-00000410: 6f63 6174 696f 6e72 0d00 0000 5a13 696e  ocationr....Z.in
-00000420: 766f 6361 7469 6f6e 5f64 656c 6567 6174  vocation_delegat
-00000430: 6572 0e00 0000 5a18 696e 766f 6361 7469  er....Z.invocati
-00000440: 6f6e 5f68 7474 705f 6465 6c65 6761 7465  on_http_delegate
-00000450: 720f 0000 005a 1969 6e76 6f63 6174 696f  r....Z.invocatio
-00000460: 6e5f 6874 7470 5f72 6573 6f75 7263 6573  n_http_resources
-00000470: 7210 0000 0072 1100 0000 7212 0000 005a  r....r....r....Z
-00000480: 1169 6e76 6f63 6174 696f 6e5f 7265 636f  .invocation_reco
-00000490: 7264 7213 0000 0072 1400 0000 7215 0000  rdr....r....r...
-000004a0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000004b0: 7219 0000 00da 075f 5f61 6c6c 5f5f a900  r......__all__..
-000004c0: 721d 0000 0072 1d00 0000 faef 2f63 6f64  r....r....../cod
-000004d0: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000004e0: 6333 3439 3732 3638 3637 302f 7372 632f  c3497268670/src/
-000004f0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
-00000500: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
-00000510: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
-00000520: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
-00000530: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
-00000540: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
-00000550: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
-00000560: 642f 726f 626f 746f 2d61 692f 726f 626f  d/roboto-ai/robo
-00000570: 746f 2d68 6f73 7465 642d 6170 702f 7061  to-hosted-app/pa
-00000580: 636b 6167 6573 2f72 6f62 6f74 6f5f 7364  ckages/roboto_sd
-00000590: 6b2f 7372 632f 726f 626f 746f 5f73 646b  k/src/roboto_sdk
-000005a0: 2f64 6f6d 6169 6e2f 6163 7469 6f6e 732f  /domain/actions/
-000005b0: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
-000005c0: 6475 6c65 3e01 0000 0073 1800 0000 0c01  dule>....s......
-000005d0: 1401 0c05 1403 0c05 1001 0c04 0c01 0c03  ................
-000005e0: 1403 2405 080a                           ..$...
+00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
+00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
+00000080: 6d10 5a10 0100 6400 6406 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+00000090: 0100 6400 6407 6c13 6d14 5a14 6d15 5a15  ..d.d.l.m.Z.m.Z.
+000000a0: 0100 6400 6408 6c16 6d17 5a17 0100 6400  ..d.d.l.m.Z...d.
+000000b0: 6409 6c18 6d19 5a19 0100 6400 640a 6c1a  d.l.m.Z...d.d.l.
+000000c0: 6d1b 5a1b 0100 6400 640b 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
+000000d0: 6d1e 5a1e 6d1f 5a1f 0100 6400 640c 6c20  m.Z.m.Z...d.d.l 
+000000e0: 6d21 5a21 6d22 5a22 6d23 5a23 6d24 5a24  m!Z!m"Z"m#Z#m$Z$
+000000f0: 6d25 5a25 6d26 5a26 6d27 5a27 0100 640d  m%Z%m&Z&m'Z'..d.
+00000100: 5a28 640e 5300 290f e901 0000 0029 01da  Z(d.S.)......)..
+00000110: 0641 6374 696f 6e29 05da 1343 6f6d 7075  .Action)...Compu
+00000120: 7465 5265 7175 6972 656d 656e 7473 da14  teRequirements..
+00000130: 436f 6e74 6169 6e65 7243 7265 6465 6e74  ContainerCredent
+00000140: 6961 6c73 da13 436f 6e74 6169 6e65 7250  ials..ContainerP
+00000150: 6172 616d 6574 6572 73da 1152 6570 6f73  arameters..Repos
+00000160: 6974 6f72 7950 7572 706f 7365 da0d 5265  itoryPurpose..Re
+00000170: 706f 7369 746f 7279 5461 6729 02da 0e41  positoryTag)...A
+00000180: 6374 696f 6e44 656c 6567 6174 65da 0f55  ctionDelegate..U
+00000190: 7064 6174 6543 6f6e 6469 7469 6f6e 2901  pdateCondition).
+000001a0: da12 4163 7469 6f6e 4874 7470 4465 6c65  ..ActionHttpDele
+000001b0: 6761 7465 2903 da1a 436f 6e74 6169 6e65  gate)...Containe
+000001c0: 7255 706c 6f61 6443 7265 6465 6e74 6961  rUploadCredentia
+000001d0: 6c73 da13 4372 6561 7465 4163 7469 6f6e  ls..CreateAction
+000001e0: 5265 7175 6573 74da 1355 7064 6174 6541  Request..UpdateA
+000001f0: 6374 696f 6e52 6571 7565 7374 2901 da0c  ctionRequest)...
+00000200: 4163 7469 6f6e 5265 636f 7264 2902 da21  ActionRecord)..!
+00000210: 4163 7469 6f6e 5570 6461 7465 436f 6e64  ActionUpdateCond
+00000220: 6974 696f 6e43 6865 636b 4661 696c 7572  itionCheckFailur
+00000230: 65da 0f49 6e76 6f63 6174 696f 6e45 7272  e..InvocationErr
+00000240: 6f72 2901 da0a 496e 766f 6361 7469 6f6e  or)...Invocation
+00000250: 2901 da12 496e 766f 6361 7469 6f6e 4465  )...InvocationDe
+00000260: 6c65 6761 7465 2901 da16 496e 766f 6361  legate)...Invoca
+00000270: 7469 6f6e 4874 7470 4465 6c65 6761 7465  tionHttpDelegate
+00000280: 2903 da17 4372 6561 7465 496e 766f 6361  )...CreateInvoca
+00000290: 7469 6f6e 5265 7175 6573 74da 1653 6574  tionRequest..Set
+000002a0: 4c6f 6773 4c6f 6361 7469 6f6e 5265 7175  LogsLocationRequ
+000002b0: 6573 74da 1655 7064 6174 6549 6e76 6f63  est..UpdateInvoc
+000002c0: 6174 696f 6e53 7461 7475 7329 07da 1449  ationStatus)...I
+000002d0: 6e76 6f63 6174 696f 6e44 6174 6153 6f75  nvocationDataSou
+000002e0: 7263 65da 1849 6e76 6f63 6174 696f 6e44  rce..InvocationD
+000002f0: 6174 6153 6f75 7263 6554 7970 65da 1449  ataSourceType..I
+00000300: 6e76 6f63 6174 696f 6e50 726f 7665 6e61  nvocationProvena
+00000310: 6e63 65da 1049 6e76 6f63 6174 696f 6e52  nce..InvocationR
+00000320: 6563 6f72 64da 1049 6e76 6f63 6174 696f  ecord..Invocatio
+00000330: 6e53 6f75 7263 65da 1049 6e76 6f63 6174  nSource..Invocat
+00000340: 696f 6e53 7461 7475 73da 1649 6e76 6f63  ionStatus..Invoc
+00000350: 6174 696f 6e53 7461 7475 7352 6563 6f72  ationStatusRecor
+00000360: 6429 1c72 0200 0000 7208 0000 0072 0a00  d).r....r....r..
+00000370: 0000 720e 0000 0072 0f00 0000 7204 0000  ..r....r....r...
+00000380: 0072 0b00 0000 7203 0000 0072 0500 0000  .r....r....r....
+00000390: 720c 0000 0072 1400 0000 7211 0000 0072  r....r....r....r
+000003a0: 1700 0000 7218 0000 0072 1200 0000 7210  ....r....r....r.
+000003b0: 0000 0072 1300 0000 7219 0000 0072 1a00  ...r....r....r..
+000003c0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000003d0: 0072 0600 0000 7207 0000 0072 1500 0000  .r....r....r....
+000003e0: 720d 0000 0072 0900 0000 7216 0000 004e  r....r....r....N
+000003f0: 2929 da06 6163 7469 6f6e 7202 0000 005a  ))..actionr....Z
+00000400: 1a61 6374 696f 6e5f 636f 6e74 6169 6e65  .action_containe
+00000410: 725f 7265 736f 7572 6365 7372 0300 0000  r_resourcesr....
+00000420: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00000430: 0700 0000 5a0f 6163 7469 6f6e 5f64 656c  ....Z.action_del
+00000440: 6567 6174 6572 0800 0000 7209 0000 005a  egater....r....Z
+00000450: 1461 6374 696f 6e5f 6874 7470 5f64 656c  .action_http_del
+00000460: 6567 6174 6572 0a00 0000 5a15 6163 7469  egater....Z.acti
+00000470: 6f6e 5f68 7474 705f 7265 736f 7572 6365  on_http_resource
+00000480: 7372 0b00 0000 720c 0000 0072 0d00 0000  sr....r....r....
+00000490: 5a0d 6163 7469 6f6e 5f72 6563 6f72 6472  Z.action_recordr
+000004a0: 0e00 0000 da05 6572 726f 7272 0f00 0000  ......errorr....
+000004b0: 7210 0000 005a 0a69 6e76 6f63 6174 696f  r....Z.invocatio
+000004c0: 6e72 1100 0000 5a13 696e 766f 6361 7469  nr....Z.invocati
+000004d0: 6f6e 5f64 656c 6567 6174 6572 1200 0000  on_delegater....
+000004e0: 5a18 696e 766f 6361 7469 6f6e 5f68 7474  Z.invocation_htt
+000004f0: 705f 6465 6c65 6761 7465 7213 0000 005a  p_delegater....Z
+00000500: 1969 6e76 6f63 6174 696f 6e5f 6874 7470  .invocation_http
+00000510: 5f72 6573 6f75 7263 6573 7214 0000 0072  _resourcesr....r
+00000520: 1500 0000 7216 0000 005a 1169 6e76 6f63  ....r....Z.invoc
+00000530: 6174 696f 6e5f 7265 636f 7264 7217 0000  ation_recordr...
+00000540: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000550: 721b 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+00000560: 075f 5f61 6c6c 5f5f a900 7221 0000 0072  .__all__..r!...r
+00000570: 2100 0000 faef 2f63 6f64 6562 7569 6c64  !...../codebuild
+00000580: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
+00000590: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+000005a0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
+000005b0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
+000005c0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
+000005d0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
+000005e0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
+000005f0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
+00000600: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
+00000610: 746f 2d61 692f 726f 626f 746f 2d68 6f73  to-ai/roboto-hos
+00000620: 7465 642d 6170 702f 7061 636b 6167 6573  ted-app/packages
+00000630: 2f72 6f62 6f74 6f5f 7364 6b2f 7372 632f  /roboto_sdk/src/
+00000640: 726f 626f 746f 5f73 646b 2f64 6f6d 6169  roboto_sdk/domai
+00000650: 6e2f 6163 7469 6f6e 732f 5f5f 696e 6974  n/actions/__init
+00000660: 5f5f 2e70 79da 083c 6d6f 6475 6c65 3e01  __.py..<module>.
+00000670: 0000 0073 1a00 0000 0c01 1c01 1007 0c04  ...s............
+00000680: 1403 0c05 1001 0c04 0c01 0c03 1403 2405  ..............$.
+00000690: 080a                                     ..
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 7427 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,403 +1,452 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 031d 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 e821 0000  o.......1..d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 6405 6406 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
-00000060: 6d0a 5a0a 0100 6405 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000070: 0100 6405 6408 6c0d 6d0e 5a0e 0100 6405  ..d.d.l.m.Z...d.
-00000080: 6409 6c0f 6d10 5a10 0100 6405 640a 6c11  d.l.m.Z...d.d.l.
-00000090: 6d12 5a12 0100 6405 640b 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-000000a0: 6d15 5a15 0100 4700 640c 640d 8400 640d  m.Z...G.d.d...d.
-000000b0: 8302 5a16 6401 5300 290e e900 0000 004e  ..Z.d.S.)......N
-000000c0: 2902 da03 416e 79da 084f 7074 696f 6e61  )...Any..Optiona
-000000d0: 6ce9 0300 0000 2901 da16 7079 6461 6e74  l.....)...pydant
-000000e0: 6963 5f6a 736f 6e61 626c 655f 6469 6374  ic_jsonable_dict
-000000f0: e901 0000 0029 03da 0e41 6374 696f 6e44  .....)...ActionD
-00000100: 656c 6567 6174 65da 1443 6f6e 7461 696e  elegate..Contain
-00000110: 6572 4372 6564 656e 7469 616c 73da 0f55  erCredentials..U
-00000120: 7064 6174 6543 6f6e 6469 7469 6f6e 2901  pdateCondition).
-00000130: da0c 4163 7469 6f6e 5265 636f 7264 2901  ..ActionRecord).
-00000140: da0f 496e 766f 6361 7469 6f6e 4572 726f  ..InvocationErro
-00000150: 7229 01da 0a49 6e76 6f63 6174 696f 6e29  r)...Invocation)
-00000160: 01da 1249 6e76 6f63 6174 696f 6e44 656c  ...InvocationDel
-00000170: 6567 6174 6529 02da 1849 6e76 6f63 6174  egate)...Invocat
-00000180: 696f 6e44 6174 6153 6f75 7263 6554 7970  ionDataSourceTyp
-00000190: 65da 1049 6e76 6f63 6174 696f 6e53 6f75  e..InvocationSou
-000001a0: 7263 6563 0000 0000 0000 0000 0000 0000  rcec............
-000001b0: 0000 0000 1400 0000 4000 0000 7316 0200  ........@...s...
-000001c0: 0065 005a 0164 005a 0255 0068 0064 01a3  .e.Z.d.Z.U.h.d..
-000001d0: 015a 0365 0465 0564 023c 0065 0665 0564  .Z.e.e.d.<.e.e.d
-000001e0: 033c 0065 0765 0564 043c 0064 055a 0865  .<.e.e.d.<.d.Z.e
-000001f0: 0965 0a19 0065 0564 063c 0065 0b09 0509  .e...e.d.<.e....
-00000200: 0509 0509 0509 0564 3664 0765 0c64 0865  .......d6d.e.d.e
-00000210: 0464 0965 0664 0a65 0965 0c19 0064 0b65  .d.e.d.e.e...d.e
-00000220: 0965 0c19 0064 0c65 0965 0d65 0c65 0e66  .e...d.e.e.e.e.f
-00000230: 0219 0019 0064 0d65 0965 0f65 0c19 0019  .....d.e.e.e....
-00000240: 0064 0e65 0965 0c19 0064 0f64 0066 1264  .d.e.e...d.d.f.d
-00000250: 1064 1184 0583 015a 1065 0b09 0564 3764  .d.....Z.e...d7d
-00000260: 0765 0c64 0865 0464 0965 0664 0a65 0965  .e.d.e.d.e.d.e.e
-00000270: 0c19 0064 0f64 0066 0a64 1264 1384 0583  ...d.d.f.d.d....
-00000280: 015a 1165 0b09 0564 3764 1465 0d65 0c65  .Z.e...d7d.e.e.e
-00000290: 0e66 0219 0064 0865 0464 0965 0664 0a65  .f...d.e.d.e.d.e
-000002a0: 0965 0c19 0064 0f65 126a 136a 1464 1519  .e...d.e.j.j.d..
-000002b0: 0066 0a64 1664 1784 0583 015a 1564 1865  .f.d.d.....Z.d.e
-000002c0: 0764 0865 0464 0965 0664 0f64 0566 0864  .d.e.d.e.d.d.f.d
-000002d0: 1964 1a84 045a 1665 1764 0f65 0c66 0264  .d...Z.e.d.e.f.d
-000002e0: 1b64 1c84 0483 015a 1865 1764 0f65 0c66  .d.....Z.e.d.e.f
-000002f0: 0264 1d64 1e84 0483 015a 1965 1764 0f65  .d.d.....Z.e.d.e
-00000300: 0965 0c19 0066 0264 1f64 2084 0483 015a  .e...f.d.d ....Z
-00000310: 1a09 0564 3764 2165 0965 0c19 0064 0f65  ...d7d!e.e...d.e
-00000320: 0a66 0464 2264 2384 055a 1b64 2465 0f65  .f.d"d#..Z.d$e.e
-00000330: 0c19 0064 2565 0c64 2665 1c64 2765 1d64  ...d%e.d&e.d'e.d
-00000340: 2865 0965 0c19 0064 0f65 1e66 0c64 2964  (e.e...d.e.f.d)d
-00000350: 2a84 045a 1f09 0564 3764 2b65 0c64 2c65  *..Z...d7d+e.d,e
-00000360: 0c64 2165 0965 0c19 0064 0f65 2065 0c65  .d!e.e...d.e e.e
-00000370: 0c66 0219 0066 0864 2d64 2e84 055a 2164  .f...f.d-d...Z!d
-00000380: 0f65 0d65 0c65 0e66 0219 0066 0264 2f64  .e.e.e.f...f.d/d
-00000390: 3084 045a 2209 0509 0509 0564 3864 3165  0..Z"......d8d1e
-000003a0: 0d65 0c65 0e66 0219 0064 3265 0965 0f65  .e.e.f...d2e.e.e
-000003b0: 2319 0019 0064 0a65 0965 0c19 0064 3365  #....d.e.e...d3e
-000003c0: 0965 0c19 0064 0f64 0566 0a64 3464 3584  .e...d.d.f.d4d5.
-000003d0: 055a 2464 0553 0029 39da 0641 6374 696f  .Z$d.S.)9..Actio
-000003e0: 6e3e 0700 0000 da08 6d6f 6469 6669 6564  n>......modified
-000003f0: da04 6e61 6d65 da0a 6372 6561 7465 645f  ..name..created_
-00000400: 6279 da06 6f72 675f 6964 da03 7572 695a  by..org_id..uriZ
-00000410: 0a63 7265 6174 6564 5f61 745a 0b6d 6f64  .created_atZ.mod
-00000420: 6966 6965 645f 6279 da18 5f41 6374 696f  ified_by.._Actio
-00000430: 6e5f 5f61 6374 696f 6e5f 6465 6c65 6761  n__action_delega
-00000440: 7465 da1c 5f41 6374 696f 6e5f 5f69 6e76  te.._Action__inv
-00000450: 6f63 6174 696f 6e5f 6465 6c65 6761 7465  ocation_delegate
-00000460: da0f 5f41 6374 696f 6e5f 5f72 6563 6f72  .._Action__recor
-00000470: 644e da23 5f41 6374 696f 6e5f 5f74 656d  dN.#_Action__tem
-00000480: 705f 636f 6e74 6169 6e65 725f 6372 6564  p_container_cred
-00000490: 656e 7469 616c 7372 1200 0000 da0f 6163  entialsr......ac
-000004a0: 7469 6f6e 5f64 656c 6567 6174 65da 1369  tion_delegate..i
-000004b0: 6e76 6f63 6174 696f 6e5f 6465 6c65 6761  nvocation_delega
-000004c0: 7465 7214 0000 00da 0b64 6573 6372 6970  ter......descrip
-000004d0: 7469 6f6e da08 6d65 7461 6461 7461 da04  tion..metadata..
-000004e0: 7461 6773 7213 0000 00da 0672 6574 7572  tagsr......retur
-000004f0: 6e63 0900 0000 0000 0000 0000 0000 0a00  nc..............
-00000500: 0000 0800 0000 4300 0000 7320 0000 007c  ......C...s ...|
-00000510: 02a0 007c 017c 047c 087c 057c 067c 07a1  ...|.|.|.|.|.|..
-00000520: 067d 097c 007c 097c 027c 0383 0353 00a9  .}.|.|.|.|...S..
-00000530: 014e 2901 5a0d 6372 6561 7465 5f61 6374  .N).Z.create_act
-00000540: 696f 6e29 0ada 0363 6c73 7212 0000 0072  ion)...clsr....r
-00000550: 1a00 0000 721b 0000 0072 1400 0000 721c  ....r....r....r.
-00000560: 0000 0072 1d00 0000 721e 0000 0072 1300  ...r....r....r..
-00000570: 0000 da06 7265 636f 7264 a900 7223 0000  ....record..r#..
-00000580: 00fa ed2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000590: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
-000005a0: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
-000005b0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
-000005c0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
-000005d0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
-000005e0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
-000005f0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
-00000600: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
-00000610: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
-00000620: 6169 2f72 6f62 6f74 6f2d 686f 7374 6564  ai/roboto-hosted
-00000630: 2d61 7070 2f70 6163 6b61 6765 732f 726f  -app/packages/ro
-00000640: 626f 746f 5f73 646b 2f73 7263 2f72 6f62  boto_sdk/src/rob
-00000650: 6f74 6f5f 7364 6b2f 646f 6d61 696e 2f61  oto_sdk/domain/a
-00000660: 6374 696f 6e73 2f61 6374 696f 6e2e 7079  ctions/action.py
-00000670: da06 6372 6561 7465 2600 0000 7312 0000  ..create&...s...
-00000680: 0004 0c02 0102 0102 0102 0102 0102 0104  ................
-00000690: fa0c 087a 0d41 6374 696f 6e2e 6372 6561  ...z.Action.crea
-000006a0: 7465 6305 0000 0000 0000 0000 0000 0006  tec.............
-000006b0: 0000 0004 0000 0043 0000 0073 1800 0000  .......C...s....
-000006c0: 7c02 a000 7c01 7c04 a102 7d05 7c00 7c05  |...|.|...}.|.|.
-000006d0: 7c02 7c03 8303 5300 7220 0000 0029 015a  |.|...S.r ...).Z
-000006e0: 1967 6574 5f61 6374 696f 6e5f 6279 5f70  .get_action_by_p
-000006f0: 7269 6d61 7279 5f6b 6579 2906 7221 0000  rimary_key).r!..
-00000700: 0072 1200 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000710: 7214 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
-00000720: 2300 0000 7224 0000 00da 0966 726f 6d5f  #...r$.....from_
-00000730: 6e61 6d65 3c00 0000 7304 0000 000c 080c  name<...s.......
-00000740: 017a 1041 6374 696f 6e2e 6672 6f6d 5f6e  .z.Action.from_n
-00000750: 616d 65da 0766 696c 7465 7273 2903 7210  ame..filters).r.
-00000760: 0000 004e 4e63 0500 0000 0000 0000 0000  ...NNc..........
-00000770: 0000 0c00 0000 0600 0000 6300 0000 73a2  ..........c...s.
-00000780: 0000 0081 0074 0074 016a 02a0 03a1 0083  .....t.t.j......
-00000790: 017d 0574 007c 01a0 03a1 0083 017d 067c  .}.t.|.......}.|
-000007a0: 067c 0518 007d 077c 0772 2c74 047c 0783  .|...}.|.r,t.|..
-000007b0: 0164 016b 047d 087c 0872 1e64 026e 0164  .d.k.}.|.r.d.n.d
-000007c0: 037d 0974 057c 079b 0064 047c 099b 0064  .}.t.|...d.|...d
-000007d0: 057c 059b 009d 0583 0182 017c 026a 067c  .|.........|.j.|
-000007e0: 017c 0464 068d 027d 0a09 007c 0a6a 0744  .|.d...}...|.j.D
-000007f0: 005d 097d 0b7c 007c 0b7c 027c 0383 0356  .].}.|.|.|.|...V
-00000800: 0001 0071 377c 0a6a 0872 4e7c 026a 067c  ...q7|.j.rN|.j.|
-00000810: 017c 047c 0a6a 0864 088d 037d 0a6e 0264  .|.|.j.d...}.n.d
-00000820: 0053 0071 3429 094e 7206 0000 007a 2261  .S.q4).Nr....z"a
-00000830: 7265 206e 6f74 206b 6e6f 776e 2061 7474  re not known att
-00000840: 7269 6275 7465 7320 6f66 2041 6374 696f  ributes of Actio
-00000850: 6e7a 2269 7320 6e6f 7420 6120 6b6e 6f77  nz"is not a know
-00000860: 6e20 6174 7472 6962 7574 6520 6f66 2041  n attribute of A
-00000870: 6374 696f 6eda 0120 7a14 2e20 4b6e 6f77  ction.. z.. Know
-00000880: 6e20 6174 7472 6962 7574 6573 3a20 2901  n attributes: ).
-00000890: 7214 0000 0054 2902 7214 0000 005a 0a70  r....T).r....Z.p
-000008a0: 6167 655f 746f 6b65 6e29 09da 0373 6574  age_token)...set
-000008b0: 720a 0000 00da 0a5f 5f66 6965 6c64 735f  r......__fields_
-000008c0: 5fda 046b 6579 73da 036c 656e da0a 5661  _..keys..len..Va
-000008d0: 6c75 6545 7272 6f72 5a0d 7175 6572 795f  lueErrorZ.query_
-000008e0: 6163 7469 6f6e 73da 0569 7465 6d73 da0a  actions..items..
-000008f0: 6e65 7874 5f74 6f6b 656e 290c 7221 0000  next_token).r!..
-00000900: 0072 2700 0000 721a 0000 0072 1b00 0000  .r'...r....r....
-00000910: 7214 0000 00da 0a6b 6e6f 776e 5f6b 6579  r......known_key
-00000920: 735a 0b61 6374 7561 6c5f 6b65 7973 5a0c  sZ.actual_keysZ.
-00000930: 756e 6b6e 6f77 6e5f 6b65 7973 da06 706c  unknown_keys..pl
-00000940: 7572 616c da03 6d73 675a 1170 6167 696e  ural..msgZ.pagin
-00000950: 6174 6564 5f72 6573 756c 7473 7222 0000  ated_resultsr"..
-00000960: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00000970: da05 7175 6572 7947 0000 0073 2a00 0000  ..queryG...s*...
-00000980: 0280 0e08 0c01 0801 0401 0c01 0203 06ff  ................
-00000990: 0202 02fd 1805 0e02 0201 0a01 1001 0601  ................
-000009a0: 0401 0801 08ff 0404 02f8 7a0c 4163 7469  ..........z.Acti
-000009b0: 6f6e 2e71 7565 7279 7222 0000 0063 0400  on.queryr"...c..
-000009c0: 0000 0000 0000 0000 0000 0400 0000 0200  ................
-000009d0: 0000 4300 0000 7316 0000 007c 027c 005f  ..C...s....|.|._
-000009e0: 007c 037c 005f 017c 017c 005f 0264 0053  .|.|._.|.|._.d.S
-000009f0: 0072 2000 0000 2903 7216 0000 0072 1700  .r ...).r....r..
-00000a00: 0000 7218 0000 0029 04da 0473 656c 6672  ..r....)...selfr
-00000a10: 2200 0000 721a 0000 0072 1b00 0000 7223  "...r....r....r#
-00000a20: 0000 0072 2300 0000 7224 0000 00da 085f  ...r#...r$....._
-00000a30: 5f69 6e69 745f 5f66 0000 0073 0600 0000  _init__f...s....
-00000a40: 0606 0601 0a01 7a0f 4163 7469 6f6e 2e5f  ......z.Action._
-00000a50: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000a60: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000a70: f308 0000 007c 006a 006a 0153 0072 2000  .....|.j.j.S.r .
-00000a80: 0000 2902 7218 0000 0072 1200 0000 a901  ..).r....r......
-00000a90: 7234 0000 0072 2300 0000 7223 0000 0072  r4...r#...r#...r
-00000aa0: 2400 0000 7212 0000 0070 0000 00f3 0200  $...r....p......
-00000ab0: 0000 0802 7a0b 4163 7469 6f6e 2e6e 616d  ....z.Action.nam
-00000ac0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000ad0: 0000 0100 0000 4300 0000 7236 0000 0072  ......C...r6...r
-00000ae0: 2000 0000 2902 7218 0000 0072 1400 0000   ...).r....r....
-00000af0: 7237 0000 0072 2300 0000 7223 0000 0072  r7...r#...r#...r
-00000b00: 2400 0000 7214 0000 0074 0000 0072 3800  $...r....t...r8.
-00000b10: 0000 7a0d 4163 7469 6f6e 2e6f 7267 5f69  ..z.Action.org_i
-00000b20: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-00000b30: 0000 0100 0000 4300 0000 7236 0000 0072  ......C...r6...r
-00000b40: 2000 0000 2902 7218 0000 0072 1500 0000   ...).r....r....
-00000b50: 7237 0000 0072 2300 0000 7223 0000 0072  r7...r#...r#...r
-00000b60: 2400 0000 7215 0000 0078 0000 0072 3800  $...r....x...r8.
-00000b70: 0000 7a0a 4163 7469 6f6e 2e75 7269 da06  ..z.Action.uri..
-00000b80: 6361 6c6c 6572 6302 0000 0000 0000 0000  callerc.........
-00000b90: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000ba0: 3000 0000 7c00 6a00 6400 7500 730a 7c00  0...|.j.d.u.s.|.
-00000bb0: 6a00 a001 a100 7215 7c00 6a02 a003 7c00  j.....r.|.j...|.
-00000bc0: 6a04 7c01 a102 7d02 7c02 7c00 5f00 7c00  j.|...}.|.|._.|.
-00000bd0: 6a00 5300 7220 0000 0029 0572 1900 0000  j.S.r ...).r....
-00000be0: da0a 6973 5f65 7870 6972 6564 7216 0000  ..is_expiredr...
-00000bf0: 005a 1e67 6574 5f74 656d 705f 636f 6e74  .Z.get_temp_cont
-00000c00: 6169 6e65 725f 6372 6564 656e 7469 616c  ainer_credential
-00000c10: 7372 1800 0000 2903 7234 0000 0072 3900  sr....).r4...r9.
-00000c20: 0000 da05 6372 6564 7372 2300 0000 7223  ....credsr#...r#
-00000c30: 0000 0072 2400 0000 da23 6765 745f 7465  ...r$....#get_te
-00000c40: 6d70 6f72 6172 795f 636f 6e74 6169 6e65  mporary_containe
-00000c50: 725f 6372 6564 656e 7469 616c 737c 0000  r_credentials|..
-00000c60: 0073 1000 0000 0a04 0801 02ff 0603 0601  .s..............
-00000c70: 04ff 0603 0602 7a2a 4163 7469 6f6e 2e67  ......z*Action.g
-00000c80: 6574 5f74 656d 706f 7261 7279 5f63 6f6e  et_temporary_con
-00000c90: 7461 696e 6572 5f63 7265 6465 6e74 6961  tainer_credentia
-00000ca0: 6c73 da0a 696e 7075 745f 6461 7461 da0e  ls..input_data..
-00000cb0: 6461 7461 5f73 6f75 7263 655f 6964 da10  data_source_id..
-00000cc0: 6461 7461 5f73 6f75 7263 655f 7479 7065  data_source_type
-00000cd0: da11 696e 766f 6361 7469 6f6e 5f73 6f75  ..invocation_sou
-00000ce0: 7263 65da 1469 6e76 6f63 6174 696f 6e5f  rce..invocation_
-00000cf0: 736f 7572 6365 5f69 6463 0600 0000 0000  source_idc......
-00000d00: 0000 0000 0000 0700 0000 0900 0000 4300  ..............C.
-00000d10: 0000 7340 0000 007c 006a 006a 0164 0175  ..s@...|.j.j.d.u
-00000d20: 0172 0a74 0264 0283 0182 017c 006a 03a0  .r.t.d.....|.j..
-00000d30: 047c 006a 006a 057c 017c 027c 037c 047c  .|.j.j.|.|.|.|.|
-00000d40: 057c 006a 006a 06a1 077d 0674 077c 067c  .|.j.j...}.t.|.|
-00000d50: 006a 0383 0253 0029 034e 547a 5941 2063  .j...S.).NTzYA c
-00000d60: 6f6e 7461 696e 6572 2069 6d61 6765 206d  ontainer image m
-00000d70: 7573 7420 6265 2061 7373 6f63 6961 7465  ust be associate
-00000d80: 6420 7769 7468 2074 6869 7320 4163 7469  d with this Acti
-00000d90: 6f6e 2061 6e64 2070 7573 6865 6420 6265  on and pushed be
-00000da0: 666f 7265 2069 7420 6361 6e20 6265 2069  fore it can be i
-00000db0: 6e76 6f6b 6564 2908 7218 0000 005a 0c69  nvoked).r....Z.i
-00000dc0: 735f 6176 6169 6c61 626c 6572 0b00 0000  s_availabler....
-00000dd0: 7217 0000 005a 1163 7265 6174 655f 696e  r....Z.create_in
-00000de0: 766f 6361 7469 6f6e 7212 0000 0072 1400  vocationr....r..
-00000df0: 0000 720c 0000 0029 0772 3400 0000 723d  ..r....).r4...r=
-00000e00: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
-00000e10: 0000 7241 0000 0072 2200 0000 7223 0000  ..rA...r"...r#..
-00000e20: 0072 2300 0000 7224 0000 00da 0669 6e76  .r#...r$.....inv
-00000e30: 6f6b 658a 0000 0073 2200 0000 0c08 0201  oke....s".......
-00000e40: 0201 04ff 0604 0601 0201 0201 0201 0201  ................
-00000e50: 0201 0601 04f9 0209 0201 0401 04fe 7a0d  ..............z.
-00000e60: 4163 7469 6f6e 2e69 6e76 6f6b 65da 0a69  Action.invoke..i
-00000e70: 6d61 6765 5f6e 616d 65da 0969 6d61 6765  mage_name..image
-00000e80: 5f74 6167 6304 0000 0000 0000 0000 0000  _tagc...........
-00000e90: 0004 0000 0006 0000 0043 0000 0073 1400  .........C...s..
-00000ea0: 0000 7c00 6a00 a001 7c00 6a02 7c01 7c02  ..|.j...|.j.|.|.
-00000eb0: 7c03 a104 5300 2901 617b 0400 000a 2020  |...S.).a{....  
-00000ec0: 2020 2020 2020 4964 656d 706f 7465 6e74        Idempotent
-00000ed0: 2067 6574 206f 7220 6372 6561 7465 2063   get or create c
-00000ee0: 6f6e 7461 696e 6572 2072 6570 6f73 6974  ontainer reposit
-00000ef0: 6f72 7920 666f 7220 7468 6973 2041 6374  ory for this Act
-00000f00: 696f 6e2c 2061 6e64 2061 7373 6f63 6961  ion, and associa
-00000f10: 7465 2069 7420 7769 7468 2074 6865 2041  te it with the A
-00000f20: 6374 696f 6e20 6173 2069 7473 2055 5249  ction as its URI
-00000f30: 2e0a 2020 2020 2020 2020 5573 6520 7468  ..        Use th
-00000f40: 6973 2074 6f20 6173 736f 6369 6174 6520  is to associate 
-00000f50: 616e 2041 6374 696f 6e20 7769 7468 2061  an Action with a
-00000f60: 2063 6f6e 7461 696e 6572 2069 6d61 6765   container image
-00000f70: 2074 6861 7420 6861 7320 7965 7420 746f   that has yet to
-00000f80: 2062 6520 7075 7368 6564 2c0a 2020 2020   be pushed,.    
-00000f90: 2020 2020 6f72 2077 6974 6820 6120 636f      or with a co
-00000fa0: 6e74 6169 6e65 7220 696d 6167 6520 7468  ntainer image th
-00000fb0: 6174 2068 6173 2061 6c72 6561 6479 2062  at has already b
-00000fc0: 6565 6e20 7075 7368 6564 2074 6f20 616e  een pushed to an
-00000fd0: 2065 7869 7374 696e 6720 7265 706f 7369   existing reposi
-00000fe0: 746f 7279 2e0a 0a20 2020 2020 2020 2041  tory...        A
-00000ff0: 2063 6f6e 7461 696e 6572 206d 6179 2062   container may b
-00001000: 6520 7075 7368 6564 2074 6f20 7468 6520  e pushed to the 
-00001010: 7265 706f 7369 7374 6f72 7920 7573 696e  reposistory usin
-00001020: 6720 6372 6564 656e 7469 616c 7320 7265  g credentials re
-00001030: 7475 726e 6564 2062 790a 2020 2020 2020  turned by.      
-00001040: 2020 6067 6574 5f74 656d 706f 7261 7279    `get_temporary
-00001050: 5f63 6f6e 7461 696e 6572 5f63 7265 6465  _container_crede
-00001060: 6e74 6961 6c73 602e 0a20 2020 2020 2020  ntials`..       
-00001070: 2049 7473 2074 6167 2064 6f65 7320 6e6f   Its tag does no
-00001080: 7420 6e65 6564 2074 6f20 6571 7561 6c20  t need to equal 
-00001090: 6069 6d61 6765 5f74 6167 602c 2062 7574  `image_tag`, but
-000010a0: 2077 6974 686f 7574 2063 616c 6c69 6e67   without calling
-000010b0: 2074 6869 7320 6d65 7468 6f64 2077 6974   this method wit
-000010c0: 6820 7468 6520 6173 736f 6369 6174 6564  h the associated
-000010d0: 2074 6167 2c0a 2020 2020 2020 2020 7468   tag,.        th
-000010e0: 6520 4163 7469 6f6e 2077 696c 6c20 6e6f  e Action will no
-000010f0: 7420 6265 2061 626c 6520 746f 2069 6e76  t be able to inv
-00001100: 6f6b 6520 7468 6520 7075 7368 6564 2063  oke the pushed c
-00001110: 6f6e 7461 696e 6572 2e0a 0a20 2020 2020  ontainer...     
-00001120: 2020 2053 6964 652d 6566 6665 6374 733a     Side-effects:
-00001130: 0a20 2020 2020 2020 2020 2020 202a 2049  .            * I
-00001140: 6620 6120 636f 6e74 6169 6e65 7220 7265  f a container re
-00001150: 706f 7369 746f 7279 2066 6f72 2067 6976  pository for giv
-00001160: 656e 2060 696d 6167 655f 6e61 6d65 603a  en `image_name`:
-00001170: 6069 6d61 6765 5f74 6167 6020 646f 6573  `image_tag` does
-00001180: 206e 6f74 2065 7869 7374 2c20 6974 2077   not exist, it w
-00001190: 696c 6c20 6265 2063 7265 6174 6564 2e0a  ill be created..
-000011a0: 2020 2020 2020 2020 2020 2020 2a20 4966              * If
-000011b0: 2061 2063 6f6e 7461 696e 6572 2072 6570   a container rep
-000011c0: 6f73 6974 6f72 7920 7761 7320 7072 6576  ository was prev
-000011d0: 696f 7573 6c79 2063 7265 6174 6564 2066  iously created f
-000011e0: 6f72 2074 6869 7320 4163 7469 6f6e 2066  or this Action f
-000011f0: 6f72 2061 2064 6966 6665 7265 6e74 2060  or a different `
-00001200: 696d 6167 655f 6e61 6d65 602c 0a20 2020  image_name`,.   
-00001210: 2020 2020 2020 2020 2020 2041 4e44 2074             AND t
-00001220: 6861 7420 7265 706f 7369 746f 7279 2069  hat repository i
-00001230: 7320 656d 7074 792c 2069 7420 7769 6c6c  s empty, it will
-00001240: 2062 6520 6465 6c65 7465 642e 0a20 2020   be deleted..   
-00001250: 2020 2020 2020 2020 202a 2053 6574 7320           * Sets 
-00001260: 7468 6520 6075 7269 6020 6174 7472 6962  the `uri` attrib
-00001270: 7574 6520 6f66 2074 6869 7320 4163 7469  ute of this Acti
-00001280: 6f6e 2074 6f20 7468 6520 5552 4920 6f66  on to the URI of
-00001290: 2074 6865 2069 6d61 6765 2065 7870 6563   the image expec
-000012a0: 7465 6420 746f 2062 6520 7075 7368 6564  ted to be pushed
-000012b0: 2074 6f20 7468 6520 7265 706f 7369 746f   to the reposito
-000012c0: 7279 2e0a 0a20 2020 2020 2020 2060 6361  ry...        `ca
-000012d0: 6c6c 6572 6020 6973 2069 676e 6f72 6564  ller` is ignored
-000012e0: 206f 6e20 7468 6520 636c 6965 6e74 2e20   on the client. 
-000012f0: 4974 2069 7320 6465 7465 726d 696e 6564  It is determined
-00001300: 2073 6572 7665 722d 7369 6465 2076 6961   server-side via
-00001310: 2074 6865 2069 6465 6e74 6974 792f 6163   the identity/ac
-00001320: 6365 7373 206d 6563 6861 6e69 736d 2e0a  cess mechanism..
-00001330: 2020 2020 2020 2020 2903 7216 0000 00da          ).r.....
-00001340: 1272 6567 6973 7465 725f 636f 6e74 6169  .register_contai
-00001350: 6e65 7272 1800 0000 2904 7234 0000 0072  nerr....).r4...r
-00001360: 4300 0000 7244 0000 0072 3900 0000 7223  C...rD...r9...r#
-00001370: 0000 0072 2300 0000 7224 0000 0072 4500  ...r#...r$...rE.
-00001380: 0000 a500 0000 7306 0000 0006 180a 0104  ......s.........
-00001390: ff7a 1941 6374 696f 6e2e 7265 6769 7374  .z.Action.regist
-000013a0: 6572 5f63 6f6e 7461 696e 6572 6301 0000  er_containerc...
-000013b0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000013c0: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-000013d0: 8301 5300 7220 0000 0029 0272 0500 0000  ..S.r ...).r....
-000013e0: 7218 0000 0072 3700 0000 7223 0000 0072  r....r7...r#...r
-000013f0: 2300 0000 7224 0000 00da 0774 6f5f 6469  #...r$.....to_di
-00001400: 6374 c100 0000 7302 0000 000a 017a 0e41  ct....s......z.A
-00001410: 6374 696f 6e2e 746f 5f64 6963 74da 0775  ction.to_dict..u
-00001420: 7064 6174 6573 da0a 636f 6e64 6974 696f  pdates..conditio
-00001430: 6e73 da0a 7570 6461 7465 645f 6279 6305  ns..updated_byc.
-00001440: 0000 0000 0000 0000 0000 000b 0000 0007  ................
-00001450: 0000 0043 0000 0073 8000 0000 7400 7401  ...C...s....t.t.
-00001460: 6a02 a003 a100 8301 7d05 7c05 7404 6a05  j.......}.|.t.j.
-00001470: 1800 7d06 7400 7c01 a003 a100 8301 7c06  ..}.t.|.......|.
-00001480: 1800 7d07 7406 7c07 8301 7230 7406 7c07  ..}.t.|...r0t.|.
-00001490: 8301 6401 6b04 7d08 7c08 7222 6402 6e01  ..d.k.}.|.r"d.n.
-000014a0: 6403 7d09 7407 7c07 9b00 6404 7c09 9b00  d.}.t.|...d.|...
-000014b0: 6405 7c06 9b00 9d05 8301 8201 7c00 6a08  d.|.........|.j.
-000014c0: a009 7c00 6a0a 7c01 7c02 7c03 7c04 a105  ..|.j.|.|.|.|...
-000014d0: 7d0a 7c0a 7c00 5f0a 6400 5300 2906 4e72  }.|.|._.d.S.).Nr
-000014e0: 0600 0000 7a1d 6172 6520 6e6f 7420 7570  ....z.are not up
-000014f0: 6461 7465 6162 6c65 2061 7474 7269 6275  dateable attribu
-00001500: 7465 737a 1e69 7320 6e6f 7420 616e 2075  tesz.is not an u
-00001510: 7064 6174 6561 626c 6520 6174 7472 6962  pdateable attrib
-00001520: 7574 6572 2800 0000 7a19 2e20 5570 6461  uter(...z.. Upda
-00001530: 7465 6162 6c65 2061 7474 7269 6275 7465  teable attribute
-00001540: 733a 2029 0b72 2900 0000 720a 0000 0072  s: ).r)...r....r
-00001550: 2a00 0000 722b 0000 0072 1000 0000 da15  *...r+...r......
-00001560: 4449 5341 4c4c 4f57 4544 5f46 4f52 5f55  DISALLOWED_FOR_U
-00001570: 5044 4154 4572 2c00 0000 722d 0000 0072  PDATEr,...r-...r
-00001580: 1600 0000 da06 7570 6461 7465 7218 0000  ......updater...
-00001590: 0029 0b72 3400 0000 7247 0000 0072 4800  .).r4...rG...rH.
-000015a0: 0000 7214 0000 0072 4900 0000 7230 0000  ..r....rI...r0..
-000015b0: 00da 0c61 6c6c 6f77 6564 5f6b 6579 735a  ...allowed_keysZ
-000015c0: 0975 6e61 6c6c 6f77 6564 7231 0000 0072  .unallowedr1...r
-000015d0: 3200 0000 da07 7570 6461 7465 6472 2300  2.....updatedr#.
-000015e0: 0000 7223 0000 0072 2400 0000 724b 0000  ..r#...r$...rK..
-000015f0: 00c4 0000 0073 2000 0000 0e07 0a01 1001  .....s .........
-00001600: 0801 0c01 0203 06ff 0202 02fd 0205 1201  ................
-00001610: 04ff 0604 0c01 04ff 0a03 7a0d 4163 7469  ..........z.Acti
-00001620: 6f6e 2e75 7064 6174 6529 054e 4e4e 4e4e  on.update).NNNNN
-00001630: 7220 0000 0029 034e 4e4e 2925 da08 5f5f  r ...).NNN)%..__
-00001640: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00001650: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00001660: 724a 0000 0072 0700 0000 da0f 5f5f 616e  rJ...r......__an
-00001670: 6e6f 7461 7469 6f6e 735f 5f72 0d00 0000  notations__r....
-00001680: 720a 0000 0072 1900 0000 7203 0000 0072  r....r....r....r
-00001690: 0800 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
-000016a0: 64da 0373 7472 da04 6469 6374 7202 0000  d..str..dictr...
-000016b0: 00da 046c 6973 7472 2500 0000 7226 0000  ...listr%...r&..
-000016c0: 00da 0b63 6f6c 6c65 6374 696f 6e73 da03  ...collections..
-000016d0: 6162 63da 0947 656e 6572 6174 6f72 7233  abc..Generatorr3
-000016e0: 0000 0072 3500 0000 da08 7072 6f70 6572  ...r5.....proper
-000016f0: 7479 7212 0000 0072 1400 0000 7215 0000  tyr....r....r...
-00001700: 0072 3c00 0000 720e 0000 0072 0f00 0000  .r<...r....r....
-00001710: 720c 0000 0072 4200 0000 da05 7475 706c  r....rB.....tupl
-00001720: 6572 4500 0000 7246 0000 0072 0900 0000  erE...rF...r....
-00001730: 724b 0000 0072 2300 0000 7223 0000 0072  rK...r#...r#...r
-00001740: 2300 0000 7224 0000 0072 1000 0000 1600  #...r$...r......
-00001750: 0000 73e8 0000 000a 0008 0108 0a08 0108  ..s.............
-00001760: 0110 0102 0202 0602 0102 0102 0102 0104  ................
-00001770: f702 0202 fe02 0302 fd02 0402 fc06 0502  ................
-00001780: fb06 0602 fa0e 0702 f90a 0802 f806 0902  ................
-00001790: f702 0a0c f602 1502 0604 fb02 0202 fe02  ................
-000017a0: 0302 fd02 0402 fc06 0502 fb02 060c fa02  ................
-000017b0: 0a02 0604 fb0a 0202 fe02 0302 fd02 0402  ................
-000017c0: fc06 0502 fb0a 060c fa02 1e02 0202 fe02  ................
-000017d0: 0302 fd02 0402 fc02 050a fb02 0a10 0102  ................
-000017e0: 0310 0102 0314 0102 0404 ff06 0102 ff02  ................
-000017f0: 020a fe02 0e06 0202 fe02 0302 fd02 0402  ................
-00001800: fc02 0502 fb06 0602 fa02 070a f902 1f04  ................
-00001810: fc02 0202 fe02 0302 fd06 0402 fc0a 050a  ................
-00001820: fb16 1c02 0602 0102 0104 fb0a 0202 fe0a  ................
-00001830: 0302 fd06 0402 fc06 0502 fb02 060e fa72  ...............r
-00001840: 1000 0000 2917 da0f 636f 6c6c 6563 7469  ....)...collecti
-00001850: 6f6e 732e 6162 6372 5600 0000 da06 7479  ons.abcrV.....ty
-00001860: 7069 6e67 7202 0000 0072 0300 0000 da05  pingr....r......
-00001870: 7365 7264 6572 0500 0000 721a 0000 0072  serder....r....r
-00001880: 0700 0000 7208 0000 0072 0900 0000 da0d  ....r....r......
-00001890: 6163 7469 6f6e 5f72 6563 6f72 6472 0a00  action_recordr..
-000018a0: 0000 da05 6572 726f 7272 0b00 0000 da0a  ....errorr......
-000018b0: 696e 766f 6361 7469 6f6e 720c 0000 0072  invocationr....r
-000018c0: 1b00 0000 720d 0000 00da 1169 6e76 6f63  ....r......invoc
-000018d0: 6174 696f 6e5f 7265 636f 7264 720e 0000  ation_recordr...
-000018e0: 0072 0f00 0000 7210 0000 0072 2300 0000  .r....r....r#...
-000018f0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00001900: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
-00001910: 0000 0800 1001 0c02 1401 0c05 0c01 0c01  ................
-00001920: 0c01 1003 1206                           ......
+00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6403  d.l.m.Z.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6405 6406 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6405  m.Z.m.Z.m.Z...d.
+00000070: 6407 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405  d.l.m.Z.m.Z...d.
+00000080: 6408 6c0f 6d10 5a10 0100 6405 6409 6c11  d.l.m.Z...d.d.l.
+00000090: 6d12 5a12 0100 6405 640a 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000a0: 0100 6405 640b 6c15 6d16 5a16 6d17 5a17  ..d.d.l.m.Z.m.Z.
+000000b0: 0100 4700 640c 640d 8400 640d 8302 5a18  ..G.d.d...d...Z.
+000000c0: 6401 5300 290e e900 0000 004e 2902 da03  d.S.)......N)...
+000000d0: 416e 79da 084f 7074 696f 6e61 6ce9 0300  Any..Optional...
+000000e0: 0000 2901 da16 7079 6461 6e74 6963 5f6a  ..)...pydantic_j
+000000f0: 736f 6e61 626c 655f 6469 6374 e901 0000  sonable_dict....
+00000100: 0029 03da 1343 6f6d 7075 7465 5265 7175  .)...ComputeRequ
+00000110: 6972 656d 656e 7473 da14 436f 6e74 6169  irements..Contai
+00000120: 6e65 7243 7265 6465 6e74 6961 6c73 da13  nerCredentials..
+00000130: 436f 6e74 6169 6e65 7250 6172 616d 6574  ContainerParamet
+00000140: 6572 7329 02da 0e41 6374 696f 6e44 656c  ers)...ActionDel
+00000150: 6567 6174 65da 0f55 7064 6174 6543 6f6e  egate..UpdateCon
+00000160: 6469 7469 6f6e 2901 da0c 4163 7469 6f6e  dition)...Action
+00000170: 5265 636f 7264 2901 da0a 496e 766f 6361  Record)...Invoca
+00000180: 7469 6f6e 2901 da12 496e 766f 6361 7469  tion)...Invocati
+00000190: 6f6e 4465 6c65 6761 7465 2902 da18 496e  onDelegate)...In
+000001a0: 766f 6361 7469 6f6e 4461 7461 536f 7572  vocationDataSour
+000001b0: 6365 5479 7065 da10 496e 766f 6361 7469  ceType..Invocati
+000001c0: 6f6e 536f 7572 6365 6300 0000 0000 0000  onSourcec.......
+000001d0: 0000 0000 0000 0000 0018 0000 0040 0000  .............@..
+000001e0: 0073 7202 0000 6500 5a01 6400 5a02 5500  .sr...e.Z.d.Z.U.
+000001f0: 6800 6401 a301 5a03 6504 6505 6402 3c00  h.d...Z.e.e.d.<.
+00000200: 6506 6505 6403 3c00 6507 6505 6404 3c00  e.e.d.<.e.e.d.<.
+00000210: 6405 5a08 6509 650a 1900 6505 6406 3c00  d.Z.e.e...e.d.<.
+00000220: 650b 0905 0905 0905 0905 0905 0905 0905  e...............
+00000230: 6440 6407 650c 6408 6504 6409 6506 640a  d@d.e.d.e.d.e.d.
+00000240: 6509 650c 1900 640b 6509 650c 1900 640c  e.e...d.e.e...d.
+00000250: 6509 650d 650c 650e 6602 1900 1900 640d  e.e.e.e.f.....d.
+00000260: 6509 650f 650c 1900 1900 640e 6509 650c  e.e.e.....d.e.e.
+00000270: 1900 640f 6509 6510 1900 6410 6509 6511  ..d.e.e...d.e.e.
+00000280: 1900 6411 6400 6616 6412 6413 8405 8301  ..d.d.f.d.d.....
+00000290: 5a12 650b 0905 6441 6407 650c 6408 6504  Z.e...dAd.e.d.e.
+000002a0: 6409 6506 640a 6509 650c 1900 6411 6400  d.e.d.e.e...d.d.
+000002b0: 660a 6414 6415 8405 8301 5a13 650b 0905  f.d.d.....Z.e...
+000002c0: 6441 6416 650d 650c 650e 6602 1900 6408  dAd.e.e.e.f...d.
+000002d0: 6504 6409 6506 640a 6509 650c 1900 6411  e.d.e.d.e.e...d.
+000002e0: 6514 6a15 6a16 6417 1900 660a 6418 6419  e.j.j.d...f.d.d.
+000002f0: 8405 8301 5a17 641a 6507 6408 6504 6409  ....Z.d.e.d.e.d.
+00000300: 6506 6411 6405 6608 641b 641c 8404 5a18  e.d.d.f.d.d...Z.
+00000310: 6519 6411 6510 6602 641d 641e 8404 8301  e.d.e.f.d.d.....
+00000320: 5a1a 6519 6411 6511 6602 641f 6420 8404  Z.e.d.e.f.d.d ..
+00000330: 8301 5a1b 6519 6411 651c 6a1c 6602 6421  ..Z.e.d.e.j.f.d!
+00000340: 6422 8404 8301 5a1d 6519 6411 650c 6602  d"....Z.e.d.e.f.
+00000350: 6423 6424 8404 8301 5a1e 6519 6411 650c  d#d$....Z.e.d.e.
+00000360: 6602 6425 6426 8404 8301 5a1f 6519 6411  f.d%d&....Z.e.d.
+00000370: 6509 650c 1900 6602 6427 6428 8404 8301  e.e...f.d'd(....
+00000380: 5a20 0905 6441 6429 6509 650c 1900 6411  Z ..dAd)e.e...d.
+00000390: 650a 6604 642a 642b 8405 5a21 0905 0905  e.f.d*d+..Z!....
+000003a0: 0905 6442 642c 650f 650c 1900 642d 650c  ..dBd,e.e...d-e.
+000003b0: 642e 6522 642f 6523 6430 6509 650c 1900  d.e"d/e#d0e.e...
+000003c0: 6431 6509 6510 1900 6432 6509 6511 1900  d1e.e...d2e.e...
+000003d0: 6411 6524 6610 6433 6434 8405 5a25 0905  d.e$f.d3d4..Z%..
+000003e0: 6441 6435 650c 6436 650c 6429 6509 650c  dAd5e.d6e.d)e.e.
+000003f0: 1900 6411 6405 6608 6437 6438 8405 5a26  ..d.d.f.d7d8..Z&
+00000400: 6411 650d 650c 650e 6602 1900 6602 6439  d.e.e.e.f...f.d9
+00000410: 643a 8404 5a27 0905 0905 0905 6442 643b  d:..Z'......dBd;
+00000420: 650d 650c 650e 6602 1900 643c 6509 650f  e.e.e.f...d<e.e.
+00000430: 6528 1900 1900 640a 6509 650c 1900 643d  e(....d.e.e...d=
+00000440: 6509 650c 1900 6411 6405 660a 643e 643f  e.e...d.d.f.d>d?
+00000450: 8405 5a29 6405 5300 2943 da06 4163 7469  ..Z)d.S.)C..Acti
+00000460: 6f6e 3e07 0000 00da 066f 7267 5f69 645a  on>......org_idZ
+00000470: 0a63 7265 6174 6564 5f61 74da 0375 7269  .created_at..uri
+00000480: da0a 6372 6561 7465 645f 6279 5a0b 6d6f  ..created_byZ.mo
+00000490: 6469 6669 6564 5f62 79da 086d 6f64 6966  dified_by..modif
+000004a0: 6965 64da 046e 616d 65da 185f 4163 7469  ied..name.._Acti
+000004b0: 6f6e 5f5f 6163 7469 6f6e 5f64 656c 6567  on__action_deleg
+000004c0: 6174 65da 1c5f 4163 7469 6f6e 5f5f 696e  ate.._Action__in
+000004d0: 766f 6361 7469 6f6e 5f64 656c 6567 6174  vocation_delegat
+000004e0: 65da 0f5f 4163 7469 6f6e 5f5f 7265 636f  e.._Action__reco
+000004f0: 7264 4eda 235f 4163 7469 6f6e 5f5f 7465  rdN.#_Action__te
+00000500: 6d70 5f63 6f6e 7461 696e 6572 5f63 7265  mp_container_cre
+00000510: 6465 6e74 6961 6c73 7216 0000 00da 0f61  dentialsr......a
+00000520: 6374 696f 6e5f 6465 6c65 6761 7465 da13  ction_delegate..
+00000530: 696e 766f 6361 7469 6f6e 5f64 656c 6567  invocation_deleg
+00000540: 6174 6572 1200 0000 da0b 6465 7363 7269  ater......descri
+00000550: 7074 696f 6eda 086d 6574 6164 6174 61da  ption..metadata.
+00000560: 0474 6167 7372 1400 0000 da14 636f 6d70  .tagsr......comp
+00000570: 7574 655f 7265 7175 6972 656d 656e 7473  ute_requirements
+00000580: da14 636f 6e74 6169 6e65 725f 7061 7261  ..container_para
+00000590: 6d65 7465 7273 da06 7265 7475 726e 630b  meters..returnc.
+000005a0: 0000 0000 0000 0000 0000 000c 0000 000a  ................
+000005b0: 0000 0043 0000 0073 2400 0000 7c02 a000  ...C...s$...|...
+000005c0: 7c01 7c04 7c08 7c05 7c06 7c07 7c09 7c0a  |.|.|.|.|.|.|.|.
+000005d0: a108 7d0b 7c00 7c0b 7c02 7c03 8303 5300  ..}.|.|.|.|...S.
+000005e0: a901 4e29 015a 0d63 7265 6174 655f 6163  ..N).Z.create_ac
+000005f0: 7469 6f6e 290c da03 636c 7372 1600 0000  tion)...clsr....
+00000600: 721b 0000 0072 1c00 0000 7212 0000 0072  r....r....r....r
+00000610: 1d00 0000 721e 0000 0072 1f00 0000 7214  ....r....r....r.
+00000620: 0000 0072 2000 0000 7221 0000 00da 0672  ...r ...r!.....r
+00000630: 6563 6f72 64a9 0072 2600 0000 faed 2f63  ecord..r&...../c
+00000640: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
+00000650: 7372 6331 3638 3931 3535 3339 392f 7372  src1689155399/sr
+00000660: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
+00000670: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
+00000680: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
+00000690: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
+000006a0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
+000006b0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
+000006c0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
+000006d0: 3939 642f 726f 626f 746f 2d61 692f 726f  99d/roboto-ai/ro
+000006e0: 626f 746f 2d68 6f73 7465 642d 6170 702f  boto-hosted-app/
+000006f0: 7061 636b 6167 6573 2f72 6f62 6f74 6f5f  packages/roboto_
+00000700: 7364 6b2f 7372 632f 726f 626f 746f 5f73  sdk/src/roboto_s
+00000710: 646b 2f64 6f6d 6169 6e2f 6163 7469 6f6e  dk/domain/action
+00000720: 732f 6163 7469 6f6e 2e70 79da 0663 7265  s/action.py..cre
+00000730: 6174 652a 0000 0073 1600 0000 040e 0201  ate*...s........
+00000740: 0201 0201 0201 0201 0201 0201 0201 04f8  ................
+00000750: 0c0a 7a0d 4163 7469 6f6e 2e63 7265 6174  ..z.Action.creat
+00000760: 6563 0500 0000 0000 0000 0000 0000 0600  ec..............
+00000770: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
+00000780: 02a0 007c 017c 04a1 027d 057c 007c 057c  ...|.|...}.|.|.|
+00000790: 027c 0383 0353 0072 2300 0000 2901 5a19  .|...S.r#...).Z.
+000007a0: 6765 745f 6163 7469 6f6e 5f62 795f 7072  get_action_by_pr
+000007b0: 696d 6172 795f 6b65 7929 0672 2400 0000  imary_key).r$...
+000007c0: 7216 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+000007d0: 1200 0000 7225 0000 0072 2600 0000 7226  ....r%...r&...r&
+000007e0: 0000 0072 2700 0000 da09 6672 6f6d 5f6e  ...r'.....from_n
+000007f0: 616d 6544 0000 0073 0400 0000 0c08 0c01  ameD...s........
+00000800: 7a10 4163 7469 6f6e 2e66 726f 6d5f 6e61  z.Action.from_na
+00000810: 6d65 da07 6669 6c74 6572 7329 0372 1100  me..filters).r..
+00000820: 0000 4e4e 6305 0000 0000 0000 0000 0000  ..NNc...........
+00000830: 000c 0000 0006 0000 0063 0000 0073 a200  .........c...s..
+00000840: 0000 8100 7400 7401 6a02 a003 a100 8301  ....t.t.j.......
+00000850: 7d05 7400 7c01 a003 a100 8301 7d06 7c06  }.t.|.......}.|.
+00000860: 7c05 1800 7d07 7c07 722c 7404 7c07 8301  |...}.|.r,t.|...
+00000870: 6401 6b04 7d08 7c08 721e 6402 6e01 6403  d.k.}.|.r.d.n.d.
+00000880: 7d09 7405 7c07 9b00 6404 7c09 9b00 6405  }.t.|...d.|...d.
+00000890: 7c05 9b00 9d05 8301 8201 7c02 6a06 7c01  |.........|.j.|.
+000008a0: 7c04 6406 8d02 7d0a 0900 7c0a 6a07 4400  |.d...}...|.j.D.
+000008b0: 5d09 7d0b 7c00 7c0b 7c02 7c03 8303 5600  ].}.|.|.|.|...V.
+000008c0: 0100 7137 7c0a 6a08 724e 7c02 6a06 7c01  ..q7|.j.rN|.j.|.
+000008d0: 7c04 7c0a 6a08 6408 8d03 7d0a 6e02 6400  |.|.j.d...}.n.d.
+000008e0: 5300 7134 2909 4e72 0600 0000 7a22 6172  S.q4).Nr....z"ar
+000008f0: 6520 6e6f 7420 6b6e 6f77 6e20 6174 7472  e not known attr
+00000900: 6962 7574 6573 206f 6620 4163 7469 6f6e  ibutes of Action
+00000910: 7a22 6973 206e 6f74 2061 206b 6e6f 776e  z"is not a known
+00000920: 2061 7474 7269 6275 7465 206f 6620 4163   attribute of Ac
+00000930: 7469 6f6e da01 207a 142e 204b 6e6f 776e  tion.. z.. Known
+00000940: 2061 7474 7269 6275 7465 733a 2029 0172   attributes: ).r
+00000950: 1200 0000 5429 0272 1200 0000 5a0a 7061  ....T).r....Z.pa
+00000960: 6765 5f74 6f6b 656e 2909 da03 7365 7472  ge_token)...setr
+00000970: 0c00 0000 da0a 5f5f 6669 656c 6473 5f5f  ......__fields__
+00000980: da04 6b65 7973 da03 6c65 6eda 0a56 616c  ..keys..len..Val
+00000990: 7565 4572 726f 725a 0d71 7565 7279 5f61  ueErrorZ.query_a
+000009a0: 6374 696f 6e73 da05 6974 656d 73da 0a6e  ctions..items..n
+000009b0: 6578 745f 746f 6b65 6e29 0c72 2400 0000  ext_token).r$...
+000009c0: 722a 0000 0072 1b00 0000 721c 0000 0072  r*...r....r....r
+000009d0: 1200 0000 da0a 6b6e 6f77 6e5f 6b65 7973  ......known_keys
+000009e0: 5a0b 6163 7475 616c 5f6b 6579 735a 0c75  Z.actual_keysZ.u
+000009f0: 6e6b 6e6f 776e 5f6b 6579 73da 0670 6c75  nknown_keys..plu
+00000a00: 7261 6cda 036d 7367 5a11 7061 6769 6e61  ral..msgZ.pagina
+00000a10: 7465 645f 7265 7375 6c74 7372 2500 0000  ted_resultsr%...
+00000a20: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
+00000a30: 0571 7565 7279 4f00 0000 732a 0000 0002  .queryO...s*....
+00000a40: 800e 080c 0108 0104 010c 0102 0306 ff02  ................
+00000a50: 0202 fd18 050e 0202 010a 0110 0106 0104  ................
+00000a60: 0108 0108 ff04 0402 f87a 0c41 6374 696f  .........z.Actio
+00000a70: 6e2e 7175 6572 7972 2500 0000 6304 0000  n.queryr%...c...
+00000a80: 0000 0000 0000 0000 0004 0000 0002 0000  ................
+00000a90: 0043 0000 0073 1600 0000 7c02 7c00 5f00  .C...s....|.|._.
+00000aa0: 7c03 7c00 5f01 7c01 7c00 5f02 6400 5300  |.|._.|.|._.d.S.
+00000ab0: 7223 0000 0029 0372 1700 0000 7218 0000  r#...).r....r...
+00000ac0: 0072 1900 0000 2904 da04 7365 6c66 7225  .r....)...selfr%
+00000ad0: 0000 0072 1b00 0000 721c 0000 0072 2600  ...r....r....r&.
+00000ae0: 0000 7226 0000 0072 2700 0000 da08 5f5f  ..r&...r'.....__
+00000af0: 696e 6974 5f5f 6e00 0000 7306 0000 0006  init__n...s.....
+00000b00: 0606 010a 017a 0f41 6374 696f 6e2e 5f5f  .....z.Action.__
+00000b10: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000b20: 0000 0001 0000 0001 0000 0043 0000 00f3  ...........C....
+00000b30: 0800 0000 7c00 6a00 6a01 5300 7223 0000  ....|.j.j.S.r#..
+00000b40: 0029 0272 1900 0000 7220 0000 00a9 0172  .).r....r .....r
+00000b50: 3700 0000 7226 0000 0072 2600 0000 7227  7...r&...r&...r'
+00000b60: 0000 0072 2000 0000 7800 0000 f302 0000  ...r ...x.......
+00000b70: 0008 027a 1b41 6374 696f 6e2e 636f 6d70  ...z.Action.comp
+00000b80: 7574 655f 7265 7175 6972 656d 656e 7473  ute_requirements
+00000b90: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000ba0: 0001 0000 0043 0000 0072 3900 0000 7223  .....C...r9...r#
+00000bb0: 0000 0029 0272 1900 0000 7221 0000 0072  ...).r....r!...r
+00000bc0: 3a00 0000 7226 0000 0072 2600 0000 7227  :...r&...r&...r'
+00000bd0: 0000 0072 2100 0000 7c00 0000 723b 0000  ...r!...|...r;..
+00000be0: 007a 1b41 6374 696f 6e2e 636f 6e74 6169  .z.Action.contai
+00000bf0: 6e65 725f 7061 7261 6d65 7465 7273 6301  ner_parametersc.
+00000c00: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000c10: 0000 0043 0000 0072 3900 0000 7223 0000  ...C...r9...r#..
+00000c20: 0029 0272 1900 0000 7215 0000 0072 3a00  .).r....r....r:.
+00000c30: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
+00000c40: 00da 0d6c 6173 745f 6d6f 6469 6669 6564  ...last_modified
+00000c50: 8000 0000 723b 0000 007a 1441 6374 696f  ....r;...z.Actio
+00000c60: 6e2e 6c61 7374 5f6d 6f64 6966 6965 6463  n.last_modifiedc
+00000c70: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000c80: 0100 0000 4300 0000 7239 0000 0072 2300  ....C...r9...r#.
+00000c90: 0000 2902 7219 0000 0072 1600 0000 723a  ..).r....r....r:
+00000ca0: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+00000cb0: 0000 7216 0000 0084 0000 0072 3b00 0000  ..r........r;...
+00000cc0: 7a0b 4163 7469 6f6e 2e6e 616d 6563 0100  z.Action.namec..
+00000cd0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000ce0: 0000 4300 0000 7239 0000 0072 2300 0000  ..C...r9...r#...
+00000cf0: 2902 7219 0000 0072 1200 0000 723a 0000  ).r....r....r:..
+00000d00: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00000d10: 7212 0000 0088 0000 0072 3b00 0000 7a0d  r........r;...z.
+00000d20: 4163 7469 6f6e 2e6f 7267 5f69 6463 0100  Action.org_idc..
+00000d30: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000d40: 0000 4300 0000 7239 0000 0072 2300 0000  ..C...r9...r#...
+00000d50: 2902 7219 0000 0072 1300 0000 723a 0000  ).r....r....r:..
+00000d60: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00000d70: 7213 0000 008c 0000 0072 3b00 0000 7a0a  r........r;...z.
+00000d80: 4163 7469 6f6e 2e75 7269 da06 6361 6c6c  Action.uri..call
+00000d90: 6572 6302 0000 0000 0000 0000 0000 0003  erc.............
+00000da0: 0000 0004 0000 0043 0000 0073 3000 0000  .......C...s0...
+00000db0: 7c00 6a00 6400 7500 730a 7c00 6a00 a001  |.j.d.u.s.|.j...
+00000dc0: a100 7215 7c00 6a02 a003 7c00 6a04 7c01  ..r.|.j...|.j.|.
+00000dd0: a102 7d02 7c02 7c00 5f00 7c00 6a00 5300  ..}.|.|._.|.j.S.
+00000de0: 7223 0000 0029 0572 1a00 0000 da0a 6973  r#...).r......is
+00000df0: 5f65 7870 6972 6564 7217 0000 005a 1e67  _expiredr....Z.g
+00000e00: 6574 5f74 656d 705f 636f 6e74 6169 6e65  et_temp_containe
+00000e10: 725f 6372 6564 656e 7469 616c 7372 1900  r_credentialsr..
+00000e20: 0000 2903 7237 0000 0072 3d00 0000 da05  ..).r7...r=.....
+00000e30: 6372 6564 7372 2600 0000 7226 0000 0072  credsr&...r&...r
+00000e40: 2700 0000 da23 6765 745f 7465 6d70 6f72  '....#get_tempor
+00000e50: 6172 795f 636f 6e74 6169 6e65 725f 6372  ary_container_cr
+00000e60: 6564 656e 7469 616c 7390 0000 0073 1000  edentials....s..
+00000e70: 0000 0a04 0801 02ff 0603 0601 04ff 0603  ................
+00000e80: 0602 7a2a 4163 7469 6f6e 2e67 6574 5f74  ..z*Action.get_t
+00000e90: 656d 706f 7261 7279 5f63 6f6e 7461 696e  emporary_contain
+00000ea0: 6572 5f63 7265 6465 6e74 6961 6c73 da0a  er_credentials..
+00000eb0: 696e 7075 745f 6461 7461 da0e 6461 7461  input_data..data
+00000ec0: 5f73 6f75 7263 655f 6964 da10 6461 7461  _source_id..data
+00000ed0: 5f73 6f75 7263 655f 7479 7065 da11 696e  _source_type..in
+00000ee0: 766f 6361 7469 6f6e 5f73 6f75 7263 65da  vocation_source.
+00000ef0: 1469 6e76 6f63 6174 696f 6e5f 736f 7572  .invocation_sour
+00000f00: 6365 5f69 64da 1d63 6f6d 7075 7465 5f72  ce_id..compute_r
+00000f10: 6571 7569 7265 6d65 6e74 5f6f 7665 7272  equirement_overr
+00000f20: 6964 6573 da1d 636f 6e74 6169 6e65 725f  ides..container_
+00000f30: 7061 7261 6d65 7465 725f 6f76 6572 7269  parameter_overri
+00000f40: 6465 7363 0800 0000 0000 0000 0000 0000  desc............
+00000f50: 0b00 0000 0a00 0000 4300 0000 7378 0000  ........C...sx..
+00000f60: 007c 006a 006a 016a 0264 017c 0672 0f7c  .|.j.j.j.d.|.r.|
+00000f70: 066a 0364 0164 0164 0164 028d 036e 0274  .j.d.d.d.d...n.t
+00000f80: 0383 0064 038d 027d 087c 006a 006a 046a  ...d...}.|.j.j.j
+00000f90: 0264 017c 0772 237c 076a 0364 0164 0164  .d.|.r#|.j.d.d.d
+00000fa0: 0164 028d 036e 0274 0383 0064 038d 027d  .d...n.t...d...}
+00000fb0: 097c 006a 05a0 067c 006a 007c 017c 087c  .|.j...|.j.|.|.|
+00000fc0: 097c 027c 037c 047c 05a1 087d 0a74 077c  .|.|.|.|...}.t.|
+00000fd0: 0a7c 006a 0583 0253 0029 044e 5429 03da  .|.j...S.).NT)..
+00000fe0: 0c65 7863 6c75 6465 5f6e 6f6e 65da 1065  .exclude_none..e
+00000ff0: 7863 6c75 6465 5f64 6566 6175 6c74 73da  xclude_defaults.
+00001000: 0d65 7863 6c75 6465 5f75 6e73 6574 2902  .exclude_unset).
+00001010: da04 6465 6570 da06 7570 6461 7465 2908  ..deep..update).
+00001020: 7219 0000 0072 2000 0000 da04 636f 7079  r....r .....copy
+00001030: da04 6469 6374 7221 0000 0072 1800 0000  ..dictr!...r....
+00001040: 5a11 6372 6561 7465 5f69 6e76 6f63 6174  Z.create_invocat
+00001050: 696f 6e72 0d00 0000 290b 7237 0000 0072  ionr....).r7...r
+00001060: 4100 0000 7242 0000 0072 4300 0000 7244  A...rB...rC...rD
+00001070: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
+00001080: 0000 5a0c 636f 6d70 7574 655f 7265 7173  ..Z.compute_reqs
+00001090: 5a10 636f 6e74 6169 6e65 725f 7061 7261  Z.container_para
+000010a0: 6d73 7225 0000 0072 2600 0000 7226 0000  msr%...r&...r&..
+000010b0: 0072 2700 0000 da06 696e 766f 6b65 9e00  .r'.....invoke..
+000010c0: 0000 733c 0000 0008 0a02 0102 0406 fd06  ..s<............
+000010d0: 0106 ff04 0406 fa08 0802 0102 0406 fd06  ................
+000010e0: 0106 ff04 0406 fa06 0804 0102 0102 0102  ................
+000010f0: 0102 0102 0102 0102 0104 f802 0a02 0104  ................
+00001100: 0104 fe7a 0d41 6374 696f 6e2e 696e 766f  ...z.Action.invo
+00001110: 6b65 da0a 696d 6167 655f 6e61 6d65 da09  ke..image_name..
+00001120: 696d 6167 655f 7461 6763 0400 0000 0000  image_tagc......
+00001130: 0000 0000 0000 0500 0000 0600 0000 4300  ..............C.
+00001140: 0000 731e 0000 007c 006a 00a0 017c 006a  ..s....|.j...|.j
+00001150: 027c 017c 027c 03a1 047d 047c 047c 005f  .|.|.|...}.|.|._
+00001160: 0264 0153 0029 0261 7b04 0000 0a20 2020  .d.S.).a{....   
+00001170: 2020 2020 2049 6465 6d70 6f74 656e 7420       Idempotent 
+00001180: 6765 7420 6f72 2063 7265 6174 6520 636f  get or create co
+00001190: 6e74 6169 6e65 7220 7265 706f 7369 746f  ntainer reposito
+000011a0: 7279 2066 6f72 2074 6869 7320 4163 7469  ry for this Acti
+000011b0: 6f6e 2c20 616e 6420 6173 736f 6369 6174  on, and associat
+000011c0: 6520 6974 2077 6974 6820 7468 6520 4163  e it with the Ac
+000011d0: 7469 6f6e 2061 7320 6974 7320 5552 492e  tion as its URI.
+000011e0: 0a20 2020 2020 2020 2055 7365 2074 6869  .        Use thi
+000011f0: 7320 746f 2061 7373 6f63 6961 7465 2061  s to associate a
+00001200: 6e20 4163 7469 6f6e 2077 6974 6820 6120  n Action with a 
+00001210: 636f 6e74 6169 6e65 7220 696d 6167 6520  container image 
+00001220: 7468 6174 2068 6173 2079 6574 2074 6f20  that has yet to 
+00001230: 6265 2070 7573 6865 642c 0a20 2020 2020  be pushed,.     
+00001240: 2020 206f 7220 7769 7468 2061 2063 6f6e     or with a con
+00001250: 7461 696e 6572 2069 6d61 6765 2074 6861  tainer image tha
+00001260: 7420 6861 7320 616c 7265 6164 7920 6265  t has already be
+00001270: 656e 2070 7573 6865 6420 746f 2061 6e20  en pushed to an 
+00001280: 6578 6973 7469 6e67 2072 6570 6f73 6974  existing reposit
+00001290: 6f72 792e 0a0a 2020 2020 2020 2020 4120  ory...        A 
+000012a0: 636f 6e74 6169 6e65 7220 6d61 7920 6265  container may be
+000012b0: 2070 7573 6865 6420 746f 2074 6865 2072   pushed to the r
+000012c0: 6570 6f73 6973 746f 7279 2075 7369 6e67  eposistory using
+000012d0: 2063 7265 6465 6e74 6961 6c73 2072 6574   credentials ret
+000012e0: 7572 6e65 6420 6279 0a20 2020 2020 2020  urned by.       
+000012f0: 2060 6765 745f 7465 6d70 6f72 6172 795f   `get_temporary_
+00001300: 636f 6e74 6169 6e65 725f 6372 6564 656e  container_creden
+00001310: 7469 616c 7360 2e0a 2020 2020 2020 2020  tials`..        
+00001320: 4974 7320 7461 6720 646f 6573 206e 6f74  Its tag does not
+00001330: 206e 6565 6420 746f 2065 7175 616c 2060   need to equal `
+00001340: 696d 6167 655f 7461 6760 2c20 6275 7420  image_tag`, but 
+00001350: 7769 7468 6f75 7420 6361 6c6c 696e 6720  without calling 
+00001360: 7468 6973 206d 6574 686f 6420 7769 7468  this method with
+00001370: 2074 6865 2061 7373 6f63 6961 7465 6420   the associated 
+00001380: 7461 672c 0a20 2020 2020 2020 2074 6865  tag,.        the
+00001390: 2041 6374 696f 6e20 7769 6c6c 206e 6f74   Action will not
+000013a0: 2062 6520 6162 6c65 2074 6f20 696e 766f   be able to invo
+000013b0: 6b65 2074 6865 2070 7573 6865 6420 636f  ke the pushed co
+000013c0: 6e74 6169 6e65 722e 0a0a 2020 2020 2020  ntainer...      
+000013d0: 2020 5369 6465 2d65 6666 6563 7473 3a0a    Side-effects:.
+000013e0: 2020 2020 2020 2020 2020 2020 2a20 4966              * If
+000013f0: 2061 2063 6f6e 7461 696e 6572 2072 6570   a container rep
+00001400: 6f73 6974 6f72 7920 666f 7220 6769 7665  ository for give
+00001410: 6e20 6069 6d61 6765 5f6e 616d 6560 3a60  n `image_name`:`
+00001420: 696d 6167 655f 7461 6760 2064 6f65 7320  image_tag` does 
+00001430: 6e6f 7420 6578 6973 742c 2069 7420 7769  not exist, it wi
+00001440: 6c6c 2062 6520 6372 6561 7465 642e 0a20  ll be created.. 
+00001450: 2020 2020 2020 2020 2020 202a 2049 6620             * If 
+00001460: 6120 636f 6e74 6169 6e65 7220 7265 706f  a container repo
+00001470: 7369 746f 7279 2077 6173 2070 7265 7669  sitory was previ
+00001480: 6f75 736c 7920 6372 6561 7465 6420 666f  ously created fo
+00001490: 7220 7468 6973 2041 6374 696f 6e20 666f  r this Action fo
+000014a0: 7220 6120 6469 6666 6572 656e 7420 6069  r a different `i
+000014b0: 6d61 6765 5f6e 616d 6560 2c0a 2020 2020  mage_name`,.    
+000014c0: 2020 2020 2020 2020 2020 414e 4420 7468            AND th
+000014d0: 6174 2072 6570 6f73 6974 6f72 7920 6973  at repository is
+000014e0: 2065 6d70 7479 2c20 6974 2077 696c 6c20   empty, it will 
+000014f0: 6265 2064 656c 6574 6564 2e0a 2020 2020  be deleted..    
+00001500: 2020 2020 2020 2020 2a20 5365 7473 2074          * Sets t
+00001510: 6865 2060 7572 6960 2061 7474 7269 6275  he `uri` attribu
+00001520: 7465 206f 6620 7468 6973 2041 6374 696f  te of this Actio
+00001530: 6e20 746f 2074 6865 2055 5249 206f 6620  n to the URI of 
+00001540: 7468 6520 696d 6167 6520 6578 7065 6374  the image expect
+00001550: 6564 2074 6f20 6265 2070 7573 6865 6420  ed to be pushed 
+00001560: 746f 2074 6865 2072 6570 6f73 6974 6f72  to the repositor
+00001570: 792e 0a0a 2020 2020 2020 2020 6063 616c  y...        `cal
+00001580: 6c65 7260 2069 7320 6967 6e6f 7265 6420  ler` is ignored 
+00001590: 6f6e 2074 6865 2063 6c69 656e 742e 2049  on the client. I
+000015a0: 7420 6973 2064 6574 6572 6d69 6e65 6420  t is determined 
+000015b0: 7365 7276 6572 2d73 6964 6520 7669 6120  server-side via 
+000015c0: 7468 6520 6964 656e 7469 7479 2f61 6363  the identity/acc
+000015d0: 6573 7320 6d65 6368 616e 6973 6d2e 0a20  ess mechanism.. 
+000015e0: 2020 2020 2020 204e 2903 7217 0000 00da         N).r.....
+000015f0: 1272 6567 6973 7465 725f 636f 6e74 6169  .register_contai
+00001600: 6e65 7272 1900 0000 2905 7237 0000 0072  nerr....).r7...r
+00001610: 5000 0000 7251 0000 0072 3d00 0000 da07  P...rQ...r=.....
+00001620: 7570 6461 7465 6472 2600 0000 7226 0000  updatedr&...r&..
+00001630: 0072 2700 0000 7252 0000 00c7 0000 0073  .r'...rR.......s
+00001640: 0800 0000 0618 0a01 04ff 0a03 7a19 4163  ............z.Ac
+00001650: 7469 6f6e 2e72 6567 6973 7465 725f 636f  tion.register_co
+00001660: 6e74 6169 6e65 7263 0100 0000 0000 0000  ntainerc........
+00001670: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00001680: 730a 0000 0074 007c 006a 0183 0153 0072  s....t.|.j...S.r
+00001690: 2300 0000 2902 7205 0000 0072 1900 0000  #...).r....r....
+000016a0: 723a 0000 0072 2600 0000 7226 0000 0072  r:...r&...r&...r
+000016b0: 2700 0000 da07 746f 5f64 6963 74e4 0000  '.....to_dict...
+000016c0: 0073 0200 0000 0a01 7a0e 4163 7469 6f6e  .s......z.Action
+000016d0: 2e74 6f5f 6469 6374 da07 7570 6461 7465  .to_dict..update
+000016e0: 73da 0a63 6f6e 6469 7469 6f6e 73da 0a75  s..conditions..u
+000016f0: 7064 6174 6564 5f62 7963 0500 0000 0000  pdated_byc......
+00001700: 0000 0000 0000 0b00 0000 0700 0000 4300  ..............C.
+00001710: 0000 7380 0000 0074 0074 016a 02a0 03a1  ..s....t.t.j....
+00001720: 0083 017d 057c 0574 046a 0518 007d 0674  ...}.|.t.j...}.t
+00001730: 007c 01a0 03a1 0083 017c 0618 007d 0774  .|.......|...}.t
+00001740: 067c 0783 0172 3074 067c 0783 0164 016b  .|...r0t.|...d.k
+00001750: 047d 087c 0872 2264 026e 0164 037d 0974  .}.|.r"d.n.d.}.t
+00001760: 077c 079b 0064 047c 099b 0064 057c 069b  .|...d.|...d.|..
+00001770: 009d 0583 0182 017c 006a 08a0 097c 006a  .......|.j...|.j
+00001780: 0a7c 017c 027c 037c 04a1 057d 0a7c 0a7c  .|.|.|.|...}.|.|
+00001790: 005f 0a64 0053 0029 064e 7206 0000 007a  ._.d.S.).Nr....z
+000017a0: 1d61 7265 206e 6f74 2075 7064 6174 6561  .are not updatea
+000017b0: 626c 6520 6174 7472 6962 7574 6573 7a1e  ble attributesz.
+000017c0: 6973 206e 6f74 2061 6e20 7570 6461 7465  is not an update
+000017d0: 6162 6c65 2061 7474 7269 6275 7465 722b  able attributer+
+000017e0: 0000 007a 192e 2055 7064 6174 6561 626c  ...z.. Updateabl
+000017f0: 6520 6174 7472 6962 7574 6573 3a20 290b  e attributes: ).
+00001800: 722c 0000 0072 0c00 0000 722d 0000 0072  r,...r....r-...r
+00001810: 2e00 0000 7211 0000 00da 1544 4953 414c  ....r......DISAL
+00001820: 4c4f 5745 445f 464f 525f 5550 4441 5445  LOWED_FOR_UPDATE
+00001830: 722f 0000 0072 3000 0000 7217 0000 0072  r/...r0...r....r
+00001840: 4c00 0000 7219 0000 0029 0b72 3700 0000  L...r....).r7...
+00001850: 7255 0000 0072 5600 0000 7212 0000 0072  rU...rV...r....r
+00001860: 5700 0000 7233 0000 00da 0c61 6c6c 6f77  W...r3.....allow
+00001870: 6564 5f6b 6579 735a 0975 6e61 6c6c 6f77  ed_keysZ.unallow
+00001880: 6564 7234 0000 0072 3500 0000 7253 0000  edr4...r5...rS..
+00001890: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+000018a0: 724c 0000 00e7 0000 0073 2000 0000 0e07  rL.......s .....
+000018b0: 0a01 1001 0801 0c01 0203 06ff 0202 02fd  ................
+000018c0: 0205 1201 04ff 0604 0c01 04ff 0a03 7a0d  ..............z.
+000018d0: 4163 7469 6f6e 2e75 7064 6174 6529 074e  Action.update).N
+000018e0: 4e4e 4e4e 4e4e 7223 0000 0029 034e 4e4e  NNNNNNr#...).NNN
+000018f0: 292a da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )*..__name__..__
+00001900: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00001910: 6e61 6d65 5f5f 7258 0000 0072 0a00 0000  name__rX...r....
+00001920: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00001930: 5f72 0e00 0000 720c 0000 0072 1a00 0000  _r....r....r....
+00001940: 7203 0000 0072 0800 0000 da0b 636c 6173  r....r......clas
+00001950: 736d 6574 686f 64da 0373 7472 724e 0000  smethod..strrN..
+00001960: 0072 0200 0000 da04 6c69 7374 7207 0000  .r......listr...
+00001970: 0072 0900 0000 7228 0000 0072 2900 0000  .r....r(...r)...
+00001980: da0b 636f 6c6c 6563 7469 6f6e 73da 0361  ..collections..a
+00001990: 6263 da09 4765 6e65 7261 746f 7272 3600  bc..Generatorr6.
+000019a0: 0000 7238 0000 00da 0870 726f 7065 7274  ..r8.....propert
+000019b0: 7972 2000 0000 7221 0000 00da 0864 6174  yr ...r!.....dat
+000019c0: 6574 696d 6572 3c00 0000 7216 0000 0072  etimer<...r....r
+000019d0: 1200 0000 7213 0000 0072 4000 0000 720f  ....r....r@...r.
+000019e0: 0000 0072 1000 0000 720d 0000 0072 4f00  ...r....r....rO.
+000019f0: 0000 7252 0000 0072 5400 0000 720b 0000  ..rR...rT...r...
+00001a00: 0072 4c00 0000 7226 0000 0072 2600 0000  .rL...r&...r&...
+00001a10: 7226 0000 0072 2700 0000 7211 0000 001a  r&...r'...r.....
+00001a20: 0000 0073 0e01 0000 0a00 0801 080a 0801  ...s............
+00001a30: 0801 1001 0202 0206 0201 0201 0201 0201  ................
+00001a40: 0201 0201 04f5 0202 02fe 0203 02fd 0204  ................
+00001a50: 02fc 0605 02fb 0606 02fa 0e07 02f9 0a08  ................
+00001a60: 02f8 0609 02f7 060a 02f6 060b 02f5 020c  ................
+00001a70: 0cf4 0219 0206 04fb 0202 02fe 0203 02fd  ................
+00001a80: 0204 02fc 0605 02fb 0206 0cfa 020a 0206  ................
+00001a90: 04fb 0a02 02fe 0203 02fd 0204 02fc 0605  ................
+00001aa0: 02fb 0a06 0cfa 021e 0202 02fe 0203 02fd  ................
+00001ab0: 0204 02fc 0205 0afb 020a 1001 0203 1001  ................
+00001ac0: 0203 1201 0203 1001 0203 1001 0203 1401  ................
+00001ad0: 0204 04ff 0601 02ff 0202 0afe 0214 0201  ................
+00001ae0: 0201 04f8 0602 02fe 0203 02fd 0204 02fc  ................
+00001af0: 0205 02fb 0606 02fa 0607 02f9 0608 02f8  ................
+00001b00: 0209 0af7 022d 04fc 0202 02fe 0203 02fd  .....-..........
+00001b10: 0604 02fc 0205 0afb 161d 0206 0201 0201  ................
+00001b20: 04fb 0a02 02fe 0a03 02fd 0604 02fc 0605  ................
+00001b30: 02fb 0206 0efa 7211 0000 0029 19da 0f63  ......r....)...c
+00001b40: 6f6c 6c65 6374 696f 6e73 2e61 6263 7261  ollections.abcra
+00001b50: 0000 0072 6500 0000 da06 7479 7069 6e67  ...re.....typing
+00001b60: 7202 0000 0072 0300 0000 da05 7365 7264  r....r......serd
+00001b70: 6572 0500 0000 da1a 6163 7469 6f6e 5f63  er......action_c
+00001b80: 6f6e 7461 696e 6572 5f72 6573 6f75 7263  ontainer_resourc
+00001b90: 6573 7207 0000 0072 0800 0000 7209 0000  esr....r....r...
+00001ba0: 0072 1b00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00001bb0: da0d 6163 7469 6f6e 5f72 6563 6f72 6472  ..action_recordr
+00001bc0: 0c00 0000 da0a 696e 766f 6361 7469 6f6e  ......invocation
+00001bd0: 720d 0000 0072 1c00 0000 720e 0000 00da  r....r....r.....
+00001be0: 1169 6e76 6f63 6174 696f 6e5f 7265 636f  .invocation_reco
+00001bf0: 7264 720f 0000 0072 1000 0000 7211 0000  rdr....r....r...
+00001c00: 0072 2600 0000 7226 0000 0072 2600 0000  .r&...r&...r&...
+00001c10: 7227 0000 00da 083c 6d6f 6475 6c65 3e01  r'.....<module>.
+00001c20: 0000 0073 1600 0000 0800 0801 1001 0c02  ...s............
+00001c30: 1401 1005 0c04 0c01 0c01 1003 1206       ..............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 3015 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,199 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 c70b 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 a708 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
-00000050: 0100 6400 6401 6c06 5a06 6403 6404 6c07  ..d.d.l.Z.d.d.l.
-00000060: 6d08 5a08 0100 6403 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6403 6406 6c0b 6d0c 5a0c 0100 6407  ..d.d.l.m.Z...d.
-00000080: 6408 6c0d 6d0e 5a0e 0100 4700 6409 640a  d.l.m.Z...G.d.d.
-00000090: 8400 640a 6506 6a0f 8303 5a10 4700 640b  ..d.e.j...Z.G.d.
-000000a0: 640c 8400 640c 6506 6a0f 8303 5a11 4700  d...d.e.j...Z.G.
-000000b0: 640d 640e 8400 640e 6500 6a12 8303 5a13  d.d...d.e.j...Z.
-000000c0: 6401 5300 290f e900 0000 004e 2903 da03  d.S.)......N)...
-000000d0: 416e 79da 074c 6974 6572 616c da08 4f70  Any..Literal..Op
-000000e0: 7469 6f6e 616c e903 0000 0029 01da 0d50  tional.....)...P
-000000f0: 6167 696e 6174 6564 4c69 7374 a901 da16  aginatedList....
-00000100: 7079 6461 6e74 6963 5f6a 736f 6e61 626c  pydantic_jsonabl
-00000110: 655f 6469 6374 2901 da06 7574 636e 6f77  e_dict)...utcnow
-00000120: e901 0000 0029 01da 0c41 6374 696f 6e52  .....)...ActionR
-00000130: 6563 6f72 6463 0000 0000 0000 0000 0000  ecordc..........
-00000140: 0000 0000 0000 0400 0000 4000 0000 7354  ..........@...sT
-00000150: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
-00000160: 0464 013c 0065 0365 0464 023c 0065 0365  .d.<.e.e.d.<.e.e
-00000170: 0464 033c 0065 056a 0565 0464 043c 0064  .d.<.e.j.e.d.<.d
-00000180: 0565 0666 0264 0664 0784 045a 0764 0565  .e.f.d.d...Z.d.e
-00000190: 0865 0365 0966 0219 0066 0264 0864 0984  .e.e.f...f.d.d..
-000001a0: 045a 0a64 0a53 0029 0bda 1443 6f6e 7461  .Z.d.S.)...Conta
-000001b0: 696e 6572 4372 6564 656e 7469 616c 73da  inerCredentials.
-000001c0: 0875 7365 726e 616d 65da 0870 6173 7377  .username..passw
-000001d0: 6f72 64da 0c72 6567 6973 7472 795f 7572  ord..registry_ur
-000001e0: 6cda 0a65 7870 6972 6174 696f 6eda 0672  l..expiration..r
-000001f0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-00000200: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
-00000210: 0000 0074 0083 007c 006a 016b 0553 00a9  ...t...|.j.k.S..
-00000220: 014e 2902 7209 0000 0072 1000 0000 a901  .N).r....r......
-00000230: da04 7365 6c66 a900 7215 0000 00fa f62f  ..self..r....../
-00000240: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000250: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
-00000260: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
-00000270: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
-00000280: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
-00000290: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
-000002a0: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
-000002b0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
-000002c0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
-000002d0: 3639 3964 2f72 6f62 6f74 6f2d 6169 2f72  699d/roboto-ai/r
-000002e0: 6f62 6f74 6f2d 686f 7374 6564 2d61 7070  oboto-hosted-app
-000002f0: 2f70 6163 6b61 6765 732f 726f 626f 746f  /packages/roboto
-00000300: 5f73 646b 2f73 7263 2f72 6f62 6f74 6f5f  _sdk/src/roboto_
-00000310: 7364 6b2f 646f 6d61 696e 2f61 6374 696f  sdk/domain/actio
-00000320: 6e73 2f61 6374 696f 6e5f 6465 6c65 6761  ns/action_delega
-00000330: 7465 2e70 79da 0a69 735f 6578 7069 7265  te.py..is_expire
-00000340: 6413 0000 0073 0200 0000 0c01 7a1f 436f  d....s......z.Co
-00000350: 6e74 6169 6e65 7243 7265 6465 6e74 6961  ntainerCredentia
-00000360: 6c73 2e69 735f 6578 7069 7265 6463 0100  ls.is_expiredc..
-00000370: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000380: 0000 4300 0000 7308 0000 0074 007c 0083  ..C...s....t.|..
-00000390: 0153 0072 1200 0000 7207 0000 0072 1300  .S.r....r....r..
-000003a0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000003b0: 00da 0774 6f5f 6469 6374 1600 0000 7302  ...to_dict....s.
-000003c0: 0000 0008 017a 1c43 6f6e 7461 696e 6572  .....z.Container
-000003d0: 4372 6564 656e 7469 616c 732e 746f 5f64  Credentials.to_d
-000003e0: 6963 744e 290b da08 5f5f 6e61 6d65 5f5f  ictN)...__name__
-000003f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000400: 7175 616c 6e61 6d65 5f5f da03 7374 72da  qualname__..str.
-00000410: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-00000420: da08 6461 7465 7469 6d65 da04 626f 6f6c  ..datetime..bool
-00000430: 7217 0000 00da 0464 6963 7472 0200 0000  r......dictr....
-00000440: 7218 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00000450: 1500 0000 7216 0000 0072 0c00 0000 0d00  ....r....r......
-00000460: 0000 730e 0000 000a 0008 0108 0108 010a  ..s.............
-00000470: 010e 021a 0372 0c00 0000 6300 0000 0000  .....r....c.....
-00000480: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000490: 0000 0073 2e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000004a0: 5500 6401 5a03 6504 6505 6402 3c00 6506  U.d.Z.e.e.d.<.e.
-000004b0: 6505 6403 3c00 6507 6404 1900 6505 6405  e.d.<.e.d...e.d.
-000004c0: 3c00 6406 5300 2907 da0f 5570 6461 7465  <.d.S.)...Update
-000004d0: 436f 6e64 6974 696f 6e61 5c01 0000 0a20  Conditiona\.... 
-000004e0: 2020 2041 2063 6f6e 6469 7469 6f6e 2074     A condition t
-000004f0: 6f20 6265 2061 7070 6c69 6564 2074 6f20  o be applied to 
-00000500: 616e 2041 6374 696f 6e20 7570 6461 7465  an Action update
-00000510: 206f 7065 7261 7469 6f6e 2e0a 0a20 2020   operation...   
-00000520: 2060 7661 6c75 6560 2069 7320 636f 6d70   `value` is comp
-00000530: 6172 6564 2074 6f20 7468 6520 4163 7469  ared to the Acti
-00000540: 6f6e 2773 2063 7572 7265 6e74 2076 616c  on's current val
-00000550: 7565 206f 6620 606b 6579 6020 7573 696e  ue of `key` usin
-00000560: 6720 6063 6f6d 7061 7261 746f 7260 2e0a  g `comparator`..
-00000570: 0a20 2020 2054 6869 7320 6973 2061 2073  .    This is a s
-00000580: 6576 6572 656c 7920 636f 6e73 7472 6169  everely constrai
-00000590: 6e74 6564 2073 7562 7365 7420 6f66 2074  nted subset of t
-000005a0: 6865 2063 6f6e 6469 7469 6f6e 7320 7375  he conditions su
-000005b0: 7070 6f72 7465 6420 6279 2044 796e 616d  pported by Dynam
-000005c0: 6f44 422e 2053 6565 3a0a 2020 2020 6874  oDB. See:.    ht
-000005d0: 7470 733a 2f2f 646f 6373 2e61 7773 2e61  tps://docs.aws.a
-000005e0: 6d61 7a6f 6e2e 636f 6d2f 616d 617a 6f6e  mazon.com/amazon
-000005f0: 6479 6e61 6d6f 6462 2f6c 6174 6573 742f  dynamodb/latest/
-00000600: 6465 7665 6c6f 7065 7267 7569 6465 2f45  developerguide/E
-00000610: 7870 7265 7373 696f 6e73 2e4f 7065 7261  xpressions.Opera
-00000620: 746f 7273 416e 6446 756e 6374 696f 6e73  torsAndFunctions
-00000630: 2e68 746d 6c0a 2020 2020 da03 6b65 79da  .html.    ..key.
-00000640: 0576 616c 7565 2902 da02 6571 da02 6e65  .value)...eq..ne
-00000650: da0a 636f 6d70 6172 6174 6f72 4e29 0872  ..comparatorN).r
-00000660: 1900 0000 721a 0000 0072 1b00 0000 da07  ....r....r......
-00000670: 5f5f 646f 635f 5f72 1c00 0000 721d 0000  __doc__r....r...
-00000680: 0072 0200 0000 7203 0000 0072 1500 0000  .r....r....r....
-00000690: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-000006a0: 2100 0000 1a00 0000 730a 0000 000a 0004  !.......s.......
-000006b0: 0108 0908 0110 0372 2100 0000 6300 0000  .......r!...c...
-000006c0: 0000 0000 0000 0000 0000 0000 0010 0000  ................
-000006d0: 0040 0000 0073 6801 0000 6500 5a01 6400  .@...sh...e.Z.d.
-000006e0: 5a02 6503 6a04 0901 0901 0901 0901 0901  Z.e.j...........
-000006f0: 641e 6402 6505 6403 6506 6505 1900 6404  d.d.e.d.e.e...d.
-00000700: 6506 6505 1900 6405 6506 6505 1900 6406  e.e...d.e.e...d.
-00000710: 6506 6507 6505 6508 6602 1900 1900 6407  e.e.e.e.f.....d.
-00000720: 6506 6509 6505 1900 1900 6408 650a 660e  e.e.e.....d.e.f.
-00000730: 6409 640a 8405 8301 5a0b 6503 6a04 0901  d.d.....Z.e.j...
-00000740: 641f 6402 6505 6403 6506 6505 1900 6408  d.d.e.d.e.e...d.
-00000750: 650a 6606 640b 640c 8405 8301 5a0c 6503  e.f.d.d.....Z.e.
-00000760: 6a04 0901 641f 640d 650a 640e 6505 640f  j...d.d.e.d.e.d.
-00000770: 6505 6410 6506 6505 1900 6408 650d 6505  e.d.e.e...d.e.e.
-00000780: 6505 6602 1900 660a 6411 6412 8405 8301  e.f...f.d.d.....
-00000790: 5a0e 6503 6a04 0901 641f 640d 650a 6410  Z.e.j...d.d.e.d.
-000007a0: 6506 6505 1900 6408 650f 6606 6413 6414  e.e...d.e.f.d.d.
-000007b0: 8405 8301 5a10 6503 6a04 0901 0901 6420  ....Z.e.j.....d 
-000007c0: 6415 6507 6505 6508 6602 1900 6403 6506  d.e.e.e.f...d.e.
-000007d0: 6505 1900 6416 6506 6507 6505 6505 6602  e...d.e.e.e.e.f.
-000007e0: 1900 1900 6408 6511 650a 1900 6608 6417  ....d.e.e...f.d.
-000007f0: 6418 8405 8301 5a12 6503 6a04 0901 0901  d.....Z.e.j.....
-00000800: 6420 640d 650a 6419 6507 6505 6508 6602  d d.e.d.e.e.e.f.
-00000810: 1900 641a 6506 6509 6513 1900 1900 6403  ..d.e.e.e.....d.
-00000820: 6506 6505 1900 641b 6506 6505 1900 6408  e.e...d.e.e...d.
-00000830: 650a 660c 641c 641d 8405 8301 5a14 6401  e.f.d.d.....Z.d.
-00000840: 5300 2921 da0e 4163 7469 6f6e 4465 6c65  S.)!..ActionDele
-00000850: 6761 7465 4eda 046e 616d 65da 066f 7267  gateN..name..org
-00000860: 5f69 64da 0a63 7265 6174 6564 5f62 79da  _id..created_by.
-00000870: 0b64 6573 6372 6970 7469 6f6e da08 6d65  .description..me
-00000880: 7461 6461 7461 da04 7461 6773 7211 0000  tadata..tagsr...
-00000890: 0063 0700 0000 0000 0000 0000 0000 0700  .c..............
-000008a0: 0000 0200 0000 4300 0000 f308 0000 0074  ......C........t
-000008b0: 0064 0183 0182 0129 024e da0d 6372 6561  .d.....).N..crea
-000008c0: 7465 5f61 6374 696f 6ea9 01da 134e 6f74  te_action....Not
-000008d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000008e0: 2907 7214 0000 0072 2900 0000 722a 0000  ).r....r)...r*..
-000008f0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00000900: 722e 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00000910: 1600 0000 7230 0000 002c 0000 0073 0200  ....r0...,...s..
-00000920: 0000 080a 7a1c 4163 7469 6f6e 4465 6c65  ....z.ActionDele
-00000930: 6761 7465 2e63 7265 6174 655f 6163 7469  gate.create_acti
-00000940: 6f6e 6303 0000 0000 0000 0000 0000 0003  onc.............
-00000950: 0000 0002 0000 0043 0000 0072 2f00 0000  .......C...r/...
-00000960: 2902 4eda 1967 6574 5f61 6374 696f 6e5f  ).N..get_action_
-00000970: 6279 5f70 7269 6d61 7279 5f6b 6579 7231  by_primary_keyr1
-00000980: 0000 0029 0372 1400 0000 7229 0000 0072  ...).r....r)...r
-00000990: 2a00 0000 7215 0000 0072 1500 0000 7216  *...r....r....r.
-000009a0: 0000 0072 3300 0000 3800 0000 7302 0000  ...r3...8...s...
-000009b0: 0008 047a 2841 6374 696f 6e44 656c 6567  ...z(ActionDeleg
-000009c0: 6174 652e 6765 745f 6163 7469 6f6e 5f62  ate.get_action_b
-000009d0: 795f 7072 696d 6172 795f 6b65 79da 0672  y_primary_key..r
-000009e0: 6563 6f72 64da 0a69 6d61 6765 5f6e 616d  ecord..image_nam
-000009f0: 65da 0969 6d61 6765 5f74 6167 da06 6361  e..image_tag..ca
-00000a00: 6c6c 6572 6305 0000 0000 0000 0000 0000  llerc...........
-00000a10: 0005 0000 0002 0000 0043 0000 0072 2f00  .........C...r/.
-00000a20: 0000 2902 4eda 1272 6567 6973 7465 725f  ..).N..register_
-00000a30: 636f 6e74 6169 6e65 7272 3100 0000 2905  containerr1...).
-00000a40: 7214 0000 0072 3400 0000 7235 0000 0072  r....r4...r5...r
-00000a50: 3600 0000 7237 0000 0072 1500 0000 7215  6...r7...r....r.
-00000a60: 0000 0072 1600 0000 7238 0000 003e 0000  ...r....r8...>..
-00000a70: 0073 0200 0000 0808 7a21 4163 7469 6f6e  .s......z!Action
-00000a80: 4465 6c65 6761 7465 2e72 6567 6973 7465  Delegate.registe
-00000a90: 725f 636f 6e74 6169 6e65 7263 0300 0000  r_containerc....
-00000aa0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000ab0: 4300 0000 722f 0000 0029 024e da1e 6765  C...r/...).N..ge
-00000ac0: 745f 7465 6d70 5f63 6f6e 7461 696e 6572  t_temp_container
-00000ad0: 5f63 7265 6465 6e74 6961 6c73 7231 0000  _credentialsr1..
-00000ae0: 0029 0372 1400 0000 7234 0000 0072 3700  .).r....r4...r7.
-00000af0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000b00: 0072 3900 0000 4800 0000 7302 0000 0008  .r9...H...s.....
-00000b10: 067a 2d41 6374 696f 6e44 656c 6567 6174  .z-ActionDelegat
-00000b20: 652e 6765 745f 7465 6d70 5f63 6f6e 7461  e.get_temp_conta
-00000b30: 696e 6572 5f63 7265 6465 6e74 6961 6c73  iner_credentials
-00000b40: da07 6669 6c74 6572 73da 0a70 6167 655f  ..filters..page_
-00000b50: 746f 6b65 6e63 0400 0000 0000 0000 0000  tokenc..........
-00000b60: 0000 0400 0000 0200 0000 4300 0000 722f  ..........C...r/
-00000b70: 0000 0029 024e da0d 7175 6572 795f 6163  ...).N..query_ac
-00000b80: 7469 6f6e 7372 3100 0000 2904 7214 0000  tionsr1...).r...
-00000b90: 0072 3a00 0000 722a 0000 0072 3b00 0000  .r:...r*...r;...
-00000ba0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000bb0: 3c00 0000 5000 0000 7302 0000 0008 077a  <...P...s......z
-00000bc0: 1c41 6374 696f 6e44 656c 6567 6174 652e  .ActionDelegate.
-00000bd0: 7175 6572 795f 6163 7469 6f6e 73da 0775  query_actions..u
-00000be0: 7064 6174 6573 da0a 636f 6e64 6974 696f  pdates..conditio
-00000bf0: 6e73 da0a 7570 6461 7465 645f 6279 6306  ns..updated_byc.
-00000c00: 0000 0000 0000 0000 0000 0006 0000 0002  ................
-00000c10: 0000 0043 0000 0072 2f00 0000 2902 4eda  ...C...r/...).N.
-00000c20: 0675 7064 6174 6572 3100 0000 2906 7214  .updater1...).r.
-00000c30: 0000 0072 3400 0000 723d 0000 0072 3e00  ...r4...r=...r>.
-00000c40: 0000 722a 0000 0072 3f00 0000 7215 0000  ..r*...r?...r...
-00000c50: 0072 1500 0000 7216 0000 0072 4000 0000  .r....r....r@...
-00000c60: 5900 0000 7302 0000 0008 097a 1541 6374  Y...s......z.Act
-00000c70: 696f 6e44 656c 6567 6174 652e 7570 6461  ionDelegate.upda
-00000c80: 7465 2905 4e4e 4e4e 4e72 1200 0000 2902  te).NNNNNr....).
-00000c90: 4e4e 2915 7219 0000 0072 1a00 0000 721b  NN).r....r....r.
-00000ca0: 0000 00da 0361 6263 da0e 6162 7374 7261  .....abc..abstra
-00000cb0: 6374 6d65 7468 6f64 721c 0000 0072 0400  ctmethodr....r..
-00000cc0: 0000 7220 0000 0072 0200 0000 da04 6c69  ..r ...r......li
-00000cd0: 7374 720b 0000 0072 3000 0000 7233 0000  str....r0...r3..
-00000ce0: 00da 0574 7570 6c65 7238 0000 0072 0c00  ...tupler8...r..
-00000cf0: 0000 7239 0000 0072 0600 0000 723c 0000  ..r9...r....r<..
-00000d00: 0072 2100 0000 7240 0000 0072 1500 0000  .r!...r@...r....
-00000d10: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000d20: 2800 0000 2b00 0000 73a2 0000 0008 0004  (...+...s.......
-00000d30: 0102 0402 0102 0102 0102 0104 f902 0202  ................
-00000d40: fe06 0302 fd06 0402 fc06 0502 fb0e 0602  ................
-00000d50: fa0a 0702 f902 080c f804 0b02 0204 ff02  ................
-00000d60: 0102 ff06 0102 ff02 020c fe04 0502 0604  ................
-00000d70: fb02 0202 fe02 0302 fd02 0402 fc06 0502  ................
-00000d80: fb0a 060c fa04 0902 0404 fd02 0202 fe06  ................
-00000d90: 0302 fd02 040c fc04 0702 0402 0104 fc0a  ................
-00000da0: 0202 fe06 0302 fd0e 0402 fc06 050c fb04  ................
-00000db0: 0802 0602 0104 fa02 0202 fe0a 0302 fd0a  ................
-00000dc0: 0402 fc06 0502 fb06 0602 fa02 0710 f972  ...............r
-00000dd0: 2800 0000 2914 7241 0000 0072 1e00 0000  (...).rA...r....
-00000de0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000df0: 0000 7204 0000 00da 0870 7964 616e 7469  ..r......pydanti
-00000e00: 63da 0a70 6167 696e 6174 696f 6e72 0600  c..paginationr..
-00000e10: 0000 da05 7365 7264 6572 0800 0000 da04  ....serder......
-00000e20: 7469 6d65 7209 0000 00da 0d61 6374 696f  timer......actio
-00000e30: 6e5f 7265 636f 7264 720b 0000 00da 0942  n_recordr......B
-00000e40: 6173 654d 6f64 656c 720c 0000 0072 2100  aseModelr....r!.
-00000e50: 0000 da03 4142 4372 2800 0000 7215 0000  ....ABCr(...r...
-00000e60: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000e70: da08 3c6d 6f64 756c 653e 0100 0000 7316  ..<module>....s.
-00000e80: 0000 0008 0008 0114 0108 020c 020c 010c  ................
-00000e90: 010c 0112 0312 0d16 11                   .........
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 6d05 5a05 0100 6400 6401 6c06 5a06 6403  m.Z...d.d.l.Z.d.
+00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6403 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000080: 0100 6407 6408 6c0d 6d0e 5a0e 0100 6409  ..d.d.l.m.Z...d.
+00000090: 640a 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
+000000a0: 0100 4700 640b 640c 8400 640c 6502 6a13  ..G.d.d...d.e.j.
+000000b0: 8303 5a14 4700 640d 640e 8400 640e 6506  ..Z.G.d.d...d.e.
+000000c0: 6a15 8303 5a16 4700 640f 6410 8400 6410  j...Z.G.d.d...d.
+000000d0: 6500 6a17 8303 5a18 6401 5300 2911 e900  e.j...Z.d.S.)...
+000000e0: 0000 004e 2902 da03 416e 79da 084f 7074  ...N)...Any..Opt
+000000f0: 696f 6e61 6ce9 0300 0000 2901 da0d 5061  ional.....)...Pa
+00000100: 6769 6e61 7465 644c 6973 74a9 01da 1670  ginatedList....p
+00000110: 7964 616e 7469 635f 6a73 6f6e 6162 6c65  ydantic_jsonable
+00000120: 5f64 6963 7429 01da 0675 7463 6e6f 77e9  _dict)...utcnow.
+00000130: 0200 0000 2901 da0a 4669 6c65 5265 636f  ....)...FileReco
+00000140: 7264 e901 0000 0029 03da 0d41 646d 696e  rd.....)...Admin
+00000150: 6973 7472 6174 6f72 da0d 4461 7461 7365  istrator..Datase
+00000160: 7452 6563 6f72 64da 0f53 746f 7261 6765  tRecord..Storage
+00000170: 4c6f 6361 7469 6f6e 6300 0000 0000 0000  Locationc.......
+00000180: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00000190: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000001a0: 5a03 6402 5a04 6403 5300 2904 da0a 4163  Z.d.Z.d.S.)...Ac
+000001b0: 6365 7373 4d6f 6465 da08 5265 6164 4f6e  cessMode..ReadOn
+000001c0: 6c79 da09 5265 6164 5772 6974 654e 2905  ly..ReadWriteN).
+000001d0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000001e0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000001f0: 6d65 5f5f 7210 0000 0072 1100 0000 a900  me__r....r......
+00000200: 7215 0000 0072 1500 0000 faf0 2f63 6f64  r....r....../cod
+00000210: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
+00000220: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
+00000230: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
+00000240: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
+00000250: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
+00000260: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
+00000270: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
+00000280: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
+00000290: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
+000002a0: 642f 726f 626f 746f 2d61 692f 726f 626f  d/roboto-ai/robo
+000002b0: 746f 2d68 6f73 7465 642d 6170 702f 7061  to-hosted-app/pa
+000002c0: 636b 6167 6573 2f72 6f62 6f74 6f5f 7364  ckages/roboto_sd
+000002d0: 6b2f 7372 632f 726f 626f 746f 5f73 646b  k/src/roboto_sdk
+000002e0: 2f64 6f6d 6169 6e2f 6461 7461 7365 7473  /domain/datasets
+000002f0: 2f64 656c 6567 6174 652e 7079 720f 0000  /delegate.pyr...
+00000300: 0013 0000 0073 0600 0000 0800 0401 0801  .....s..........
+00000310: 720f 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000320: 0000 0000 0000 0400 0000 4000 0000 7364  ..........@...sd
+00000330: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
+00000340: 0464 013c 0065 0365 0464 023c 0065 056a  .d.<.e.e.d.<.e.j
+00000350: 0565 0464 033c 0065 0365 0464 043c 0065  .e.d.<.e.e.d.<.e
+00000360: 0365 0464 053c 0065 0365 0464 063c 0064  .e.d.<.e.e.d.<.d
+00000370: 0765 0666 0264 0864 0984 045a 0764 0765  .e.f.d.d...Z.d.e
+00000380: 0865 0365 0966 0219 0066 0264 0a64 0b84  .e.e.f...f.d.d..
+00000390: 045a 0a64 0c53 0029 0dda 0b43 7265 6465  .Z.d.S.)...Crede
+000003a0: 6e74 6961 6c73 da0d 6163 6365 7373 5f6b  ntials..access_k
+000003b0: 6579 5f69 64da 0662 7563 6b65 74da 0a65  ey_id..bucket..e
+000003c0: 7870 6972 6174 696f 6eda 1173 6563 7265  xpiration..secre
+000003d0: 745f 6163 6365 7373 5f6b 6579 da0d 7365  t_access_key..se
+000003e0: 7373 696f 6e5f 746f 6b65 6eda 0f72 6571  ssion_token..req
+000003f0: 7569 7265 645f 7072 6566 6978 da06 7265  uired_prefix..re
+00000400: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
+00000410: 0001 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00000420: 0000 7400 8300 7c00 6a01 6b05 5300 a901  ..t...|.j.k.S...
+00000430: 4e29 0272 0800 0000 721a 0000 00a9 01da  N).r....r.......
+00000440: 0473 656c 6672 1500 0000 7215 0000 0072  .selfr....r....r
+00000450: 1600 0000 da0a 6973 5f65 7870 6972 6564  ......is_expired
+00000460: 2000 0000 7302 0000 000c 017a 1643 7265   ...s......z.Cre
+00000470: 6465 6e74 6961 6c73 2e69 735f 6578 7069  dentials.is_expi
+00000480: 7265 6463 0100 0000 0000 0000 0000 0000  redc............
+00000490: 0100 0000 0200 0000 4300 0000 7308 0000  ........C...s...
+000004a0: 0074 007c 0083 0153 0072 1f00 0000 7206  .t.|...S.r....r.
+000004b0: 0000 0072 2000 0000 7215 0000 0072 1500  ...r ...r....r..
+000004c0: 0000 7216 0000 00da 0774 6f5f 6469 6374  ..r......to_dict
+000004d0: 2300 0000 7302 0000 0008 017a 1343 7265  #...s......z.Cre
+000004e0: 6465 6e74 6961 6c73 2e74 6f5f 6469 6374  dentials.to_dict
+000004f0: 4e29 0b72 1200 0000 7213 0000 0072 1400  N).r....r....r..
+00000500: 0000 da03 7374 72da 0f5f 5f61 6e6e 6f74  ....str..__annot
+00000510: 6174 696f 6e73 5f5f da08 6461 7465 7469  ations__..dateti
+00000520: 6d65 da04 626f 6f6c 7222 0000 00da 0464  me..boolr".....d
+00000530: 6963 7472 0200 0000 7223 0000 0072 1500  ictr....r#...r..
+00000540: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000550: 0072 1700 0000 1800 0000 7312 0000 000a  .r........s.....
+00000560: 0008 0108 010a 0108 0108 0108 010e 021a  ................
+00000570: 0372 1700 0000 6300 0000 0000 0000 0000  .r....c.........
+00000580: 0000 0000 0000 0010 0000 0040 0000 0073  ...........@...s
+00000590: 2e01 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+000005a0: 6505 6a06 6401 6507 6a08 6401 6401 6401  e.j.d.e.j.d.d.d.
+000005b0: 6606 6402 6505 6403 6509 650a 650b 650c  f.d.e.d.e.e.e.e.
+000005c0: 6602 1900 1900 6404 6507 6405 6509 650d  f.....d.e.d.e.e.
+000005d0: 650b 1900 1900 6406 6509 650b 1900 6407  e.....d.e.e...d.
+000005e0: 6509 650b 1900 6408 650e 660e 6409 640a  e.e...d.e.f.d.d.
+000005f0: 8405 8301 5a0f 6503 6a04 0901 6419 640b  ....Z.e.j...d.d.
+00000600: 650b 6406 6509 650b 1900 6408 650e 6606  e.d.e.e...d.e.f.
+00000610: 640c 640d 8405 8301 5a10 6503 6a04 0901  d.d.....Z.e.j...
+00000620: 6419 640e 650e 640f 6511 6410 6509 650b  d.d.e.d.e.d.e.e.
+00000630: 1900 6408 6512 6608 6411 6412 8405 8301  ..d.e.f.d.d.....
+00000640: 5a13 6503 6a04 0901 0901 641a 640b 650b  Z.e.j.....d.d.e.
+00000650: 6406 6509 650b 1900 6413 6509 650a 650b  d.e.e...d.e.e.e.
+00000660: 650b 6602 1900 1900 6408 6514 6515 1900  e.f.....d.e.e...
+00000670: 6608 6414 6415 8405 8301 5a16 6503 6a04  f.d.d.....Z.e.j.
+00000680: 0901 0901 641a 6416 650a 650b 650c 6602  ....d.d.e.e.e.f.
+00000690: 1900 6406 6509 650b 1900 6413 6509 650a  ..d.e.e...d.e.e.
+000006a0: 650b 650b 6602 1900 1900 6408 6514 650e  e.e.f.....d.e.e.
+000006b0: 1900 6608 6417 6418 8405 8301 5a17 6401  ..f.d.d.....Z.d.
+000006c0: 5300 291b da0f 4461 7461 7365 7444 656c  S.)...DatasetDel
+000006d0: 6567 6174 654e da0d 6164 6d69 6e69 7374  egateN..administ
+000006e0: 7261 746f 72da 086d 6574 6164 6174 61da  rator..metadata.
+000006f0: 1073 746f 7261 6765 5f6c 6f63 6174 696f  .storage_locatio
+00000700: 6eda 0474 6167 73da 066f 7267 5f69 64da  n..tags..org_id.
+00000710: 0a63 7265 6174 6564 5f62 7972 1e00 0000  .created_byr....
+00000720: 6307 0000 0000 0000 0000 0000 0007 0000  c...............
+00000730: 0002 0000 0043 0000 00f3 0800 0000 7400  .....C........t.
+00000740: 6401 8301 8201 2902 4eda 0e63 7265 6174  d.....).N..creat
+00000750: 655f 6461 7461 7365 74a9 01da 134e 6f74  e_dataset....Not
+00000760: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00000770: 2907 7221 0000 0072 2a00 0000 722b 0000  ).r!...r*...r+..
+00000780: 0072 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
+00000790: 722f 0000 0072 1500 0000 7215 0000 0072  r/...r....r....r
+000007a0: 1600 0000 7231 0000 0028 0000 0073 0200  ....r1...(...s..
+000007b0: 0000 080a 7a1e 4461 7461 7365 7444 656c  ....z.DatasetDel
+000007c0: 6567 6174 652e 6372 6561 7465 5f64 6174  egate.create_dat
+000007d0: 6173 6574 da0a 6461 7461 7365 745f 6964  aset..dataset_id
+000007e0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+000007f0: 0002 0000 0043 0000 0072 3000 0000 2902  .....C...r0...).
+00000800: 4eda 1a67 6574 5f64 6174 6173 6574 5f62  N..get_dataset_b
+00000810: 795f 7072 696d 6172 795f 6b65 7972 3200  y_primary_keyr2.
+00000820: 0000 2903 7221 0000 0072 3400 0000 722e  ..).r!...r4...r.
+00000830: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000840: 0000 7235 0000 0034 0000 0073 0200 0000  ..r5...4...s....
+00000850: 0806 7a2a 4461 7461 7365 7444 656c 6567  ..z*DatasetDeleg
+00000860: 6174 652e 6765 745f 6461 7461 7365 745f  ate.get_dataset_
+00000870: 6279 5f70 7269 6d61 7279 5f6b 6579 da06  by_primary_key..
+00000880: 7265 636f 7264 da04 6d6f 6465 da06 6361  record..mode..ca
+00000890: 6c6c 6572 6304 0000 0000 0000 0000 0000  llerc...........
+000008a0: 0004 0000 0002 0000 0043 0000 0072 3000  .........C...r0.
+000008b0: 0000 2902 4eda 1967 6574 5f74 656d 706f  ..).N..get_tempo
+000008c0: 7261 7279 5f63 7265 6465 6e74 6961 6c73  rary_credentials
+000008d0: 7232 0000 0029 0472 2100 0000 7236 0000  r2...).r!...r6..
+000008e0: 0072 3700 0000 7238 0000 0072 1500 0000  .r7...r8...r....
+000008f0: 7215 0000 0072 1600 0000 7239 0000 003c  r....r....r9...<
+00000900: 0000 0073 0200 0000 0804 7a29 4461 7461  ...s......z)Data
+00000910: 7365 7444 656c 6567 6174 652e 6765 745f  setDelegate.get_
+00000920: 7465 6d70 6f72 6172 795f 6372 6564 656e  temporary_creden
+00000930: 7469 616c 73da 0a70 6167 655f 746f 6b65  tials..page_toke
+00000940: 6e63 0400 0000 0000 0000 0000 0000 0400  nc..............
+00000950: 0000 0200 0000 4300 0000 7230 0000 0029  ......C...r0...)
+00000960: 024e da0a 6c69 7374 5f66 696c 6573 7232  .N..list_filesr2
+00000970: 0000 0029 0472 2100 0000 7234 0000 0072  ...).r!...r4...r
+00000980: 2e00 0000 723a 0000 0072 1500 0000 7215  ....r:...r....r.
+00000990: 0000 0072 1600 0000 723b 0000 0042 0000  ...r....r;...B..
+000009a0: 00f3 0200 0000 0807 7a1a 4461 7461 7365  ........z.Datase
+000009b0: 7444 656c 6567 6174 652e 6c69 7374 5f66  tDelegate.list_f
+000009c0: 696c 6573 da07 6669 6c74 6572 7363 0400  iles..filtersc..
+000009d0: 0000 0000 0000 0000 0000 0400 0000 0200  ................
+000009e0: 0000 4300 0000 7230 0000 0029 024e da0e  ..C...r0...).N..
+000009f0: 7175 6572 795f 6461 7461 7365 7473 7232  query_datasetsr2
+00000a00: 0000 0029 0472 2100 0000 723d 0000 0072  ...).r!...r=...r
+00000a10: 2e00 0000 723a 0000 0072 1500 0000 7215  ....r:...r....r.
+00000a20: 0000 0072 1600 0000 723e 0000 004b 0000  ...r....r>...K..
+00000a30: 0072 3c00 0000 7a1e 4461 7461 7365 7444  .r<...z.DatasetD
+00000a40: 656c 6567 6174 652e 7175 6572 795f 6461  elegate.query_da
+00000a50: 7461 7365 7473 721f 0000 0029 024e 4e29  tasetsr....).NN)
+00000a60: 1872 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000a70: da03 6162 63da 0e61 6273 7472 6163 746d  ..abc..abstractm
+00000a80: 6574 686f 6472 0c00 0000 da06 526f 626f  ethodr......Robo
+00000a90: 746f 720e 0000 00da 0253 3372 0300 0000  tor......S3r....
+00000aa0: 7228 0000 0072 2400 0000 7202 0000 00da  r(...r$...r.....
+00000ab0: 046c 6973 7472 0d00 0000 7231 0000 0072  .listr....r1...r
+00000ac0: 3500 0000 720f 0000 0072 1700 0000 7239  5...r....r....r9
+00000ad0: 0000 0072 0500 0000 720a 0000 0072 3b00  ...r....r....r;.
+00000ae0: 0000 723e 0000 0072 1500 0000 7215 0000  ..r>...r....r...
+00000af0: 0072 1500 0000 7216 0000 0072 2900 0000  .r....r....r)...
+00000b00: 2700 0000 7386 0000 0008 0004 0104 0302  '...s...........
+00000b10: 0104 0102 0102 0102 0104 f902 0202 fe0e  ................
+00000b20: 0302 fd02 0402 fc0a 0502 fb06 0602 fa06  ................
+00000b30: 0702 f902 080c f804 0b02 0404 fd02 0202  ................
+00000b40: fe06 0302 fd02 040c fc04 0702 0204 ff02  ................
+00000b50: 0102 ff02 0102 ff06 0102 ff02 020c fe04  ................
+00000b60: 0502 0402 0104 fc02 0202 fe06 0302 fd0e  ................
+00000b70: 0402 fc06 050c fb04 0802 0402 0104 fc0a  ................
+00000b80: 0202 fe06 0302 fd0e 0402 fc06 0510 fb72  ...............r
+00000b90: 2900 0000 2919 723f 0000 0072 2600 0000  )...).r?...r&...
+00000ba0: da04 656e 756d da06 7479 7069 6e67 7202  ..enum..typingr.
+00000bb0: 0000 0072 0300 0000 da08 7079 6461 6e74  ...r......pydant
+00000bc0: 6963 da0a 7061 6769 6e61 7469 6f6e 7205  ic..paginationr.
+00000bd0: 0000 00da 0573 6572 6465 7207 0000 00da  .....serder.....
+00000be0: 0474 696d 6572 0800 0000 da05 6669 6c65  .timer......file
+00000bf0: 7372 0a00 0000 7236 0000 0072 0c00 0000  sr....r6...r....
+00000c00: 720d 0000 0072 0e00 0000 da04 456e 756d  r....r......Enum
+00000c10: 720f 0000 00da 0942 6173 654d 6f64 656c  r......BaseModel
+00000c20: 7217 0000 00da 0341 4243 7229 0000 0072  r......ABCr)...r
+00000c30: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000c40: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000c50: 0073 1a00 0000 0800 0801 0801 1001 0802  .s..............
+00000c60: 0c02 0c01 0c01 0c01 1401 1207 1205 160f  ................
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 5168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,324 +1,342 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 3014 0000  o.......Ms.d0...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 fd15 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
-00000050: 6404 6c00 6d05 5a05 6d06 5a06 6d07 5a07  d.l.m.Z.m.Z.m.Z.
-00000060: 6d08 5a08 0100 6403 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000050: 6404 6c05 6d06 5a06 0100 6403 6405 6c00  d.l.m.Z...d.d.l.
+00000060: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6403 6406 6c0b 6d0c 5a0c 0100 6403  ..d.d.l.m.Z...d.
-00000080: 6407 6c0d 6d0e 5a0e 0100 6408 6409 6c0f  d.l.m.Z...d.d.l.
-00000090: 6d10 5a10 6d11 5a11 6d12 5a12 0100 6408  m.Z.m.Z.m.Z...d.
-000000a0: 640a 6c13 6d14 5a14 6d15 5a15 0100 6408  d.l.m.Z.m.Z...d.
-000000b0: 640b 6c16 6d17 5a17 0100 6408 640c 6c18  d.l.m.Z...d.d.l.
-000000c0: 6d19 5a19 0100 650a 8300 5a1a 4700 640d  m.Z...e...Z.G.d.
-000000d0: 640e 8400 640e 6510 8303 5a1b 6401 5300  d...d.e...Z.d.S.
-000000e0: 290f e900 0000 004e 2902 da03 416e 79da  )......N)...Any.
-000000f0: 084f 7074 696f 6e61 6ce9 0300 0000 2904  .Optional.....).
-00000100: da13 4f52 475f 4f56 4552 5249 4445 5f48  ..ORG_OVERRIDE_H
-00000110: 4541 4445 52da 1455 5345 525f 4f56 4552  EADER..USER_OVER
-00000120: 5249 4445 5f48 4541 4445 52da 0b43 6c69  RIDE_HEADER..Cli
-00000130: 656e 7445 7272 6f72 da0a 4874 7470 436c  entError..HttpCl
-00000140: 6965 6e74 2901 da0e 6465 6661 756c 745f  ient)...default_
-00000150: 6c6f 6767 6572 2901 da0d 5061 6769 6e61  logger)...Pagina
-00000160: 7465 644c 6973 7429 01da 1670 7964 616e  tedList)...pydan
-00000170: 7469 635f 6a73 6f6e 6162 6c65 5f64 6963  tic_jsonable_dic
-00000180: 74e9 0100 0000 2903 da0e 4163 7469 6f6e  t.....)...Action
-00000190: 4465 6c65 6761 7465 da14 436f 6e74 6169  Delegate..Contai
-000001a0: 6e65 7243 7265 6465 6e74 6961 6c73 da0f  nerCredentials..
-000001b0: 5570 6461 7465 436f 6e64 6974 696f 6e29  UpdateCondition)
-000001c0: 02da 1343 7265 6174 6541 6374 696f 6e52  ...CreateActionR
-000001d0: 6571 7565 7374 da13 5570 6461 7465 4163  equest..UpdateAc
-000001e0: 7469 6f6e 5265 7175 6573 7429 01da 0c41  tionRequest)...A
-000001f0: 6374 696f 6e52 6563 6f72 6429 01da 2141  ctionRecord)..!A
-00000200: 6374 696f 6e55 7064 6174 6543 6f6e 6469  ctionUpdateCondi
-00000210: 7469 6f6e 4368 6563 6b46 6169 6c75 7265  tionCheckFailure
-00000220: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000230: 000f 0000 0000 0000 0073 a201 0000 6500  .........s....e.
-00000240: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
-00000250: 6402 3c00 6506 6505 6403 3c00 6404 6506  d.<.e.e.d.<.d.e.
-00000260: 6405 6504 6406 6407 6606 8700 6601 6408  d.e.d.d.f...f.d.
-00000270: 6409 840c 5a07 0907 6428 640a 6508 6506  d...Z...d(d.e.e.
-00000280: 1900 640b 6508 6506 1900 6406 6509 6506  ..d.e.e...d.e.e.
-00000290: 6506 6602 1900 6606 640c 640d 8405 5a0a  e.f...f.d.d...Z.
-000002a0: 0907 0907 0907 0907 0907 6429 640e 6506  ..........d)d.e.
-000002b0: 640a 6508 6506 1900 640f 6508 6506 1900  d.e.e...d.e.e...
-000002c0: 6410 6508 6506 1900 6411 6508 6509 6506  d.e.e...d.e.e.e.
-000002d0: 650b 6602 1900 1900 6412 6508 650c 6506  e.f.....d.e.e.e.
-000002e0: 1900 1900 6406 650d 660e 6413 6414 8405  ....d.e.f.d.d...
-000002f0: 5a0e 0907 642a 640e 6506 640a 6508 6506  Z...d*d.e.d.e.e.
-00000300: 1900 6406 650d 6606 6415 6416 8405 5a0f  ..d.e.f.d.d...Z.
-00000310: 0907 642a 6417 650d 6418 6506 6419 6506  ..d*d.e.d.e.d.e.
-00000320: 641a 6508 6506 1900 6406 6510 6506 6506  d.e.e...d.e.e.e.
-00000330: 6602 1900 660a 641b 641c 8405 5a11 0907  f...f.d.d...Z...
-00000340: 642a 6417 650d 641a 6508 6506 1900 6406  d*d.e.d.e.e...d.
-00000350: 6512 6606 641d 641e 8405 5a13 0907 0907  e.f.d.d...Z.....
-00000360: 6428 641f 6509 6506 650b 6602 1900 640a  d(d.e.e.e.f...d.
-00000370: 6508 6506 1900 6420 6508 6509 6506 6506  e.e...d e.e.e.e.
-00000380: 6602 1900 1900 6406 6514 650d 1900 6608  f.....d.e.e...f.
-00000390: 6421 6422 8405 5a15 0907 0907 6428 6417  d!d"..Z.....d(d.
-000003a0: 650d 6423 6509 6506 650b 6602 1900 6424  e.d#e.e.e.f...d$
-000003b0: 6508 650c 6516 1900 1900 640a 6508 6506  e.e.e.....d.e.e.
-000003c0: 1900 6425 6508 6506 1900 6406 650d 660c  ..d%e.e...d.e.f.
-000003d0: 6426 6427 8405 5a17 8700 0400 5a18 5300  d&d'..Z.....Z.S.
-000003e0: 292b da12 4163 7469 6f6e 4874 7470 4465  )+..ActionHttpDe
-000003f0: 6c65 6761 7465 7a47 0a20 2020 2055 7365  legatezG.    Use
-00000400: 2069 6e20 616e 7920 636f 6e74 6578 7420   in any context 
-00000410: 7468 6174 2064 6f65 7320 6e6f 7420 6861  that does not ha
-00000420: 7665 2064 6972 6563 7420 6461 7461 6261  ve direct databa
-00000430: 7365 2061 6363 6573 732e 0a20 2020 20da  se access..    .
-00000440: 205f 4163 7469 6f6e 4874 7470 4465 6c65   _ActionHttpDele
-00000450: 6761 7465 5f5f 6874 7470 5f63 6c69 656e  gate__http_clien
-00000460: 74da 2c5f 4163 7469 6f6e 4874 7470 4465  t.,_ActionHttpDe
-00000470: 6c65 6761 7465 5f5f 726f 626f 746f 5f73  legate__roboto_s
-00000480: 6572 7669 6365 5f62 6173 655f 7572 6cda  ervice_base_url.
-00000490: 1772 6f62 6f74 6f5f 7365 7276 6963 655f  .roboto_service_
-000004a0: 6261 7365 5f75 726c da0b 6874 7470 5f63  base_url..http_c
-000004b0: 6c69 656e 74da 0672 6574 7572 6e4e 6303  lient..returnNc.
-000004c0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-000004d0: 0000 0003 0000 0073 1a00 0000 7400 8300  .......s....t...
-000004e0: a001 a100 0100 7c02 7c00 5f02 7c01 7c00  ......|.|._.|.|.
-000004f0: 5f03 6400 5300 a901 4e29 04da 0573 7570  _.d.S...N)...sup
-00000500: 6572 da08 5f5f 696e 6974 5f5f 7215 0000  er..__init__r...
-00000510: 0072 1600 0000 2903 da04 7365 6c66 7217  .r....)...selfr.
-00000520: 0000 0072 1800 0000 a901 da09 5f5f 636c  ...r........__cl
-00000530: 6173 735f 5fa9 00fa fb2f 636f 6465 6275  ass__..../codebu
-00000540: 696c 642f 6f75 7470 7574 2f73 7263 3334  ild/output/src34
-00000550: 3937 3236 3836 3730 2f73 7263 2f63 6f64  97268670/src/cod
-00000560: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
-00000570: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
-00000580: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
-00000590: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
-000005a0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
-000005b0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
-000005c0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
-000005d0: 6f62 6f74 6f2d 6169 2f72 6f62 6f74 6f2d  oboto-ai/roboto-
-000005e0: 686f 7374 6564 2d61 7070 2f70 6163 6b61  hosted-app/packa
-000005f0: 6765 732f 726f 626f 746f 5f73 646b 2f73  ges/roboto_sdk/s
-00000600: 7263 2f72 6f62 6f74 6f5f 7364 6b2f 646f  rc/roboto_sdk/do
-00000610: 6d61 696e 2f61 6374 696f 6e73 2f61 6374  main/actions/act
-00000620: 696f 6e5f 6874 7470 5f64 656c 6567 6174  ion_http_delegat
-00000630: 652e 7079 721c 0000 0027 0000 0073 0600  e.pyr....'...s..
-00000640: 0000 0a01 0601 0a01 7a1b 4163 7469 6f6e  ........z.Action
-00000650: 4874 7470 4465 6c65 6761 7465 2e5f 5f69  HttpDelegate.__i
-00000660: 6e69 745f 5fda 066f 7267 5f69 64da 0775  nit__..org_id..u
-00000670: 7365 725f 6964 6303 0000 0000 0000 0000  ser_idc.........
-00000680: 0000 0004 0000 0003 0000 0043 0000 0073  ...........C...s
-00000690: 2400 0000 6401 6402 6901 7d03 7c01 720a  $...d.d.i.}.|.r.
-000006a0: 7c01 7c03 7400 3c00 7c02 7210 7c02 7c03  |.|.t.<.|.r.|.|.
-000006b0: 7401 3c00 7c03 5300 2903 4e7a 0c43 6f6e  t.<.|.S.).Nz.Con
-000006c0: 7465 6e74 2d54 7970 657a 1061 7070 6c69  tent-Typez.appli
-000006d0: 6361 7469 6f6e 2f6a 736f 6e29 0272 0500  cation/json).r..
-000006e0: 0000 7206 0000 0029 0472 1d00 0000 7222  ..r....).r....r"
-000006f0: 0000 0072 2300 0000 da07 6865 6164 6572  ...r#.....header
-00000700: 7372 2000 0000 7220 0000 0072 2100 0000  sr ...r ...r!...
-00000710: 7224 0000 002c 0000 0073 0c00 0000 0803  r$...,...s......
-00000720: 0401 0801 0401 0801 0401 7a1a 4163 7469  ..........z.Acti
-00000730: 6f6e 4874 7470 4465 6c65 6761 7465 2e68  onHttpDelegate.h
-00000740: 6561 6465 7273 da04 6e61 6d65 da0a 6372  eaders..name..cr
-00000750: 6561 7465 645f 6279 da0b 6465 7363 7269  eated_by..descri
-00000760: 7074 696f 6eda 086d 6574 6164 6174 61da  ption..metadata.
-00000770: 0474 6167 7363 0700 0000 0000 0000 0000  .tagsc..........
-00000780: 0000 0a00 0000 0700 0000 4300 0000 7352  ..........C...sR
-00000790: 0000 007c 006a 009b 0064 019d 027d 0774  ...|.j...d...}.t
-000007a0: 017c 017c 047c 057c 0664 028d 047d 087c  .|.|.|.|.d...}.|
-000007b0: 006a 026a 037c 0774 047c 0864 0364 048d  .j.j.|.t.|.d.d..
-000007c0: 027c 00a0 057c 027c 03a1 0264 058d 037d  .|...|.|...d...}
-000007d0: 0974 06a0 077c 096a 0864 0667 0164 078d  .t...|.j.d.g.d..
-000007e0: 01a1 0153 0029 084e 7a0b 2f76 312f 6163  ...S.).Nz./v1/ac
-000007f0: 7469 6f6e 7329 0472 2500 0000 7227 0000  tions).r%...r'..
-00000800: 0072 2800 0000 7229 0000 0054 2901 da0c  .r(...r)...T)...
-00000810: 6578 636c 7564 655f 6e6f 6e65 a902 da04  exclude_none....
-00000820: 6461 7461 7224 0000 0072 2c00 0000 a901  datar$...r,.....
-00000830: da09 6a73 6f6e 5f70 6174 6829 0972 1600  ..json_path).r..
-00000840: 0000 7210 0000 0072 1500 0000 da04 706f  ..r....r......po
-00000850: 7374 720b 0000 0072 2400 0000 7212 0000  str....r$...r...
-00000860: 00da 0970 6172 7365 5f6f 626a da09 6672  ...parse_obj..fr
-00000870: 6f6d 5f6a 736f 6e29 0a72 1d00 0000 7225  om_json).r....r%
-00000880: 0000 0072 2200 0000 7226 0000 0072 2700  ...r"...r&...r'.
-00000890: 0000 7228 0000 0072 2900 0000 da03 7572  ..r(...r).....ur
-000008a0: 6cda 0c72 6571 7565 7374 5f62 6f64 79da  l..request_body.
-000008b0: 0872 6573 706f 6e73 6572 2000 0000 7220  .responser ...r 
-000008c0: 0000 0072 2100 0000 da0d 6372 6561 7465  ...r!.....create
-000008d0: 5f61 6374 696f 6e36 0000 0073 1a00 0000  _action6...s....
-000008e0: 0c09 0201 0201 0201 0201 0201 06fc 0606  ................
-000008f0: 0201 0a01 0a01 06fd 1405 7a20 4163 7469  ..........z Acti
-00000900: 6f6e 4874 7470 4465 6c65 6761 7465 2e63  onHttpDelegate.c
-00000910: 7265 6174 655f 6163 7469 6f6e 6303 0000  reate_actionc...
-00000920: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-00000930: 0043 0000 0073 3a00 0000 7c00 6a00 9b00  .C...s:...|.j...
-00000940: 6401 7c01 9b00 9d03 7d03 7c00 6a01 6a02  d.|.....}.|.j.j.
-00000950: 7c03 7c00 a003 7c02 a101 6402 8d02 7d04  |.|...|...d...}.
-00000960: 7404 a005 7c04 6a06 6403 6701 6404 8d01  t...|.j.d.g.d...
-00000970: a101 5300 2905 4efa 0c2f 7631 2f61 6374  ..S.).N../v1/act
-00000980: 696f 6e73 2fa9 0172 2400 0000 722c 0000  ions/..r$...r,..
-00000990: 0072 2d00 0000 2907 7216 0000 0072 1500  .r-...).r....r..
-000009a0: 0000 da03 6765 7472 2400 0000 7212 0000  ....getr$...r...
-000009b0: 0072 3000 0000 7231 0000 0029 0572 1d00  .r0...r1...).r..
-000009c0: 0000 7225 0000 0072 2200 0000 7232 0000  ..r%...r"...r2..
-000009d0: 00da 0372 6573 7220 0000 0072 2000 0000  ...resr ...r ...
-000009e0: 7221 0000 00da 1967 6574 5f61 6374 696f  r!.....get_actio
-000009f0: 6e5f 6279 5f70 7269 6d61 7279 5f6b 6579  n_by_primary_key
-00000a00: 4d00 0000 7306 0000 0010 0316 0114 017a  M...s..........z
-00000a10: 2c41 6374 696f 6e48 7474 7044 656c 6567  ,ActionHttpDeleg
-00000a20: 6174 652e 6765 745f 6163 7469 6f6e 5f62  ate.get_action_b
-00000a30: 795f 7072 696d 6172 795f 6b65 79da 0672  y_primary_key..r
-00000a40: 6563 6f72 64da 0a69 6d61 6765 5f6e 616d  ecord..image_nam
-00000a50: 65da 0969 6d61 6765 5f74 6167 da06 6361  e..image_tag..ca
-00000a60: 6c6c 6572 6305 0000 0000 0000 0000 0000  llerc...........
-00000a70: 0009 0000 0006 0000 0043 0000 0073 5600  .........C...sV.
-00000a80: 0000 7c00 6a00 9b00 6401 7c01 6a01 9b00  ..|.j...d.|.j...
-00000a90: 6402 9d04 7d05 7c02 7c03 6403 9c02 7d06  d...}.|.|.d...}.
-00000aa0: 7c00 6a02 6a03 7c05 7c06 7c00 6a04 7c04  |.j.j.|.|.|.j.|.
-00000ab0: 6404 8d01 6405 8d03 7d07 7c07 6a05 6406  d...d...}.|.j.d.
-00000ac0: 6701 6407 8d01 7d08 7c08 6408 1900 7c08  g.d...}.|.d...|.
-00000ad0: 6409 1900 6602 5300 290a 4e72 3600 0000  d...f.S.).Nr6...
-00000ae0: 7a0a 2f63 6f6e 7461 696e 6572 2902 723c  z./container).r<
-00000af0: 0000 0072 3d00 0000 a901 7223 0000 0072  ...r=.....r#...r
-00000b00: 2b00 0000 722c 0000 0072 2d00 0000 5a0e  +...r,...r-...Z.
-00000b10: 7265 706f 7369 746f 7279 5f75 7269 5a09  repository_uriZ.
-00000b20: 696d 6167 655f 7572 6929 0672 1600 0000  image_uri).r....
-00000b30: 7225 0000 0072 1500 0000 da03 7075 7472  r%...r......putr
-00000b40: 2400 0000 7231 0000 0029 0972 1d00 0000  $...r1...).r....
-00000b50: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
-00000b60: 3e00 0000 7232 0000 0072 2c00 0000 7239  >...r2...r,...r9
-00000b70: 0000 005a 0a70 6172 7365 645f 7265 7372  ...Z.parsed_resr
-00000b80: 2000 0000 7220 0000 0072 2100 0000 da12   ...r ...r!.....
-00000b90: 7265 6769 7374 6572 5f63 6f6e 7461 696e  register_contain
-00000ba0: 6572 5400 0000 7312 0000 0014 0702 0202  erT...s.........
-00000bb0: 0106 fe06 050e 0106 ff0e 0310 017a 2541  .............z%A
-00000bc0: 6374 696f 6e48 7474 7044 656c 6567 6174  ctionHttpDelegat
-00000bd0: 652e 7265 6769 7374 6572 5f63 6f6e 7461  e.register_conta
-00000be0: 696e 6572 6303 0000 0000 0000 0000 0000  inerc...........
-00000bf0: 0005 0000 0005 0000 0043 0000 0073 4000  .........C...s@.
-00000c00: 0000 7c00 6a00 9b00 6401 7c01 6a01 9b00  ..|.j...d.|.j...
-00000c10: 6402 9d04 7d03 7c00 6a02 6a03 7c03 7c00  d...}.|.j.j.|.|.
-00000c20: 6a04 7c02 6403 8d01 6404 8d02 7d04 7405  j.|.d...d...}.t.
-00000c30: a006 7c04 6a07 6405 6701 6406 8d01 a101  ..|.j.d.g.d.....
-00000c40: 5300 2907 4e72 3600 0000 7a16 2f63 6f6e  S.).Nr6...z./con
-00000c50: 7461 696e 6572 2f63 7265 6465 6e74 6961  tainer/credentia
-00000c60: 6c73 723f 0000 0072 3700 0000 722c 0000  lsr?...r7...r,..
-00000c70: 0072 2d00 0000 2908 7216 0000 0072 2500  .r-...).r....r%.
-00000c80: 0000 7215 0000 0072 3800 0000 7224 0000  ..r....r8...r$..
-00000c90: 0072 0e00 0000 7230 0000 0072 3100 0000  .r....r0...r1...
-00000ca0: 2905 721d 0000 0072 3b00 0000 723e 0000  ).r....r;...r>..
-00000cb0: 0072 3200 0000 7239 0000 0072 2000 0000  .r2...r9...r ...
-00000cc0: 7220 0000 0072 2100 0000 da1e 6765 745f  r ...r!.....get_
-00000cd0: 7465 6d70 5f63 6f6e 7461 696e 6572 5f63  temp_container_c
-00000ce0: 7265 6465 6e74 6961 6c73 6700 0000 7306  redentialsg...s.
-00000cf0: 0000 0014 0518 0114 017a 3141 6374 696f  .........z1Actio
-00000d00: 6e48 7474 7044 656c 6567 6174 652e 6765  nHttpDelegate.ge
-00000d10: 745f 7465 6d70 5f63 6f6e 7461 696e 6572  t_temp_container
-00000d20: 5f63 7265 6465 6e74 6961 6c73 da07 6669  _credentials..fi
-00000d30: 6c74 6572 73da 0a70 6167 655f 746f 6b65  lters..page_toke
-00000d40: 6e63 0400 0000 0000 0000 0000 0000 0800  nc..............
-00000d50: 0000 0600 0000 4300 0000 736c 0000 007c  ......C...sl...|
-00000d60: 0372 067c 037c 0164 013c 0074 00a0 0174  .r.|.|.d.<.t...t
-00000d70: 00a0 027c 01a1 01a1 017d 047c 006a 039b  ...|.....}.|.j..
-00000d80: 0064 029d 027d 057c 006a 046a 057c 057c  .d...}.|.j.j.|.|
-00000d90: 047c 00a0 067c 02a1 0164 038d 037d 067c  .|...|...d...}.|
-00000da0: 066a 0764 0467 0164 058d 017d 0774 0864  .j.d.g.d...}.t.d
-00000db0: 0664 0784 007c 0764 0819 0044 0083 017c  .d...|.d...D...|
-00000dc0: 0764 0919 0064 0a8d 0253 0029 0b4e 7244  .d...d...S.).NrD
-00000dd0: 0000 007a 112f 7631 2f61 6374 696f 6e73  ...z./v1/actions
-00000de0: 2f71 7565 7279 722b 0000 0072 2c00 0000  /queryr+...r,...
-00000df0: 722d 0000 0063 0100 0000 0000 0000 0000  r-...c..........
-00000e00: 0000 0200 0000 0500 0000 5300 0000 7316  ..........S...s.
-00000e10: 0000 0067 007c 005d 077d 0174 00a0 017c  ...g.|.].}.t...|
-00000e20: 01a1 0191 0271 0253 0072 2000 0000 2902  .....q.S.r ...).
-00000e30: 7212 0000 0072 3000 0000 2902 da02 2e30  r....r0...)....0
-00000e40: 5a07 6461 7461 7365 7472 2000 0000 7220  Z.datasetr ...r 
-00000e50: 0000 0072 2100 0000 da0a 3c6c 6973 7463  ...r!.....<listc
-00000e60: 6f6d 703e 8000 0000 7306 0000 0006 000a  omp>....s.......
-00000e70: 0106 ff7a 3441 6374 696f 6e48 7474 7044  ...z4ActionHttpD
-00000e80: 656c 6567 6174 652e 7175 6572 795f 6163  elegate.query_ac
-00000e90: 7469 6f6e 732e 3c6c 6f63 616c 733e 2e3c  tions.<locals>.<
-00000ea0: 6c69 7374 636f 6d70 3eda 0569 7465 6d73  listcomp>..items
-00000eb0: da0a 6e65 7874 5f74 6f6b 656e 2902 7247  ..next_token).rG
-00000ec0: 0000 0072 4800 0000 2909 da04 6a73 6f6e  ...rH...)...json
-00000ed0: da05 6c6f 6164 73da 0564 756d 7073 7216  ..loads..dumpsr.
-00000ee0: 0000 0072 1500 0000 722f 0000 0072 2400  ...r....r/...r$.
-00000ef0: 0000 7231 0000 0072 0a00 0000 2908 721d  ..r1...r....).r.
-00000f00: 0000 0072 4300 0000 7222 0000 0072 4400  ...rC...r"...rD.
-00000f10: 0000 5a0c 7361 6665 5f66 696c 7465 7273  ..Z.safe_filters
-00000f20: 7232 0000 0072 3900 0000 5a0c 756e 6d61  r2...r9...Z.unma
-00000f30: 7273 6861 6c6c 6564 7220 0000 0072 2000  rshalledr ...r .
-00000f40: 0000 7221 0000 00da 0d71 7565 7279 5f61  ..r!.....query_a
-00000f50: 6374 696f 6e73 7000 0000 731c 0000 0004  ctionsp...s.....
-00000f60: 0608 0110 020c 0106 010c 0106 ff0e 0302  ................
-00000f70: 0106 0106 0104 ff06 0306 fc7a 2041 6374  ...........z Act
-00000f80: 696f 6e48 7474 7044 656c 6567 6174 652e  ionHttpDelegate.
-00000f90: 7175 6572 795f 6163 7469 6f6e 73da 0775  query_actions..u
-00000fa0: 7064 6174 6573 da0a 636f 6e64 6974 696f  pdates..conditio
-00000fb0: 6e73 da0a 7570 6461 7465 645f 6279 6306  ns..updated_byc.
-00000fc0: 0000 0000 0000 0000 0000 000a 0000 000a  ................
-00000fd0: 0000 0043 0000 0073 9400 0000 7c00 6a00  ...C...s....|.j.
-00000fe0: 9b00 6401 7c01 6a01 9b00 9d03 7d06 7402  ..d.|.j.....}.t.
-00000ff0: 7c02 7c03 6400 7501 7211 7c03 6e01 6700  |.|.d.u.r.|.n.g.
-00001000: 6402 8d02 7d07 7a1a 7c00 6a03 6a04 7c06  d...}.z.|.j.j.|.
-00001010: 7c07 a005 a100 7c00 a006 7c04 7c05 a102  |.....|...|.|...
-00001020: 6403 8d03 7d08 7407 a008 7c08 6a09 6404  d...}.t...|.j.d.
-00001030: 6701 6405 8d01 a101 5700 5300 0400 740a  g.d.....W.S...t.
-00001040: 7949 0100 7d09 0100 7a0e 7c09 6a0b 740c  yI..}...z.|.j.t.
-00001050: 6a0d 6a0e 6b02 7244 740f 7c09 6a10 8301  j.j.k.rDt.|.j...
-00001060: 6400 8202 8200 6400 7d09 7e09 7701 7700  d.....d.}.~.w.w.
-00001070: 2906 4e72 3600 0000 2902 724d 0000 0072  ).Nr6...).rM...r
-00001080: 4e00 0000 722b 0000 0072 2c00 0000 722d  N...r+...r,...r-
-00001090: 0000 0029 1172 1600 0000 7225 0000 0072  ...).r....r%...r
-000010a0: 1100 0000 7215 0000 00da 0570 6174 6368  ....r......patch
-000010b0: da04 6469 6374 7224 0000 0072 1200 0000  ..dictr$...r....
-000010c0: 7230 0000 0072 3100 0000 7207 0000 00da  r0...r1...r.....
-000010d0: 0673 7461 7475 73da 0468 7474 70da 0a48  .status..http..H
-000010e0: 5454 5053 7461 7475 73da 0843 4f4e 464c  TTPStatus..CONFL
-000010f0: 4943 5472 1300 0000 da03 6d73 6729 0a72  ICTr......msg).r
-00001100: 1d00 0000 723b 0000 0072 4d00 0000 724e  ....r;...rM...rN
-00001110: 0000 0072 2200 0000 724f 0000 0072 3200  ...r"...rO...r2.
-00001120: 0000 da07 7061 796c 6f61 6472 3900 0000  ....payloadr9...
-00001130: da03 6578 6372 2000 0000 7220 0000 0072  ..excr ...r ...r
-00001140: 2100 0000 da06 7570 6461 7465 8600 0000  !.....update....
-00001150: 7320 0000 0012 0802 0102 010e 0106 fe02  s ..............
-00001160: 0406 0112 0106 ff16 030e 010e 010c 0102  ................
-00001170: 0108 8002 fd7a 1941 6374 696f 6e48 7474  .....z.ActionHtt
-00001180: 7044 656c 6567 6174 652e 7570 6461 7465  pDelegate.update
-00001190: 2902 4e4e 2905 4e4e 4e4e 4e72 1a00 0000  ).NN).NNNNNr....
-000011a0: 2919 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000011b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000011c0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000011d0: 0800 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
-000011e0: 6f6e 735f 5fda 0373 7472 721c 0000 0072  ons__..strr....r
-000011f0: 0300 0000 7251 0000 0072 2400 0000 7202  ....rQ...r$...r.
-00001200: 0000 00da 046c 6973 7472 1200 0000 7235  .....listr....r5
-00001210: 0000 0072 3a00 0000 da05 7475 706c 6572  ...r:.....tupler
-00001220: 4100 0000 720e 0000 0072 4200 0000 720a  A...r....rB...r.
-00001230: 0000 0072 4c00 0000 720f 0000 0072 5900  ...rL...r....rY.
-00001240: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00001250: 5f72 2000 0000 7220 0000 0072 1e00 0000  _r ...r ...r....
-00001260: 7221 0000 0072 1400 0000 1f00 0000 73ae  r!...r........s.
-00001270: 0000 000a 0004 0108 0408 011a 0202 0604  ................
-00001280: ff06 0102 ff06 0102 ff0a 020a fe02 0d02  ................
-00001290: 0102 0102 0102 0104 f902 0202 fe06 0302  ................
-000012a0: fd06 0402 fc06 0502 fb0e 0602 fa0a 0702  ................
-000012b0: f902 080a f802 1804 ff02 0102 ff06 0102  ................
-000012c0: ff02 020a fe02 0c04 fb02 0202 fe02 0302  ................
-000012d0: fd02 0402 fc06 0502 fb0a 060a fa02 1604  ................
-000012e0: fd02 0202 fe06 0302 fd02 040a fc02 0c02  ................
-000012f0: 0104 fc0a 0202 fe06 0302 fd0e 0402 fc06  ................
-00001300: 050a fb02 1b02 0104 fa02 0202 fe0a 0302  ................
-00001310: fd0a 0402 fc06 0502 fb06 0602 fa02 0712  ................
-00001320: f972 1400 0000 291c 7253 0000 0072 4900  .r....).rS...rI.
-00001330: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
-00001340: 0300 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00001350: 0000 0072 0800 0000 da07 6c6f 6767 696e  ...r......loggin
-00001360: 6772 0900 0000 da0a 7061 6769 6e61 7469  gr......paginati
-00001370: 6f6e 720a 0000 00da 0573 6572 6465 720b  onr......serder.
-00001380: 0000 00da 0f61 6374 696f 6e5f 6465 6c65  .....action_dele
-00001390: 6761 7465 720d 0000 0072 0e00 0000 720f  gater....r....r.
-000013a0: 0000 00da 1561 6374 696f 6e5f 6874 7470  .....action_http
-000013b0: 5f72 6573 6f75 7263 6573 7210 0000 0072  _resourcesr....r
-000013c0: 1100 0000 da0d 6163 7469 6f6e 5f72 6563  ......action_rec
-000013d0: 6f72 6472 1200 0000 da05 6572 726f 7272  ordr......errorr
-000013e0: 1300 0000 da06 6c6f 6767 6572 7214 0000  ......loggerr...
-000013f0: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
-00001400: 7221 0000 00da 083c 6d6f 6475 6c65 3e01  r!.....<module>.
-00001410: 0000 0073 1a00 0000 0800 0801 1001 1802  ...s............
-00001420: 0c06 0c01 0c01 1401 1005 0c04 0c01 0604  ................
-00001430: 1403                                     ..
+00000080: 6407 6c0d 6d0e 5a0e 0100 6403 6408 6c0f  d.l.m.Z...d.d.l.
+00000090: 6d10 5a10 0100 6409 640a 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+000000a0: 6d13 5a13 6d14 5a14 0100 6409 640b 6c15  m.Z.m.Z...d.d.l.
+000000b0: 6d16 5a16 6d17 5a17 0100 6409 640c 6c18  m.Z.m.Z...d.d.l.
+000000c0: 6d19 5a19 6d1a 5a1a 0100 6409 640d 6c1b  m.Z.m.Z...d.d.l.
+000000d0: 6d1c 5a1c 0100 6409 640e 6c1d 6d1e 5a1e  m.Z...d.d.l.m.Z.
+000000e0: 0100 650c 8300 5a1f 4700 640f 6410 8400  ..e...Z.G.d.d...
+000000f0: 6410 6516 8303 5a20 6401 5300 2911 e900  d.e...Z d.S.)...
+00000100: 0000 004e 2902 da03 416e 79da 084f 7074  ...N)...Any..Opt
+00000110: 696f 6e61 6ce9 0300 0000 2901 da15 526f  ional.....)...Ro
+00000120: 626f 746f 446f 6d61 696e 4578 6365 7074  botoDomainExcept
+00000130: 696f 6e29 04da 134f 5247 5f4f 5645 5252  ion)...ORG_OVERR
+00000140: 4944 455f 4845 4144 4552 da14 5553 4552  IDE_HEADER..USER
+00000150: 5f4f 5645 5252 4944 455f 4845 4144 4552  _OVERRIDE_HEADER
+00000160: da0b 436c 6965 6e74 4572 726f 72da 0a48  ..ClientError..H
+00000170: 7474 7043 6c69 656e 7429 01da 0e64 6566  ttpClient)...def
+00000180: 6175 6c74 5f6c 6f67 6765 7229 01da 0d50  ault_logger)...P
+00000190: 6167 696e 6174 6564 4c69 7374 2901 da16  aginatedList)...
+000001a0: 7079 6461 6e74 6963 5f6a 736f 6e61 626c  pydantic_jsonabl
+000001b0: 655f 6469 6374 e901 0000 0029 03da 1343  e_dict.....)...C
+000001c0: 6f6d 7075 7465 5265 7175 6972 656d 656e  omputeRequiremen
+000001d0: 7473 da14 436f 6e74 6169 6e65 7243 7265  ts..ContainerCre
+000001e0: 6465 6e74 6961 6c73 da13 436f 6e74 6169  dentials..Contai
+000001f0: 6e65 7250 6172 616d 6574 6572 7329 02da  nerParameters)..
+00000200: 0e41 6374 696f 6e44 656c 6567 6174 65da  .ActionDelegate.
+00000210: 0f55 7064 6174 6543 6f6e 6469 7469 6f6e  .UpdateCondition
+00000220: 2902 da13 4372 6561 7465 4163 7469 6f6e  )...CreateAction
+00000230: 5265 7175 6573 74da 1355 7064 6174 6541  Request..UpdateA
+00000240: 6374 696f 6e52 6571 7565 7374 2901 da0c  ctionRequest)...
+00000250: 4163 7469 6f6e 5265 636f 7264 2901 da21  ActionRecord)..!
+00000260: 4163 7469 6f6e 5570 6461 7465 436f 6e64  ActionUpdateCond
+00000270: 6974 696f 6e43 6865 636b 4661 696c 7572  itionCheckFailur
+00000280: 6563 0000 0000 0000 0000 0000 0000 0000  ec..............
+00000290: 0000 1300 0000 0000 0000 73ae 0100 0065  ..........s....e
+000002a0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+000002b0: 0564 023c 0065 0665 0564 033c 0064 0465  .d.<.e.e.d.<.d.e
+000002c0: 0664 0565 0464 0664 0766 0687 0066 0164  .d.e.d.d.f...f.d
+000002d0: 0864 0984 0c5a 0709 0764 2a64 0a65 0865  .d...Z...d*d.e.e
+000002e0: 0619 0064 0b65 0865 0619 0064 0665 0965  ...d.e.e...d.e.e
+000002f0: 0665 0666 0219 0066 0664 0c64 0d84 055a  .e.f...f.d.d...Z
+00000300: 0a09 0709 0709 0709 0709 0709 0709 0764  ...............d
+00000310: 2b64 0e65 0664 0a65 0865 0619 0064 0f65  +d.e.d.e.e...d.e
+00000320: 0865 0619 0064 1065 0865 0619 0064 1165  .e...d.e.e...d.e
+00000330: 0865 0965 0665 0b66 0219 0019 0064 1265  .e.e.e.f.....d.e
+00000340: 0865 0c65 0619 0019 0064 1365 0865 0d19  .e.e.....d.e.e..
+00000350: 0064 1465 0865 0e19 0064 0665 0f66 1264  .d.e.e...d.e.f.d
+00000360: 1564 1684 055a 1009 0764 2c64 0e65 0664  .d...Z...d,d.e.d
+00000370: 0a65 0865 0619 0064 0665 0f66 0664 1764  .e.e...d.e.f.d.d
+00000380: 1884 055a 1109 0764 2c64 1965 0f64 1a65  ...Z...d,d.e.d.e
+00000390: 0664 1b65 0664 1c65 0865 0619 0064 0665  .d.e.d.e.e...d.e
+000003a0: 0f66 0a64 1d64 1e84 055a 1209 0764 2c64  .f.d.d...Z...d,d
+000003b0: 1965 0f64 1c65 0865 0619 0064 0665 1366  .e.d.e.e...d.e.f
+000003c0: 0664 1f64 2084 055a 1409 0709 0764 2a64  .d.d ..Z.....d*d
+000003d0: 2165 0965 0665 0b66 0219 0064 0a65 0865  !e.e.e.f...d.e.e
+000003e0: 0619 0064 2265 0865 0965 0665 0666 0219  ...d"e.e.e.e.f..
+000003f0: 0019 0064 0665 1565 0f19 0066 0864 2364  ...d.e.e...f.d#d
+00000400: 2484 055a 1609 0709 0764 2a64 1965 0f64  $..Z.....d*d.e.d
+00000410: 2565 0965 0665 0b66 0219 0064 2665 0865  %e.e.e.f...d&e.e
+00000420: 0c65 1719 0019 0064 0a65 0865 0619 0064  .e.....d.e.e...d
+00000430: 2765 0865 0619 0064 0665 0f66 0c64 2864  'e.e...d.e.f.d(d
+00000440: 2984 055a 1887 0004 005a 1953 0029 2dda  )..Z.....Z.S.)-.
+00000450: 1241 6374 696f 6e48 7474 7044 656c 6567  .ActionHttpDeleg
+00000460: 6174 657a 470a 2020 2020 5573 6520 696e  atezG.    Use in
+00000470: 2061 6e79 2063 6f6e 7465 7874 2074 6861   any context tha
+00000480: 7420 646f 6573 206e 6f74 2068 6176 6520  t does not have 
+00000490: 6469 7265 6374 2064 6174 6162 6173 6520  direct database 
+000004a0: 6163 6365 7373 2e0a 2020 2020 da20 5f41  access..    . _A
+000004b0: 6374 696f 6e48 7474 7044 656c 6567 6174  ctionHttpDelegat
+000004c0: 655f 5f68 7474 705f 636c 6965 6e74 da2c  e__http_client.,
+000004d0: 5f41 6374 696f 6e48 7474 7044 656c 6567  _ActionHttpDeleg
+000004e0: 6174 655f 5f72 6f62 6f74 6f5f 7365 7276  ate__roboto_serv
+000004f0: 6963 655f 6261 7365 5f75 726c da17 726f  ice_base_url..ro
+00000500: 626f 746f 5f73 6572 7669 6365 5f62 6173  boto_service_bas
+00000510: 655f 7572 6cda 0b68 7474 705f 636c 6965  e_url..http_clie
+00000520: 6e74 da06 7265 7475 726e 4e63 0300 0000  nt..returnNc....
+00000530: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+00000540: 0300 0000 731a 0000 0074 0083 00a0 01a1  ....s....t......
+00000550: 0001 007c 027c 005f 027c 017c 005f 0364  ...|.|._.|.|._.d
+00000560: 0053 00a9 014e 2904 da05 7375 7065 72da  .S...N)...super.
+00000570: 085f 5f69 6e69 745f 5f72 1800 0000 7219  .__init__r....r.
+00000580: 0000 0029 03da 0473 656c 6672 1a00 0000  ...)...selfr....
+00000590: 721b 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
+000005a0: 5f5f a900 fafb 2f63 6f64 6562 7569 6c64  __..../codebuild
+000005b0: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
+000005c0: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+000005d0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
+000005e0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
+000005f0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
+00000600: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
+00000610: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
+00000620: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
+00000630: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
+00000640: 746f 2d61 692f 726f 626f 746f 2d68 6f73  to-ai/roboto-hos
+00000650: 7465 642d 6170 702f 7061 636b 6167 6573  ted-app/packages
+00000660: 2f72 6f62 6f74 6f5f 7364 6b2f 7372 632f  /roboto_sdk/src/
+00000670: 726f 626f 746f 5f73 646b 2f64 6f6d 6169  roboto_sdk/domai
+00000680: 6e2f 6163 7469 6f6e 732f 6163 7469 6f6e  n/actions/action
+00000690: 5f68 7474 705f 6465 6c65 6761 7465 2e70  _http_delegate.p
+000006a0: 7972 1f00 0000 2c00 0000 7306 0000 000a  yr....,...s.....
+000006b0: 0106 010a 017a 1b41 6374 696f 6e48 7474  .....z.ActionHtt
+000006c0: 7044 656c 6567 6174 652e 5f5f 696e 6974  pDelegate.__init
+000006d0: 5f5f da06 6f72 675f 6964 da07 7573 6572  __..org_id..user
+000006e0: 5f69 6463 0300 0000 0000 0000 0000 0000  _idc............
+000006f0: 0400 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
+00000700: 0064 0164 0269 017d 037c 0172 0a7c 017c  .d.d.i.}.|.r.|.|
+00000710: 0374 003c 007c 0272 107c 027c 0374 013c  .t.<.|.r.|.|.t.<
+00000720: 007c 0353 0029 034e 7a0c 436f 6e74 656e  .|.S.).Nz.Conten
+00000730: 742d 5479 7065 7a10 6170 706c 6963 6174  t-Typez.applicat
+00000740: 696f 6e2f 6a73 6f6e 2902 7206 0000 0072  ion/json).r....r
+00000750: 0700 0000 2904 7220 0000 0072 2500 0000  ....).r ...r%...
+00000760: 7226 0000 00da 0768 6561 6465 7273 7223  r&.....headersr#
+00000770: 0000 0072 2300 0000 7224 0000 0072 2700  ...r#...r$...r'.
+00000780: 0000 3100 0000 730c 0000 0008 0304 0108  ..1...s.........
+00000790: 0104 0108 0104 017a 1a41 6374 696f 6e48  .......z.ActionH
+000007a0: 7474 7044 656c 6567 6174 652e 6865 6164  ttpDelegate.head
+000007b0: 6572 73da 046e 616d 65da 0a63 7265 6174  ers..name..creat
+000007c0: 6564 5f62 79da 0b64 6573 6372 6970 7469  ed_by..descripti
+000007d0: 6f6e da08 6d65 7461 6461 7461 da04 7461  on..metadata..ta
+000007e0: 6773 da14 636f 6d70 7574 655f 7265 7175  gs..compute_requ
+000007f0: 6972 656d 656e 7473 da14 636f 6e74 6169  irements..contai
+00000800: 6e65 725f 7061 7261 6d65 7465 7273 6309  ner_parametersc.
+00000810: 0000 0000 0000 0000 0000 000c 0000 0008  ................
+00000820: 0000 0043 0000 0073 5600 0000 7c00 6a00  ...C...sV...|.j.
+00000830: 9b00 6401 9d02 7d09 7401 7c01 7c04 7c05  ..d...}.t.|.|.|.
+00000840: 7c06 7c07 7c08 6402 8d06 7d0a 7c00 6a02  |.|.|.d...}.|.j.
+00000850: 6a03 7c09 7404 7c0a 6403 6404 8d02 7c00  j.|.t.|.d.d...|.
+00000860: a005 7c02 7c03 a102 6405 8d03 7d0b 7406  ..|.|...d...}.t.
+00000870: a007 7c0b 6a08 6406 6701 6407 8d01 a101  ..|.j.d.g.d.....
+00000880: 5300 2908 4e7a 0b2f 7631 2f61 6374 696f  S.).Nz./v1/actio
+00000890: 6e73 2906 7228 0000 0072 2a00 0000 722b  ns).r(...r*...r+
+000008a0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+000008b0: 0000 5429 01da 0c65 7863 6c75 6465 5f6e  ..T)...exclude_n
+000008c0: 6f6e 65a9 02da 0464 6174 6172 2700 0000  one....datar'...
+000008d0: 7231 0000 00a9 01da 096a 736f 6e5f 7061  r1.......json_pa
+000008e0: 7468 2909 7219 0000 0072 1300 0000 7218  th).r....r....r.
+000008f0: 0000 00da 0470 6f73 7472 0c00 0000 7227  .....postr....r'
+00000900: 0000 0072 1500 0000 da09 7061 7273 655f  ...r......parse_
+00000910: 6f62 6ada 0966 726f 6d5f 6a73 6f6e 290c  obj..from_json).
+00000920: 7220 0000 0072 2800 0000 7225 0000 0072  r ...r(...r%...r
+00000930: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
+00000940: 0000 0072 2d00 0000 722e 0000 00da 0375  ...r-...r......u
+00000950: 726c da0c 7265 7175 6573 745f 626f 6479  rl..request_body
+00000960: da08 7265 7370 6f6e 7365 7223 0000 0072  ..responser#...r
+00000970: 2300 0000 7224 0000 00da 0d63 7265 6174  #...r$.....creat
+00000980: 655f 6163 7469 6f6e 3b00 0000 731e 0000  e_action;...s...
+00000990: 000c 0b02 0102 0102 0102 0102 0102 0102  ................
+000009a0: 0106 fa06 0802 010a 010a 0106 fd14 057a  ...............z
+000009b0: 2041 6374 696f 6e48 7474 7044 656c 6567   ActionHttpDeleg
+000009c0: 6174 652e 6372 6561 7465 5f61 6374 696f  ate.create_actio
+000009d0: 6e63 0300 0000 0000 0000 0000 0000 0600  nc..............
+000009e0: 0000 0a00 0000 4300 0000 7360 0000 007c  ......C...s`...|
+000009f0: 006a 009b 0064 017c 019b 009d 037d 037a  .j...d.|.....}.z
+00000a00: 167c 006a 016a 027c 037c 00a0 037c 02a1  .|.j.j.|.|...|..
+00000a10: 0164 028d 027d 0474 04a0 057c 046a 0664  .d...}.t...|.j.d
+00000a20: 0367 0164 048d 01a1 0157 0053 0004 0074  .g.d.....W.S...t
+00000a30: 0779 2f01 007d 0501 007a 0574 08a0 097c  .y/..}...z.t...|
+00000a40: 05a1 0182 0164 007d 057e 0577 0177 0029  .....d.}.~.w.w.)
+00000a50: 054e fa0c 2f76 312f 6163 7469 6f6e 732f  .N../v1/actions/
+00000a60: a901 7227 0000 0072 3100 0000 7232 0000  ..r'...r1...r2..
+00000a70: 0029 0a72 1900 0000 7218 0000 00da 0367  .).r....r......g
+00000a80: 6574 7227 0000 0072 1500 0000 7235 0000  etr'...r....r5..
+00000a90: 0072 3600 0000 7208 0000 0072 0500 0000  .r6...r....r....
+00000aa0: 5a11 6672 6f6d 5f63 6c69 656e 745f 6572  Z.from_client_er
+00000ab0: 726f 7229 0672 2000 0000 7228 0000 0072  ror).r ...r(...r
+00000ac0: 2500 0000 7237 0000 00da 0372 6573 da03  %...r7.....res..
+00000ad0: 6578 6372 2300 0000 7223 0000 0072 2400  excr#...r#...r$.
+00000ae0: 0000 da19 6765 745f 6163 7469 6f6e 5f62  ....get_action_b
+00000af0: 795f 7072 696d 6172 795f 6b65 7956 0000  y_primary_keyV..
+00000b00: 0073 1000 0000 1003 0201 1601 1601 0e01  .s..............
+00000b10: 0a01 0880 02ff 7a2c 4163 7469 6f6e 4874  ......z,ActionHt
+00000b20: 7470 4465 6c65 6761 7465 2e67 6574 5f61  tpDelegate.get_a
+00000b30: 6374 696f 6e5f 6279 5f70 7269 6d61 7279  ction_by_primary
+00000b40: 5f6b 6579 da06 7265 636f 7264 da0a 696d  _key..record..im
+00000b50: 6167 655f 6e61 6d65 da09 696d 6167 655f  age_name..image_
+00000b60: 7461 67da 0663 616c 6c65 7263 0500 0000  tag..callerc....
+00000b70: 0000 0000 0000 0000 0800 0000 0600 0000  ................
+00000b80: 4300 0000 734c 0000 007c 006a 009b 0064  C...sL...|.j...d
+00000b90: 017c 016a 019b 0064 029d 047d 057c 027c  .|.j...d...}.|.|
+00000ba0: 0364 039c 027d 067c 006a 026a 037c 057c  .d...}.|.j.j.|.|
+00000bb0: 067c 006a 047c 0464 048d 0164 058d 037d  .|.j.|.d...d...}
+00000bc0: 0774 05a0 067c 076a 0764 0667 0164 078d  .t...|.j.d.g.d..
+00000bd0: 01a1 0153 0029 084e 723b 0000 007a 0a2f  ...S.).Nr;...z./
+00000be0: 636f 6e74 6169 6e65 7229 0272 4200 0000  container).rB...
+00000bf0: 7243 0000 00a9 0172 2600 0000 7230 0000  rC.....r&...r0..
+00000c00: 0072 3100 0000 7232 0000 0029 0872 1900  .r1...r2...).r..
+00000c10: 0000 7228 0000 0072 1800 0000 da03 7075  ..r(...r......pu
+00000c20: 7472 2700 0000 7215 0000 0072 3500 0000  tr'...r....r5...
+00000c30: 7236 0000 0029 0872 2000 0000 7241 0000  r6...).r ...rA..
+00000c40: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
+00000c50: 7237 0000 0072 3100 0000 7239 0000 0072  r7...r1...r9...r
+00000c60: 2300 0000 7223 0000 0072 2400 0000 da12  #...r#...r$.....
+00000c70: 7265 6769 7374 6572 5f63 6f6e 7461 696e  register_contain
+00000c80: 6572 6000 0000 7310 0000 0014 0702 0202  er`...s.........
+00000c90: 0106 fe06 050e 0106 ff14 037a 2541 6374  ...........z%Act
+00000ca0: 696f 6e48 7474 7044 656c 6567 6174 652e  ionHttpDelegate.
+00000cb0: 7265 6769 7374 6572 5f63 6f6e 7461 696e  register_contain
+00000cc0: 6572 6303 0000 0000 0000 0000 0000 0005  erc.............
+00000cd0: 0000 0005 0000 0043 0000 0073 4000 0000  .......C...s@...
+00000ce0: 7c00 6a00 9b00 6401 7c01 6a01 9b00 6402  |.j...d.|.j...d.
+00000cf0: 9d04 7d03 7c00 6a02 6a03 7c03 7c00 6a04  ..}.|.j.j.|.|.j.
+00000d00: 7c02 6403 8d01 6404 8d02 7d04 7405 a006  |.d...d...}.t...
+00000d10: 7c04 6a07 6405 6701 6406 8d01 a101 5300  |.j.d.g.d.....S.
+00000d20: 2907 4e72 3b00 0000 7a16 2f63 6f6e 7461  ).Nr;...z./conta
+00000d30: 696e 6572 2f63 7265 6465 6e74 6961 6c73  iner/credentials
+00000d40: 7245 0000 0072 3c00 0000 7231 0000 0072  rE...r<...r1...r
+00000d50: 3200 0000 2908 7219 0000 0072 2800 0000  2...).r....r(...
+00000d60: 7218 0000 0072 3d00 0000 7227 0000 0072  r....r=...r'...r
+00000d70: 0f00 0000 7235 0000 0072 3600 0000 2905  ....r5...r6...).
+00000d80: 7220 0000 0072 4100 0000 7244 0000 0072  r ...rA...rD...r
+00000d90: 3700 0000 723e 0000 0072 2300 0000 7223  7...r>...r#...r#
+00000da0: 0000 0072 2400 0000 da1e 6765 745f 7465  ...r$.....get_te
+00000db0: 6d70 5f63 6f6e 7461 696e 6572 5f63 7265  mp_container_cre
+00000dc0: 6465 6e74 6961 6c73 7200 0000 7306 0000  dentialsr...s...
+00000dd0: 0014 0518 0114 017a 3141 6374 696f 6e48  .......z1ActionH
+00000de0: 7474 7044 656c 6567 6174 652e 6765 745f  ttpDelegate.get_
+00000df0: 7465 6d70 5f63 6f6e 7461 696e 6572 5f63  temp_container_c
+00000e00: 7265 6465 6e74 6961 6c73 da07 6669 6c74  redentials..filt
+00000e10: 6572 73da 0a70 6167 655f 746f 6b65 6e63  ers..page_tokenc
+00000e20: 0400 0000 0000 0000 0000 0000 0800 0000  ................
+00000e30: 0600 0000 4300 0000 736c 0000 007c 0372  ....C...sl...|.r
+00000e40: 067c 037c 0164 013c 0074 00a0 0174 00a0  .|.|.d.<.t...t..
+00000e50: 027c 01a1 01a1 017d 047c 006a 039b 0064  .|.....}.|.j...d
+00000e60: 029d 027d 057c 006a 046a 057c 057c 047c  ...}.|.j.j.|.|.|
+00000e70: 00a0 067c 02a1 0164 038d 037d 067c 066a  ...|...d...}.|.j
+00000e80: 0764 0467 0164 058d 017d 0774 0864 0664  .d.g.d...}.t.d.d
+00000e90: 0784 007c 0764 0819 0044 0083 017c 0764  ...|.d...D...|.d
+00000ea0: 0919 0064 0a8d 0253 0029 0b4e 724a 0000  ...d...S.).NrJ..
+00000eb0: 007a 112f 7631 2f61 6374 696f 6e73 2f71  .z./v1/actions/q
+00000ec0: 7565 7279 7230 0000 0072 3100 0000 7232  ueryr0...r1...r2
+00000ed0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000ee0: 0200 0000 0500 0000 5300 0000 7316 0000  ........S...s...
+00000ef0: 0067 007c 005d 077d 0174 00a0 017c 01a1  .g.|.].}.t...|..
+00000f00: 0191 0271 0253 0072 2300 0000 2902 7215  ...q.S.r#...).r.
+00000f10: 0000 0072 3500 0000 2902 da02 2e30 5a07  ...r5...)....0Z.
+00000f20: 6461 7461 7365 7472 2300 0000 7223 0000  datasetr#...r#..
+00000f30: 0072 2400 0000 da0a 3c6c 6973 7463 6f6d  .r$.....<listcom
+00000f40: 703e 8b00 0000 7306 0000 0006 000a 0106  p>....s.........
+00000f50: ff7a 3441 6374 696f 6e48 7474 7044 656c  .z4ActionHttpDel
+00000f60: 6567 6174 652e 7175 6572 795f 6163 7469  egate.query_acti
+00000f70: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6c69  ons.<locals>.<li
+00000f80: 7374 636f 6d70 3eda 0569 7465 6d73 da0a  stcomp>..items..
+00000f90: 6e65 7874 5f74 6f6b 656e 2902 724d 0000  next_token).rM..
+00000fa0: 0072 4e00 0000 2909 da04 6a73 6f6e da05  .rN...)...json..
+00000fb0: 6c6f 6164 73da 0564 756d 7073 7219 0000  loads..dumpsr...
+00000fc0: 0072 1800 0000 7234 0000 0072 2700 0000  .r....r4...r'...
+00000fd0: 7236 0000 0072 0b00 0000 2908 7220 0000  r6...r....).r ..
+00000fe0: 0072 4900 0000 7225 0000 0072 4a00 0000  .rI...r%...rJ...
+00000ff0: 5a0c 7361 6665 5f66 696c 7465 7273 7237  Z.safe_filtersr7
+00001000: 0000 0072 3e00 0000 5a0c 756e 6d61 7273  ...r>...Z.unmars
+00001010: 6861 6c6c 6564 7223 0000 0072 2300 0000  halledr#...r#...
+00001020: 7224 0000 00da 0d71 7565 7279 5f61 6374  r$.....query_act
+00001030: 696f 6e73 7b00 0000 731c 0000 0004 0608  ions{...s.......
+00001040: 0110 020c 0106 010c 0106 ff0e 0302 0106  ................
+00001050: 0106 0104 ff06 0306 fc7a 2041 6374 696f  .........z Actio
+00001060: 6e48 7474 7044 656c 6567 6174 652e 7175  nHttpDelegate.qu
+00001070: 6572 795f 6163 7469 6f6e 73da 0775 7064  ery_actions..upd
+00001080: 6174 6573 da0a 636f 6e64 6974 696f 6e73  ates..conditions
+00001090: da0a 7570 6461 7465 645f 6279 6306 0000  ..updated_byc...
+000010a0: 0000 0000 0000 0000 000a 0000 000a 0000  ................
+000010b0: 0043 0000 0073 9400 0000 7c00 6a00 9b00  .C...s....|.j...
+000010c0: 6401 7c01 6a01 9b00 9d03 7d06 7402 7c02  d.|.j.....}.t.|.
+000010d0: 7c03 6400 7501 7211 7c03 6e01 6700 6402  |.d.u.r.|.n.g.d.
+000010e0: 8d02 7d07 7a1a 7c00 6a03 6a04 7c06 7c07  ..}.z.|.j.j.|.|.
+000010f0: a005 a100 7c00 a006 7c04 7c05 a102 6403  ....|...|.|...d.
+00001100: 8d03 7d08 7407 a008 7c08 6a09 6404 6701  ..}.t...|.j.d.g.
+00001110: 6405 8d01 a101 5700 5300 0400 740a 7949  d.....W.S...t.yI
+00001120: 0100 7d09 0100 7a0e 7c09 6a0b 740c 6a0d  ..}...z.|.j.t.j.
+00001130: 6a0e 6b02 7244 740f 7c09 6a10 8301 6400  j.k.rDt.|.j...d.
+00001140: 8202 8200 6400 7d09 7e09 7701 7700 2906  ....d.}.~.w.w.).
+00001150: 4e72 3b00 0000 2902 7253 0000 0072 5400  Nr;...).rS...rT.
+00001160: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
+00001170: 0029 1172 1900 0000 7228 0000 0072 1400  .).r....r(...r..
+00001180: 0000 7218 0000 00da 0570 6174 6368 da04  ..r......patch..
+00001190: 6469 6374 7227 0000 0072 1500 0000 7235  dictr'...r....r5
+000011a0: 0000 0072 3600 0000 7208 0000 00da 0673  ...r6...r......s
+000011b0: 7461 7475 73da 0468 7474 70da 0a48 5454  tatus..http..HTT
+000011c0: 5053 7461 7475 73da 0843 4f4e 464c 4943  PStatus..CONFLIC
+000011d0: 5472 1600 0000 da03 6d73 6729 0a72 2000  Tr......msg).r .
+000011e0: 0000 7241 0000 0072 5300 0000 7254 0000  ..rA...rS...rT..
+000011f0: 0072 2500 0000 7255 0000 0072 3700 0000  .r%...rU...r7...
+00001200: da07 7061 796c 6f61 6472 3e00 0000 723f  ..payloadr>...r?
+00001210: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00001220: 0000 da06 7570 6461 7465 9100 0000 7320  ....update....s 
+00001230: 0000 0012 0802 0102 010e 0106 fe02 0406  ................
+00001240: 0112 0106 ff16 030e 010e 010c 0102 0108  ................
+00001250: 8002 fd7a 1941 6374 696f 6e48 7474 7044  ...z.ActionHttpD
+00001260: 656c 6567 6174 652e 7570 6461 7465 2902  elegate.update).
+00001270: 4e4e 2907 4e4e 4e4e 4e4e 4e72 1d00 0000  NN).NNNNNNNr....
+00001280: 291a da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00001290: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000012a0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+000012b0: 0900 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
+000012c0: 6f6e 735f 5fda 0373 7472 721f 0000 0072  ons__..strr....r
+000012d0: 0300 0000 7257 0000 0072 2700 0000 7202  ....rW...r'...r.
+000012e0: 0000 00da 046c 6973 7472 0e00 0000 7210  .....listr....r.
+000012f0: 0000 0072 1500 0000 723a 0000 0072 4000  ...r....r:...r@.
+00001300: 0000 7247 0000 0072 0f00 0000 7248 0000  ..rG...r....rH..
+00001310: 0072 0b00 0000 7252 0000 0072 1200 0000  .r....rR...r....
+00001320: 725e 0000 00da 0d5f 5f63 6c61 7373 6365  r^.....__classce
+00001330: 6c6c 5f5f 7223 0000 0072 2300 0000 7221  ll__r#...r#...r!
+00001340: 0000 0072 2400 0000 7217 0000 0024 0000  ...r$...r....$..
+00001350: 0073 ba00 0000 0a00 0401 0804 0801 1a02  .s..............
+00001360: 0206 04ff 0601 02ff 0601 02ff 0a02 0afe  ................
+00001370: 020d 0201 0201 0201 0201 0201 0201 04f7  ................
+00001380: 0202 02fe 0603 02fd 0604 02fc 0605 02fb  ................
+00001390: 0e06 02fa 0a07 02f9 0608 02f8 0609 02f7  ................
+000013a0: 020a 0af6 021c 04ff 0201 02ff 0601 02ff  ................
+000013b0: 0202 0afe 020f 04fb 0202 02fe 0203 02fd  ................
+000013c0: 0204 02fc 0605 02fb 0206 0afa 0215 04fd  ................
+000013d0: 0202 02fe 0603 02fd 0204 0afc 020c 0201  ................
+000013e0: 04fc 0a02 02fe 0603 02fd 0e04 02fc 0605  ................
+000013f0: 0afb 021b 0201 04fa 0202 02fe 0a03 02fd  ................
+00001400: 0a04 02fc 0605 02fb 0606 02fa 0207 12f9  ................
+00001410: 7217 0000 0029 2172 5900 0000 724f 0000  r....)!rY...rO..
+00001420: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+00001430: 0000 00da 0a65 7863 6570 7469 6f6e 7372  .....exceptionsr
+00001440: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
+00001450: 0000 0072 0900 0000 da07 6c6f 6767 696e  ...r......loggin
+00001460: 6772 0a00 0000 da0a 7061 6769 6e61 7469  gr......paginati
+00001470: 6f6e 720b 0000 00da 0573 6572 6465 720c  onr......serder.
+00001480: 0000 00da 1a61 6374 696f 6e5f 636f 6e74  .....action_cont
+00001490: 6169 6e65 725f 7265 736f 7572 6365 7372  ainer_resourcesr
+000014a0: 0e00 0000 720f 0000 0072 1000 0000 da0f  ....r....r......
+000014b0: 6163 7469 6f6e 5f64 656c 6567 6174 6572  action_delegater
+000014c0: 1100 0000 7212 0000 00da 1561 6374 696f  ....r......actio
+000014d0: 6e5f 6874 7470 5f72 6573 6f75 7263 6573  n_http_resources
+000014e0: 7213 0000 0072 1400 0000 da0d 6163 7469  r....r......acti
+000014f0: 6f6e 5f72 6563 6f72 6472 1500 0000 da05  on_recordr......
+00001500: 6572 726f 7272 1600 0000 da06 6c6f 6767  errorr......logg
+00001510: 6572 7217 0000 0072 2300 0000 7223 0000  err....r#...r#..
+00001520: 0072 2300 0000 7224 0000 00da 083c 6d6f  .r#...r$.....<mo
+00001530: 6475 6c65 3e01 0000 0073 1e00 0000 0800  dule>....s......
+00001540: 0801 1001 0c02 1801 0c06 0c01 0c01 1401  ................
+00001550: 1005 1004 0c04 0c01 0604 1403            ............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 640 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,99 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 8002 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 5c03 0000  o.......1..d\...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
+00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6403 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 0100 4700 6405 6406 8400 6406 6503 6a06  ..G.d.d...d.e.j.
-00000060: 8303 5a07 4700 6407 6408 8400 6408 6503  ..Z.G.d.d...d.e.
-00000070: 6a06 8303 5a08 4700 6409 640a 8400 640a  j...Z.G.d.d...d.
-00000080: 6503 6a06 8303 5a09 6402 5300 290b e900  e.j...Z.d.S.)...
-00000090: 0000 0029 02da 0341 6e79 da08 4f70 7469  ...)...Any..Opti
-000000a0: 6f6e 616c 4ee9 0100 0000 2901 da0f 5570  onalN.....)...Up
-000000b0: 6461 7465 436f 6e64 6974 696f 6e63 0000  dateConditionc..
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-000000d0: 0000 4000 0000 7362 0000 0065 005a 0164  ..@...sb...e.Z.d
-000000e0: 005a 0255 0065 0365 0464 013c 0064 025a  .Z.U.e.e.d.<.d.Z
-000000f0: 0565 0665 0319 0065 0464 033c 0065 076a  .e.e...e.d.<.e.j
-00000100: 0865 0964 048d 015a 0a65 0665 0965 0365  .e.d...Z.e.e.e.e
-00000110: 0b66 0219 0019 0065 0464 053c 0065 076a  .f.....e.d.<.e.j
-00000120: 0865 0c64 048d 015a 0d65 0665 0c65 0319  .e.d...Z.e.e.e..
-00000130: 0019 0065 0464 063c 0064 0253 0029 07da  ...e.d.<.d.S.)..
-00000140: 1343 7265 6174 6541 6374 696f 6e52 6571  .CreateActionReq
-00000150: 7565 7374 da04 6e61 6d65 4eda 0b64 6573  uest..nameN..des
-00000160: 6372 6970 7469 6f6e 2901 da0f 6465 6661  cription)...defa
-00000170: 756c 745f 6661 6374 6f72 79da 086d 6574  ult_factory..met
-00000180: 6164 6174 61da 0474 6167 7329 0eda 085f  adata..tags)..._
-00000190: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000001a0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000001b0: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
-000001c0: 7469 6f6e 735f 5f72 0800 0000 7203 0000  tions__r....r...
-000001d0: 00da 0870 7964 616e 7469 63da 0546 6965  ...pydantic..Fie
-000001e0: 6c64 da04 6469 6374 720a 0000 0072 0200  ld..dictr....r..
-000001f0: 0000 da04 6c69 7374 720b 0000 00a9 0072  ....listr......r
-00000200: 1500 0000 7215 0000 00fa fc2f 636f 6465  ....r....../code
-00000210: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000220: 3334 3937 3236 3836 3730 2f73 7263 2f63  3497268670/src/c
-00000230: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
-00000240: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
-00000250: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
-00000260: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
-00000270: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
-00000280: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
-00000290: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
-000002a0: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
-000002b0: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
-000002c0: 6b61 6765 732f 726f 626f 746f 5f73 646b  kages/roboto_sdk
-000002d0: 2f73 7263 2f72 6f62 6f74 6f5f 7364 6b2f  /src/roboto_sdk/
-000002e0: 646f 6d61 696e 2f61 6374 696f 6e73 2f61  domain/actions/a
-000002f0: 6374 696f 6e5f 6874 7470 5f72 6573 6f75  ction_http_resou
-00000300: 7263 6573 2e70 7972 0600 0000 0800 0000  rces.pyr........
-00000310: 730a 0000 000a 0008 0210 0320 0120 0172  s.......... . .r
-00000320: 0600 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000330: 0000 0000 0003 0000 0040 0000 0073 2e00  .........@...s..
-00000340: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000350: 6401 3c00 6503 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
-00000360: 6403 3c00 6503 6504 6404 3c00 6405 5300  d.<.e.e.d.<.d.S.
-00000370: 2906 da1a 436f 6e74 6169 6e65 7255 706c  )...ContainerUpl
-00000380: 6f61 6443 7265 6465 6e74 6961 6c73 da08  oadCredentials..
-00000390: 7573 6572 6e61 6d65 da08 7061 7373 776f  username..passwo
-000003a0: 7264 da0c 7265 6769 7374 7279 5f75 726c  rd..registry_url
-000003b0: da09 696d 6167 655f 7572 694e 2905 720c  ..image_uriN).r.
-000003c0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-000003d0: 0000 7210 0000 0072 1500 0000 7215 0000  ..r....r....r...
-000003e0: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-000003f0: 1200 0000 730a 0000 000a 0008 0108 0108  ....s...........
-00000400: 010c 0172 1700 0000 6300 0000 0000 0000  ...r....c.......
-00000410: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000420: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
-00000430: 6503 6504 6505 6602 1900 6506 6401 3c00  e.e.e.f...e.d.<.
-00000440: 6402 5a07 6508 6509 650a 1900 1900 6506  d.Z.e.e.e.....e.
-00000450: 6403 3c00 6402 5300 2904 da13 5570 6461  d.<.d.S.)...Upda
-00000460: 7465 4163 7469 6f6e 5265 7175 6573 74da  teActionRequest.
-00000470: 0775 7064 6174 6573 4eda 0a63 6f6e 6469  .updatesN..condi
-00000480: 7469 6f6e 7329 0b72 0c00 0000 720d 0000  tions).r....r...
-00000490: 0072 0e00 0000 7213 0000 0072 0f00 0000  .r....r....r....
-000004a0: 7202 0000 0072 1000 0000 721e 0000 0072  r....r....r....r
-000004b0: 0300 0000 7214 0000 0072 0500 0000 7215  ....r....r....r.
-000004c0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000004d0: 0000 721c 0000 0019 0000 0073 0600 0000  ..r........s....
-000004e0: 0a00 1001 1801 721c 0000 0029 0ada 0674  ......r....)...t
-000004f0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-00000500: 1100 0000 da0f 6163 7469 6f6e 5f64 656c  ......action_del
-00000510: 6567 6174 6572 0500 0000 da09 4261 7365  egater......Base
-00000520: 4d6f 6465 6c72 0600 0000 7217 0000 0072  Modelr....r....r
-00000530: 1c00 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
-00000540: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000550: 653e 0100 0000 730c 0000 0010 0008 020c  e>....s.........
-00000560: 0212 0312 0a16 07                        .......
+00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 4700 6406 6407 8400 6407 6503 6a09  ..G.d.d...d.e.j.
+00000070: 8303 5a0a 4700 6408 6409 8400 6409 6503  ..Z.G.d.d...d.e.
+00000080: 6a09 8303 5a0b 4700 640a 640b 8400 640b  j...Z.G.d.d...d.
+00000090: 6503 6a09 8303 5a0c 6402 5300 290c e900  e.j...Z.d.S.)...
+000000a0: 0000 0029 02da 0341 6e79 da08 4f70 7469  ...)...Any..Opti
+000000b0: 6f6e 616c 4ee9 0100 0000 2902 da13 436f  onalN.....)...Co
+000000c0: 6d70 7574 6552 6571 7569 7265 6d65 6e74  mputeRequirement
+000000d0: 73da 1343 6f6e 7461 696e 6572 5061 7261  s..ContainerPara
+000000e0: 6d65 7465 7273 2901 da0f 5570 6461 7465  meters)...Update
+000000f0: 436f 6e64 6974 696f 6e63 0000 0000 0000  Conditionc......
+00000100: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000110: 0000 7382 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
+00000120: 0065 0365 0464 013c 0064 025a 0565 0665  .e.e.d.<.d.Z.e.e
+00000130: 0319 0065 0464 033c 0065 076a 0865 0964  ...e.d.<.e.j.e.d
+00000140: 048d 015a 0a65 0665 0965 0365 0b66 0219  ...Z.e.e.e.e.f..
+00000150: 0019 0065 0464 053c 0065 076a 0865 0c64  ...e.d.<.e.j.e.d
+00000160: 048d 015a 0d65 0665 0c65 0319 0019 0065  ...Z.e.e.e.....e
+00000170: 0464 063c 0064 025a 0e65 0665 0f19 0065  .d.<.d.Z.e.e...e
+00000180: 0464 073c 0064 025a 1065 0665 1119 0065  .d.<.d.Z.e.e...e
+00000190: 0464 083c 0064 0253 0029 09da 1343 7265  .d.<.d.S.)...Cre
+000001a0: 6174 6541 6374 696f 6e52 6571 7565 7374  ateActionRequest
+000001b0: da04 6e61 6d65 4eda 0b64 6573 6372 6970  ..nameN..descrip
+000001c0: 7469 6f6e 2901 da0f 6465 6661 756c 745f  tion)...default_
+000001d0: 6661 6374 6f72 79da 086d 6574 6164 6174  factory..metadat
+000001e0: 61da 0474 6167 73da 1463 6f6d 7075 7465  a..tags..compute
+000001f0: 5f72 6571 7569 7265 6d65 6e74 73da 1463  _requirements..c
+00000200: 6f6e 7461 696e 6572 5f70 6172 616d 6574  ontainer_paramet
+00000210: 6572 7329 12da 085f 5f6e 616d 655f 5fda  ers)...__name__.
+00000220: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000230: 7561 6c6e 616d 655f 5fda 0373 7472 da0f  ualname__..str..
+00000240: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+00000250: 0a00 0000 7203 0000 00da 0870 7964 616e  ....r......pydan
+00000260: 7469 63da 0546 6965 6c64 da04 6469 6374  tic..Field..dict
+00000270: 720c 0000 0072 0200 0000 da04 6c69 7374  r....r......list
+00000280: 720d 0000 0072 0e00 0000 7205 0000 0072  r....r....r....r
+00000290: 0f00 0000 7206 0000 00a9 0072 1900 0000  ....r......r....
+000002a0: 7219 0000 00fa fc2f 636f 6465 6275 696c  r....../codebuil
+000002b0: 642f 6f75 7470 7574 2f73 7263 3136 3839  d/output/src1689
+000002c0: 3135 3533 3939 2f73 7263 2f63 6f64 6573  155399/src/codes
+000002d0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
+000002e0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
+000002f0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
+00000300: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
+00000310: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
+00000320: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
+00000330: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
+00000340: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
+00000350: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
+00000360: 732f 726f 626f 746f 5f73 646b 2f73 7263  s/roboto_sdk/src
+00000370: 2f72 6f62 6f74 6f5f 7364 6b2f 646f 6d61  /roboto_sdk/doma
+00000380: 696e 2f61 6374 696f 6e73 2f61 6374 696f  in/actions/actio
+00000390: 6e5f 6874 7470 5f72 6573 6f75 7263 6573  n_http_resources
+000003a0: 2e70 7972 0800 0000 0c00 0000 730e 0000  .pyr........s...
+000003b0: 000a 0008 0210 0320 011c 0110 0114 0172  ....... .......r
+000003c0: 0800 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000003d0: 0000 0000 0003 0000 0040 0000 0073 2e00  .........@...s..
+000003e0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+000003f0: 6401 3c00 6503 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
+00000400: 6403 3c00 6503 6504 6404 3c00 6405 5300  d.<.e.e.d.<.d.S.
+00000410: 2906 da1a 436f 6e74 6169 6e65 7255 706c  )...ContainerUpl
+00000420: 6f61 6443 7265 6465 6e74 6961 6c73 da08  oadCredentials..
+00000430: 7573 6572 6e61 6d65 da08 7061 7373 776f  username..passwo
+00000440: 7264 da0c 7265 6769 7374 7279 5f75 726c  rd..registry_url
+00000450: 5a09 696d 6167 655f 7572 694e 2905 7210  Z.image_uriN).r.
+00000460: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00000470: 0000 7214 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00000480: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000490: 1800 0000 730a 0000 000a 0008 0108 0108  ....s...........
+000004a0: 010c 0172 1b00 0000 6300 0000 0000 0000  ...r....c.......
+000004b0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000004c0: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+000004d0: 6503 6504 6505 6602 1900 6506 6401 3c00  e.e.e.f...e.d.<.
+000004e0: 6402 5a07 6508 6509 650a 1900 1900 6506  d.Z.e.e.e.....e.
+000004f0: 6403 3c00 6402 5300 2904 da13 5570 6461  d.<.d.S.)...Upda
+00000500: 7465 4163 7469 6f6e 5265 7175 6573 74da  teActionRequest.
+00000510: 0775 7064 6174 6573 4eda 0a63 6f6e 6469  .updatesN..condi
+00000520: 7469 6f6e 7329 0b72 1000 0000 7211 0000  tions).r....r...
+00000530: 0072 1200 0000 7217 0000 0072 1300 0000  .r....r....r....
+00000540: 7202 0000 0072 1400 0000 7221 0000 0072  r....r....r!...r
+00000550: 0300 0000 7218 0000 0072 0700 0000 7219  ....r....r....r.
+00000560: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00000570: 0000 721f 0000 001f 0000 0073 0600 0000  ..r........s....
+00000580: 0a00 1001 1801 721f 0000 0029 0dda 0674  ......r....)...t
+00000590: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
+000005a0: 1500 0000 da1a 6163 7469 6f6e 5f63 6f6e  ......action_con
+000005b0: 7461 696e 6572 5f72 6573 6f75 7263 6573  tainer_resources
+000005c0: 7205 0000 0072 0600 0000 da0f 6163 7469  r....r......acti
+000005d0: 6f6e 5f64 656c 6567 6174 6572 0700 0000  on_delegater....
+000005e0: da09 4261 7365 4d6f 6465 6c72 0800 0000  ..BaseModelr....
+000005f0: 721b 0000 0072 1f00 0000 7219 0000 0072  r....r....r....r
+00000600: 1900 0000 7219 0000 0072 1a00 0000 da08  ....r....r......
+00000610: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
+00000620: 0010 0008 0210 020c 0412 0312 0c16 07    ...............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 6a00 0000  o.......Ms.dj...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 6a00 0000  o.......1..dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 4700  .....@...s$...G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 4700  d.d...d.e...Z.G.
 00000040: 6402 6403 8400 6403 6500 8303 5a02 6404  d.d...d.e...Z.d.
 00000050: 5300 2905 6300 0000 0000 0000 0000 0000  S.).c...........
 00000060: 0000 0000 0001 0000 0040 0000 00f3 0c00  .........@......
 00000070: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
 00000080: da21 4163 7469 6f6e 5570 6461 7465 436f  .!ActionUpdateCo
 00000090: 6e64 6974 696f 6e43 6865 636b 4661 696c  nditionCheckFail
 000000a0: 7572 654e a903 da08 5f5f 6e61 6d65 5f5f  ureN....__name__
 000000b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 000000c0: 7175 616c 6e61 6d65 5f5f a900 7207 0000  qualname__..r...
 000000d0: 0072 0700 0000 faec 2f63 6f64 6562 7569  .r....../codebui
-000000e0: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
-000000f0: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
+000000e0: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+000000f0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
 00000100: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000110: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000120: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000130: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000140: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000150: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000160: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 4499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,299 +1,327 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 9311 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 e412 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
+00000020: 0003 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 6405 6406 6c07 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
-00000060: 6407 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
-00000070: 0100 4700 6408 6409 8400 6409 8302 5a0d  ..G.d.d...d...Z.
-00000080: 6401 5300 290a e900 0000 004e 2902 da03  d.S.)......N)...
-00000090: 416e 79da 084f 7074 696f 6e61 6ce9 0300  Any..Optional...
-000000a0: 0000 2901 da16 7079 6461 6e74 6963 5f6a  ..)...pydantic_j
-000000b0: 736f 6e61 626c 655f 6469 6374 e901 0000  sonable_dict....
-000000c0: 0029 01da 1249 6e76 6f63 6174 696f 6e44  .)...InvocationD
-000000d0: 656c 6567 6174 6529 03da 1449 6e76 6f63  elegate)...Invoc
-000000e0: 6174 696f 6e44 6174 6153 6f75 7263 65da  ationDataSource.
-000000f0: 1049 6e76 6f63 6174 696f 6e52 6563 6f72  .InvocationRecor
-00000100: 64da 1049 6e76 6f63 6174 696f 6e53 7461  d..InvocationSta
-00000110: 7475 7363 0000 0000 0000 0000 0000 0000  tusc............
-00000120: 0000 0000 0b00 0000 4000 0000 7376 0100  ........@...sv..
-00000130: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-00000140: 013c 0065 0565 0464 023c 0065 0609 0364  .<.e.e.d.<.e...d
-00000150: 2c64 0465 0764 0565 0364 0665 0865 0719  ,d.e.d.e.d.e.e..
-00000160: 0064 0764 0066 0864 0864 0984 0583 015a  .d.d.f.d.d.....Z
-00000170: 0965 0609 0364 2c64 0a65 0a65 0765 0b66  .e...d,d.e.e.e.f
-00000180: 0219 0064 0565 0364 0665 0865 0719 0064  ...d.e.d.e.e...d
-00000190: 0765 0c6a 0d6a 0e64 0b19 0066 0864 0c64  .e.j.j.d...f.d.d
-000001a0: 0d84 0583 015a 0f64 0e65 0564 0565 0364  .....Z.d.e.d.e.d
-000001b0: 0764 0366 0664 0f64 1084 045a 1065 1164  .d.f.d.d...Z.e.d
-000001c0: 0765 0766 0264 1164 1284 0483 015a 1265  .e.f.d.d.....Z.e
-000001d0: 1164 0765 1366 0264 1364 1484 0483 015a  .d.e.f.d.d.....Z
-000001e0: 1465 1164 0765 0766 0264 1564 1684 0483  .e.d.e.f.d.d....
-000001f0: 015a 1565 1164 0765 1665 0719 0066 0264  .Z.e.d.e.e...f.d
-00000200: 1764 1884 0483 015a 1765 1164 0765 0865  .d.....Z.e.d.e.e
-00000210: 1865 0765 0766 0219 0019 0066 0264 1964  .e.e.f.....f.d.d
-00000220: 1a84 0483 015a 1965 1164 0765 0766 0264  .....Z.e.d.e.f.d
-00000230: 1b64 1c84 0483 015a 1a65 1164 0765 1b66  .d.....Z.e.d.e.f
-00000240: 0264 1d64 1e84 0483 015a 1c64 0765 1d66  .d.d.....Z.d.e.f
-00000250: 0264 1f64 2084 045a 1e64 2165 0764 2265  .d.d ..Z.d!e.d"e
-00000260: 0764 0764 0366 0664 2364 2484 045a 1f64  .d.d.f.d#d$..Z.d
-00000270: 0765 0a65 0765 0b66 0219 0066 0264 2564  .e.e.e.f...f.d%d
-00000280: 2684 045a 2009 2764 2d64 2865 1b64 2965  &..Z .'d-d(e.d)e
-00000290: 0865 0719 0064 0764 0366 0664 2a64 2b84  .e...d.d.f.d*d+.
-000002a0: 055a 2164 0353 0029 2eda 0a49 6e76 6f63  .Z!d.S.)...Invoc
-000002b0: 6174 696f 6eda 205f 496e 766f 6361 7469  ation. _Invocati
-000002c0: 6f6e 5f5f 696e 766f 6361 7469 6f6e 5f64  on__invocation_d
-000002d0: 656c 6567 6174 65da 135f 496e 766f 6361  elegate.._Invoca
-000002e0: 7469 6f6e 5f5f 7265 636f 7264 4eda 0d69  tion__recordN..i
-000002f0: 6e76 6f63 6174 696f 6e5f 6964 da13 696e  nvocation_id..in
-00000300: 766f 6361 7469 6f6e 5f64 656c 6567 6174  vocation_delegat
-00000310: 65da 066f 7267 5f69 64da 0672 6574 7572  e..org_id..retur
-00000320: 6e63 0400 0000 0000 0000 0000 0000 0500  nc..............
-00000330: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
-00000340: 02a0 007c 017c 03a1 027d 047c 007c 047c  ...|.|...}.|.|.|
-00000350: 0283 0253 00a9 014e 2901 5a09 6765 745f  ...S...N).Z.get_
-00000360: 6279 5f69 6429 05da 0363 6c73 720e 0000  by_id)...clsr...
-00000370: 0072 0f00 0000 7210 0000 00da 0672 6563  .r....r......rec
-00000380: 6f72 64a9 0072 1500 0000 faf1 2f63 6f64  ord..r....../cod
-00000390: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000003a0: 6333 3439 3732 3638 3637 302f 7372 632f  c3497268670/src/
-000003b0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
-000003c0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
-000003d0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
-000003e0: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
-000003f0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
-00000400: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
-00000410: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
-00000420: 642f 726f 626f 746f 2d61 692f 726f 626f  d/roboto-ai/robo
-00000430: 746f 2d68 6f73 7465 642d 6170 702f 7061  to-hosted-app/pa
-00000440: 636b 6167 6573 2f72 6f62 6f74 6f5f 7364  ckages/roboto_sd
-00000450: 6b2f 7372 632f 726f 626f 746f 5f73 646b  k/src/roboto_sdk
-00000460: 2f64 6f6d 6169 6e2f 6163 7469 6f6e 732f  /domain/actions/
-00000470: 696e 766f 6361 7469 6f6e 2e70 79da 0766  invocation.py..f
-00000480: 726f 6d5f 6964 1300 0000 7304 0000 000c  rom_id....s.....
-00000490: 070a 017a 1249 6e76 6f63 6174 696f 6e2e  ...z.Invocation.
-000004a0: 6672 6f6d 5f69 64da 0766 696c 7465 7273  from_id..filters
-000004b0: 2903 720b 0000 004e 4e63 0400 0000 0000  ).r....NNc......
-000004c0: 0000 0000 0000 0b00 0000 0600 0000 6300  ..............c.
-000004d0: 0000 73a0 0000 0081 0074 0074 016a 02a0  ..s......t.t.j..
-000004e0: 03a1 0083 017d 0474 007c 01a0 03a1 0083  .....}.t.|......
-000004f0: 017d 057c 057c 0418 007d 067c 0672 2c74  .}.|.|...}.|.r,t
-00000500: 047c 0683 0164 016b 047d 077c 0772 1e64  .|...d.k.}.|.r.d
-00000510: 026e 0164 037d 0874 057c 069b 0064 047c  .n.d.}.t.|...d.|
-00000520: 089b 0064 057c 049b 009d 0583 0182 017c  ...d.|.........|
-00000530: 026a 067c 017c 0364 068d 027d 0909 007c  .j.|.|.d...}...|
-00000540: 096a 0744 005d 087d 0a7c 007c 0a7c 0283  .j.D.].}.|.|.|..
-00000550: 0256 0001 0071 377c 096a 0872 4d7c 026a  .V...q7|.j.rM|.j
-00000560: 067c 017c 037c 096a 0864 088d 037d 096e  .|.|.|.j.d...}.n
-00000570: 0264 0053 0071 3429 094e 7206 0000 007a  .d.S.q4).Nr....z
-00000580: 2661 7265 206e 6f74 206b 6e6f 776e 2061  &are not known a
-00000590: 7474 7269 6275 7465 7320 6f66 2049 6e76  ttributes of Inv
-000005a0: 6f63 6174 696f 6e7a 2669 7320 6e6f 7420  ocationz&is not 
-000005b0: 6120 6b6e 6f77 6e20 6174 7472 6962 7574  a known attribut
-000005c0: 6520 6f66 2049 6e76 6f63 6174 696f 6eda  e of Invocation.
-000005d0: 0120 7a14 2e20 4b6e 6f77 6e20 6174 7472  . z.. Known attr
-000005e0: 6962 7574 6573 3a20 2901 7210 0000 0054  ibutes: ).r....T
-000005f0: 2902 7210 0000 00da 0a70 6167 655f 746f  ).r......page_to
-00000600: 6b65 6e29 09da 0373 6574 7209 0000 00da  ken)...setr.....
-00000610: 0a5f 5f66 6965 6c64 735f 5fda 046b 6579  .__fields__..key
-00000620: 73da 036c 656e da0a 5661 6c75 6545 7272  s..len..ValueErr
-00000630: 6f72 5a11 7175 6572 795f 696e 766f 6361  orZ.query_invoca
-00000640: 7469 6f6e 73da 0569 7465 6d73 da0a 6e65  tions..items..ne
-00000650: 7874 5f74 6f6b 656e 290b 7213 0000 0072  xt_token).r....r
-00000660: 1800 0000 720f 0000 0072 1000 0000 da0a  ....r....r......
-00000670: 6b6e 6f77 6e5f 6b65 7973 da0b 6163 7475  known_keys..actu
-00000680: 616c 5f6b 6579 73da 0c75 6e6b 6e6f 776e  al_keys..unknown
-00000690: 5f6b 6579 73da 0670 6c75 7261 6cda 036d  _keys..plural..m
-000006a0: 7367 da11 7061 6769 6e61 7465 645f 7265  sg..paginated_re
-000006b0: 7375 6c74 7372 1400 0000 7215 0000 0072  sultsr....r....r
-000006c0: 1500 0000 7216 0000 00da 0571 7565 7279  ....r......query
-000006d0: 1d00 0000 732e 0000 0002 800e 070c 0108  ....s...........
-000006e0: 0104 010c 0102 0306 ff02 0202 fd18 0504  ................
-000006f0: 0204 0106 ff02 030a 010e 0106 0104 0108  ................
-00000700: 0108 ff04 0402 f87a 1049 6e76 6f63 6174  .......z.Invocat
-00000710: 696f 6e2e 7175 6572 7972 1400 0000 6303  ion.queryr....c.
-00000720: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-00000730: 0000 0043 0000 0073 1000 0000 7c02 7c00  ...C...s....|.|.
-00000740: 5f00 7c01 7c00 5f01 6400 5300 7212 0000  _.|.|._.d.S.r...
-00000750: 0029 0272 0c00 0000 720d 0000 0029 03da  .).r....r....)..
-00000760: 0473 656c 6672 1400 0000 720f 0000 0072  .selfr....r....r
-00000770: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
-00000780: 5f5f 696e 6974 5f5f 3d00 0000 7304 0000  __init__=...s...
-00000790: 0006 030a 017a 1349 6e76 6f63 6174 696f  .....z.Invocatio
-000007a0: 6e2e 5f5f 696e 6974 5f5f 6301 0000 0000  n.__init__c.....
-000007b0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000007c0: 0000 00f3 0800 0000 7c00 6a00 6a01 5300  ........|.j.j.S.
-000007d0: 7212 0000 0029 0272 0d00 0000 da0b 6163  r....).r......ac
-000007e0: 7469 6f6e 5f6e 616d 65a9 0172 2900 0000  tion_name..r)...
-000007f0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000800: 2c00 0000 4300 0000 f302 0000 0008 027a  ,...C..........z
-00000810: 1649 6e76 6f63 6174 696f 6e2e 6163 7469  .Invocation.acti
-00000820: 6f6e 5f6e 616d 6563 0100 0000 0000 0000  on_namec........
-00000830: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000840: 722b 0000 0072 1200 0000 2902 720d 0000  r+...r....).r...
-00000850: 00da 0b64 6174 615f 736f 7572 6365 722d  ...data_sourcer-
-00000860: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000870: 0000 722f 0000 0047 0000 0072 2e00 0000  ..r/...G...r....
-00000880: 7a16 496e 766f 6361 7469 6f6e 2e64 6174  z.Invocation.dat
-00000890: 615f 736f 7572 6365 6301 0000 0000 0000  a_sourcec.......
-000008a0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000008b0: 0072 2b00 0000 7212 0000 0029 0272 0d00  .r+...r....).r..
-000008c0: 0000 720e 0000 0072 2d00 0000 7215 0000  ..r....r-...r...
-000008d0: 0072 1500 0000 7216 0000 00da 0269 644b  .r....r......idK
-000008e0: 0000 0072 2e00 0000 7a0d 496e 766f 6361  ...r....z.Invoca
-000008f0: 7469 6f6e 2e69 6463 0100 0000 0000 0000  tion.idc........
-00000900: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000910: 722b 0000 0072 1200 0000 2902 720d 0000  r+...r....).r...
-00000920: 00da 0a69 6e70 7574 5f64 6174 6172 2d00  ...input_datar-.
-00000930: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000940: 0072 3100 0000 4f00 0000 722e 0000 007a  .r1...O...r....z
-00000950: 1549 6e76 6f63 6174 696f 6e2e 696e 7075  .Invocation.inpu
-00000960: 745f 6461 7461 6301 0000 0000 0000 0000  t_datac.........
-00000970: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00000980: 2400 0000 7c00 6a00 6a01 7208 7c00 6a00  $...|.j.j.r.|.j.
-00000990: 6a02 730a 6400 5300 7c00 6a00 6a01 7c00  j.s.d.S.|.j.j.|.
-000009a0: 6a00 6a02 6602 5300 7212 0000 0029 0372  j.j.f.S.r....).r
-000009b0: 0d00 0000 5a0b 6c6f 6773 5f62 7563 6b65  ....Z.logs_bucke
-000009c0: 745a 0b6c 6f67 735f 7072 6566 6978 722d  tZ.logs_prefixr-
-000009d0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000009e0: 0000 da0d 6c6f 6773 5f6c 6f63 6174 696f  ....logs_locatio
-000009f0: 6e53 0000 0073 0600 0000 1002 0401 1002  nS...s..........
-00000a00: 7a18 496e 766f 6361 7469 6f6e 2e6c 6f67  z.Invocation.log
-00000a10: 735f 6c6f 6361 7469 6f6e 6301 0000 0000  s_locationc.....
-00000a20: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000a30: 0000 0072 2b00 0000 7212 0000 0029 0272  ...r+...r....).r
-00000a40: 0d00 0000 7210 0000 0072 2d00 0000 7215  ....r....r-...r.
-00000a50: 0000 0072 1500 0000 7216 0000 0072 1000  ...r....r....r..
-00000a60: 0000 5a00 0000 722e 0000 007a 1149 6e76  ..Z...r....z.Inv
-00000a70: 6f63 6174 696f 6e2e 6f72 675f 6964 6301  ocation.org_idc.
-00000a80: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000a90: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
-00000aa0: 6a01 6401 1900 7d01 7c01 6a01 5300 2902  j.d...}.|.j.S.).
-00000ab0: 4ee9 ffff ffff 2902 720d 0000 00da 0673  N.....).r......s
-00000ac0: 7461 7475 7329 0272 2900 0000 da0d 7374  tatus).r).....st
-00000ad0: 6174 7573 5f72 6563 6f72 6472 1500 0000  atus_recordr....
-00000ae0: 7215 0000 0072 1600 0000 7234 0000 005e  r....r....r4...^
-00000af0: 0000 0073 0400 0000 0c02 0601 7a11 496e  ...s........z.In
-00000b00: 766f 6361 7469 6f6e 2e73 7461 7475 7363  vocation.statusc
-00000b10: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000b20: 0400 0000 0300 0000 7326 0000 0074 006a  ........s&...t.j
-00000b30: 0174 006a 0266 0289 0074 0387 0066 0164  .t.j.f...t...f.d
-00000b40: 0164 0284 087c 006a 046a 0544 0083 0183  .d...|.j.j.D....
-00000b50: 0153 0029 037a 890a 2020 2020 2020 2020  .S.).z..        
-00000b60: 416e 2069 6e76 6f63 6174 696f 6e20 6973  An invocation is
-00000b70: 2071 7565 7565 6420 666f 7220 7363 6865   queued for sche
-00000b80: 6475 6c69 6e67 2069 6620 6974 2068 6173  duling if it has
-00000b90: 206e 6f74 2079 6574 2072 6561 6368 6564   not yet reached
-00000ba0: 2074 6865 2022 5363 6865 6475 6c65 6422   the "Scheduled"
-00000bb0: 2073 7461 7475 730a 2020 2020 2020 2020   status.        
-00000bc0: 616e 6420 6974 2069 7320 6e6f 7420 2244  and it is not "D
-00000bd0: 6561 646c 7922 2e0a 2020 2020 2020 2020  eadly"..        
-00000be0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000bf0: 0003 0000 0033 0000 0073 1a00 0000 8100  .....3...s......
-00000c00: 7c00 5d08 7d01 7c01 6a00 8800 7601 5600  |.].}.|.j...v.V.
-00000c10: 0100 7102 6400 5300 7212 0000 0029 0172  ..q.d.S.r....).r
-00000c20: 3400 0000 a902 da02 2e30 7235 0000 00a9  4........0r5....
-00000c30: 015a 1e70 7265 7669 6f75 736c 795f 7363  .Z.previously_sc
-00000c40: 6865 6475 6c65 645f 6f72 5f64 6561 646c  heduled_or_deadl
-00000c50: 7972 1500 0000 7216 0000 00da 093c 6765  yr....r......<ge
-00000c60: 6e65 7870 723e 6c00 0000 730a 0000 0002  nexpr>l...s.....
-00000c70: 8004 0002 0208 ff0a ff7a 3649 6e76 6f63  .........z6Invoc
-00000c80: 6174 696f 6e2e 6973 5f71 7565 7565 645f  ation.is_queued_
-00000c90: 666f 725f 7363 6865 6475 6c69 6e67 2e3c  for_scheduling.<
-00000ca0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00000cb0: 3e29 0672 0a00 0000 5a09 5363 6865 6475  >).r....Z.Schedu
-00000cc0: 6c65 64da 0644 6561 646c 79da 0361 6c6c  led..Deadly..all
-00000cd0: 720d 0000 0072 3400 0000 722d 0000 0072  r....r4...r-...r
-00000ce0: 1500 0000 7238 0000 0072 1600 0000 da18  ....r8...r......
-00000cf0: 6973 5f71 7565 7565 645f 666f 725f 7363  is_queued_for_sc
-00000d00: 6865 6475 6c69 6e67 6300 0000 730c 0000  hedulingc...s...
-00000d10: 0004 0604 0104 fe0c 0406 0208 fe7a 2349  .............z#I
-00000d20: 6e76 6f63 6174 696f 6e2e 6973 5f71 7565  nvocation.is_que
-00000d30: 7565 645f 666f 725f 7363 6865 6475 6c69  ued_for_scheduli
-00000d40: 6e67 da06 6275 636b 6574 da06 7072 6566  ng..bucket..pref
-00000d50: 6978 6303 0000 0000 0000 0000 0000 0004  ixc.............
-00000d60: 0000 0005 0000 0043 0000 0073 1c00 0000  .......C...s....
-00000d70: 7c00 6a00 a001 7c00 6a02 7c01 7c02 a103  |.j...|.j.|.|...
-00000d80: 7d03 7c03 7c00 5f02 6400 5300 7212 0000  }.|.|._.d.S.r...
-00000d90: 0029 0372 0c00 0000 da11 7365 745f 6c6f  .).r......set_lo
-00000da0: 6773 5f6c 6f63 6174 696f 6e72 0d00 0000  gs_locationr....
-00000db0: 2904 7229 0000 0072 3d00 0000 723e 0000  ).r)...r=...r>..
-00000dc0: 00da 0e75 7064 6174 6564 5f72 6563 6f72  ...updated_recor
-00000dd0: 6472 1500 0000 7215 0000 0072 1600 0000  dr....r....r....
-00000de0: 723f 0000 0071 0000 0073 0800 0000 0601  r?...q...s......
-00000df0: 0801 04ff 0a03 7a1c 496e 766f 6361 7469  ......z.Invocati
-00000e00: 6f6e 2e73 6574 5f6c 6f67 735f 6c6f 6361  on.set_logs_loca
-00000e10: 7469 6f6e 6301 0000 0000 0000 0000 0000  tionc...........
-00000e20: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00000e30: 0000 7400 7c00 6a01 8301 5300 7212 0000  ..t.|.j...S.r...
-00000e40: 0029 0272 0500 0000 720d 0000 0072 2d00  .).r....r....r-.
-00000e50: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000e60: 00da 0774 6f5f 6469 6374 7700 0000 7302  ...to_dictw...s.
-00000e70: 0000 000a 017a 1249 6e76 6f63 6174 696f  .....z.Invocatio
-00000e80: 6e2e 746f 5f64 6963 74da 044e 6f6e 65da  n.to_dict..None.
-00000e90: 0b6e 6578 745f 7374 6174 7573 da06 6465  .next_status..de
-00000ea0: 7461 696c 6303 0000 0000 0000 0000 0000  tailc...........
-00000eb0: 0005 0000 0005 0000 0043 0000 0073 4a00  .........C...sJ.
-00000ec0: 0000 7c01 7400 6a01 6b02 7217 7402 6401  ..|.t.j.k.r.t.d.
-00000ed0: 6402 8400 7c00 6a03 6a04 4400 8301 8301  d...|.j.j.D.....
-00000ee0: 7d03 7c03 6403 6b05 7217 7400 6a05 7d01  }.|.d.k.r.t.j.}.
-00000ef0: 7c00 6a06 a007 7c00 6a03 7c01 7c02 a103  |.j...|.j.|.|...
-00000f00: 7d04 7c04 7c00 5f03 6400 5300 2904 4e63  }.|.|._.d.S.).Nc
-00000f10: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000f20: 0400 0000 5300 0000 731c 0000 0067 007c  ....S...s....g.|
-00000f30: 005d 0a7d 017c 016a 0074 016a 026b 0272  .].}.|.j.t.j.k.r
-00000f40: 027c 0191 0271 0253 0072 1500 0000 2903  .|...q.S.r....).
-00000f50: 7234 0000 0072 0a00 0000 da06 4661 696c  r4...r......Fail
-00000f60: 6564 7236 0000 0072 1500 0000 7215 0000  edr6...r....r...
-00000f70: 0072 1600 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00000f80: 703e 8000 0000 730a 0000 0006 0002 020c  p>....s.........
-00000f90: 0102 fe06 027a 2c49 6e76 6f63 6174 696f  .....z,Invocatio
-00000fa0: 6e2e 7570 6461 7465 5f73 7461 7475 732e  n.update_status.
-00000fb0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000fc0: 6d70 3ee9 0200 0000 2908 720a 0000 0072  mp>.....).r....r
-00000fd0: 4500 0000 721e 0000 0072 0d00 0000 7234  E...r....r....r4
-00000fe0: 0000 0072 3a00 0000 720c 0000 005a 1875  ...r:...r....Z.u
-00000ff0: 7064 6174 655f 696e 766f 6361 7469 6f6e  pdate_invocation
-00001000: 5f73 7461 7475 7329 0572 2900 0000 7243  _status).r)...rC
-00001010: 0000 0072 4400 0000 5a0c 6e75 6d5f 6661  ...rD...Z.num_fa
-00001020: 696c 7572 6573 7240 0000 0072 1500 0000  iluresr@...r....
-00001030: 7215 0000 0072 1600 0000 da0d 7570 6461  r....r......upda
-00001040: 7465 5f73 7461 7475 737a 0000 0073 1800  te_statusz...s..
-00001050: 0000 0a03 0202 0601 0602 04fe 04ff 0807  ................
-00001060: 0601 0601 0801 04ff 0a03 7a18 496e 766f  ..........z.Invo
-00001070: 6361 7469 6f6e 2e75 7064 6174 655f 7374  cation.update_st
-00001080: 6174 7573 7212 0000 0029 0172 4200 0000  atusr....).rB...
-00001090: 2922 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )"..__name__..__
-000010a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000010b0: 6e61 6d65 5f5f 7207 0000 00da 0f5f 5f61  name__r......__a
-000010c0: 6e6e 6f74 6174 696f 6e73 5f5f 7209 0000  nnotations__r...
-000010d0: 00da 0b63 6c61 7373 6d65 7468 6f64 da03  ...classmethod..
-000010e0: 7374 7272 0300 0000 7217 0000 00da 0464  strr....r......d
-000010f0: 6963 7472 0200 0000 da0b 636f 6c6c 6563  ictr......collec
-00001100: 7469 6f6e 73da 0361 6263 da09 4765 6e65  tions..abc..Gene
-00001110: 7261 746f 7272 2800 0000 722a 0000 00da  ratorr(...r*....
-00001120: 0870 726f 7065 7274 7972 2c00 0000 7208  .propertyr,...r.
-00001130: 0000 0072 2f00 0000 7230 0000 00da 046c  ...r/...r0.....l
-00001140: 6973 7472 3100 0000 da05 7475 706c 6572  istr1.....tupler
-00001150: 3200 0000 7210 0000 0072 0a00 0000 7234  2...r....r....r4
-00001160: 0000 00da 0462 6f6f 6c72 3c00 0000 723f  .....boolr<...r?
-00001170: 0000 0072 4100 0000 7248 0000 0072 1500  ...rA...rH...r..
-00001180: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001190: 0072 0b00 0000 0f00 0000 7372 0000 000a  .r........sr....
-000011a0: 0008 0108 0102 0202 0504 fc02 0202 fe02  ................
-000011b0: 0302 fd06 0402 fc02 050c fb02 0902 0504  ................
-000011c0: fc0a 0202 fe02 0302 fd06 0402 fc0a 050c  ................
-000011d0: fb02 1f02 0102 ff02 0102 ff02 020a fe02  ................
-000011e0: 0610 0102 0310 0102 0310 0102 0314 0102  ................
-000011f0: 031c 0102 0610 0102 0310 010e 0416 0e16  ................
-00001200: 0602 0404 ff02 0102 ff06 0102 ff02 020e  ................
-00001210: fe72 0b00 0000 290e da0f 636f 6c6c 6563  .r....)...collec
-00001220: 7469 6f6e 732e 6162 6372 5000 0000 da06  tions.abcrP.....
-00001230: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00001240: da05 7365 7264 6572 0500 0000 720f 0000  ..serder....r...
-00001250: 0072 0700 0000 da11 696e 766f 6361 7469  .r......invocati
-00001260: 6f6e 5f72 6563 6f72 6472 0800 0000 7209  on_recordr....r.
-00001270: 0000 0072 0a00 0000 720b 0000 0072 1500  ...r....r....r..
-00001280: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001290: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000012a0: 0c00 0000 0800 1001 0c02 0c01 1403 1207  ................
+00000050: 0100 6405 6406 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
+00000060: 0100 6405 6407 6c0a 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
+00000070: 6408 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
+00000080: 6d10 5a10 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
+00000090: 8302 5a11 6401 5300 290b e900 0000 004e  ..Z.d.S.)......N
+000000a0: 2902 da03 416e 79da 084f 7074 696f 6e61  )...Any..Optiona
+000000b0: 6ce9 0300 0000 2901 da16 7079 6461 6e74  l.....)...pydant
+000000c0: 6963 5f6a 736f 6e61 626c 655f 6469 6374  ic_jsonable_dict
+000000d0: e901 0000 0029 02da 1343 6f6d 7075 7465  .....)...Compute
+000000e0: 5265 7175 6972 656d 656e 7473 da13 436f  Requirements..Co
+000000f0: 6e74 6169 6e65 7250 6172 616d 6574 6572  ntainerParameter
+00000100: 7329 01da 1249 6e76 6f63 6174 696f 6e44  s)...InvocationD
+00000110: 656c 6567 6174 6529 04da 1449 6e76 6f63  elegate)...Invoc
+00000120: 6174 696f 6e44 6174 6153 6f75 7263 65da  ationDataSource.
+00000130: 1049 6e76 6f63 6174 696f 6e52 6563 6f72  .InvocationRecor
+00000140: 64da 1049 6e76 6f63 6174 696f 6e53 7461  d..InvocationSta
+00000150: 7475 73da 1649 6e76 6f63 6174 696f 6e53  tus..InvocationS
+00000160: 7461 7475 7352 6563 6f72 6463 0000 0000  tatusRecordc....
+00000170: 0000 0000 0000 0000 0000 0000 0b00 0000  ................
+00000180: 4000 0000 739e 0100 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000190: 0255 0065 0365 0464 013c 0065 0565 0464  .U.e.e.d.<.e.e.d
+000001a0: 023c 0065 0609 0364 3064 0465 0764 0565  .<.e...d0d.e.d.e
+000001b0: 0364 0665 0865 0719 0064 0764 0066 0864  .d.e.e...d.d.f.d
+000001c0: 0864 0984 0583 015a 0965 0609 0364 3064  .d.....Z.e...d0d
+000001d0: 0a65 0a65 0765 0b66 0219 0064 0565 0364  .e.e.e.f...d.e.d
+000001e0: 0665 0865 0719 0064 0765 0c6a 0d6a 0e64  .e.e...d.e.j.j.d
+000001f0: 0b19 0066 0864 0c64 0d84 0583 015a 0f64  ...f.d.d.....Z.d
+00000200: 0e65 0564 0565 0364 0764 0366 0664 0f64  .e.d.e.d.d.f.d.d
+00000210: 1084 045a 1065 1164 0765 0766 0264 1164  ...Z.e.d.e.f.d.d
+00000220: 1284 0483 015a 1265 1164 0765 1366 0264  .....Z.e.d.e.f.d
+00000230: 1364 1484 0483 015a 1465 1164 0765 1566  .d.....Z.e.d.e.f
+00000240: 0264 1564 1684 0483 015a 1665 1164 0765  .d.d.....Z.e.d.e
+00000250: 1766 0264 1764 1884 0483 015a 1865 1164  .f.d.d.....Z.e.d
+00000260: 0765 0766 0264 1964 1a84 0483 015a 1965  .e.f.d.d.....Z.e
+00000270: 1164 0765 1a65 0719 0066 0264 1b64 1c84  .d.e.e...f.d.d..
+00000280: 0483 015a 1b65 1164 0765 0865 1c65 0765  ...Z.e.d.e.e.e.e
+00000290: 0766 0219 0019 0066 0264 1d64 1e84 0483  .f.....f.d.d....
+000002a0: 015a 1d65 1164 0765 0766 0264 1f64 2084  .Z.e.d.e.f.d.d .
+000002b0: 0483 015a 1e65 1164 0765 1a65 1f19 0066  ...Z.e.d.e.e...f
+000002c0: 0264 2164 2284 0483 015a 2064 0765 2166  .d!d"....Z d.e!f
+000002d0: 0264 2364 2484 045a 2264 2565 0764 2665  .d#d$..Z"d%e.d&e
+000002e0: 0764 0764 0366 0664 2764 2884 045a 2364  .d.d.f.d'd(..Z#d
+000002f0: 0765 0a65 0765 0b66 0219 0066 0264 2964  .e.e.e.f...f.d)d
+00000300: 2a84 045a 2409 2b64 3164 2c65 2564 2d65  *..Z$.+d1d,e%d-e
+00000310: 0865 0719 0064 0764 0366 0664 2e64 2f84  .e...d.d.f.d.d/.
+00000320: 055a 2664 0353 0029 32da 0a49 6e76 6f63  .Z&d.S.)2..Invoc
+00000330: 6174 696f 6eda 205f 496e 766f 6361 7469  ation. _Invocati
+00000340: 6f6e 5f5f 696e 766f 6361 7469 6f6e 5f64  on__invocation_d
+00000350: 656c 6567 6174 65da 135f 496e 766f 6361  elegate.._Invoca
+00000360: 7469 6f6e 5f5f 7265 636f 7264 4eda 0d69  tion__recordN..i
+00000370: 6e76 6f63 6174 696f 6e5f 6964 da13 696e  nvocation_id..in
+00000380: 766f 6361 7469 6f6e 5f64 656c 6567 6174  vocation_delegat
+00000390: 65da 066f 7267 5f69 64da 0672 6574 7572  e..org_id..retur
+000003a0: 6e63 0400 0000 0000 0000 0000 0000 0500  nc..............
+000003b0: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
+000003c0: 02a0 007c 017c 03a1 027d 047c 007c 047c  ...|.|...}.|.|.|
+000003d0: 0283 0253 00a9 014e 2901 5a09 6765 745f  ...S...N).Z.get_
+000003e0: 6279 5f69 6429 05da 0363 6c73 7211 0000  by_id)...clsr...
+000003f0: 0072 1200 0000 7213 0000 00da 0672 6563  .r....r......rec
+00000400: 6f72 64a9 0072 1800 0000 faf1 2f63 6f64  ord..r....../cod
+00000410: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
+00000420: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
+00000430: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
+00000440: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
+00000450: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
+00000460: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
+00000470: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
+00000480: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
+00000490: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
+000004a0: 642f 726f 626f 746f 2d61 692f 726f 626f  d/roboto-ai/robo
+000004b0: 746f 2d68 6f73 7465 642d 6170 702f 7061  to-hosted-app/pa
+000004c0: 636b 6167 6573 2f72 6f62 6f74 6f5f 7364  ckages/roboto_sd
+000004d0: 6b2f 7372 632f 726f 626f 746f 5f73 646b  k/src/roboto_sdk
+000004e0: 2f64 6f6d 6169 6e2f 6163 7469 6f6e 732f  /domain/actions/
+000004f0: 696e 766f 6361 7469 6f6e 2e70 79da 0766  invocation.py..f
+00000500: 726f 6d5f 6964 1800 0000 7304 0000 000c  rom_id....s.....
+00000510: 070a 017a 1249 6e76 6f63 6174 696f 6e2e  ...z.Invocation.
+00000520: 6672 6f6d 5f69 64da 0766 696c 7465 7273  from_id..filters
+00000530: 2903 720e 0000 004e 4e63 0400 0000 0000  ).r....NNc......
+00000540: 0000 0000 0000 0b00 0000 0600 0000 6300  ..............c.
+00000550: 0000 73a0 0000 0081 0074 0074 016a 02a0  ..s......t.t.j..
+00000560: 03a1 0083 017d 0474 007c 01a0 03a1 0083  .....}.t.|......
+00000570: 017d 057c 057c 0418 007d 067c 0672 2c74  .}.|.|...}.|.r,t
+00000580: 047c 0683 0164 016b 047d 077c 0772 1e64  .|...d.k.}.|.r.d
+00000590: 026e 0164 037d 0874 057c 069b 0064 047c  .n.d.}.t.|...d.|
+000005a0: 089b 0064 057c 049b 009d 0583 0182 017c  ...d.|.........|
+000005b0: 026a 067c 017c 0364 068d 027d 0909 007c  .j.|.|.d...}...|
+000005c0: 096a 0744 005d 087d 0a7c 007c 0a7c 0283  .j.D.].}.|.|.|..
+000005d0: 0256 0001 0071 377c 096a 0872 4d7c 026a  .V...q7|.j.rM|.j
+000005e0: 067c 017c 037c 096a 0864 088d 037d 096e  .|.|.|.j.d...}.n
+000005f0: 0264 0053 0071 3429 094e 7206 0000 007a  .d.S.q4).Nr....z
+00000600: 2661 7265 206e 6f74 206b 6e6f 776e 2061  &are not known a
+00000610: 7474 7269 6275 7465 7320 6f66 2049 6e76  ttributes of Inv
+00000620: 6f63 6174 696f 6e7a 2669 7320 6e6f 7420  ocationz&is not 
+00000630: 6120 6b6e 6f77 6e20 6174 7472 6962 7574  a known attribut
+00000640: 6520 6f66 2049 6e76 6f63 6174 696f 6eda  e of Invocation.
+00000650: 0120 7a14 2e20 4b6e 6f77 6e20 6174 7472  . z.. Known attr
+00000660: 6962 7574 6573 3a20 2901 7213 0000 0054  ibutes: ).r....T
+00000670: 2902 7213 0000 00da 0a70 6167 655f 746f  ).r......page_to
+00000680: 6b65 6e29 09da 0373 6574 720b 0000 00da  ken)...setr.....
+00000690: 0a5f 5f66 6965 6c64 735f 5fda 046b 6579  .__fields__..key
+000006a0: 73da 036c 656e da0a 5661 6c75 6545 7272  s..len..ValueErr
+000006b0: 6f72 5a11 7175 6572 795f 696e 766f 6361  orZ.query_invoca
+000006c0: 7469 6f6e 73da 0569 7465 6d73 da0a 6e65  tions..items..ne
+000006d0: 7874 5f74 6f6b 656e 290b 7216 0000 0072  xt_token).r....r
+000006e0: 1b00 0000 7212 0000 0072 1300 0000 da0a  ....r....r......
+000006f0: 6b6e 6f77 6e5f 6b65 7973 da0b 6163 7475  known_keys..actu
+00000700: 616c 5f6b 6579 73da 0c75 6e6b 6e6f 776e  al_keys..unknown
+00000710: 5f6b 6579 73da 0670 6c75 7261 6cda 036d  _keys..plural..m
+00000720: 7367 da11 7061 6769 6e61 7465 645f 7265  sg..paginated_re
+00000730: 7375 6c74 7372 1700 0000 7218 0000 0072  sultsr....r....r
+00000740: 1800 0000 7219 0000 00da 0571 7565 7279  ....r......query
+00000750: 2200 0000 732e 0000 0002 800e 070c 0108  "...s...........
+00000760: 0104 010c 0102 0306 ff02 0202 fd18 0504  ................
+00000770: 0204 0106 ff02 030a 010e 0106 0104 0108  ................
+00000780: 0108 ff04 0402 f87a 1049 6e76 6f63 6174  .......z.Invocat
+00000790: 696f 6e2e 7175 6572 7972 1700 0000 6303  ion.queryr....c.
+000007a0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+000007b0: 0000 0043 0000 0073 1000 0000 7c02 7c00  ...C...s....|.|.
+000007c0: 5f00 7c01 7c00 5f01 6400 5300 7215 0000  _.|.|._.d.S.r...
+000007d0: 0029 0272 0f00 0000 7210 0000 0029 03da  .).r....r....)..
+000007e0: 0473 656c 6672 1700 0000 7212 0000 0072  .selfr....r....r
+000007f0: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
+00000800: 5f5f 696e 6974 5f5f 4200 0000 7304 0000  __init__B...s...
+00000810: 0006 030a 017a 1349 6e76 6f63 6174 696f  .....z.Invocatio
+00000820: 6e2e 5f5f 696e 6974 5f5f 6301 0000 0000  n.__init__c.....
+00000830: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000840: 0000 00f3 0800 0000 7c00 6a00 6a01 5300  ........|.j.j.S.
+00000850: 7215 0000 0029 0272 1000 0000 da0b 6163  r....).r......ac
+00000860: 7469 6f6e 5f6e 616d 65a9 0172 2c00 0000  tion_name..r,...
+00000870: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000880: 2f00 0000 4800 0000 f302 0000 0008 027a  /...H..........z
+00000890: 1649 6e76 6f63 6174 696f 6e2e 6163 7469  .Invocation.acti
+000008a0: 6f6e 5f6e 616d 6563 0100 0000 0000 0000  on_namec........
+000008b0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000008c0: 722e 0000 0072 1500 0000 2902 7210 0000  r....r....).r...
+000008d0: 00da 1463 6f6d 7075 7465 5f72 6571 7569  ...compute_requi
+000008e0: 7265 6d65 6e74 7372 3000 0000 7218 0000  rementsr0...r...
+000008f0: 0072 1800 0000 7219 0000 0072 3200 0000  .r....r....r2...
+00000900: 4c00 0000 7231 0000 007a 1f49 6e76 6f63  L...r1...z.Invoc
+00000910: 6174 696f 6e2e 636f 6d70 7574 655f 7265  ation.compute_re
+00000920: 7175 6972 656d 656e 7473 6301 0000 0000  quirementsc.....
+00000930: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000940: 0000 0072 2e00 0000 7215 0000 0029 0272  ...r....r....).r
+00000950: 1000 0000 da14 636f 6e74 6169 6e65 725f  ......container_
+00000960: 7061 7261 6d65 7465 7273 7230 0000 0072  parametersr0...r
+00000970: 1800 0000 7218 0000 0072 1900 0000 7233  ....r....r....r3
+00000980: 0000 0050 0000 0072 3100 0000 7a1f 496e  ...P...r1...z.In
+00000990: 766f 6361 7469 6f6e 2e63 6f6e 7461 696e  vocation.contain
+000009a0: 6572 5f70 6172 616d 6574 6572 7363 0100  er_parametersc..
+000009b0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000009c0: 0000 4300 0000 722e 0000 0072 1500 0000  ..C...r....r....
+000009d0: 2902 7210 0000 00da 0b64 6174 615f 736f  ).r......data_so
+000009e0: 7572 6365 7230 0000 0072 1800 0000 7218  urcer0...r....r.
+000009f0: 0000 0072 1900 0000 7234 0000 0054 0000  ...r....r4...T..
+00000a00: 0072 3100 0000 7a16 496e 766f 6361 7469  .r1...z.Invocati
+00000a10: 6f6e 2e64 6174 615f 736f 7572 6365 6301  on.data_sourcec.
+00000a20: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000a30: 0000 0043 0000 0072 2e00 0000 7215 0000  ...C...r....r...
+00000a40: 0029 0272 1000 0000 7211 0000 0072 3000  .).r....r....r0.
+00000a50: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000a60: 00da 0269 6458 0000 0072 3100 0000 7a0d  ...idX...r1...z.
+00000a70: 496e 766f 6361 7469 6f6e 2e69 6463 0100  Invocation.idc..
+00000a80: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000a90: 0000 4300 0000 722e 0000 0072 1500 0000  ..C...r....r....
+00000aa0: 2902 7210 0000 00da 0a69 6e70 7574 5f64  ).r......input_d
+00000ab0: 6174 6172 3000 0000 7218 0000 0072 1800  atar0...r....r..
+00000ac0: 0000 7219 0000 0072 3600 0000 5c00 0000  ..r....r6...\...
+00000ad0: 7231 0000 007a 1549 6e76 6f63 6174 696f  r1...z.Invocatio
+00000ae0: 6e2e 696e 7075 745f 6461 7461 6301 0000  n.input_datac...
+00000af0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000b00: 0043 0000 0073 2400 0000 7c00 6a00 6a01  .C...s$...|.j.j.
+00000b10: 7208 7c00 6a00 6a02 730a 6400 5300 7c00  r.|.j.j.s.d.S.|.
+00000b20: 6a00 6a01 7c00 6a00 6a02 6602 5300 7215  j.j.|.j.j.f.S.r.
+00000b30: 0000 0029 0372 1000 0000 5a0b 6c6f 6773  ...).r....Z.logs
+00000b40: 5f62 7563 6b65 745a 0b6c 6f67 735f 7072  _bucketZ.logs_pr
+00000b50: 6566 6978 7230 0000 0072 1800 0000 7218  efixr0...r....r.
+00000b60: 0000 0072 1900 0000 da0d 6c6f 6773 5f6c  ...r......logs_l
+00000b70: 6f63 6174 696f 6e60 0000 0073 0600 0000  ocation`...s....
+00000b80: 1002 0401 1002 7a18 496e 766f 6361 7469  ......z.Invocati
+00000b90: 6f6e 2e6c 6f67 735f 6c6f 6361 7469 6f6e  on.logs_location
+00000ba0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000bb0: 0001 0000 0043 0000 0072 2e00 0000 7215  .....C...r....r.
+00000bc0: 0000 0029 0272 1000 0000 7213 0000 0072  ...).r....r....r
+00000bd0: 3000 0000 7218 0000 0072 1800 0000 7219  0...r....r....r.
+00000be0: 0000 0072 1300 0000 6700 0000 7231 0000  ...r....g...r1..
+00000bf0: 007a 1149 6e76 6f63 6174 696f 6e2e 6f72  .z.Invocation.or
+00000c00: 675f 6964 6301 0000 0000 0000 0000 0000  g_idc...........
+00000c10: 0001 0000 0001 0000 0043 0000 0072 2e00  .........C...r..
+00000c20: 0000 7215 0000 0029 0272 1000 0000 da06  ..r....).r......
+00000c30: 7374 6174 7573 7230 0000 0072 1800 0000  statusr0...r....
+00000c40: 7218 0000 0072 1900 0000 da0a 7374 6174  r....r......stat
+00000c50: 7573 5f6c 6f67 6b00 0000 7231 0000 007a  us_logk...r1...z
+00000c60: 1549 6e76 6f63 6174 696f 6e2e 7374 6174  .Invocation.stat
+00000c70: 7573 5f6c 6f67 6301 0000 0000 0000 0000  us_logc.........
+00000c80: 0000 0001 0000 0004 0000 0003 0000 0073  ...............s
+00000c90: 2600 0000 7400 6a01 7400 6a02 6602 8900  &...t.j.t.j.f...
+00000ca0: 7403 8700 6601 6401 6402 8408 7c00 6a04  t...f.d.d...|.j.
+00000cb0: 6a05 4400 8301 8301 5300 2903 7a89 0a20  j.D.....S.).z.. 
+00000cc0: 2020 2020 2020 2041 6e20 696e 766f 6361         An invoca
+00000cd0: 7469 6f6e 2069 7320 7175 6575 6564 2066  tion is queued f
+00000ce0: 6f72 2073 6368 6564 756c 696e 6720 6966  or scheduling if
+00000cf0: 2069 7420 6861 7320 6e6f 7420 7965 7420   it has not yet 
+00000d00: 7265 6163 6865 6420 7468 6520 2253 6368  reached the "Sch
+00000d10: 6564 756c 6564 2220 7374 6174 7573 0a20  eduled" status. 
+00000d20: 2020 2020 2020 2061 6e64 2069 7420 6973         and it is
+00000d30: 206e 6f74 2022 4465 6164 6c79 222e 0a20   not "Deadly".. 
+00000d40: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+00000d50: 0000 0000 0200 0000 0300 0000 3300 0000  ............3...
+00000d60: 731a 0000 0081 007c 005d 087d 017c 016a  s......|.].}.|.j
+00000d70: 0088 0076 0156 0001 0071 0264 0053 0072  ...v.V...q.d.S.r
+00000d80: 1500 0000 2901 7238 0000 00a9 02da 022e  ....).r8........
+00000d90: 305a 0d73 7461 7475 735f 7265 636f 7264  0Z.status_record
+00000da0: a901 5a1e 7072 6576 696f 7573 6c79 5f73  ..Z.previously_s
+00000db0: 6368 6564 756c 6564 5f6f 725f 6465 6164  cheduled_or_dead
+00000dc0: 6c79 7218 0000 0072 1900 0000 da09 3c67  lyr....r......<g
+00000dd0: 656e 6578 7072 3e78 0000 0073 0a00 0000  enexpr>x...s....
+00000de0: 0280 0400 0202 08ff 0aff 7a36 496e 766f  ..........z6Invo
+00000df0: 6361 7469 6f6e 2e69 735f 7175 6575 6564  cation.is_queued
+00000e00: 5f66 6f72 5f73 6368 6564 756c 696e 672e  _for_scheduling.
+00000e10: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000e20: 723e 2906 720c 0000 005a 0953 6368 6564  r>).r....Z.Sched
+00000e30: 756c 6564 da06 4465 6164 6c79 da03 616c  uled..Deadly..al
+00000e40: 6c72 1000 0000 7238 0000 0072 3000 0000  lr....r8...r0...
+00000e50: 7218 0000 0072 3c00 0000 7219 0000 00da  r....r<...r.....
+00000e60: 1869 735f 7175 6575 6564 5f66 6f72 5f73  .is_queued_for_s
+00000e70: 6368 6564 756c 696e 676f 0000 0073 0c00  chedulingo...s..
+00000e80: 0000 0406 0401 04fe 0c04 0602 08fe 7a23  ..............z#
+00000e90: 496e 766f 6361 7469 6f6e 2e69 735f 7175  Invocation.is_qu
+00000ea0: 6575 6564 5f66 6f72 5f73 6368 6564 756c  eued_for_schedul
+00000eb0: 696e 67da 0662 7563 6b65 74da 0670 7265  ing..bucket..pre
+00000ec0: 6669 7863 0300 0000 0000 0000 0000 0000  fixc............
+00000ed0: 0400 0000 0500 0000 4300 0000 731c 0000  ........C...s...
+00000ee0: 007c 006a 00a0 017c 006a 027c 017c 02a1  .|.j...|.j.|.|..
+00000ef0: 037d 037c 037c 005f 0264 0053 0072 1500  .}.|.|._.d.S.r..
+00000f00: 0000 2903 720f 0000 00da 1173 6574 5f6c  ..).r......set_l
+00000f10: 6f67 735f 6c6f 6361 7469 6f6e 7210 0000  ogs_locationr...
+00000f20: 0029 0472 2c00 0000 7241 0000 0072 4200  .).r,...rA...rB.
+00000f30: 0000 da0e 7570 6461 7465 645f 7265 636f  ....updated_reco
+00000f40: 7264 7218 0000 0072 1800 0000 7219 0000  rdr....r....r...
+00000f50: 0072 4300 0000 7d00 0000 7308 0000 0006  .rC...}...s.....
+00000f60: 0108 0104 ff0a 037a 1c49 6e76 6f63 6174  .......z.Invocat
+00000f70: 696f 6e2e 7365 745f 6c6f 6773 5f6c 6f63  ion.set_logs_loc
+00000f80: 6174 696f 6e63 0100 0000 0000 0000 0000  ationc..........
+00000f90: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000fa0: 0000 0074 007c 006a 0183 0153 0072 1500  ...t.|.j...S.r..
+00000fb0: 0000 2902 7205 0000 0072 1000 0000 7230  ..).r....r....r0
+00000fc0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000fd0: 0000 da07 746f 5f64 6963 7483 0000 0073  ....to_dict....s
+00000fe0: 0200 0000 0a01 7a12 496e 766f 6361 7469  ......z.Invocati
+00000ff0: 6f6e 2e74 6f5f 6469 6374 da04 4e6f 6e65  on.to_dict..None
+00001000: da0b 6e65 7874 5f73 7461 7475 73da 0664  ..next_status..d
+00001010: 6574 6169 6c63 0300 0000 0000 0000 0000  etailc..........
+00001020: 0000 0500 0000 0500 0000 4300 0000 734a  ..........C...sJ
+00001030: 0000 007c 0174 006a 016b 0272 1774 0264  ...|.t.j.k.r.t.d
+00001040: 0164 0284 007c 006a 036a 0444 0083 0183  .d...|.j.j.D....
+00001050: 017d 037c 0364 036b 0572 1774 006a 057d  .}.|.d.k.r.t.j.}
+00001060: 017c 006a 06a0 077c 006a 037c 017c 02a1  .|.j...|.j.|.|..
+00001070: 037d 047c 047c 005f 0364 0053 0029 044e  .}.|.|._.d.S.).N
+00001080: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001090: 0004 0000 0053 0000 0073 1c00 0000 6700  .....S...s....g.
+000010a0: 7c00 5d0a 7d01 7c01 6a00 7401 6a02 6b02  |.].}.|.j.t.j.k.
+000010b0: 7202 7c01 9102 7102 5300 7218 0000 0029  r.|...q.S.r....)
+000010c0: 0372 3800 0000 720c 0000 00da 0646 6169  .r8...r......Fai
+000010d0: 6c65 6472 3a00 0000 7218 0000 0072 1800  ledr:...r....r..
+000010e0: 0000 7219 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+000010f0: 6d70 3e8c 0000 0073 0a00 0000 0600 0202  mp>....s........
+00001100: 0c01 02fe 0602 7a2c 496e 766f 6361 7469  ......z,Invocati
+00001110: 6f6e 2e75 7064 6174 655f 7374 6174 7573  on.update_status
+00001120: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001130: 6f6d 703e e902 0000 0029 0872 0c00 0000  omp>.....).r....
+00001140: 7249 0000 0072 2100 0000 7210 0000 0072  rI...r!...r....r
+00001150: 3800 0000 723e 0000 0072 0f00 0000 5a18  8...r>...r....Z.
+00001160: 7570 6461 7465 5f69 6e76 6f63 6174 696f  update_invocatio
+00001170: 6e5f 7374 6174 7573 2905 722c 0000 0072  n_status).r,...r
+00001180: 4700 0000 7248 0000 005a 0c6e 756d 5f66  G...rH...Z.num_f
+00001190: 6169 6c75 7265 7372 4400 0000 7218 0000  ailuresrD...r...
+000011a0: 0072 1800 0000 7219 0000 00da 0d75 7064  .r....r......upd
+000011b0: 6174 655f 7374 6174 7573 8600 0000 7318  ate_status....s.
+000011c0: 0000 000a 0302 0206 0106 0204 fe04 ff08  ................
+000011d0: 0706 0106 0108 0104 ff0a 037a 1849 6e76  ...........z.Inv
+000011e0: 6f63 6174 696f 6e2e 7570 6461 7465 5f73  ocation.update_s
+000011f0: 7461 7475 7372 1500 0000 2901 7246 0000  tatusr....).rF..
+00001200: 0029 27da 085f 5f6e 616d 655f 5fda 0a5f  .)'..__name__.._
+00001210: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001220: 6c6e 616d 655f 5f72 0900 0000 da0f 5f5f  lname__r......__
+00001230: 616e 6e6f 7461 7469 6f6e 735f 5f72 0b00  annotations__r..
+00001240: 0000 da0b 636c 6173 736d 6574 686f 64da  ....classmethod.
+00001250: 0373 7472 7203 0000 0072 1a00 0000 da04  .strr....r......
+00001260: 6469 6374 7202 0000 00da 0b63 6f6c 6c65  dictr......colle
+00001270: 6374 696f 6e73 da03 6162 63da 0947 656e  ctions..abc..Gen
+00001280: 6572 6174 6f72 722b 0000 0072 2d00 0000  eratorr+...r-...
+00001290: da08 7072 6f70 6572 7479 722f 0000 0072  ..propertyr/...r
+000012a0: 0700 0000 7232 0000 0072 0800 0000 7233  ....r2...r....r3
+000012b0: 0000 0072 0a00 0000 7234 0000 0072 3500  ...r....r4...r5.
+000012c0: 0000 da04 6c69 7374 7236 0000 00da 0574  ....listr6.....t
+000012d0: 7570 6c65 7237 0000 0072 1300 0000 720d  upler7...r....r.
+000012e0: 0000 0072 3900 0000 da04 626f 6f6c 7240  ...r9.....boolr@
+000012f0: 0000 0072 4300 0000 7245 0000 0072 0c00  ...rC...rE...r..
+00001300: 0000 724c 0000 0072 1800 0000 7218 0000  ..rL...r....r...
+00001310: 0072 1800 0000 7219 0000 0072 0e00 0000  .r....r....r....
+00001320: 1400 0000 737a 0000 000a 0008 0108 0102  ....sz..........
+00001330: 0202 0504 fc02 0202 fe02 0302 fd06 0402  ................
+00001340: fc02 050c fb02 0902 0504 fc0a 0202 fe02  ................
+00001350: 0302 fd06 0402 fc0a 050c fb02 1f02 0102  ................
+00001360: ff02 0102 ff02 020a fe02 0610 0102 0310  ................
+00001370: 0102 0310 0102 0310 0102 0310 0102 0314  ................
+00001380: 0102 031c 0102 0610 0102 0314 010e 0316  ................
+00001390: 0e16 0602 0404 ff02 0102 ff06 0102 ff02  ................
+000013a0: 020e fe72 0e00 0000 2912 da0f 636f 6c6c  ...r....)...coll
+000013b0: 6563 7469 6f6e 732e 6162 6372 5400 0000  ections.abcrT...
+000013c0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
+000013d0: 0000 da05 7365 7264 6572 0500 0000 da1a  ....serder......
+000013e0: 6163 7469 6f6e 5f63 6f6e 7461 696e 6572  action_container
+000013f0: 5f72 6573 6f75 7263 6573 7207 0000 0072  _resourcesr....r
+00001400: 0800 0000 7212 0000 0072 0900 0000 da11  ....r....r......
+00001410: 696e 766f 6361 7469 6f6e 5f72 6563 6f72  invocation_recor
+00001420: 6472 0a00 0000 720b 0000 0072 0c00 0000  dr....r....r....
+00001430: 720d 0000 0072 0e00 0000 7218 0000 0072  r....r....r....r
+00001440: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
+00001450: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
+00001460: 0008 0010 010c 0210 010c 0418 0312 08    ...............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,158 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 be06 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 9307 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
+00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
-00000070: 8400 6408 6500 6a0b 8303 5a0c 6401 5300  ..d.e.j...Z.d.S.
-00000080: 2909 e900 0000 004e 2902 da03 416e 79da  )......N)...Any.
-00000090: 084f 7074 696f 6e61 6ce9 0300 0000 2901  .Optional.....).
-000000a0: da0d 5061 6769 6e61 7465 644c 6973 74e9  ..PaginatedList.
-000000b0: 0100 0000 2904 da18 496e 766f 6361 7469  ....)...Invocati
-000000c0: 6f6e 4461 7461 536f 7572 6365 5479 7065  onDataSourceType
-000000d0: da10 496e 766f 6361 7469 6f6e 5265 636f  ..InvocationReco
-000000e0: 7264 da10 496e 766f 6361 7469 6f6e 536f  rd..InvocationSo
-000000f0: 7572 6365 da10 496e 766f 6361 7469 6f6e  urce..Invocation
-00000100: 5374 6174 7573 6300 0000 0000 0000 0000  Statusc.........
-00000110: 0000 0000 0000 0012 0000 0040 0000 0073  ...........@...s
-00000120: fc00 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
-00000130: 0901 0901 641c 6402 6505 6403 6506 6505  ....d.d.e.d.e.e.
-00000140: 1900 6404 6505 6405 6507 6406 6508 6407  ..d.e.d.e.d.e.d.
-00000150: 6509 6505 1900 6408 6509 6505 1900 6409  e.e...d.e.e...d.
-00000160: 650a 6610 640a 640b 8405 8301 5a0b 6503  e.f.d.d.....Z.e.
-00000170: 6a04 0901 641d 640c 6505 6408 6509 6505  j...d.d.e.d.e.e.
-00000180: 1900 6409 650a 6606 640d 640e 8405 8301  ..d.e.f.d.d.....
-00000190: 5a0c 6503 6a04 640f 650a 6410 6505 6411  Z.e.j.d.e.d.e.d.
-000001a0: 6505 6409 650a 6608 6412 6413 8404 8301  e.d.e.f.d.d.....
-000001b0: 5a0d 6503 6a04 0901 641d 640f 650a 6414  Z.e.j...d.d.e.d.
-000001c0: 650e 6415 6509 6505 1900 6409 650a 6608  e.d.e.e...d.e.f.
-000001d0: 6416 6417 8405 8301 5a0f 6503 6a04 0901  d.d.....Z.e.j...
-000001e0: 0901 641c 6418 6510 6505 6511 6602 1900  ..d.d.e.e.e.f...
-000001f0: 6408 6509 6505 1900 6419 6509 6510 6505  d.e.e...d.e.e.e.
-00000200: 6505 6602 1900 1900 6409 6512 650a 1900  e.f.....d.e.e...
-00000210: 6608 641a 641b 8405 8301 5a13 6401 5300  f.d.d.....Z.d.S.
-00000220: 291e da12 496e 766f 6361 7469 6f6e 4465  )...InvocationDe
-00000230: 6c65 6761 7465 4eda 0b61 6374 696f 6e5f  legateN..action_
-00000240: 6e61 6d65 da0a 696e 7075 745f 6461 7461  name..input_data
-00000250: da0e 6461 7461 5f73 6f75 7263 655f 6964  ..data_source_id
-00000260: da10 6461 7461 5f73 6f75 7263 655f 7479  ..data_source_ty
-00000270: 7065 da11 696e 766f 6361 7469 6f6e 5f73  pe..invocation_s
-00000280: 6f75 7263 65da 1469 6e76 6f63 6174 696f  ource..invocatio
-00000290: 6e5f 736f 7572 6365 5f69 64da 066f 7267  n_source_id..org
-000002a0: 5f69 64da 0672 6574 7572 6e63 0800 0000  _id..returnc....
-000002b0: 0000 0000 0000 0000 0800 0000 0200 0000  ................
-000002c0: 4300 0000 f308 0000 0074 0064 0183 0182  C........t.d....
-000002d0: 0129 027a 1443 7265 6174 6520 616e 2049  .).z.Create an I
-000002e0: 6e76 6f63 6174 696f 6eda 1163 7265 6174  nvocation..creat
-000002f0: 655f 696e 766f 6361 7469 6f6e a901 da13  e_invocation....
-00000300: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00000310: 726f 7229 08da 0473 656c 6672 0c00 0000  ror)...selfr....
-00000320: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000330: 1000 0000 7211 0000 0072 1200 0000 a900  ....r....r......
-00000340: 7219 0000 00fa fa2f 636f 6465 6275 696c  r....../codebuil
-00000350: 642f 6f75 7470 7574 2f73 7263 3334 3937  d/output/src3497
-00000360: 3236 3836 3730 2f73 7263 2f63 6f64 6573  268670/src/codes
-00000370: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
-00000380: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
-00000390: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
-000003a0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
-000003b0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
-000003c0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
-000003d0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
-000003e0: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
-000003f0: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
-00000400: 732f 726f 626f 746f 5f73 646b 2f73 7263  s/roboto_sdk/src
-00000410: 2f72 6f62 6f74 6f5f 7364 6b2f 646f 6d61  /roboto_sdk/doma
-00000420: 696e 2f61 6374 696f 6e73 2f69 6e76 6f63  in/actions/invoc
-00000430: 6174 696f 6e5f 6465 6c65 6761 7465 2e70  ation_delegate.p
-00000440: 7972 1500 0000 0e00 0000 7302 0000 0008  yr........s.....
-00000450: 0c7a 2449 6e76 6f63 6174 696f 6e44 656c  .z$InvocationDel
-00000460: 6567 6174 652e 6372 6561 7465 5f69 6e76  egate.create_inv
-00000470: 6f63 6174 696f 6eda 0d69 6e76 6f63 6174  ocation..invocat
-00000480: 696f 6e5f 6964 6303 0000 0000 0000 0000  ion_idc.........
-00000490: 0000 0003 0000 0002 0000 0043 0000 0072  ...........C...r
-000004a0: 1400 0000 2902 7a17 4765 7420 616e 2049  ....).z.Get an I
-000004b0: 6e76 6f63 6174 696f 6e20 6279 2049 44da  nvocation by ID.
-000004c0: 0967 6574 5f62 795f 6964 7216 0000 0029  .get_by_idr....)
-000004d0: 0372 1800 0000 721b 0000 0072 1200 0000  .r....r....r....
-000004e0: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-000004f0: 1c00 0000 1c00 0000 7302 0000 0008 057a  ........s......z
-00000500: 1c49 6e76 6f63 6174 696f 6e44 656c 6567  .InvocationDeleg
-00000510: 6174 652e 6765 745f 6279 5f69 64da 0672  ate.get_by_id..r
-00000520: 6563 6f72 64da 0662 7563 6b65 74da 0670  ecord..bucket..p
-00000530: 7265 6669 7863 0400 0000 0000 0000 0000  refixc..........
-00000540: 0000 0400 0000 0200 0000 4300 0000 7214  ..........C...r.
-00000550: 0000 0029 024e da11 7365 745f 6c6f 6773  ...).N..set_logs
-00000560: 5f6c 6f63 6174 696f 6e72 1600 0000 2904  _locationr....).
-00000570: 7218 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000580: 1f00 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00000590: 0000 0072 2000 0000 2300 0000 7302 0000  ...r ...#...s...
-000005a0: 0008 047a 2449 6e76 6f63 6174 696f 6e44  ...z$InvocationD
-000005b0: 656c 6567 6174 652e 7365 745f 6c6f 6773  elegate.set_logs
-000005c0: 5f6c 6f63 6174 696f 6eda 0673 7461 7475  _location..statu
-000005d0: 73da 0664 6574 6169 6c63 0400 0000 0000  s..detailc......
-000005e0: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
-000005f0: 0000 7214 0000 0029 027a 2255 7064 6174  ..r....).z"Updat
-00000600: 6520 7468 6520 7374 6174 7573 206f 6620  e the status of 
-00000610: 616e 2049 6e76 6f63 6174 696f 6eda 1875  an Invocation..u
-00000620: 7064 6174 655f 696e 766f 6361 7469 6f6e  pdate_invocation
-00000630: 5f73 7461 7475 7372 1600 0000 2904 7218  _statusr....).r.
-00000640: 0000 0072 1d00 0000 7221 0000 0072 2200  ...r....r!...r".
-00000650: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000660: 0072 2300 0000 2900 0000 7302 0000 0008  .r#...)...s.....
-00000670: 087a 2b49 6e76 6f63 6174 696f 6e44 656c  .z+InvocationDel
-00000680: 6567 6174 652e 7570 6461 7465 5f69 6e76  egate.update_inv
-00000690: 6f63 6174 696f 6e5f 7374 6174 7573 da07  ocation_status..
-000006a0: 6669 6c74 6572 73da 0a70 6167 655f 746f  filters..page_to
-000006b0: 6b65 6e63 0400 0000 0000 0000 0000 0000  kenc............
-000006c0: 0400 0000 0200 0000 4300 0000 7214 0000  ........C...r...
-000006d0: 0029 024e da0d 7175 6572 795f 6163 7469  .).N..query_acti
-000006e0: 6f6e 7372 1600 0000 2904 7218 0000 0072  onsr....).r....r
-000006f0: 2400 0000 7212 0000 0072 2500 0000 7219  $...r....r%...r.
-00000700: 0000 0072 1900 0000 721a 0000 00da 1171  ...r....r......q
-00000710: 7565 7279 5f69 6e76 6f63 6174 696f 6e73  uery_invocations
-00000720: 3300 0000 7302 0000 0008 077a 2449 6e76  3...s......z$Inv
-00000730: 6f63 6174 696f 6e44 656c 6567 6174 652e  ocationDelegate.
-00000740: 7175 6572 795f 696e 766f 6361 7469 6f6e  query_invocation
-00000750: 7329 024e 4e29 014e 2914 da08 5f5f 6e61  s).NN).N)...__na
-00000760: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000770: da0c 5f5f 7175 616c 6e61 6d65 5f5f da03  ..__qualname__..
-00000780: 6162 63da 0e61 6273 7472 6163 746d 6574  abc..abstractmet
-00000790: 686f 64da 0373 7472 da04 6c69 7374 7207  hod..str..listr.
-000007a0: 0000 0072 0900 0000 7203 0000 0072 0800  ...r....r....r..
-000007b0: 0000 7215 0000 0072 1c00 0000 7220 0000  ..r....r....r ..
-000007c0: 0072 0a00 0000 7223 0000 00da 0464 6963  .r....r#.....dic
-000007d0: 7472 0200 0000 7205 0000 0072 2700 0000  tr....r....r'...
-000007e0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000007f0: 1a00 0000 720b 0000 000d 0000 0073 7e00  ....r........s~.
-00000800: 0000 0800 0401 0208 0201 04f8 0202 02fe  ................
-00000810: 0603 02fd 0204 02fc 0205 02fb 0206 02fa  ................
-00000820: 0607 02f9 0608 02f8 0209 0cf7 040d 0202  ................
-00000830: 04ff 0201 02ff 0601 02ff 0202 0cfe 0406  ................
-00000840: 0201 0201 02ff 0201 02ff 0201 02ff 0202  ................
-00000850: 0cfe 0405 0205 04fc 0202 02fe 0203 02fd  ................
-00000860: 0604 02fc 0205 0cfb 0409 0204 0201 04fc  ................
-00000870: 0a02 02fe 0603 02fd 0e04 02fc 0605 10fb  ................
-00000880: 720b 0000 0029 0d72 2b00 0000 da06 7479  r....).r+.....ty
-00000890: 7069 6e67 7202 0000 0072 0300 0000 da0a  pingr....r......
-000008a0: 7061 6769 6e61 7469 6f6e 7205 0000 00da  paginationr.....
-000008b0: 1169 6e76 6f63 6174 696f 6e5f 7265 636f  .invocation_reco
-000008c0: 7264 7207 0000 0072 0800 0000 7209 0000  rdr....r....r...
-000008d0: 0072 0a00 0000 da03 4142 4372 0b00 0000  .r......ABCr....
-000008e0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000008f0: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000900: 0000 730a 0000 0008 0010 010c 0218 0116  ..s.............
-00000910: 08                                       .
+00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
+00000070: 6408 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
+00000080: 6d0f 5a0f 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
+00000090: 6500 6a10 8303 5a11 6401 5300 290b e900  e.j...Z.d.S.)...
+000000a0: 0000 004e 2902 da03 416e 79da 084f 7074  ...N)...Any..Opt
+000000b0: 696f 6e61 6ce9 0300 0000 2901 da0d 5061  ional.....)...Pa
+000000c0: 6769 6e61 7465 644c 6973 74e9 0100 0000  ginatedList.....
+000000d0: 2902 da13 436f 6d70 7574 6552 6571 7569  )...ComputeRequi
+000000e0: 7265 6d65 6e74 73da 1343 6f6e 7461 696e  rements..Contain
+000000f0: 6572 5061 7261 6d65 7465 7273 2901 da0c  erParameters)...
+00000100: 4163 7469 6f6e 5265 636f 7264 2904 da18  ActionRecord)...
+00000110: 496e 766f 6361 7469 6f6e 4461 7461 536f  InvocationDataSo
+00000120: 7572 6365 5479 7065 da10 496e 766f 6361  urceType..Invoca
+00000130: 7469 6f6e 5265 636f 7264 da10 496e 766f  tionRecord..Invo
+00000140: 6361 7469 6f6e 536f 7572 6365 da10 496e  cationSource..In
+00000150: 766f 6361 7469 6f6e 5374 6174 7573 6300  vocationStatusc.
+00000160: 0000 0000 0000 0000 0000 0000 0000 0014  ................
+00000170: 0000 0040 0000 0073 fa00 0000 6500 5a01  ...@...s....e.Z.
+00000180: 6400 5a02 6503 6a04 0901 641e 6402 6505  d.Z.e.j...d.d.e.
+00000190: 6403 6506 6507 1900 6404 6508 6405 6509  d.e.e...d.e.d.e.
+000001a0: 6406 6507 6407 650a 6408 650b 6409 650c  d.e.d.e.d.e.d.e.
+000001b0: 6507 1900 640a 650d 6612 640b 640c 8405  e...d.e.f.d.d...
+000001c0: 8301 5a0e 6503 6a04 0901 641e 640d 6507  ..Z.e.j...d.d.e.
+000001d0: 640e 650c 6507 1900 640a 650d 6606 640f  d.e.e...d.e.f.d.
+000001e0: 6410 8405 8301 5a0f 6503 6a04 6411 650d  d.....Z.e.j.d.e.
+000001f0: 6412 6507 6413 6507 640a 650d 6608 6414  d.e.d.e.d.e.f.d.
+00000200: 6415 8404 8301 5a10 6503 6a04 0901 641e  d.....Z.e.j...d.
+00000210: 6411 650d 6416 6511 6417 650c 6507 1900  d.e.d.e.d.e.e...
+00000220: 640a 650d 6608 6418 6419 8405 8301 5a12  d.e.f.d.d.....Z.
+00000230: 6503 6a04 0901 0901 641f 641a 6513 6507  e.j.....d.d.e.e.
+00000240: 6514 6602 1900 640e 650c 6507 1900 641b  e.f...d.e.e...d.
+00000250: 650c 6513 6507 6507 6602 1900 1900 640a  e.e.e.e.f.....d.
+00000260: 6515 650d 1900 6608 641c 641d 8405 8301  e.e...f.d.d.....
+00000270: 5a16 6401 5300 2920 da12 496e 766f 6361  Z.d.S.) ..Invoca
+00000280: 7469 6f6e 4465 6c65 6761 7465 4eda 0d61  tionDelegateN..a
+00000290: 6374 696f 6e5f 7265 636f 7264 da0a 696e  ction_record..in
+000002a0: 7075 745f 6461 7461 da14 636f 6d70 7574  put_data..comput
+000002b0: 655f 7265 7175 6972 656d 656e 7473 da14  e_requirements..
+000002c0: 636f 6e74 6169 6e65 725f 7061 7261 6d65  container_parame
+000002d0: 7465 7273 da0e 6461 7461 5f73 6f75 7263  ters..data_sourc
+000002e0: 655f 6964 da10 6461 7461 5f73 6f75 7263  e_id..data_sourc
+000002f0: 655f 7479 7065 da11 696e 766f 6361 7469  e_type..invocati
+00000300: 6f6e 5f73 6f75 7263 65da 1469 6e76 6f63  on_source..invoc
+00000310: 6174 696f 6e5f 736f 7572 6365 5f69 64da  ation_source_id.
+00000320: 0672 6574 7572 6e63 0900 0000 0000 0000  .returnc........
+00000330: 0000 0000 0900 0000 0200 0000 4300 0000  ............C...
+00000340: f308 0000 0074 0064 0183 0182 0129 027a  .....t.d.....).z
+00000350: 1443 7265 6174 6520 616e 2049 6e76 6f63  .Create an Invoc
+00000360: 6174 696f 6eda 1163 7265 6174 655f 696e  ation..create_in
+00000370: 766f 6361 7469 6f6e a901 da13 4e6f 7449  vocation....NotI
+00000380: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
+00000390: 09da 0473 656c 6672 0f00 0000 7210 0000  ...selfr....r...
+000003a0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000003b0: 7214 0000 0072 1500 0000 7216 0000 00a9  r....r....r.....
+000003c0: 0072 1d00 0000 fafa 2f63 6f64 6562 7569  .r....../codebui
+000003d0: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+000003e0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+000003f0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
+00000400: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
+00000410: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
+00000420: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
+00000430: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
+00000440: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
+00000450: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
+00000460: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
+00000470: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
+00000480: 6573 2f72 6f62 6f74 6f5f 7364 6b2f 7372  es/roboto_sdk/sr
+00000490: 632f 726f 626f 746f 5f73 646b 2f64 6f6d  c/roboto_sdk/dom
+000004a0: 6169 6e2f 6163 7469 6f6e 732f 696e 766f  ain/actions/invo
+000004b0: 6361 7469 6f6e 5f64 656c 6567 6174 652e  cation_delegate.
+000004c0: 7079 7219 0000 0013 0000 0073 0200 0000  pyr........s....
+000004d0: 080d 7a24 496e 766f 6361 7469 6f6e 4465  ..z$InvocationDe
+000004e0: 6c65 6761 7465 2e63 7265 6174 655f 696e  legate.create_in
+000004f0: 766f 6361 7469 6f6e da0d 696e 766f 6361  vocation..invoca
+00000500: 7469 6f6e 5f69 64da 066f 7267 5f69 6463  tion_id..org_idc
+00000510: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000520: 0200 0000 4300 0000 7218 0000 0029 027a  ....C...r....).z
+00000530: 1747 6574 2061 6e20 496e 766f 6361 7469  .Get an Invocati
+00000540: 6f6e 2062 7920 4944 da09 6765 745f 6279  on by ID..get_by
+00000550: 5f69 6472 1a00 0000 2903 721c 0000 0072  _idr....).r....r
+00000560: 1f00 0000 7220 0000 0072 1d00 0000 721d  ....r ...r....r.
+00000570: 0000 0072 1e00 0000 7221 0000 0022 0000  ...r....r!..."..
+00000580: 0073 0200 0000 0805 7a1c 496e 766f 6361  .s......z.Invoca
+00000590: 7469 6f6e 4465 6c65 6761 7465 2e67 6574  tionDelegate.get
+000005a0: 5f62 795f 6964 da06 7265 636f 7264 da06  _by_id..record..
+000005b0: 6275 636b 6574 da06 7072 6566 6978 6304  bucket..prefixc.
+000005c0: 0000 0000 0000 0000 0000 0004 0000 0002  ................
+000005d0: 0000 0043 0000 0072 1800 0000 2902 4eda  ...C...r....).N.
+000005e0: 1173 6574 5f6c 6f67 735f 6c6f 6361 7469  .set_logs_locati
+000005f0: 6f6e 721a 0000 0029 0472 1c00 0000 7222  onr....).r....r"
+00000600: 0000 0072 2300 0000 7224 0000 0072 1d00  ...r#...r$...r..
+00000610: 0000 721d 0000 0072 1e00 0000 7225 0000  ..r....r....r%..
+00000620: 0029 0000 0073 0200 0000 0804 7a24 496e  .)...s......z$In
+00000630: 766f 6361 7469 6f6e 4465 6c65 6761 7465  vocationDelegate
+00000640: 2e73 6574 5f6c 6f67 735f 6c6f 6361 7469  .set_logs_locati
+00000650: 6f6e da06 7374 6174 7573 da06 6465 7461  on..status..deta
+00000660: 696c 6304 0000 0000 0000 0000 0000 0004  ilc.............
+00000670: 0000 0002 0000 0043 0000 0072 1800 0000  .......C...r....
+00000680: 2902 7a22 5570 6461 7465 2074 6865 2073  ).z"Update the s
+00000690: 7461 7475 7320 6f66 2061 6e20 496e 766f  tatus of an Invo
+000006a0: 6361 7469 6f6e da18 7570 6461 7465 5f69  cation..update_i
+000006b0: 6e76 6f63 6174 696f 6e5f 7374 6174 7573  nvocation_status
+000006c0: 721a 0000 0029 0472 1c00 0000 7222 0000  r....).r....r"..
+000006d0: 0072 2600 0000 7227 0000 0072 1d00 0000  .r&...r'...r....
+000006e0: 721d 0000 0072 1e00 0000 7228 0000 002f  r....r....r(.../
+000006f0: 0000 0073 0200 0000 0808 7a2b 496e 766f  ...s......z+Invo
+00000700: 6361 7469 6f6e 4465 6c65 6761 7465 2e75  cationDelegate.u
+00000710: 7064 6174 655f 696e 766f 6361 7469 6f6e  pdate_invocation
+00000720: 5f73 7461 7475 73da 0766 696c 7465 7273  _status..filters
+00000730: da0a 7061 6765 5f74 6f6b 656e 6304 0000  ..page_tokenc...
+00000740: 0000 0000 0000 0000 0004 0000 0002 0000  ................
+00000750: 0043 0000 0072 1800 0000 2902 4eda 1171  .C...r....).N..q
+00000760: 7565 7279 5f69 6e76 6f63 6174 696f 6e73  uery_invocations
+00000770: 721a 0000 0029 0472 1c00 0000 7229 0000  r....).r....r)..
+00000780: 0072 2000 0000 722a 0000 0072 1d00 0000  .r ...r*...r....
+00000790: 721d 0000 0072 1e00 0000 722b 0000 0039  r....r....r+...9
+000007a0: 0000 0073 0200 0000 0807 7a24 496e 766f  ...s......z$Invo
+000007b0: 6361 7469 6f6e 4465 6c65 6761 7465 2e71  cationDelegate.q
+000007c0: 7565 7279 5f69 6e76 6f63 6174 696f 6e73  uery_invocations
+000007d0: 2901 4e29 024e 4e29 17da 085f 5f6e 616d  ).N).NN)...__nam
+000007e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000007f0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0361  .__qualname__..a
+00000800: 6263 da0e 6162 7374 7261 6374 6d65 7468  bc..abstractmeth
+00000810: 6f64 7209 0000 00da 046c 6973 74da 0373  odr......list..s
+00000820: 7472 7207 0000 0072 0800 0000 720a 0000  trr....r....r...
+00000830: 0072 0c00 0000 7203 0000 0072 0b00 0000  .r....r....r....
+00000840: 7219 0000 0072 2100 0000 7225 0000 0072  r....r!...r%...r
+00000850: 0d00 0000 7228 0000 00da 0464 6963 7472  ....r(.....dictr
+00000860: 0200 0000 7205 0000 0072 2b00 0000 721d  ....r....r+...r.
+00000870: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000880: 0000 720e 0000 0012 0000 0073 8000 0000  ..r........s....
+00000890: 0800 0401 020a 04f7 0202 02fe 0603 02fd  ................
+000008a0: 0204 02fc 0205 02fb 0206 02fa 0207 02f9  ................
+000008b0: 0208 02f8 0609 02f7 020a 0cf6 040e 0202  ................
+000008c0: 04ff 0201 02ff 0601 02ff 0202 0cfe 0406  ................
+000008d0: 0201 0201 02ff 0201 02ff 0201 02ff 0202  ................
+000008e0: 0cfe 0405 0205 04fc 0202 02fe 0203 02fd  ................
+000008f0: 0604 02fc 0205 0cfb 0409 0204 0201 04fc  ................
+00000900: 0a02 02fe 0603 02fd 0e04 02fc 0605 10fb  ................
+00000910: 720e 0000 0029 1272 2f00 0000 da06 7479  r....).r/.....ty
+00000920: 7069 6e67 7202 0000 0072 0300 0000 da0a  pingr....r......
+00000930: 7061 6769 6e61 7469 6f6e 7205 0000 00da  paginationr.....
+00000940: 1a61 6374 696f 6e5f 636f 6e74 6169 6e65  .action_containe
+00000950: 725f 7265 736f 7572 6365 7372 0700 0000  r_resourcesr....
+00000960: 7208 0000 0072 0f00 0000 7209 0000 00da  r....r....r.....
+00000970: 1169 6e76 6f63 6174 696f 6e5f 7265 636f  .invocation_reco
+00000980: 7264 720a 0000 0072 0b00 0000 720c 0000  rdr....r....r...
+00000990: 0072 0d00 0000 da03 4142 4372 0e00 0000  .r......ABCr....
+000009a0: 721d 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+000009b0: 1e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000009c0: 0000 730e 0000 0008 0010 010c 0210 010c  ..s.............
+000009d0: 0418 0116 08                             .....
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 4768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,293 +1,308 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 a012 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 f413 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6403 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6403 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6407 6c0c 6d0d 5a0d 0100 6408  ..d.d.l.m.Z...d.
-00000080: 6409 6c0e 6d0f 5a0f 0100 6408 640a 6c10  d.l.m.Z...d.d.l.
-00000090: 6d11 5a11 6d12 5a12 0100 6408 640b 6c13  m.Z.m.Z...d.d.l.
-000000a0: 6d14 5a14 6d15 5a15 6d16 5a16 6d17 5a17  m.Z.m.Z.m.Z.m.Z.
-000000b0: 0100 6509 8300 5a18 4700 640c 640d 8400  ..e...Z.G.d.d...
-000000c0: 640d 650f 8303 5a19 6401 5300 290e e900  d.e...Z.d.S.)...
-000000d0: 0000 004e 2902 da03 416e 79da 084f 7074  ...N)...Any..Opt
-000000e0: 696f 6e61 6ce9 0300 0000 2903 da13 4f52  ional.....)...OR
-000000f0: 475f 4f56 4552 5249 4445 5f48 4541 4445  G_OVERRIDE_HEADE
-00000100: 52da 1455 5345 525f 4f56 4552 5249 4445  R..USER_OVERRIDE
-00000110: 5f48 4541 4445 52da 0a48 7474 7043 6c69  _HEADER..HttpCli
-00000120: 656e 7429 01da 0e64 6566 6175 6c74 5f6c  ent)...default_l
-00000130: 6f67 6765 7229 01da 0d50 6167 696e 6174  ogger)...Paginat
-00000140: 6564 4c69 7374 2901 da16 7079 6461 6e74  edList)...pydant
-00000150: 6963 5f6a 736f 6e61 626c 655f 6469 6374  ic_jsonable_dict
-00000160: e901 0000 0029 01da 1249 6e76 6f63 6174  .....)...Invocat
-00000170: 696f 6e44 656c 6567 6174 6529 02da 1743  ionDelegate)...C
-00000180: 7265 6174 6549 6e76 6f63 6174 696f 6e52  reateInvocationR
-00000190: 6571 7565 7374 da16 5365 744c 6f67 734c  equest..SetLogsL
-000001a0: 6f63 6174 696f 6e52 6571 7565 7374 2904  ocationRequest).
-000001b0: da18 496e 766f 6361 7469 6f6e 4461 7461  ..InvocationData
-000001c0: 536f 7572 6365 5479 7065 da10 496e 766f  SourceType..Invo
-000001d0: 6361 7469 6f6e 5265 636f 7264 da10 496e  cationRecord..In
-000001e0: 766f 6361 7469 6f6e 536f 7572 6365 da10  vocationSource..
-000001f0: 496e 766f 6361 7469 6f6e 5374 6174 7573  InvocationStatus
-00000200: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000210: 0011 0000 0000 0000 0073 3c01 0000 6500  .........s<...e.
-00000220: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
-00000230: 6402 3c00 6506 6505 6403 3c00 6404 6506  d.<.e.e.d.<.d.e.
-00000240: 6405 6504 6406 6407 6606 8700 6601 6408  d.e.d.d.f...f.d.
-00000250: 6409 840c 5a07 0907 6426 640a 6508 6506  d...Z...d&d.e.e.
-00000260: 1900 640b 6508 6506 1900 6406 6509 6506  ..d.e.e...d.e.e.
-00000270: 6506 6602 1900 6606 640c 640d 8405 5a0a  e.f...f.d.d...Z.
-00000280: 0907 0907 6426 640e 6506 640f 650b 6506  ....d&d.e.d.e.e.
-00000290: 1900 6410 6506 6411 650c 6412 650d 6413  ..d.e.d.e.d.e.d.
-000002a0: 6508 6506 1900 640a 6508 6506 1900 6406  e.e...d.e.e...d.
-000002b0: 650e 6610 6414 6415 8405 5a0f 0907 6427  e.f.d.d...Z...d'
-000002c0: 6416 6506 640a 6508 6506 1900 6406 650e  d.e.d.e.e...d.e.
-000002d0: 6606 6417 6418 8405 5a10 6419 650e 641a  f.d.d...Z.d.e.d.
-000002e0: 6506 641b 6506 6406 650e 6608 641c 641d  e.d.e.d.e.f.d.d.
-000002f0: 8404 5a11 0907 6427 6419 650e 641e 6512  ..Z...d'd.e.d.e.
-00000300: 641f 6508 6506 1900 6406 650e 6608 6420  d.e.e...d.e.f.d 
-00000310: 6421 8405 5a13 0907 0907 6426 6422 6509  d!..Z.....d&d"e.
-00000320: 6506 6514 6602 1900 640a 6508 6506 1900  e.e.f...d.e.e...
-00000330: 6423 6508 6509 6506 6506 6602 1900 1900  d#e.e.e.e.f.....
-00000340: 6406 6515 650e 1900 6608 6424 6425 8405  d.e.e...f.d$d%..
-00000350: 5a16 8700 0400 5a17 5300 2928 da16 496e  Z.....Z.S.)(..In
-00000360: 766f 6361 7469 6f6e 4874 7470 4465 6c65  vocationHttpDele
-00000370: 6761 7465 7a47 0a20 2020 2055 7365 2069  gatezG.    Use i
-00000380: 6e20 616e 7920 636f 6e74 6578 7420 7468  n any context th
-00000390: 6174 2064 6f65 7320 6e6f 7420 6861 7665  at does not have
-000003a0: 2064 6972 6563 7420 6461 7461 6261 7365   direct database
-000003b0: 2061 6363 6573 732e 0a20 2020 20da 245f   access..    .$_
-000003c0: 496e 766f 6361 7469 6f6e 4874 7470 4465  InvocationHttpDe
-000003d0: 6c65 6761 7465 5f5f 6874 7470 5f63 6c69  legate__http_cli
-000003e0: 656e 74da 305f 496e 766f 6361 7469 6f6e  ent.0_Invocation
-000003f0: 4874 7470 4465 6c65 6761 7465 5f5f 726f  HttpDelegate__ro
-00000400: 626f 746f 5f73 6572 7669 6365 5f62 6173  boto_service_bas
-00000410: 655f 7572 6cda 1772 6f62 6f74 6f5f 7365  e_url..roboto_se
-00000420: 7276 6963 655f 6261 7365 5f75 726c da0b  rvice_base_url..
-00000430: 6874 7470 5f63 6c69 656e 74da 0672 6574  http_client..ret
-00000440: 7572 6e4e 6303 0000 0000 0000 0000 0000  urnNc...........
-00000450: 0003 0000 0002 0000 0003 0000 0073 1a00  .............s..
-00000460: 0000 7400 8300 a001 a100 0100 7c02 7c00  ..t.........|.|.
-00000470: 5f02 7c01 7c00 5f03 6400 5300 a901 4e29  _.|.|._.d.S...N)
-00000480: 04da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
-00000490: 5f5f 7214 0000 0072 1500 0000 2903 da04  __r....r....)...
-000004a0: 7365 6c66 7216 0000 0072 1700 0000 a901  selfr....r......
-000004b0: da09 5f5f 636c 6173 735f 5fa9 00fa ff2f  ..__class__..../
-000004c0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-000004d0: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
-000004e0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
-000004f0: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
-00000500: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
-00000510: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
-00000520: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
-00000530: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
-00000540: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
-00000550: 3639 3964 2f72 6f62 6f74 6f2d 6169 2f72  699d/roboto-ai/r
-00000560: 6f62 6f74 6f2d 686f 7374 6564 2d61 7070  oboto-hosted-app
-00000570: 2f70 6163 6b61 6765 732f 726f 626f 746f  /packages/roboto
-00000580: 5f73 646b 2f73 7263 2f72 6f62 6f74 6f5f  _sdk/src/roboto_
-00000590: 7364 6b2f 646f 6d61 696e 2f61 6374 696f  sdk/domain/actio
-000005a0: 6e73 2f69 6e76 6f63 6174 696f 6e5f 6874  ns/invocation_ht
-000005b0: 7470 5f64 656c 6567 6174 652e 7079 721b  tp_delegate.pyr.
-000005c0: 0000 0025 0000 0073 0600 0000 0a01 0601  ...%...s........
-000005d0: 0a01 7a1f 496e 766f 6361 7469 6f6e 4874  ..z.InvocationHt
-000005e0: 7470 4465 6c65 6761 7465 2e5f 5f69 6e69  tpDelegate.__ini
-000005f0: 745f 5fda 066f 7267 5f69 64da 0775 7365  t__..org_id..use
-00000600: 725f 6964 6303 0000 0000 0000 0000 0000  r_idc...........
-00000610: 0004 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
-00000620: 0000 6401 6402 6901 7d03 7c01 720a 7c01  ..d.d.i.}.|.r.|.
-00000630: 7c03 7400 3c00 7c02 7210 7c02 7c03 7401  |.t.<.|.r.|.|.t.
-00000640: 3c00 7c03 5300 2903 4e7a 0c43 6f6e 7465  <.|.S.).Nz.Conte
-00000650: 6e74 2d54 7970 657a 1061 7070 6c69 6361  nt-Typez.applica
-00000660: 7469 6f6e 2f6a 736f 6e29 0272 0500 0000  tion/json).r....
-00000670: 7206 0000 0029 0472 1c00 0000 7221 0000  r....).r....r!..
-00000680: 0072 2200 0000 da07 6865 6164 6572 7372  .r".....headersr
-00000690: 1f00 0000 721f 0000 0072 2000 0000 7223  ....r....r ...r#
-000006a0: 0000 002a 0000 0073 0c00 0000 0803 0401  ...*...s........
-000006b0: 0801 0401 0801 0401 7a1e 496e 766f 6361  ........z.Invoca
-000006c0: 7469 6f6e 4874 7470 4465 6c65 6761 7465  tionHttpDelegate
-000006d0: 2e68 6561 6465 7273 da0b 6163 7469 6f6e  .headers..action
-000006e0: 5f6e 616d 65da 0a69 6e70 7574 5f64 6174  _name..input_dat
-000006f0: 61da 0e64 6174 615f 736f 7572 6365 5f69  a..data_source_i
-00000700: 64da 1064 6174 615f 736f 7572 6365 5f74  d..data_source_t
-00000710: 7970 65da 1169 6e76 6f63 6174 696f 6e5f  ype..invocation_
-00000720: 736f 7572 6365 da14 696e 766f 6361 7469  source..invocati
-00000730: 6f6e 5f73 6f75 7263 655f 6964 6308 0000  on_source_idc...
-00000740: 0000 0000 0000 0000 000b 0000 0007 0000  ................
-00000750: 0043 0000 0073 6a00 0000 7c00 6a00 9b00  .C...sj...|.j...
-00000760: 6401 7c01 9b00 6402 9d04 7d08 7401 7c02  d.|...d...}.t.|.
-00000770: 7c03 7c04 7c05 7c06 6403 8d05 7d09 7c00  |.|.|.|.d...}.|.
-00000780: 6a02 6a03 7c08 7404 7c09 6404 6405 8d02  j.j.|.t.|.d.d...
-00000790: 7c00 6a05 7c07 7c05 7406 6a07 6b02 7225  |.j.|.|.t.j.k.r%
-000007a0: 7c06 6e01 6400 6406 8d02 6407 8d03 7d0a  |.n.d.d...d...}.
-000007b0: 7408 a009 7c0a 6a0a 6408 6701 6409 8d01  t...|.j.d.g.d...
-000007c0: a101 5300 290a 4e7a 0c2f 7631 2f61 6374  ..S.).Nz./v1/act
-000007d0: 696f 6e73 2f7a 072f 696e 766f 6b65 2905  ions/z./invoke).
-000007e0: 7225 0000 0072 2600 0000 7227 0000 0072  r%...r&...r'...r
-000007f0: 2800 0000 7229 0000 0054 a901 da0c 6578  (...r)...T....ex
-00000800: 636c 7564 655f 6e6f 6e65 2902 7221 0000  clude_none).r!..
-00000810: 0072 2200 0000 a902 da04 6461 7461 7223  .r".......datar#
-00000820: 0000 0072 2d00 0000 a901 da09 6a73 6f6e  ...r-.......json
-00000830: 5f70 6174 6829 0b72 1500 0000 720d 0000  _path).r....r...
-00000840: 0072 1400 0000 da04 706f 7374 720a 0000  .r......postr...
-00000850: 0072 2300 0000 7211 0000 00da 064d 616e  .r#...r......Man
-00000860: 7561 6c72 1000 0000 da09 7061 7273 655f  ualr......parse_
-00000870: 6f62 6ada 0966 726f 6d5f 6a73 6f6e 290b  obj..from_json).
-00000880: 721c 0000 0072 2400 0000 7225 0000 0072  r....r$...r%...r
-00000890: 2600 0000 7227 0000 0072 2800 0000 7229  &...r'...r(...r)
-000008a0: 0000 0072 2100 0000 da03 7572 6cda 0c72  ...r!.....url..r
-000008b0: 6571 7565 7374 5f62 6f64 79da 0872 6573  equest_body..res
-000008c0: 706f 6e73 6572 1f00 0000 721f 0000 0072  ponser....r....r
-000008d0: 2000 0000 da11 6372 6561 7465 5f69 6e76   .....create_inv
-000008e0: 6f63 6174 696f 6e34 0000 0073 2600 0000  ocation4...s&...
-000008f0: 120a 0201 0201 0201 0201 0201 0201 06fb  ................
-00000900: 0607 0201 0a01 0401 0201 0a02 04ff 0202  ................
-00000910: 04fc 06fd 140a 7a28 496e 766f 6361 7469  ......z(Invocati
-00000920: 6f6e 4874 7470 4465 6c65 6761 7465 2e63  onHttpDelegate.c
-00000930: 7265 6174 655f 696e 766f 6361 7469 6f6e  reate_invocation
-00000940: da0d 696e 766f 6361 7469 6f6e 5f69 6463  ..invocation_idc
-00000950: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-00000960: 0500 0000 4300 0000 733a 0000 007c 006a  ....C...s:...|.j
-00000970: 009b 0064 017c 019b 009d 037d 037c 006a  ...d.|.....}.|.j
-00000980: 016a 027c 037c 00a0 037c 02a1 0164 028d  .j.|.|...|...d..
-00000990: 027d 0474 04a0 057c 046a 0664 0367 0164  .}.t...|.j.d.g.d
-000009a0: 048d 01a1 0153 0029 054e fa18 2f76 312f  .....S.).N../v1/
-000009b0: 6163 7469 6f6e 732f 696e 766f 6361 7469  actions/invocati
-000009c0: 6f6e 732f 2901 7223 0000 0072 2d00 0000  ons/).r#...r-...
-000009d0: 722e 0000 0029 0772 1500 0000 7214 0000  r....).r....r...
-000009e0: 00da 0367 6574 7223 0000 0072 1000 0000  ...getr#...r....
-000009f0: 7232 0000 0072 3300 0000 2905 721c 0000  r2...r3...).r...
-00000a00: 0072 3800 0000 7221 0000 0072 3400 0000  .r8...r!...r4...
-00000a10: 7236 0000 0072 1f00 0000 721f 0000 0072  r6...r....r....r
-00000a20: 2000 0000 da09 6765 745f 6279 5f69 6452   .....get_by_idR
-00000a30: 0000 0073 0600 0000 1003 1601 1401 7a20  ...s..........z 
-00000a40: 496e 766f 6361 7469 6f6e 4874 7470 4465  InvocationHttpDe
-00000a50: 6c65 6761 7465 2e67 6574 5f62 795f 6964  legate.get_by_id
-00000a60: da06 7265 636f 7264 da06 6275 636b 6574  ..record..bucket
-00000a70: da06 7072 6566 6978 6304 0000 0000 0000  ..prefixc.......
-00000a80: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
-00000a90: 0073 5600 0000 7c00 6a00 9b00 6401 7c01  .sV...|.j...d.|.
-00000aa0: 6a01 9b00 6402 9d04 7d04 7402 7c02 7c03  j...d...}.t.|.|.
-00000ab0: 6403 8d02 7d05 7c00 6a03 6a04 7c04 7405  d...}.|.j.j.|.t.
-00000ac0: 7c05 6404 6405 8d02 7c00 a006 7c01 6a07  |.d.d...|...|.j.
-00000ad0: a101 6406 8d03 7d06 7408 a009 7c06 6a0a  ..d...}.t...|.j.
-00000ae0: 6407 6701 6408 8d01 a101 5300 2909 4e72  d.g.d.....S.).Nr
-00000af0: 3900 0000 7a05 2f6c 6f67 7329 0272 3d00  9...z./logs).r=.
-00000b00: 0000 723e 0000 0054 722a 0000 0072 2c00  ..r>...Tr*...r,.
-00000b10: 0000 722d 0000 0072 2e00 0000 290b 7215  ..r-...r....).r.
-00000b20: 0000 0072 3800 0000 720e 0000 0072 1400  ...r8...r....r..
-00000b30: 0000 da05 7061 7463 6872 0a00 0000 7223  ....patchr....r#
-00000b40: 0000 0072 2100 0000 7210 0000 0072 3200  ...r!...r....r2.
-00000b50: 0000 7233 0000 0029 0772 1c00 0000 723c  ..r3...).r....r<
-00000b60: 0000 0072 3d00 0000 723e 0000 0072 3400  ...r=...r>...r4.
-00000b70: 0000 7235 0000 0072 3600 0000 721f 0000  ..r5...r6...r...
-00000b80: 0072 1f00 0000 7220 0000 00da 1173 6574  .r....r .....set
-00000b90: 5f6c 6f67 735f 6c6f 6361 7469 6f6e 5900  _logs_locationY.
-00000ba0: 0000 7310 0000 0014 030c 0106 0102 010a  ..s.............
-00000bb0: 010a 0106 fd14 057a 2849 6e76 6f63 6174  .......z(Invocat
-00000bc0: 696f 6e48 7474 7044 656c 6567 6174 652e  ionHttpDelegate.
-00000bd0: 7365 745f 6c6f 6773 5f6c 6f63 6174 696f  set_logs_locatio
-00000be0: 6eda 0673 7461 7475 73da 0664 6574 6169  n..status..detai
-00000bf0: 6c63 0400 0000 0000 0000 0000 0000 0600  lc..............
-00000c00: 0000 0600 0000 4300 0000 734a 0000 007c  ......C...sJ...|
-00000c10: 006a 009b 0064 017c 016a 019b 0064 029d  .j...d.|.j...d..
-00000c20: 047d 047c 006a 026a 037c 047c 026a 047c  .}.|.j.j.|.|.j.|
-00000c30: 0364 039c 027c 00a0 057c 016a 06a1 0164  .d...|...|.j...d
-00000c40: 048d 037d 0574 07a0 087c 056a 0964 0567  ...}.t...|.j.d.g
-00000c50: 0164 068d 01a1 0153 0029 074e 7239 0000  .d.....S.).Nr9..
-00000c60: 007a 072f 7374 6174 7573 2902 7241 0000  .z./status).rA..
-00000c70: 0072 4200 0000 722c 0000 0072 2d00 0000  .rB...r,...r-...
-00000c80: 722e 0000 0029 0a72 1500 0000 7238 0000  r....).r....r8..
-00000c90: 0072 1400 0000 7230 0000 00da 0576 616c  .r....r0.....val
-00000ca0: 7565 7223 0000 0072 2100 0000 7210 0000  uer#...r!...r...
-00000cb0: 0072 3200 0000 7233 0000 0029 0672 1c00  .r2...r3...).r..
-00000cc0: 0000 723c 0000 0072 4100 0000 7242 0000  ..r<...rA...rB..
-00000cd0: 0072 3400 0000 7236 0000 0072 1f00 0000  .r4...r6...r....
-00000ce0: 721f 0000 0072 2000 0000 da18 7570 6461  r....r .....upda
-00000cf0: 7465 5f69 6e76 6f63 6174 696f 6e5f 7374  te_invocation_st
-00000d00: 6174 7573 6500 0000 730e 0000 0014 0606  atuse...s.......
-00000d10: 0102 010a 010a 0106 fd14 057a 2f49 6e76  ...........z/Inv
-00000d20: 6f63 6174 696f 6e48 7474 7044 656c 6567  ocationHttpDeleg
-00000d30: 6174 652e 7570 6461 7465 5f69 6e76 6f63  ate.update_invoc
-00000d40: 6174 696f 6e5f 7374 6174 7573 da07 6669  ation_status..fi
-00000d50: 6c74 6572 73da 0a70 6167 655f 746f 6b65  lters..page_toke
-00000d60: 6e63 0400 0000 0000 0000 0000 0000 0800  nc..............
-00000d70: 0000 0600 0000 4300 0000 736c 0000 007c  ......C...sl...|
-00000d80: 0372 067c 037c 0164 013c 0074 00a0 0174  .r.|.|.d.<.t...t
-00000d90: 00a0 027c 01a1 01a1 017d 047c 006a 039b  ...|.....}.|.j..
-00000da0: 0064 029d 027d 057c 006a 046a 057c 057c  .d...}.|.j.j.|.|
-00000db0: 047c 00a0 067c 02a1 0164 038d 037d 067c  .|...|...d...}.|
-00000dc0: 066a 0764 0467 0164 058d 017d 0774 0864  .j.d.g.d...}.t.d
-00000dd0: 0664 0784 007c 0764 0819 0044 0083 017c  .d...|.d...D...|
-00000de0: 0764 0919 0064 0a8d 0253 0029 0b4e 7246  .d...d...S.).NrF
-00000df0: 0000 007a 1d2f 7631 2f61 6374 696f 6e73  ...z./v1/actions
-00000e00: 2f69 6e76 6f63 6174 696f 6e73 2f71 7565  /invocations/que
-00000e10: 7279 722c 0000 0072 2d00 0000 722e 0000  ryr,...r-...r...
-00000e20: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000e30: 0000 0500 0000 5300 0000 7316 0000 0067  ......S...s....g
-00000e40: 007c 005d 077d 0174 00a0 017c 01a1 0191  .|.].}.t...|....
-00000e50: 0271 0253 0072 1f00 0000 2902 7210 0000  .q.S.r....).r...
-00000e60: 0072 3200 0000 2902 da02 2e30 da07 6461  .r2...)....0..da
-00000e70: 7461 7365 7472 1f00 0000 721f 0000 0072  tasetr....r....r
-00000e80: 2000 0000 da0a 3c6c 6973 7463 6f6d 703e   .....<listcomp>
-00000e90: 8300 0000 7306 0000 0006 000a 0106 ff7a  ....s..........z
-00000ea0: 3c49 6e76 6f63 6174 696f 6e48 7474 7044  <InvocationHttpD
-00000eb0: 656c 6567 6174 652e 7175 6572 795f 696e  elegate.query_in
-00000ec0: 766f 6361 7469 6f6e 732e 3c6c 6f63 616c  vocations.<local
-00000ed0: 733e 2e3c 6c69 7374 636f 6d70 3eda 0569  s>.<listcomp>..i
-00000ee0: 7465 6d73 da0a 6e65 7874 5f74 6f6b 656e  tems..next_token
-00000ef0: 2902 724a 0000 0072 4b00 0000 2909 da04  ).rJ...rK...)...
-00000f00: 6a73 6f6e da05 6c6f 6164 73da 0564 756d  json..loads..dum
-00000f10: 7073 7215 0000 0072 1400 0000 7230 0000  psr....r....r0..
-00000f20: 0072 2300 0000 7233 0000 0072 0900 0000  .r#...r3...r....
-00000f30: 2908 721c 0000 0072 4500 0000 7221 0000  ).r....rE...r!..
-00000f40: 0072 4600 0000 da0c 7361 6665 5f66 696c  .rF.....safe_fil
-00000f50: 7465 7273 7234 0000 00da 0372 6573 da0c  tersr4.....res..
-00000f60: 756e 6d61 7273 6861 6c6c 6564 721f 0000  unmarshalledr...
-00000f70: 0072 1f00 0000 7220 0000 00da 1171 7565  .r....r .....que
-00000f80: 7279 5f69 6e76 6f63 6174 696f 6e73 7300  ry_invocationss.
-00000f90: 0000 731c 0000 0004 0608 0110 020c 0106  ..s.............
-00000fa0: 010c 0106 ff0e 0302 0106 0106 0104 ff06  ................
-00000fb0: 0306 fc7a 2849 6e76 6f63 6174 696f 6e48  ...z(InvocationH
-00000fc0: 7474 7044 656c 6567 6174 652e 7175 6572  ttpDelegate.quer
-00000fd0: 795f 696e 766f 6361 7469 6f6e 7329 024e  y_invocations).N
-00000fe0: 4e72 1900 0000 2918 da08 5f5f 6e61 6d65  Nr....)...__name
-00000ff0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001000: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00001010: 646f 635f 5f72 0700 0000 da0f 5f5f 616e  doc__r......__an
-00001020: 6e6f 7461 7469 6f6e 735f 5fda 0373 7472  notations__..str
-00001030: 721b 0000 0072 0300 0000 da04 6469 6374  r....r......dict
-00001040: 7223 0000 00da 046c 6973 7472 0f00 0000  r#.....listr....
-00001050: 7211 0000 0072 1000 0000 7237 0000 0072  r....r....r7...r
-00001060: 3b00 0000 7240 0000 0072 1200 0000 7244  ;...r@...r....rD
-00001070: 0000 0072 0200 0000 7209 0000 0072 5200  ...r....r....rR.
-00001080: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00001090: 5f72 1f00 0000 721f 0000 0072 1d00 0000  _r....r....r....
-000010a0: 7220 0000 0072 1300 0000 1d00 0000 738c  r ...r........s.
-000010b0: 0000 000a 0004 0108 0408 011a 0202 0604  ................
-000010c0: ff06 0102 ff06 0102 ff0a 020a fe02 1102  ................
-000010d0: 0104 f802 0202 fe06 0302 fd02 0402 fc02  ................
-000010e0: 0502 fb02 0602 fa06 0702 f906 0802 f802  ................
-000010f0: 090a f702 1f04 ff02 0102 ff06 0102 ff02  ................
-00001100: 020a fe02 0702 0102 ff02 0102 ff02 0102  ................
-00001110: ff02 020a fe02 1004 fc02 0202 fe02 0302  ................
-00001120: fd06 0402 fc02 050a fb02 1102 0104 fc0a  ................
-00001130: 0202 fe06 0302 fd0e 0402 fc06 0512 fb72  ...............r
-00001140: 1300 0000 291a 724c 0000 00da 0674 7970  ....).rL.....typ
-00001150: 696e 6772 0200 0000 7203 0000 00da 0468  ingr....r......h
-00001160: 7474 7072 0500 0000 7206 0000 0072 0700  ttpr....r....r..
-00001170: 0000 da07 6c6f 6767 696e 6772 0800 0000  ....loggingr....
-00001180: da0a 7061 6769 6e61 7469 6f6e 7209 0000  ..paginationr...
-00001190: 00da 0573 6572 6465 720a 0000 00da 1369  ...serder......i
-000011a0: 6e76 6f63 6174 696f 6e5f 6465 6c65 6761  nvocation_delega
-000011b0: 7465 720c 0000 00da 1969 6e76 6f63 6174  ter......invocat
-000011c0: 696f 6e5f 6874 7470 5f72 6573 6f75 7263  ion_http_resourc
-000011d0: 6573 720d 0000 0072 0e00 0000 da11 696e  esr....r......in
-000011e0: 766f 6361 7469 6f6e 5f72 6563 6f72 6472  vocation_recordr
-000011f0: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
-00001200: 0000 00da 066c 6f67 6765 7272 1300 0000  .....loggerr....
-00001210: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-00001220: 2000 0000 da08 3c6d 6f64 756c 653e 0100   .....<module>..
-00001230: 0000 7316 0000 0008 0010 0114 020c 050c  ..s.............
-00001240: 010c 010c 0110 0318 0406 0714 03         .............
+00000080: 6409 6c0e 6d0f 5a0f 6d10 5a10 0100 6408  d.l.m.Z.m.Z...d.
+00000090: 640a 6c11 6d12 5a12 0100 6408 640b 6c13  d.l.m.Z...d.d.l.
+000000a0: 6d14 5a14 0100 6408 640c 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
+000000b0: 6d17 5a17 0100 6408 640d 6c18 6d19 5a19  m.Z...d.d.l.m.Z.
+000000c0: 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c 0100 6509  m.Z.m.Z.m.Z...e.
+000000d0: 8300 5a1d 4700 640e 640f 8400 640f 6514  ..Z.G.d.d...d.e.
+000000e0: 8303 5a1e 6401 5300 2910 e900 0000 004e  ..Z.d.S.)......N
+000000f0: 2902 da03 416e 79da 084f 7074 696f 6e61  )...Any..Optiona
+00000100: 6ce9 0300 0000 2903 da13 4f52 475f 4f56  l.....)...ORG_OV
+00000110: 4552 5249 4445 5f48 4541 4445 52da 1455  ERRIDE_HEADER..U
+00000120: 5345 525f 4f56 4552 5249 4445 5f48 4541  SER_OVERRIDE_HEA
+00000130: 4445 52da 0a48 7474 7043 6c69 656e 7429  DER..HttpClient)
+00000140: 01da 0e64 6566 6175 6c74 5f6c 6f67 6765  ...default_logge
+00000150: 7229 01da 0d50 6167 696e 6174 6564 4c69  r)...PaginatedLi
+00000160: 7374 2901 da16 7079 6461 6e74 6963 5f6a  st)...pydantic_j
+00000170: 736f 6e61 626c 655f 6469 6374 e901 0000  sonable_dict....
+00000180: 0029 02da 1343 6f6d 7075 7465 5265 7175  .)...ComputeRequ
+00000190: 6972 656d 656e 7473 da13 436f 6e74 6169  irements..Contai
+000001a0: 6e65 7250 6172 616d 6574 6572 7329 01da  nerParameters)..
+000001b0: 0c41 6374 696f 6e52 6563 6f72 6429 01da  .ActionRecord)..
+000001c0: 1249 6e76 6f63 6174 696f 6e44 656c 6567  .InvocationDeleg
+000001d0: 6174 6529 02da 1743 7265 6174 6549 6e76  ate)...CreateInv
+000001e0: 6f63 6174 696f 6e52 6571 7565 7374 da16  ocationRequest..
+000001f0: 5365 744c 6f67 734c 6f63 6174 696f 6e52  SetLogsLocationR
+00000200: 6571 7565 7374 2904 da18 496e 766f 6361  equest)...Invoca
+00000210: 7469 6f6e 4461 7461 536f 7572 6365 5479  tionDataSourceTy
+00000220: 7065 da10 496e 766f 6361 7469 6f6e 5265  pe..InvocationRe
+00000230: 636f 7264 da10 496e 766f 6361 7469 6f6e  cord..Invocation
+00000240: 536f 7572 6365 da10 496e 766f 6361 7469  Source..Invocati
+00000250: 6f6e 5374 6174 7573 6300 0000 0000 0000  onStatusc.......
+00000260: 0000 0000 0000 0000 0013 0000 0000 0000  ................
+00000270: 0073 3a01 0000 6500 5a01 6400 5a02 5500  .s:...e.Z.d.Z.U.
+00000280: 6401 5a03 6504 6505 6402 3c00 6506 6505  d.Z.e.e.d.<.e.e.
+00000290: 6403 3c00 6404 6506 6405 6504 6406 6407  d.<.d.e.d.e.d.d.
+000002a0: 6606 8700 6601 6408 6409 840c 5a07 0907  f...f.d.d...Z...
+000002b0: 6428 640a 6508 6506 1900 640b 6508 6506  d(d.e.e...d.e.e.
+000002c0: 1900 6406 6509 6506 6506 6602 1900 6606  ..d.e.e.e.f...f.
+000002d0: 640c 640d 8405 5a0a 0907 6429 640e 650b  d.d...Z...d)d.e.
+000002e0: 640f 650c 6506 1900 6410 650d 6411 650e  d.e.e...d.e.d.e.
+000002f0: 6412 6506 6413 650f 6414 6510 6415 6508  d.e.d.e.d.e.d.e.
+00000300: 6506 1900 6406 6511 6612 6416 6417 8405  e...d.e.f.d.d...
+00000310: 5a12 0907 6429 6418 6506 640a 6508 6506  Z...d)d.e.d.e.e.
+00000320: 1900 6406 6511 6606 6419 641a 8405 5a13  ..d.e.f.d.d...Z.
+00000330: 641b 6511 641c 6506 641d 6506 6406 6511  d.e.d.e.d.e.d.e.
+00000340: 6608 641e 641f 8404 5a14 0907 6429 641b  f.d.d...Z...d)d.
+00000350: 6511 6420 6515 6421 6508 6506 1900 6406  e.d e.d!e.e...d.
+00000360: 6511 6608 6422 6423 8405 5a16 0907 0907  e.f.d"d#..Z.....
+00000370: 6428 6424 6509 6506 6517 6602 1900 640a  d(d$e.e.e.f...d.
+00000380: 6508 6506 1900 6425 6508 6509 6506 6506  e.e...d%e.e.e.e.
+00000390: 6602 1900 1900 6406 6518 6511 1900 6608  f.....d.e.e...f.
+000003a0: 6426 6427 8405 5a19 8700 0400 5a1a 5300  d&d'..Z.....Z.S.
+000003b0: 292a da16 496e 766f 6361 7469 6f6e 4874  )*..InvocationHt
+000003c0: 7470 4465 6c65 6761 7465 7a47 0a20 2020  tpDelegatezG.   
+000003d0: 2055 7365 2069 6e20 616e 7920 636f 6e74   Use in any cont
+000003e0: 6578 7420 7468 6174 2064 6f65 7320 6e6f  ext that does no
+000003f0: 7420 6861 7665 2064 6972 6563 7420 6461  t have direct da
+00000400: 7461 6261 7365 2061 6363 6573 732e 0a20  tabase access.. 
+00000410: 2020 20da 245f 496e 766f 6361 7469 6f6e     .$_Invocation
+00000420: 4874 7470 4465 6c65 6761 7465 5f5f 6874  HttpDelegate__ht
+00000430: 7470 5f63 6c69 656e 74da 305f 496e 766f  tp_client.0_Invo
+00000440: 6361 7469 6f6e 4874 7470 4465 6c65 6761  cationHttpDelega
+00000450: 7465 5f5f 726f 626f 746f 5f73 6572 7669  te__roboto_servi
+00000460: 6365 5f62 6173 655f 7572 6cda 1772 6f62  ce_base_url..rob
+00000470: 6f74 6f5f 7365 7276 6963 655f 6261 7365  oto_service_base
+00000480: 5f75 726c da0b 6874 7470 5f63 6c69 656e  _url..http_clien
+00000490: 74da 0672 6574 7572 6e4e 6303 0000 0000  t..returnNc.....
+000004a0: 0000 0000 0000 0003 0000 0002 0000 0003  ................
+000004b0: 0000 0073 1a00 0000 7400 8300 a001 a100  ...s....t.......
+000004c0: 0100 7c02 7c00 5f02 7c01 7c00 5f03 6400  ..|.|._.|.|._.d.
+000004d0: 5300 a901 4e29 04da 0573 7570 6572 da08  S...N)...super..
+000004e0: 5f5f 696e 6974 5f5f 7217 0000 0072 1800  __init__r....r..
+000004f0: 0000 2903 da04 7365 6c66 7219 0000 0072  ..)...selfr....r
+00000500: 1a00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00000510: 5fa9 00fa ff2f 636f 6465 6275 696c 642f  _..../codebuild/
+00000520: 6f75 7470 7574 2f73 7263 3136 3839 3135  output/src168915
+00000530: 3533 3939 2f73 7263 2f63 6f64 6573 7461  5399/src/codesta
+00000540: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
+00000550: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
+00000560: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
+00000570: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
+00000580: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
+00000590: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
+000005a0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
+000005b0: 6f2d 6169 2f72 6f62 6f74 6f2d 686f 7374  o-ai/roboto-host
+000005c0: 6564 2d61 7070 2f70 6163 6b61 6765 732f  ed-app/packages/
+000005d0: 726f 626f 746f 5f73 646b 2f73 7263 2f72  roboto_sdk/src/r
+000005e0: 6f62 6f74 6f5f 7364 6b2f 646f 6d61 696e  oboto_sdk/domain
+000005f0: 2f61 6374 696f 6e73 2f69 6e76 6f63 6174  /actions/invocat
+00000600: 696f 6e5f 6874 7470 5f64 656c 6567 6174  ion_http_delegat
+00000610: 652e 7079 721e 0000 002a 0000 0073 0600  e.pyr....*...s..
+00000620: 0000 0a01 0601 0a01 7a1f 496e 766f 6361  ........z.Invoca
+00000630: 7469 6f6e 4874 7470 4465 6c65 6761 7465  tionHttpDelegate
+00000640: 2e5f 5f69 6e69 745f 5fda 066f 7267 5f69  .__init__..org_i
+00000650: 64da 0775 7365 725f 6964 6303 0000 0000  d..user_idc.....
+00000660: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00000670: 0000 0073 2400 0000 6401 6402 6901 7d03  ...s$...d.d.i.}.
+00000680: 7c01 720a 7c01 7c03 7400 3c00 7c02 7210  |.r.|.|.t.<.|.r.
+00000690: 7c02 7c03 7401 3c00 7c03 5300 2903 4e7a  |.|.t.<.|.S.).Nz
+000006a0: 0c43 6f6e 7465 6e74 2d54 7970 657a 1061  .Content-Typez.a
+000006b0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e29  pplication/json)
+000006c0: 0272 0500 0000 7206 0000 0029 0472 1f00  .r....r....).r..
+000006d0: 0000 7224 0000 0072 2500 0000 da07 6865  ..r$...r%.....he
+000006e0: 6164 6572 7372 2200 0000 7222 0000 0072  adersr"...r"...r
+000006f0: 2300 0000 7226 0000 002f 0000 0073 0c00  #...r&.../...s..
+00000700: 0000 0803 0401 0801 0401 0801 0401 7a1e  ..............z.
+00000710: 496e 766f 6361 7469 6f6e 4874 7470 4465  InvocationHttpDe
+00000720: 6c65 6761 7465 2e68 6561 6465 7273 da0d  legate.headers..
+00000730: 6163 7469 6f6e 5f72 6563 6f72 64da 0a69  action_record..i
+00000740: 6e70 7574 5f64 6174 61da 1463 6f6d 7075  nput_data..compu
+00000750: 7465 5f72 6571 7569 7265 6d65 6e74 73da  te_requirements.
+00000760: 1463 6f6e 7461 696e 6572 5f70 6172 616d  .container_param
+00000770: 6574 6572 73da 0e64 6174 615f 736f 7572  eters..data_sour
+00000780: 6365 5f69 64da 1064 6174 615f 736f 7572  ce_id..data_sour
+00000790: 6365 5f74 7970 65da 1169 6e76 6f63 6174  ce_type..invocat
+000007a0: 696f 6e5f 736f 7572 6365 da14 696e 766f  ion_source..invo
+000007b0: 6361 7469 6f6e 5f73 6f75 7263 655f 6964  cation_source_id
+000007c0: 6309 0000 0000 0000 0000 0000 000c 0000  c...............
+000007d0: 0009 0000 0043 0000 0073 7200 0000 7c00  .....C...sr...|.
+000007e0: 6a00 9b00 6401 7c01 6a01 9b00 6402 9d04  j...d.|.j...d...
+000007f0: 7d09 7402 7c02 7c05 7c06 7c07 7c08 7c03  }.t.|.|.|.|.|.|.
+00000800: 7c04 6403 8d07 7d0a 7c00 6a03 6a04 7c09  |.d...}.|.j.j.|.
+00000810: 7405 7c0a 6404 6405 8d02 7c00 6a06 7c01  t.|.d.d...|.j.|.
+00000820: 6a07 7c07 7408 6a09 6b02 7229 7c08 6e01  j.|.t.j.k.r)|.n.
+00000830: 6400 6406 8d02 6407 8d03 7d0b 740a a00b  d.d...d...}.t...
+00000840: 7c0b 6a0c 6408 6701 6409 8d01 a101 5300  |.j.d.g.d.....S.
+00000850: 290a 4e7a 0c2f 7631 2f61 6374 696f 6e73  ).Nz./v1/actions
+00000860: 2f7a 072f 696e 766f 6b65 2907 7228 0000  /z./invoke).r(..
+00000870: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000880: 722e 0000 0072 2900 0000 722a 0000 0054  r....r)...r*...T
+00000890: a901 da0c 6578 636c 7564 655f 6e6f 6e65  ....exclude_none
+000008a0: 2902 7224 0000 0072 2500 0000 a902 da04  ).r$...r%.......
+000008b0: 6461 7461 7226 0000 0072 3200 0000 a901  datar&...r2.....
+000008c0: da09 6a73 6f6e 5f70 6174 6829 0d72 1800  ..json_path).r..
+000008d0: 0000 da04 6e61 6d65 7210 0000 0072 1700  ....namer....r..
+000008e0: 0000 da04 706f 7374 720a 0000 0072 2600  ....postr....r&.
+000008f0: 0000 7224 0000 0072 1400 0000 da06 4d61  ..r$...r......Ma
+00000900: 6e75 616c 7213 0000 00da 0970 6172 7365  nualr......parse
+00000910: 5f6f 626a da09 6672 6f6d 5f6a 736f 6e29  _obj..from_json)
+00000920: 0c72 1f00 0000 7227 0000 0072 2800 0000  .r....r'...r(...
+00000930: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
+00000940: 2c00 0000 722d 0000 0072 2e00 0000 da03  ,...r-...r......
+00000950: 7572 6cda 0c72 6571 7565 7374 5f62 6f64  url..request_bod
+00000960: 79da 0872 6573 706f 6e73 6572 2200 0000  y..responser"...
+00000970: 7222 0000 0072 2300 0000 da11 6372 6561  r"...r#.....crea
+00000980: 7465 5f69 6e76 6f63 6174 696f 6e39 0000  te_invocation9..
+00000990: 0073 2a00 0000 140b 0201 0201 0201 0201  .s*.............
+000009a0: 0201 0201 0201 0201 06f9 0609 0201 0a01  ................
+000009b0: 0401 0401 0a02 04ff 0202 04fc 06fd 140a  ................
+000009c0: 7a28 496e 766f 6361 7469 6f6e 4874 7470  z(InvocationHttp
+000009d0: 4465 6c65 6761 7465 2e63 7265 6174 655f  Delegate.create_
+000009e0: 696e 766f 6361 7469 6f6e da0d 696e 766f  invocation..invo
+000009f0: 6361 7469 6f6e 5f69 6463 0300 0000 0000  cation_idc......
+00000a00: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+00000a10: 0000 733a 0000 007c 006a 009b 0064 017c  ..s:...|.j...d.|
+00000a20: 019b 009d 037d 037c 006a 016a 027c 037c  .....}.|.j.j.|.|
+00000a30: 00a0 037c 02a1 0164 028d 027d 0474 04a0  ...|...d...}.t..
+00000a40: 057c 046a 0664 0367 0164 048d 01a1 0153  .|.j.d.g.d.....S
+00000a50: 0029 054e fa18 2f76 312f 6163 7469 6f6e  .).N../v1/action
+00000a60: 732f 696e 766f 6361 7469 6f6e 732f 2901  s/invocations/).
+00000a70: 7226 0000 0072 3200 0000 7233 0000 0029  r&...r2...r3...)
+00000a80: 0772 1800 0000 7217 0000 00da 0367 6574  .r....r......get
+00000a90: 7226 0000 0072 1300 0000 7238 0000 0072  r&...r....r8...r
+00000aa0: 3900 0000 2905 721f 0000 0072 3e00 0000  9...).r....r>...
+00000ab0: 7224 0000 0072 3a00 0000 723c 0000 0072  r$...r:...r<...r
+00000ac0: 2200 0000 7222 0000 0072 2300 0000 da09  "...r"...r#.....
+00000ad0: 6765 745f 6279 5f69 645a 0000 0073 0600  get_by_idZ...s..
+00000ae0: 0000 1003 1601 1401 7a20 496e 766f 6361  ........z Invoca
+00000af0: 7469 6f6e 4874 7470 4465 6c65 6761 7465  tionHttpDelegate
+00000b00: 2e67 6574 5f62 795f 6964 da06 7265 636f  .get_by_id..reco
+00000b10: 7264 da06 6275 636b 6574 da06 7072 6566  rd..bucket..pref
+00000b20: 6978 6304 0000 0000 0000 0000 0000 0007  ixc.............
+00000b30: 0000 0006 0000 0043 0000 0073 5600 0000  .......C...sV...
+00000b40: 7c00 6a00 9b00 6401 7c01 6a01 9b00 6402  |.j...d.|.j...d.
+00000b50: 9d04 7d04 7402 7c02 7c03 6403 8d02 7d05  ..}.t.|.|.d...}.
+00000b60: 7c00 6a03 6a04 7c04 7405 7c05 6404 6405  |.j.j.|.t.|.d.d.
+00000b70: 8d02 7c00 a006 7c01 6a07 a101 6406 8d03  ..|...|.j...d...
+00000b80: 7d06 7408 a009 7c06 6a0a 6407 6701 6408  }.t...|.j.d.g.d.
+00000b90: 8d01 a101 5300 2909 4e72 3f00 0000 7a05  ....S.).Nr?...z.
+00000ba0: 2f6c 6f67 7329 0272 4300 0000 7244 0000  /logs).rC...rD..
+00000bb0: 0054 722f 0000 0072 3100 0000 7232 0000  .Tr/...r1...r2..
+00000bc0: 0072 3300 0000 290b 7218 0000 0072 3e00  .r3...).r....r>.
+00000bd0: 0000 7211 0000 0072 1700 0000 da05 7061  ..r....r......pa
+00000be0: 7463 6872 0a00 0000 7226 0000 0072 2400  tchr....r&...r$.
+00000bf0: 0000 7213 0000 0072 3800 0000 7239 0000  ..r....r8...r9..
+00000c00: 0029 0772 1f00 0000 7242 0000 0072 4300  .).r....rB...rC.
+00000c10: 0000 7244 0000 0072 3a00 0000 723b 0000  ..rD...r:...r;..
+00000c20: 0072 3c00 0000 7222 0000 0072 2200 0000  .r<...r"...r"...
+00000c30: 7223 0000 00da 1173 6574 5f6c 6f67 735f  r#.....set_logs_
+00000c40: 6c6f 6361 7469 6f6e 6100 0000 7310 0000  locationa...s...
+00000c50: 0014 030c 0106 0102 010a 010a 0106 fd14  ................
+00000c60: 057a 2849 6e76 6f63 6174 696f 6e48 7474  .z(InvocationHtt
+00000c70: 7044 656c 6567 6174 652e 7365 745f 6c6f  pDelegate.set_lo
+00000c80: 6773 5f6c 6f63 6174 696f 6eda 0673 7461  gs_location..sta
+00000c90: 7475 73da 0664 6574 6169 6c63 0400 0000  tus..detailc....
+00000ca0: 0000 0000 0000 0000 0600 0000 0600 0000  ................
+00000cb0: 4300 0000 734a 0000 007c 006a 009b 0064  C...sJ...|.j...d
+00000cc0: 017c 016a 019b 0064 029d 047d 047c 006a  .|.j...d...}.|.j
+00000cd0: 026a 037c 047c 026a 047c 0364 039c 027c  .j.|.|.j.|.d...|
+00000ce0: 00a0 057c 016a 06a1 0164 048d 037d 0574  ...|.j...d...}.t
+00000cf0: 07a0 087c 056a 0964 0567 0164 068d 01a1  ...|.j.d.g.d....
+00000d00: 0153 0029 074e 723f 0000 007a 072f 7374  .S.).Nr?...z./st
+00000d10: 6174 7573 2902 7247 0000 0072 4800 0000  atus).rG...rH...
+00000d20: 7231 0000 0072 3200 0000 7233 0000 0029  r1...r2...r3...)
+00000d30: 0a72 1800 0000 723e 0000 0072 1700 0000  .r....r>...r....
+00000d40: 7236 0000 00da 0576 616c 7565 7226 0000  r6.....valuer&..
+00000d50: 0072 2400 0000 7213 0000 0072 3800 0000  .r$...r....r8...
+00000d60: 7239 0000 0029 0672 1f00 0000 7242 0000  r9...).r....rB..
+00000d70: 0072 4700 0000 7248 0000 0072 3a00 0000  .rG...rH...r:...
+00000d80: 723c 0000 0072 2200 0000 7222 0000 0072  r<...r"...r"...r
+00000d90: 2300 0000 da18 7570 6461 7465 5f69 6e76  #.....update_inv
+00000da0: 6f63 6174 696f 6e5f 7374 6174 7573 6d00  ocation_statusm.
+00000db0: 0000 730e 0000 0014 0606 0102 010a 010a  ..s.............
+00000dc0: 0106 fd14 057a 2f49 6e76 6f63 6174 696f  .....z/Invocatio
+00000dd0: 6e48 7474 7044 656c 6567 6174 652e 7570  nHttpDelegate.up
+00000de0: 6461 7465 5f69 6e76 6f63 6174 696f 6e5f  date_invocation_
+00000df0: 7374 6174 7573 da07 6669 6c74 6572 73da  status..filters.
+00000e00: 0a70 6167 655f 746f 6b65 6e63 0400 0000  .page_tokenc....
+00000e10: 0000 0000 0000 0000 0800 0000 0600 0000  ................
+00000e20: 4300 0000 736c 0000 007c 0372 067c 037c  C...sl...|.r.|.|
+00000e30: 0164 013c 0074 00a0 0174 00a0 027c 01a1  .d.<.t...t...|..
+00000e40: 01a1 017d 047c 006a 039b 0064 029d 027d  ...}.|.j...d...}
+00000e50: 057c 006a 046a 057c 057c 047c 00a0 067c  .|.j.j.|.|.|...|
+00000e60: 02a1 0164 038d 037d 067c 066a 0764 0467  ...d...}.|.j.d.g
+00000e70: 0164 058d 017d 0774 0864 0664 0784 007c  .d...}.t.d.d...|
+00000e80: 0764 0819 0044 0083 017c 0764 0919 0064  .d...D...|.d...d
+00000e90: 0a8d 0253 0029 0b4e 724c 0000 007a 1d2f  ...S.).NrL...z./
+00000ea0: 7631 2f61 6374 696f 6e73 2f69 6e76 6f63  v1/actions/invoc
+00000eb0: 6174 696f 6e73 2f71 7565 7279 7231 0000  ations/queryr1..
+00000ec0: 0072 3200 0000 7233 0000 0063 0100 0000  .r2...r3...c....
+00000ed0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00000ee0: 5300 0000 7316 0000 0067 007c 005d 077d  S...s....g.|.].}
+00000ef0: 0174 00a0 017c 01a1 0191 0271 0253 0072  .t...|.....q.S.r
+00000f00: 2200 0000 2902 7213 0000 0072 3800 0000  "...).r....r8...
+00000f10: 2902 da02 2e30 da07 6461 7461 7365 7472  )....0..datasetr
+00000f20: 2200 0000 7222 0000 0072 2300 0000 da0a  "...r"...r#.....
+00000f30: 3c6c 6973 7463 6f6d 703e 8b00 0000 7306  <listcomp>....s.
+00000f40: 0000 0006 000a 0106 ff7a 3c49 6e76 6f63  .........z<Invoc
+00000f50: 6174 696f 6e48 7474 7044 656c 6567 6174  ationHttpDelegat
+00000f60: 652e 7175 6572 795f 696e 766f 6361 7469  e.query_invocati
+00000f70: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6c69  ons.<locals>.<li
+00000f80: 7374 636f 6d70 3eda 0569 7465 6d73 da0a  stcomp>..items..
+00000f90: 6e65 7874 5f74 6f6b 656e 2902 7250 0000  next_token).rP..
+00000fa0: 0072 5100 0000 2909 da04 6a73 6f6e da05  .rQ...)...json..
+00000fb0: 6c6f 6164 73da 0564 756d 7073 7218 0000  loads..dumpsr...
+00000fc0: 0072 1700 0000 7236 0000 0072 2600 0000  .r....r6...r&...
+00000fd0: 7239 0000 0072 0900 0000 2908 721f 0000  r9...r....).r...
+00000fe0: 0072 4b00 0000 7224 0000 0072 4c00 0000  .rK...r$...rL...
+00000ff0: da0c 7361 6665 5f66 696c 7465 7273 723a  ..safe_filtersr:
+00001000: 0000 00da 0372 6573 da0c 756e 6d61 7273  .....res..unmars
+00001010: 6861 6c6c 6564 7222 0000 0072 2200 0000  halledr"...r"...
+00001020: 7223 0000 00da 1171 7565 7279 5f69 6e76  r#.....query_inv
+00001030: 6f63 6174 696f 6e73 7b00 0000 731c 0000  ocations{...s...
+00001040: 0004 0608 0110 020c 0106 010c 0106 ff0e  ................
+00001050: 0302 0106 0106 0104 ff06 0306 fc7a 2849  .............z(I
+00001060: 6e76 6f63 6174 696f 6e48 7474 7044 656c  nvocationHttpDel
+00001070: 6567 6174 652e 7175 6572 795f 696e 766f  egate.query_invo
+00001080: 6361 7469 6f6e 7329 024e 4e72 1c00 0000  cations).NNr....
+00001090: 291b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000010a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000010b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+000010c0: 0700 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
+000010d0: 6f6e 735f 5fda 0373 7472 721e 0000 0072  ons__..strr....r
+000010e0: 0300 0000 da04 6469 6374 7226 0000 0072  ......dictr&...r
+000010f0: 0e00 0000 da04 6c69 7374 720c 0000 0072  ......listr....r
+00001100: 0d00 0000 7212 0000 0072 1400 0000 7213  ....r....r....r.
+00001110: 0000 0072 3d00 0000 7241 0000 0072 4600  ...r=...rA...rF.
+00001120: 0000 7215 0000 0072 4a00 0000 7202 0000  ..r....rJ...r...
+00001130: 0072 0900 0000 7258 0000 00da 0d5f 5f63  .r....rX.....__c
+00001140: 6c61 7373 6365 6c6c 5f5f 7222 0000 0072  lasscell__r"...r
+00001150: 2200 0000 7220 0000 0072 2300 0000 7216  "...r ...r#...r.
+00001160: 0000 0022 0000 0073 8e00 0000 0a00 0401  ..."...s........
+00001170: 0804 0801 1a02 0206 04ff 0601 02ff 0601  ................
+00001180: 02ff 0a02 0afe 0213 04f7 0202 02fe 0603  ................
+00001190: 02fd 0204 02fc 0205 02fb 0206 02fa 0207  ................
+000011a0: 02f9 0208 02f8 0609 02f7 020a 0af6 0222  ..............."
+000011b0: 04ff 0201 02ff 0601 02ff 0202 0afe 0207  ................
+000011c0: 0201 02ff 0201 02ff 0201 02ff 0202 0afe  ................
+000011d0: 0210 04fc 0202 02fe 0203 02fd 0604 02fc  ................
+000011e0: 0205 0afb 0211 0201 04fc 0a02 02fe 0603  ................
+000011f0: 02fd 0e04 02fc 0605 12fb 7216 0000 0029  ..........r....)
+00001200: 1f72 5200 0000 da06 7479 7069 6e67 7202  .rR.....typingr.
+00001210: 0000 0072 0300 0000 da04 6874 7470 7205  ...r......httpr.
+00001220: 0000 0072 0600 0000 7207 0000 00da 076c  ...r....r......l
+00001230: 6f67 6769 6e67 7208 0000 00da 0a70 6167  oggingr......pag
+00001240: 696e 6174 696f 6e72 0900 0000 da05 7365  inationr......se
+00001250: 7264 6572 0a00 0000 da1a 6163 7469 6f6e  rder......action
+00001260: 5f63 6f6e 7461 696e 6572 5f72 6573 6f75  _container_resou
+00001270: 7263 6573 720c 0000 0072 0d00 0000 7227  rcesr....r....r'
+00001280: 0000 0072 0e00 0000 da13 696e 766f 6361  ...r......invoca
+00001290: 7469 6f6e 5f64 656c 6567 6174 6572 0f00  tion_delegater..
+000012a0: 0000 da19 696e 766f 6361 7469 6f6e 5f68  ....invocation_h
+000012b0: 7474 705f 7265 736f 7572 6365 7372 1000  ttp_resourcesr..
+000012c0: 0000 7211 0000 00da 1169 6e76 6f63 6174  ..r......invocat
+000012d0: 696f 6e5f 7265 636f 7264 7212 0000 0072  ion_recordr....r
+000012e0: 1300 0000 7214 0000 0072 1500 0000 da06  ....r....r......
+000012f0: 6c6f 6767 6572 7216 0000 0072 2200 0000  loggerr....r"...
+00001300: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
+00001310: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
+00001320: 0000 0800 1001 1402 0c05 0c01 0c01 1001  ................
+00001330: 0c04 0c01 1003 1804 0607 1403            ............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import collections.abc
+import datetime
 from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerCredentials,
+    ContainerParameters,
+)
 from .action_delegate import (
     ActionDelegate,
-    ContainerCredentials,
     UpdateCondition,
 )
 from .action_record import ActionRecord
-from .error import InvocationError
 from .invocation import Invocation
 from .invocation_delegate import (
     InvocationDelegate,
 )
 from .invocation_record import (
     InvocationDataSourceType,
     InvocationSource,
@@ -42,22 +46,26 @@
         action_delegate: ActionDelegate,
         invocation_delegate: InvocationDelegate,
         org_id: Optional[str] = None,
         description: Optional[str] = None,
         metadata: Optional[dict[str, Any]] = None,
         tags: Optional[list[str]] = None,
         created_by: Optional[str] = None,
+        compute_requirements: Optional[ComputeRequirements] = None,
+        container_parameters: Optional[ContainerParameters] = None,
     ) -> "Action":
         record = action_delegate.create_action(
             name,
             org_id,
             created_by,
             description,
             metadata,
             tags,
+            compute_requirements,
+            container_parameters,
         )
         return cls(record, action_delegate, invocation_delegate)
 
     @classmethod
     def from_name(
         cls,
         name: str,
@@ -106,14 +114,26 @@
         invocation_delegate: InvocationDelegate,
     ) -> None:
         self.__action_delegate = action_delegate
         self.__invocation_delegate = invocation_delegate
         self.__record = record
 
     @property
+    def compute_requirements(self) -> ComputeRequirements:
+        return self.__record.compute_requirements
+
+    @property
+    def container_parameters(self) -> ContainerParameters:
+        return self.__record.container_parameters
+
+    @property
+    def last_modified(self) -> datetime.datetime:
+        return self.__record.modified
+
+    @property
     def name(self) -> str:
         return self.__record.name
 
     @property
     def org_id(self) -> str:
         return self.__record.org_id
 
@@ -137,41 +157,55 @@
 
     def invoke(
         self,
         input_data: list[str],
         data_source_id: str,
         data_source_type: InvocationDataSourceType,
         invocation_source: InvocationSource,
-        invocation_source_id: Optional[str],
+        invocation_source_id: Optional[str] = None,
+        compute_requirement_overrides: Optional[ComputeRequirements] = None,
+        container_parameter_overrides: Optional[ContainerParameters] = None,
     ) -> Invocation:
-        if self.__record.is_available is not True:
-            raise InvocationError(
-                "A container image must be associated with this Action and pushed before it can be invoked"
+        compute_reqs = self.__record.compute_requirements.copy(
+            deep=True,
+            update=compute_requirement_overrides.dict(
+                exclude_none=True, exclude_defaults=True, exclude_unset=True
             )
-
+            if compute_requirement_overrides
+            else dict(),
+        )
+        container_params = self.__record.container_parameters.copy(
+            deep=True,
+            update=container_parameter_overrides.dict(
+                exclude_none=True, exclude_defaults=True, exclude_unset=True
+            )
+            if container_parameter_overrides
+            else dict(),
+        )
         record = self.__invocation_delegate.create_invocation(
-            self.__record.name,
+            self.__record,
             input_data,
+            compute_reqs,
+            container_params,
             data_source_id,
             data_source_type,
             invocation_source,
             invocation_source_id,
-            self.__record.org_id,
         )
         return Invocation(
             record,
             self.__invocation_delegate,
         )
 
     def register_container(
         self,
         image_name: str,
         image_tag: str,
         caller: Optional[str] = None,  # A Roboto user_id
-    ) -> tuple[str, str]:
+    ) -> None:
         """
         Idempotent get or create container repository for this Action, and associate it with the Action as its URI.
         Use this to associate an Action with a container image that has yet to be pushed,
         or with a container image that has already been pushed to an existing repository.
 
         A container may be pushed to the reposistory using credentials returned by
         `get_temporary_container_credentials`.
@@ -182,17 +216,18 @@
             * If a container repository for given `image_name`:`image_tag` does not exist, it will be created.
             * If a container repository was previously created for this Action for a different `image_name`,
               AND that repository is empty, it will be deleted.
             * Sets the `uri` attribute of this Action to the URI of the image expected to be pushed to the repository.
 
         `caller` is ignored on the client. It is determined server-side via the identity/access mechanism.
         """
-        return self.__action_delegate.register_container(
+        updated = self.__action_delegate.register_container(
             self.__record, image_name, image_tag, caller
         )
+        self.__record = updated
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
 
     def update(
         self,
         updates: dict[str, Any],
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 import abc
-import datetime
 from typing import Any, Literal, Optional
 
 import pydantic
 
 from ...pagination import PaginatedList
-from ...serde import pydantic_jsonable_dict
-from ...time import utcnow
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerCredentials,
+    ContainerParameters,
+)
 from .action_record import ActionRecord
 
 
-class ContainerCredentials(pydantic.BaseModel):
-    username: str
-    password: str
-    registry_url: str
-    expiration: datetime.datetime
-
-    def is_expired(self) -> bool:
-        return utcnow() >= self.expiration
-
-    def to_dict(self) -> dict[str, Any]:
-        return pydantic_jsonable_dict(self)
-
-
 class UpdateCondition(pydantic.BaseModel):
     """
     A condition to be applied to an Action update operation.
 
     `value` is compared to the Action's current value of `key` using `comparator`.
 
     This is a severely constrainted subset of the conditions supported by DynamoDB. See:
@@ -46,14 +35,16 @@
         self,
         name: str,
         org_id: Optional[str] = None,
         created_by: Optional[str] = None,  # A Roboto user_id
         description: Optional[str] = None,
         metadata: Optional[dict[str, Any]] = None,
         tags: Optional[list[str]] = None,
+        compute_requirements: Optional[ComputeRequirements] = None,
+        container_parameters: Optional[ContainerParameters] = None,
     ) -> ActionRecord:
         raise NotImplementedError("create_action")
 
     @abc.abstractmethod
     def get_action_by_primary_key(
         self, name: str, org_id: Optional[str] = None
     ) -> ActionRecord:
@@ -62,15 +53,15 @@
     @abc.abstractmethod
     def register_container(
         self,
         record: ActionRecord,
         image_name: str,
         image_tag: str,
         caller: Optional[str] = None,  # A Roboto user_id
-    ) -> tuple[str, str]:
+    ) -> ActionRecord:
         raise NotImplementedError("register_container")
 
     @abc.abstractmethod
     def get_temp_container_credentials(
         self,
         record: ActionRecord,
         caller: Optional[str] = None,  # A Roboto user_id
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import http
 import json
 from typing import Any, Optional
 
+from ...exceptions import RobotoDomainException
 from ...http import (
     ORG_OVERRIDE_HEADER,
     USER_OVERRIDE_HEADER,
     ClientError,
     HttpClient,
 )
 from ...logging import default_logger
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerCredentials,
+    ContainerParameters,
+)
 from .action_delegate import (
     ActionDelegate,
-    ContainerCredentials,
     UpdateCondition,
 )
 from .action_http_resources import (
     CreateActionRequest,
     UpdateActionRequest,
 )
 from .action_record import ActionRecord
@@ -55,54 +60,60 @@
         self,
         name: str,
         org_id: Optional[str] = None,
         created_by: Optional[str] = None,
         description: Optional[str] = None,
         metadata: Optional[dict[str, Any]] = None,
         tags: Optional[list[str]] = None,
+        compute_requirements: Optional[ComputeRequirements] = None,
+        container_parameters: Optional[ContainerParameters] = None,
     ) -> ActionRecord:
         url = f"{self.__roboto_service_base_url}/v1/actions"
         request_body = CreateActionRequest(
             name=name,
             description=description,
             metadata=metadata,
             tags=tags,
+            compute_requirements=compute_requirements,
+            container_parameters=container_parameters,
         )
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
             headers=self.headers(org_id, created_by),
         )
         return ActionRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_action_by_primary_key(
         self, name: str, org_id: Optional[str] = None
     ) -> ActionRecord:
         url = f"{self.__roboto_service_base_url}/v1/actions/{name}"
-        res = self.__http_client.get(url, headers=self.headers(org_id))
-        return ActionRecord.parse_obj(res.from_json(json_path=["data"]))
+        try:
+            res = self.__http_client.get(url, headers=self.headers(org_id))
+            return ActionRecord.parse_obj(res.from_json(json_path=["data"]))
+        except ClientError as exc:
+            raise RobotoDomainException.from_client_error(exc)
 
     def register_container(
         self,
         record: ActionRecord,
         image_name: str,
         image_tag: str,
         caller: Optional[str] = None,
-    ) -> tuple[str, str]:
+    ) -> ActionRecord:
         url = f"{self.__roboto_service_base_url}/v1/actions/{record.name}/container"
         data = {
             "image_name": image_name,
             "image_tag": image_tag,
         }
 
-        res = self.__http_client.put(
+        response = self.__http_client.put(
             url, data=data, headers=self.headers(user_id=caller)
         )
-        parsed_res = res.from_json(json_path=["data"])
-        return (parsed_res["repository_uri"], parsed_res["image_uri"])
+        return ActionRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_temp_container_credentials(
         self,
         record: ActionRecord,
         caller: Optional[str] = None,
     ) -> ContainerCredentials:
         url = f"{self.__roboto_service_base_url}/v1/actions/{record.name}/container/credentials"
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import collections.abc
 from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerParameters,
+)
 from .invocation_delegate import (
     InvocationDelegate,
 )
 from .invocation_record import (
     InvocationDataSource,
     InvocationRecord,
     InvocationStatus,
+    InvocationStatusRecord,
 )
 
 
 class Invocation:
     __invocation_delegate: InvocationDelegate
     __record: InvocationRecord
 
@@ -65,14 +70,22 @@
         self.__record = record
 
     @property
     def action_name(self) -> str:
         return self.__record.action_name
 
     @property
+    def compute_requirements(self) -> ComputeRequirements:
+        return self.__record.compute_requirements
+
+    @property
+    def container_parameters(self) -> ContainerParameters:
+        return self.__record.container_parameters
+
+    @property
     def data_source(self) -> InvocationDataSource:
         return self.__record.data_source
 
     @property
     def id(self) -> str:
         return self.__record.invocation_id
 
@@ -88,17 +101,16 @@
         return self.__record.logs_bucket, self.__record.logs_prefix
 
     @property
     def org_id(self) -> str:
         return self.__record.org_id
 
     @property
-    def status(self) -> InvocationStatus:
-        status_record = self.__record.status[-1]
-        return status_record.status
+    def status_log(self) -> list[InvocationStatusRecord]:
+        return self.__record.status
 
     def is_queued_for_scheduling(self) -> bool:
         """
         An invocation is queued for scheduling if it has not yet reached the "Scheduled" status
         and it is not "Deadly".
         """
         previously_scheduled_or_deadly = (
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import abc
 from typing import Any, Optional
 
 from ...pagination import PaginatedList
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerParameters,
+)
+from .action_record import ActionRecord
 from .invocation_record import (
     InvocationDataSourceType,
     InvocationRecord,
     InvocationSource,
     InvocationStatus,
 )
 
 
 class InvocationDelegate(abc.ABC):
     @abc.abstractmethod
     def create_invocation(
         self,
-        action_name: str,
+        action_record: ActionRecord,
         input_data: list[str],
+        compute_requirements: ComputeRequirements,
+        container_parameters: ContainerParameters,
         data_source_id: str,
         data_source_type: InvocationDataSourceType,
         invocation_source: InvocationSource,
         invocation_source_id: Optional[str] = None,
-        org_id: Optional[str] = None,
     ) -> InvocationRecord:
         """Create an Invocation"""
         raise NotImplementedError("create_invocation")
 
     @abc.abstractmethod
     def get_by_id(
         self, invocation_id: str, org_id: Optional[str] = None
@@ -51,8 +57,8 @@
     @abc.abstractmethod
     def query_invocations(
         self,
         filters: dict[str, Any],
         org_id: Optional[str] = None,
         page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[InvocationRecord]:
-        raise NotImplementedError("query_actions")
+        raise NotImplementedError("query_invocations")
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,19 @@
     ORG_OVERRIDE_HEADER,
     USER_OVERRIDE_HEADER,
     HttpClient,
 )
 from ...logging import default_logger
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerParameters,
+)
+from .action_record import ActionRecord
 from .invocation_delegate import (
     InvocationDelegate,
 )
 from .invocation_http_resources import (
     CreateInvocationRequest,
     SetLogsLocationRequest,
 )
@@ -47,35 +52,38 @@
             headers[ORG_OVERRIDE_HEADER] = org_id
         if user_id:
             headers[USER_OVERRIDE_HEADER] = user_id
         return headers
 
     def create_invocation(
         self,
-        action_name: str,
+        action_record: ActionRecord,
         input_data: list[str],
+        compute_requirements: ComputeRequirements,
+        container_parameters: ContainerParameters,
         data_source_id: str,
         data_source_type: InvocationDataSourceType,
         invocation_source: InvocationSource,
         invocation_source_id: Optional[str] = None,
-        org_id: Optional[str] = None,
     ) -> InvocationRecord:
-        url = f"{self.__roboto_service_base_url}/v1/actions/{action_name}/invoke"
+        url = f"{self.__roboto_service_base_url}/v1/actions/{action_record.name}/invoke"
         request_body = CreateInvocationRequest(
             input_data=input_data,
             data_source_id=data_source_id,
             data_source_type=data_source_type,
             invocation_source=invocation_source,
             invocation_source_id=invocation_source_id,
+            compute_requirements=compute_requirements,
+            container_parameters=container_parameters,
         )
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
             headers=self.headers(
-                org_id=org_id,
+                org_id=action_record.org_id,
                 user_id=invocation_source_id
                 if invocation_source == InvocationSource.Manual
                 else None,
             ),
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 import enum
 from typing import Optional
 
 import pydantic
 
+from .action_container_resources import (
+    ComputeRequirements,
+    ContainerParameters,
+)
+
 
 class InvocationDataSourceType(enum.Enum):
     """Source of data for an Action's InputBinding"""
 
     Dataset = "Dataset"
 
 
@@ -45,17 +50,19 @@
 class InvocationStatusRecord(pydantic.BaseModel):
     status: InvocationStatus
     detail: Optional[str] = None
     timestamp: datetime.datetime  # Persisted as ISO 8601 string in UTC
 
 
 class InvocationRecord(pydantic.BaseModel):
-    invocation_id: str  # Partition key
-    org_id: str
     action_name: str
     created: datetime.datetime  # Persisted as ISO 8601 string in UTC
     data_source: InvocationDataSource
     input_data: list[str]
-    provenance: InvocationProvenance
+    invocation_id: str  # Partition key
     logs_bucket: Optional[str] = None
     logs_prefix: Optional[str] = None
+    compute_requirements: ComputeRequirements
+    container_parameters: ContainerParameters
+    org_id: str
+    provenance: InvocationProvenance
     status: list[InvocationStatusRecord] = pydantic.Field(default_factory=list)
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 2202 0000  o.......Ms.d"...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 2202 0000  o.......1..d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6406 5a0e 6407  m.Z.m.Z...d.Z.d.
@@ -24,15 +24,15 @@
 00000170: 0400 0000 7205 0000 005a 0d68 7474 705f  ....r....Z.http_
 00000180: 6465 6c65 6761 7465 7206 0000 005a 0e68  delegater....Z.h
 00000190: 7474 705f 7265 736f 7572 6365 7372 0700  ttp_resourcesr..
 000001a0: 0000 da06 7265 636f 7264 7208 0000 0072  ....recordr....r
 000001b0: 0900 0000 720a 0000 00da 075f 5f61 6c6c  ....r......__all
 000001c0: 5f5f a900 720e 0000 0072 0e00 0000 faf0  __..r....r......
 000001d0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001e0: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+000001e0: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 000001f0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000200: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000210: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000220: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000230: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000240: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000250: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 9836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 6c26 0000  o.......Ms.dl&..
+00000000: 6f0d 0d0a 0000 0000 3192 a764 ed27 0000  o.......1..d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6405 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6407 6408 6c0e  m.Z.m.Z...d.d.l.
@@ -19,15 +19,15 @@
 00000120: e901 0000 0029 04da 0a41 6363 6573 734d  .....)...AccessM
 00000130: 6f64 65da 0b43 7265 6465 6e74 6961 6c73  ode..Credentials
 00000140: da0f 4461 7461 7365 7444 656c 6567 6174  ..DatasetDelegat
 00000150: 65da 0f53 746f 7261 6765 4c6f 6361 7469  e..StorageLocati
 00000160: 6f6e 2902 da0d 4164 6d69 6e69 7374 7261  on)...Administra
 00000170: 746f 72da 0d44 6174 6173 6574 5265 636f  tor..DatasetReco
 00000180: 7264 6300 0000 0000 0000 0000 0000 0000  rdc.............
-00000190: 0000 0014 0000 0040 0000 0073 f801 0000  .......@...s....
+00000190: 0000 0014 0000 0040 0000 0073 1602 0000  .......@...s....
 000001a0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 000001b0: 3c00 6505 6504 6402 3c00 6403 5a06 6507  <.e.e.d.<.d.Z.e.
 000001c0: 6508 1900 6504 6404 3c00 6403 5a09 6507  e...e.d.<.d.Z.e.
 000001d0: 650a 1900 6504 6405 3c00 650b 650c 6a0d  e...e.d.<.e.e.j.
 000001e0: 650e 6a0f 6403 6403 6403 6403 6403 6607  e.j.d.d.d.d.d.f.
 000001f0: 6406 6503 6407 650c 6408 650e 6409 6507  d.e.d.e.d.e.d.e.
 00000200: 6510 1900 640a 6507 6510 1900 640b 6507  e...d.e.e...d.e.
@@ -44,420 +44,434 @@
 000002b0: 0903 6431 6418 6505 6419 6503 640d 6507  ..d1d.e.d.e.d.e.
 000002c0: 6508 1900 640e 6403 6608 641a 641b 8405  e...d.d.f.d.d...
 000002d0: 5a1a 0903 0903 6430 641c 651b 6a1c 641d  Z.....d0d.e.j.d.
 000002e0: 6507 6513 6510 1900 1900 641e 6507 6513  e.e.e.....d.e.e.
 000002f0: 6510 1900 1900 640e 6403 6608 641f 6420  e.....d.d.f.d.d 
 00000300: 8405 5a1d 651e 6a1f 6403 6602 6421 651e  ..Z.e.j.d.f.d!e.
 00000310: 6422 6507 6510 1900 640e 650a 6606 6423  d"e.e...d.e.f.d#
-00000320: 6424 8405 5a20 640e 6516 6a17 6a18 6521  d$..Z d.e.j.j.e!
-00000330: 6403 6403 6603 1900 6602 6425 6426 8404  d.d.f...f.d%d&..
-00000340: 5a22 640e 6511 6510 6512 6602 1900 6602  Z"d.e.e.e.f...f.
-00000350: 6427 6428 8404 5a23 0903 6431 6429 651b  d'd(..Z#..d1d)e.
-00000360: 6a1c 641e 6507 6513 6510 1900 1900 640e  j.d.e.e.e.....d.
-00000370: 6403 6606 642a 642b 8405 5a24 642c 651b  d.f.d*d+..Z$d,e.
-00000380: 6a1c 642d 6510 640e 6403 6606 642e 642f  j.d-e.d.d.f.d.d/
-00000390: 8404 5a25 6403 5300 2932 da07 4461 7461  ..Z%d.S.)2..Data
-000003a0: 7365 74da 125f 4461 7461 7365 745f 5f64  set.._Dataset__d
-000003b0: 656c 6567 6174 65da 105f 4461 7461 7365  elegate.._Datase
-000003c0: 745f 5f72 6563 6f72 644e da18 5f44 6174  t__recordN.._Dat
-000003d0: 6173 6574 5f5f 6669 6c65 735f 6465 6c65  aset__files_dele
-000003e0: 6761 7465 da1a 5f44 6174 6173 6574 5f5f  gate.._Dataset__
-000003f0: 7465 6d70 5f63 7265 6465 6e74 6961 6c73  temp_credentials
-00000400: da10 6461 7461 7365 745f 6465 6c65 6761  ..dataset_delega
-00000410: 7465 da0d 6164 6d69 6e69 7374 7261 746f  te..administrato
-00000420: 72da 1073 746f 7261 6765 5f6c 6f63 6174  r..storage_locat
-00000430: 696f 6eda 066f 7267 5f69 64da 0a63 7265  ion..org_id..cre
-00000440: 6174 6564 5f62 79da 086d 6574 6164 6174  ated_by..metadat
-00000450: 61da 0474 6167 73da 0e66 696c 6573 5f64  a..tags..files_d
-00000460: 656c 6567 6174 65da 0672 6574 7572 6e63  elegate..returnc
-00000470: 0900 0000 0000 0000 0000 0000 0a00 0000  ................
-00000480: 0800 0000 4300 0000 7320 0000 007c 01a0  ....C...s ...|..
-00000490: 007c 027c 067c 037c 077c 047c 05a1 067d  .|.|.|.|.|.|...}
-000004a0: 097c 007c 097c 017c 0883 0353 00a9 014e  .|.|.|.|...S...N
-000004b0: 2901 5a0e 6372 6561 7465 5f64 6174 6173  ).Z.create_datas
-000004c0: 6574 290a da03 636c 7372 1700 0000 7218  et)...clsr....r.
-000004d0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-000004e0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000004f0: 00da 0672 6563 6f72 64a9 0072 2300 0000  ...record..r#...
-00000500: faef 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000510: 7075 742f 7372 6333 3439 3732 3638 3637  put/src349726867
-00000520: 302f 7372 632f 636f 6465 7374 6172 2d63  0/src/codestar-c
-00000530: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
-00000540: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
-00000550: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
-00000560: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
-00000570: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
-00000580: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
-00000590: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
-000005a0: 692f 726f 626f 746f 2d68 6f73 7465 642d  i/roboto-hosted-
-000005b0: 6170 702f 7061 636b 6167 6573 2f72 6f62  app/packages/rob
-000005c0: 6f74 6f5f 7364 6b2f 7372 632f 726f 626f  oto_sdk/src/robo
-000005d0: 746f 5f73 646b 2f64 6f6d 6169 6e2f 6461  to_sdk/domain/da
-000005e0: 7461 7365 7473 2f64 6174 6173 6574 2e70  tasets/dataset.p
-000005f0: 79da 0663 7265 6174 651d 0000 0073 0800  y..create....s..
-00000600: 0000 040c 0c01 04ff 0c03 7a0e 4461 7461  ..........z.Data
-00000610: 7365 742e 6372 6561 7465 da0a 6461 7461  set.create..data
-00000620: 7365 745f 6964 6305 0000 0000 0000 0000  set_idc.........
-00000630: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
-00000640: 1800 0000 7c02 a000 7c01 7c03 a102 7d05  ....|...|.|...}.
-00000650: 7c00 7c05 7c02 7c04 8303 5300 7220 0000  |.|.|.|...S.r ..
-00000660: 0029 015a 1a67 6574 5f64 6174 6173 6574  .).Z.get_dataset
-00000670: 5f62 795f 7072 696d 6172 795f 6b65 7929  _by_primary_key)
-00000680: 0672 2100 0000 7226 0000 0072 1700 0000  .r!...r&...r....
-00000690: 721a 0000 0072 1e00 0000 7222 0000 0072  r....r....r"...r
-000006a0: 2300 0000 7223 0000 0072 2400 0000 da07  #...r#...r$.....
-000006b0: 6672 6f6d 5f69 642e 0000 0073 0400 0000  from_id....s....
-000006c0: 0c08 0c01 7a0f 4461 7461 7365 742e 6672  ....z.Dataset.fr
-000006d0: 6f6d 5f69 64da 0766 696c 7465 7273 2903  om_id..filters).
-000006e0: 7212 0000 004e 4e63 0500 0000 0000 0000  r....NNc........
-000006f0: 0000 0000 0c00 0000 0600 0000 6300 0000  ............c...
-00000700: 73a2 0000 0081 0074 0074 016a 02a0 03a1  s......t.t.j....
-00000710: 0083 017d 0574 007c 01a0 03a1 0083 017d  ...}.t.|.......}
-00000720: 067c 067c 0518 007d 077c 0772 2c74 047c  .|.|...}.|.r,t.|
-00000730: 0783 0164 016b 047d 087c 0872 1e64 026e  ...d.k.}.|.r.d.n
-00000740: 0164 037d 0974 057c 079b 0064 047c 099b  .d.}.t.|...d.|..
-00000750: 0064 057c 059b 009d 0583 0182 017c 026a  .d.|.........|.j
-00000760: 067c 017c 0464 068d 027d 0a09 007c 0a6a  .|.|.d...}...|.j
-00000770: 0744 005d 097d 0b7c 007c 0b7c 027c 0383  .D.].}.|.|.|.|..
-00000780: 0356 0001 0071 377c 0a6a 0872 4e7c 026a  .V...q7|.j.rN|.j
-00000790: 067c 017c 047c 0a6a 0864 088d 037d 0a6e  .|.|.|.j.d...}.n
-000007a0: 0264 0053 0071 3429 094e 720b 0000 007a  .d.S.q4).Nr....z
-000007b0: 2361 7265 206e 6f74 206b 6e6f 776e 2061  #are not known a
-000007c0: 7474 7269 6275 7465 7320 6f66 2044 6174  ttributes of Dat
-000007d0: 6173 6574 7a23 6973 206e 6f74 2061 206b  asetz#is not a k
-000007e0: 6e6f 776e 2061 7474 7269 6275 7465 206f  nown attribute o
-000007f0: 6620 4461 7461 7365 74da 0120 7a14 2e20  f Dataset.. z.. 
-00000800: 4b6e 6f77 6e20 6174 7472 6962 7574 6573  Known attributes
-00000810: 3a20 2901 721a 0000 0054 2902 721a 0000  : ).r....T).r...
-00000820: 00da 0a70 6167 655f 746f 6b65 6e29 09da  ...page_token)..
-00000830: 0373 6574 7211 0000 00da 0a5f 5f66 6965  .setr......__fie
-00000840: 6c64 735f 5fda 046b 6579 73da 036c 656e  lds__..keys..len
-00000850: da0a 5661 6c75 6545 7272 6f72 5a0e 7175  ..ValueErrorZ.qu
-00000860: 6572 795f 6461 7461 7365 7473 da05 6974  ery_datasets..it
-00000870: 656d 73da 0a6e 6578 745f 746f 6b65 6e29  ems..next_token)
-00000880: 0c72 2100 0000 7228 0000 0072 1700 0000  .r!...r(...r....
-00000890: 721e 0000 0072 1a00 0000 da0a 6b6e 6f77  r....r......know
-000008a0: 6e5f 6b65 7973 da0b 6163 7475 616c 5f6b  n_keys..actual_k
-000008b0: 6579 73da 0c75 6e6b 6e6f 776e 5f6b 6579  eys..unknown_key
-000008c0: 73da 0670 6c75 7261 6cda 036d 7367 da11  s..plural..msg..
-000008d0: 7061 6769 6e61 7465 645f 7265 7375 6c74  paginated_result
-000008e0: 7372 2200 0000 7223 0000 0072 2300 0000  sr"...r#...r#...
-000008f0: 7224 0000 00da 0571 7565 7279 3900 0000  r$.....query9...
-00000900: 732a 0000 0002 800e 080c 0108 0104 010c  s*..............
-00000910: 0102 0306 ff02 0202 fd18 050e 0202 010a  ................
-00000920: 0110 0106 0104 0108 0108 ff04 0402 f87a  ...............z
-00000930: 0d44 6174 6173 6574 2e71 7565 7279 7222  .Dataset.queryr"
-00000940: 0000 00da 0864 656c 6567 6174 6563 0400  .....delegatec..
-00000950: 0000 0000 0000 0000 0000 0400 0000 0200  ................
-00000960: 0000 4300 0000 7316 0000 007c 027c 005f  ..C...s....|.|._
-00000970: 007c 037c 005f 017c 017c 005f 0264 0053  .|.|._.|.|._.d.S
-00000980: 0072 2000 0000 2903 7213 0000 0072 1500  .r ...).r....r..
-00000990: 0000 7214 0000 0029 04da 0473 656c 6672  ..r....)...selfr
-000009a0: 2200 0000 7239 0000 0072 1e00 0000 7223  "...r9...r....r#
-000009b0: 0000 0072 2300 0000 7224 0000 00da 085f  ...r#...r$....._
-000009c0: 5f69 6e69 745f 5f58 0000 0073 0600 0000  _init__X...s....
-000009d0: 0606 0601 0a01 7a10 4461 7461 7365 742e  ......z.Dataset.
-000009e0: 5f5f 696e 6974 5f5f da08 6f75 745f 7061  __init__..out_pa
-000009f0: 7468 da10 696e 636c 7564 655f 7061 7474  th..include_patt
-00000a00: 6572 6e73 da10 6578 636c 7564 655f 7061  erns..exclude_pa
-00000a10: 7474 6572 6e73 6304 0000 0000 0000 0000  tternsc.........
-00000a20: 0000 000a 0000 0005 0000 0043 0000 0073  ...........C...s
-00000a30: ea00 0000 7c00 6a00 6a01 7402 6a03 6b03  ....|.j.j.t.j.k.
-00000a40: 730e 7c00 6a00 6a04 7405 6a06 6b03 7212  s.|.j.j.t.j.k.r.
-00000a50: 7407 6401 8301 8201 6402 7d04 7c02 6402  t.d.....d.}.|.d.
-00000a60: 7501 7221 7408 6a09 a00a 7408 6a0b 6a0c  u.r!t.j...t.j.j.
-00000a70: 7c02 a102 7d04 6402 7d05 7c03 6402 7501  |...}.d.}.|.d.u.
-00000a80: 722d 7408 6a0d a00a 7c03 a101 7d05 7c01  r-t.j...|...}.|.
-00000a90: a00e a100 7337 7c01 6a0f 6403 6404 8d01  ....s7|.j.d.d...
-00000aa0: 0100 7c00 a010 7411 6a12 a101 7d06 7c00  ..|...t.j...}.|.
-00000ab0: 6a13 6402 7501 7245 7c00 6a13 6e06 7414  j.d.u.rE|.j.n.t.
-00000ac0: 7c06 6a15 7c06 6405 8d02 7d07 7c00 a016  |.j.|.d...}.|...
-00000ad0: a100 4400 5d22 7d08 7c04 725c 7c04 a017  ..D.]"}.|.r\|...
-00000ae0: 7c08 6a18 a101 735c 0900 7150 7c05 7266  |.j...s\..qP|.rf
-00000af0: 7c05 a017 7c08 6a18 a101 7266 0900 7150  |...|.j...rf..qP
-00000b00: 7c01 7c08 6a18 1b00 7d09 7c07 a019 7c08  |.|.j...}.|...|.
-00000b10: 6a1a 7c09 a102 0100 7150 6402 5300 2906  j.|.....qPd.S.).
-00000b20: 613f 0200 000a 2020 2020 2020 2020 446f  a?....        Do
-00000b30: 776e 6c6f 6164 2066 696c 6573 2061 7373  wnload files ass
-00000b40: 6f63 6961 7465 6420 7769 7468 2074 6869  ociated with thi
-00000b50: 7320 6461 7461 7365 7420 746f 2074 6865  s dataset to the
-00000b60: 2067 6976 656e 2064 6972 6563 746f 7279   given directory
-00000b70: 2e0a 2020 2020 2020 2020 4966 2060 6f75  ..        If `ou
-00000b80: 745f 7061 7468 6020 646f 6573 206e 6f74  t_path` does not
-00000b90: 2065 7869 7374 2c20 6974 2077 696c 6c20   exist, it will 
-00000ba0: 6265 2063 7265 6174 6564 2e0a 0a20 2020  be created...   
-00000bb0: 2020 2020 2060 696e 636c 7564 655f 7061       `include_pa
-00000bc0: 7474 6572 6e73 6020 616e 6420 6065 7863  tterns` and `exc
-00000bd0: 6c75 6465 5f70 6174 7465 726e 7360 2061  lude_patterns` a
-00000be0: 7265 206c 6973 7473 206f 6620 6769 7469  re lists of giti
-00000bf0: 676e 6f72 652d 7374 796c 6520 7061 7474  gnore-style patt
-00000c00: 6572 6e73 2e0a 2020 2020 2020 2020 5365  erns..        Se
-00000c10: 6520 6874 7470 733a 2f2f 6769 742d 7363  e https://git-sc
-00000c20: 6d2e 636f 6d2f 646f 6373 2f67 6974 6967  m.com/docs/gitig
-00000c30: 6e6f 7265 2e0a 0a20 2020 2020 2020 2045  nore...        E
-00000c40: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-00000c50: 6060 600a 2020 2020 2020 2020 6461 7461  ```.        data
-00000c60: 7365 7420 3d20 6461 7461 7365 7473 2e44  set = datasets.D
-00000c70: 6174 6173 6574 2e62 795f 6964 2822 3c64  ataset.by_id("<d
-00000c80: 6174 6173 6574 5f69 643e 222c 2064 6174  ataset_id>", dat
-00000c90: 6173 6574 5f64 656c 6567 6174 6529 0a20  aset_delegate). 
-00000ca0: 2020 2020 2020 2064 6174 6173 6574 2e64         dataset.d
-00000cb0: 6f77 6e6c 6f61 645f 6669 6c65 7328 0a20  ownload_files(. 
-00000cc0: 2020 2020 2020 2020 2020 2070 6174 686c             pathl
-00000cd0: 6962 2e50 6174 6828 222f 746d 702f 746d  ib.Path("/tmp/tm
-00000ce0: 702e 6e56 3167 6457 3557 4856 2229 2c0a  p.nV1gdW5WHV"),.
-00000cf0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-00000d00: 7564 655f 7061 7474 6572 6e73 3d5b 222a  ude_patterns=["*
-00000d10: 2a2f 2a2e 6734 225d 2c0a 2020 2020 2020  */*.g4"],.      
-00000d20: 2020 2020 2020 6578 636c 7564 655f 7061        exclude_pa
-00000d30: 7474 6572 6e73 3d5b 222a 2a2f 7465 7374  tterns=["**/test
-00000d40: 2f2a 2a22 5d0a 2020 2020 2020 2020 290a  /**"].        ).
-00000d50: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
-00000d60: 2020 2020 fa48 4f6e 6c79 2053 332d 6261      .HOnly S3-ba
-00000d70: 636b 6564 2073 746f 7261 6765 2061 646d  cked storage adm
-00000d80: 696e 6973 7465 7265 6420 6279 2052 6f62  inistered by Rob
-00000d90: 6f74 6f20 6973 2073 7570 706f 7274 6564  oto is supported
-00000da0: 2061 7420 7468 6973 2074 696d 652e 4e54   at this time.NT
-00000db0: 2901 da07 7061 7265 6e74 73a9 02da 0b62  )...parents....b
-00000dc0: 7563 6b65 745f 6e61 6d65 da0b 6372 6564  ucket_name..cred
-00000dd0: 656e 7469 616c 7329 1b72 1400 0000 7219  entials).r....r.
-00000de0: 0000 0072 0f00 0000 da02 5333 7218 0000  ...r......S3r...
-00000df0: 0072 1000 0000 da06 526f 626f 746f da13  .r......Roboto..
-00000e00: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00000e10: 726f 72da 0870 6174 6873 7065 635a 0850  ror..pathspecZ.P
-00000e20: 6174 6853 7065 63da 0a66 726f 6d5f 6c69  athSpec..from_li
-00000e30: 6e65 73da 0870 6174 7465 726e 735a 1347  nes..patternsZ.G
-00000e40: 6974 5769 6c64 4d61 7463 6850 6174 7465  itWildMatchPatte
-00000e50: 726e da0d 4769 7449 676e 6f72 6553 7065  rn..GitIgnoreSpe
-00000e60: 63da 0669 735f 6469 72da 056d 6b64 6972  c..is_dir..mkdir
-00000e70: da19 6765 745f 7465 6d70 6f72 6172 795f  ..get_temporary_
-00000e80: 6372 6564 656e 7469 616c 7372 0c00 0000  credentialsr....
-00000e90: da08 5265 6164 4f6e 6c79 7215 0000 0072  ..ReadOnlyr....r
-00000ea0: 0900 0000 da06 6275 636b 6574 da0a 6c69  ......bucket..li
-00000eb0: 7374 5f66 696c 6573 da0a 6d61 7463 685f  st_files..match_
-00000ec0: 6669 6c65 da0d 7265 6c61 7469 7665 5f70  file..relative_p
-00000ed0: 6174 68da 0d64 6f77 6e6c 6f61 645f 6669  ath..download_fi
-00000ee0: 6c65 da03 6b65 7929 0a72 3a00 0000 723c  le..key).r:...r<
-00000ef0: 0000 0072 3d00 0000 723e 0000 005a 1469  ...r=...r>...Z.i
-00000f00: 6e63 6c75 6465 5f70 6174 7465 726e 5f73  nclude_pattern_s
-00000f10: 7065 635a 1465 7863 6c75 6465 5f70 6174  pecZ.exclude_pat
-00000f20: 7465 726e 5f73 7065 6372 4300 0000 721e  tern_specrC...r.
-00000f30: 0000 00da 0466 696c 655a 0a6c 6f63 616c  .....fileZ.local
-00000f40: 5f70 6174 6872 2300 0000 7223 0000 0072  _pathr#...r#...r
-00000f50: 2400 0000 da0e 646f 776e 6c6f 6164 5f66  $.....download_f
-00000f60: 696c 6573 6200 0000 734a 0000 000e 180e  ilesb...sJ......
-00000f70: 0102 0202 0104 ff04 0408 0106 0108 0104  ................
-00000f80: ff04 0408 010c 0108 020c 010c 020a 0306  ................
-00000f90: ff02 0204 0102 0104 fe02 fd0c 0808 0104  ................
-00000fa0: 0104 ff02 0302 0108 0104 0104 ff02 0302  ................
-00000fb0: 010a 0210 0104 f37a 1644 6174 6173 6574  .......z.Dataset
-00000fc0: 2e64 6f77 6e6c 6f61 645f 6669 6c65 73da  .download_files.
-00000fd0: 046d 6f64 65da 0663 616c 6c65 7263 0300  .mode..callerc..
-00000fe0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00000ff0: 0000 4300 0000 732e 0000 007c 006a 0064  ..C...s....|.j.d
-00001000: 0075 0073 0a7c 006a 00a0 01a1 0072 147c  .u.s.|.j.....r.|
-00001010: 006a 02a0 037c 006a 047c 017c 02a1 037c  .j...|.j.|.|...|
-00001020: 005f 007c 006a 0053 0072 2000 0000 2905  ._.|.j.S.r ...).
-00001030: 7216 0000 00da 0a69 735f 6578 7069 7265  r......is_expire
-00001040: 6472 1300 0000 724d 0000 0072 1400 0000  dr....rM...r....
-00001050: 2903 723a 0000 0072 5700 0000 7258 0000  ).r:...rW...rX..
-00001060: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00001070: 724d 0000 00a6 0000 0073 0a00 0000 1405  rM.......s......
-00001080: 0601 0801 06ff 0603 7a21 4461 7461 7365  ........z!Datase
-00001090: 742e 6765 745f 7465 6d70 6f72 6172 795f  t.get_temporary_
-000010a0: 6372 6564 656e 7469 616c 7363 0100 0000  credentialsc....
-000010b0: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-000010c0: 6300 0000 7358 0000 0081 007c 006a 00a0  c...sX.....|.j..
-000010d0: 017c 006a 026a 037c 006a 026a 04a1 027d  .|.j.j.|.j.j...}
-000010e0: 0109 007c 016a 0544 005d 077d 0274 067c  ...|.j.D.].}.t.|
-000010f0: 0283 0156 0001 0071 107c 016a 0772 297c  ...V...q.|.j.r)|
-00001100: 006a 00a0 017c 006a 026a 037c 006a 026a  .j...|.j.j.|.j.j
-00001110: 047c 016a 07a1 037d 016e 0264 0053 0071  .|.j...}.n.d.S.q
-00001120: 0d72 2000 0000 2908 7213 0000 0072 5000  .r ...).r....rP.
-00001130: 0000 7214 0000 0072 2600 0000 721a 0000  ..r....r&...r...
-00001140: 0072 3000 0000 7207 0000 0072 3100 0000  .r0...r....r1...
-00001150: 2903 723a 0000 0072 3700 0000 7222 0000  ).r:...r7...r"..
-00001160: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00001170: 7250 0000 00b1 0000 0073 1e00 0000 0280  rP.......s......
-00001180: 0601 0c01 04ff 0203 0a01 0c01 0601 0601  ................
-00001190: 0601 0601 0401 06fd 0406 02f6 7a12 4461  ............z.Da
-000011a0: 7461 7365 742e 6c69 7374 5f66 696c 6573  taset.list_files
-000011b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000011c0: 0002 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
-000011d0: 7c00 6a01 8301 5300 7220 0000 0029 0272  |.j...S.r ...).r
-000011e0: 0500 0000 7214 0000 0029 0172 3a00 0000  ....r....).r:...
-000011f0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00001200: 0774 6f5f 6469 6374 c100 0000 7302 0000  .to_dict....s...
-00001210: 000a 017a 0f44 6174 6173 6574 2e74 6f5f  ...z.Dataset.to_
-00001220: 6469 6374 da0e 6469 7265 6374 6f72 795f  dict..directory_
-00001230: 7061 7468 6303 0000 0000 0000 0000 0000  pathc...........
-00001240: 0003 0000 0006 0000 0003 0000 0073 5c00  .............s\.
-00001250: 0000 7c01 a000 a100 730b 7401 7c01 9b00  ..|.....s.t.|...
-00001260: 6401 9d02 8301 8201 6402 8901 7c02 6402  d.......d...|.d.
-00001270: 7501 7217 7402 6a03 a004 7c02 a101 8901  u.r.t.j...|.....
-00001280: 6403 7405 6a06 6404 7407 6405 6402 6606  d.t.j.d.t.d.d.f.
-00001290: 8700 8701 8702 6603 6406 6407 840c 8900  ......f.d.d.....
-000012a0: 8800 7c01 6408 8302 0100 6402 5300 2909  ..|.d.....d.S.).
-000012b0: 6122 0200 000a 2020 2020 2020 2020 5570  a"....        Up
-000012c0: 6c6f 6164 2065 7665 7279 7468 696e 672c  load everything,
-000012d0: 2072 6563 7572 7369 7665 6c79 2c20 696e   recursively, in
-000012e0: 2064 6972 6563 746f 7279 2c20 6967 6e6f   directory, igno
-000012f0: 7269 6e67 2066 696c 6573 2074 6861 7420  ring files that 
-00001300: 6d61 7463 6820 616e 7920 6f66 2074 6865  match any of the
-00001310: 2069 676e 6f72 6520 7061 7474 6572 6e73   ignore patterns
-00001320: 2e0a 0a20 2020 2020 2020 2060 6578 636c  ...        `excl
-00001330: 7564 655f 7061 7474 6572 6e73 6020 6973  ude_patterns` is
-00001340: 2061 206c 6973 7420 6f66 2067 6974 6967   a list of gitig
-00001350: 6e6f 7265 2d73 7479 6c65 2070 6174 7465  nore-style patte
-00001360: 726e 732e 0a20 2020 2020 2020 2053 6565  rns..        See
-00001370: 2068 7474 7073 3a2f 2f67 6974 2d73 636d   https://git-scm
-00001380: 2e63 6f6d 2f64 6f63 732f 6769 7469 676e  .com/docs/gitign
-00001390: 6f72 6523 5f70 6174 7465 726e 5f66 6f72  ore#_pattern_for
-000013a0: 6d61 742e 0a0a 2020 2020 2020 2020 4578  mat...        Ex
-000013b0: 616d 706c 653a 0a20 2020 2020 2020 2060  ample:.        `
-000013c0: 6060 0a20 2020 2020 2020 2064 6174 6173  ``.        datas
-000013d0: 6574 2e75 706c 6f61 645f 6469 7265 6374  et.upload_direct
-000013e0: 6f72 7928 0a20 2020 2020 2020 2020 2020  ory(.           
-000013f0: 2070 6174 686c 6962 2e50 6174 6828 222f   pathlib.Path("/
-00001400: 7061 7468 2f74 6f2f 6469 7265 6374 6f72  path/to/director
-00001410: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
-00001420: 2065 7863 6c75 6465 5f70 6174 7465 726e   exclude_pattern
-00001430: 733d 5b0a 2020 2020 2020 2020 2020 2020  s=[.            
-00001440: 2020 2020 225f 5f70 7963 6163 6865 5f5f      "__pycache__
-00001450: 2f22 2c0a 2020 2020 2020 2020 2020 2020  /",.            
-00001460: 2020 2020 222a 2e70 7963 222c 0a20 2020      "*.pyc",.   
-00001470: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00001480: 6465 5f6d 6f64 756c 6573 2f22 2c0a 2020  de_modules/",.  
-00001490: 2020 2020 2020 2020 2020 2020 2020 222a                "*
-000014a0: 2a2f 2a2e 6c6f 6722 2c0a 2020 2020 2020  */*.log",.      
-000014b0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-000014c0: 2029 0a20 2020 2020 2020 2060 6060 0a20   ).        ```. 
-000014d0: 2020 2020 2020 207a 1320 6973 206e 6f74         z. is not
-000014e0: 2061 2064 6972 6563 746f 7279 4e72 5b00   a directoryNr[.
-000014f0: 0000 da0a 6b65 795f 7072 6566 6978 721f  ....key_prefixr.
-00001500: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001510: 0300 0000 0700 0000 1300 0000 735e 0000  ............s^..
-00001520: 007c 00a0 00a1 0044 005d 287d 027c 02a0  .|.....D.](}.|..
-00001530: 01a1 0072 1688 007c 027c 019b 0064 017c  ...r...|.|...d.|
-00001540: 026a 029b 009d 0383 0201 0071 0488 0164  .j.........q...d
-00001550: 0075 0172 2088 01a0 037c 02a1 0172 2071  .u.r ....|...r q
-00001560: 0488 02a0 047c 027c 019b 0064 017c 026a  .....|.|...d.|.j
-00001570: 029b 009d 03a1 0201 0071 0464 0053 0029  .........q.d.S.)
-00001580: 024e fa01 2f29 05da 0769 7465 7264 6972  .N../)...iterdir
-00001590: 724b 0000 00da 046e 616d 6572 5100 0000  rK.....namerQ...
-000015a0: da0b 7570 6c6f 6164 5f66 696c 6529 0372  ..upload_file).r
-000015b0: 5b00 0000 725c 0000 00da 0470 6174 68a9  [...r\.....path.
-000015c0: 03da 115f 7570 6c6f 6164 5f64 6972 6563  ..._upload_direc
-000015d0: 746f 7279 5a0c 6578 636c 7564 655f 7370  toryZ.exclude_sp
-000015e0: 6563 723a 0000 0072 2300 0000 7224 0000  ecr:...r#...r$..
-000015f0: 0072 6300 0000 e500 0000 730e 0000 000c  .rc.......s.....
-00001600: 0108 0118 0112 0202 011a 0104 fa7a 3344  .............z3D
-00001610: 6174 6173 6574 2e75 706c 6f61 645f 6469  ataset.upload_di
-00001620: 7265 6374 6f72 792e 3c6c 6f63 616c 733e  rectory.<locals>
-00001630: 2e5f 7570 6c6f 6164 5f64 6972 6563 746f  ._upload_directo
-00001640: 7279 da00 2908 724b 0000 0072 2f00 0000  ry..).rK...r/...
-00001650: 7247 0000 0072 4a00 0000 7248 0000 00da  rG...rJ...rH....
-00001660: 0770 6174 686c 6962 da04 5061 7468 da03  .pathlib..Path..
-00001670: 7374 7229 0372 3a00 0000 725b 0000 0072  str).r:...r[...r
-00001680: 3e00 0000 7223 0000 0072 6200 0000 7224  >...r#...rb...r$
-00001690: 0000 00da 1075 706c 6f61 645f 6469 7265  .....upload_dire
-000016a0: 6374 6f72 79c4 0000 0073 1200 0000 0818  ctory....s......
-000016b0: 0e01 0402 0801 0601 0201 04ff 2004 0e09  ............ ...
-000016c0: 7a18 4461 7461 7365 742e 7570 6c6f 6164  z.Dataset.upload
-000016d0: 5f64 6972 6563 746f 7279 da0f 6c6f 6361  _directory..loca
-000016e0: 6c5f 6669 6c65 5f70 6174 6872 5400 0000  l_file_pathrT...
-000016f0: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
-00001700: 0009 0000 0043 0000 0073 aa00 0000 7c01  .....C...s....|.
-00001710: a000 a100 730b 7401 7c01 9b00 6401 9d02  ....s.t.|...d...
-00001720: 8301 8201 7c00 6a02 6a03 7404 6a05 6b03  ....|.j.j.t.j.k.
-00001730: 7319 7c00 6a02 6a06 7407 6a08 6b03 721d  s.|.j.j.t.j.k.r.
-00001740: 7409 6402 8301 8201 7c00 a00a 740b 6a0c  t.d.....|...t.j.
-00001750: a101 7d03 7c00 6a0d 6403 7501 722b 7c00  ..}.|.j.d.u.r+|.
-00001760: 6a0d 6e06 740e 7c03 6a0f 7c03 6404 8d02  j.n.t.|.j.|.d...
-00001770: 7d04 7c03 6a10 9b00 6405 7c02 a011 6405  }.|.j...d.|...d.
-00001780: a101 9b00 9d03 7d02 7c04 6a12 7c01 7c02  ......}.|.j.|.|.
-00001790: 7413 6a14 7c00 6a02 6a15 7413 6a16 7c00  t.j.|.j.j.t.j.|.
-000017a0: 6a02 6a17 7413 6a18 7c03 6a10 6903 6406  j.j.t.j.|.j.i.d.
-000017b0: 8d03 0100 6403 5300 2907 611c 0100 000a  ....d.S.).a.....
-000017c0: 2020 2020 2020 2020 5570 6c6f 6164 7320          Uploads 
-000017d0: 6120 6669 6c65 2074 6f20 7468 6520 6461  a file to the da
-000017e0: 7461 7365 7427 7320 7374 6f72 6167 6520  taset's storage 
-000017f0: 6c6f 6361 7469 6f6e 2e0a 0a20 2020 2020  location...     
-00001800: 2020 203a 7061 7261 6d20 6669 6c65 5f70     :param file_p
-00001810: 6174 683a 2054 6865 2070 6174 6820 746f  ath: The path to
-00001820: 2074 6865 2066 696c 6520 746f 2075 706c   the file to upl
-00001830: 6f61 642e 0a20 2020 2020 2020 203a 7061  oad..        :pa
-00001840: 7261 6d20 6b65 793a 2054 6865 206b 6579  ram key: The key
-00001850: 2074 6f20 7573 6520 666f 7220 7468 6520   to use for the 
-00001860: 6669 6c65 2069 6e20 7468 6520 6461 7461  file in the data
-00001870: 7365 7427 7320 7374 6f72 6167 6520 6c6f  set's storage lo
-00001880: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
-00001890: 2020 2020 2020 2020 2020 2020 4974 2077              It w
-000018a0: 696c 6c20 6265 2070 7265 6669 7865 6420  ill be prefixed 
-000018b0: 7769 7468 2074 6865 2064 6174 6173 6574  with the dataset
-000018c0: 2773 2073 746f 7261 6765 2070 7265 6669  's storage prefi
-000018d0: 782e 0a20 2020 2020 2020 207a 0e20 6973  x..        z. is
-000018e0: 206e 6f74 2061 2066 696c 6572 3f00 0000   not a filer?...
-000018f0: 4e72 4100 0000 725d 0000 0029 0172 1d00  NrA...r]...).r..
-00001900: 0000 2919 da07 6973 5f66 696c 6572 2f00  ..)...is_filer/.
-00001910: 0000 7214 0000 0072 1900 0000 720f 0000  ..r....r....r...
-00001920: 0072 4400 0000 7218 0000 0072 1000 0000  .rD...r....r....
-00001930: 7245 0000 0072 4600 0000 724d 0000 0072  rE...rF...rM...r
-00001940: 0c00 0000 5a09 5265 6164 5772 6974 6572  ....Z.ReadWriter
-00001950: 1500 0000 7209 0000 0072 4f00 0000 5a0f  ....r....rO...Z.
-00001960: 7265 7175 6972 6564 5f70 7265 6669 78da  required_prefix.
-00001970: 066c 7374 7269 7072 6000 0000 720a 0000  .lstripr`...r...
-00001980: 005a 0944 6174 6173 6574 4964 7226 0000  .Z.DatasetIdr&..
-00001990: 005a 054f 7267 4964 721a 0000 005a 0c43  .Z.OrgIdr....Z.C
-000019a0: 6f6d 6d6f 6e50 7265 6669 7829 0572 3a00  ommonPrefix).r:.
-000019b0: 0000 7269 0000 0072 5400 0000 7243 0000  ..ri...rT...rC..
-000019c0: 0072 1e00 0000 7223 0000 0072 2300 0000  .r....r#...r#...
-000019d0: 7224 0000 0072 6000 0000 f000 0000 7330  r$...r`.......s0
-000019e0: 0000 0008 0c0e 010e 030e 0102 0202 0104  ................
-000019f0: ff0c 040a 0306 ff02 0204 0102 0104 fe02  ................
-00001a00: fd16 0804 0102 0102 010a 020a 0108 0102  ................
-00001a10: fd0a fd7a 1344 6174 6173 6574 2e75 706c  ...z.Dataset.upl
-00001a20: 6f61 645f 6669 6c65 2902 4e4e 7220 0000  oad_file).NNr ..
-00001a30: 0029 26da 085f 5f6e 616d 655f 5fda 0a5f  .)&..__name__.._
-00001a40: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001a50: 6c6e 616d 655f 5f72 0e00 0000 da0f 5f5f  lname__r......__
-00001a60: 616e 6e6f 7461 7469 6f6e 735f 5f72 1100  annotations__r..
-00001a70: 0000 7215 0000 0072 0300 0000 7208 0000  ..r....r....r...
-00001a80: 0072 1600 0000 720d 0000 00da 0b63 6c61  .r....r......cla
-00001a90: 7373 6d65 7468 6f64 7210 0000 0072 4500  ssmethodr....rE.
-00001aa0: 0000 720f 0000 0072 4400 0000 7267 0000  ..r....rD...rg..
-00001ab0: 00da 0464 6963 7472 0200 0000 da04 6c69  ...dictr......li
-00001ac0: 7374 7225 0000 0072 2700 0000 da0b 636f  str%...r'.....co
-00001ad0: 6c6c 6563 7469 6f6e 73da 0361 6263 da09  llections..abc..
-00001ae0: 4765 6e65 7261 746f 7272 3800 0000 723b  Generatorr8...r;
-00001af0: 0000 0072 6500 0000 7266 0000 0072 5600  ...re...rf...rV.
-00001b00: 0000 720c 0000 0072 4e00 0000 724d 0000  ..r....rN...rM..
-00001b10: 0072 0700 0000 7250 0000 0072 5a00 0000  .r....rP...rZ...
-00001b20: 7268 0000 0072 6000 0000 7223 0000 0072  rh...r`...r#...r
-00001b30: 2300 0000 7223 0000 0072 2400 0000 7212  #...r#...r$...r.
-00001b40: 0000 0017 0000 0073 d600 0000 0a00 0801  .......s........
-00001b50: 0801 1001 1001 0202 0404 0401 0201 0201  ................
-00001b60: 0201 0201 0201 04f7 0202 02fe 0203 02fd  ................
-00001b70: 0204 02fc 0605 02fb 0606 02fa 0e07 02f9  ................
-00001b80: 0a08 02f8 0609 02f7 020a 0cf6 0210 0205  ................
-00001b90: 0201 04fb 0202 02fe 0203 02fd 0604 02fc  ................
-00001ba0: 0605 02fb 0206 0cfa 020a 0205 0201 04fb  ................
-00001bb0: 0a02 02fe 0203 02fd 0604 02fc 0605 02fb  ................
-00001bc0: 0a06 0cfa 0222 04fc 0202 02fe 0203 02fd  ....."..........
-00001bd0: 0604 02fc 0205 0afb 020d 0201 04fc 0402  ................
-00001be0: 02fe 0a03 02fd 0a04 02fc 0205 0afb 0446  ...............F
-00001bf0: 0201 04fd 0202 02fe 0603 02fd 0204 0afc  ................
-00001c00: 1c0b 1610 0206 04fd 0402 02fe 0a03 02fd  ................
-00001c10: 0204 0afc 022c 0402 02fe 0203 02fd 0204  .....,..........
-00001c20: 0efc 7212 0000 0029 17da 0f63 6f6c 6c65  ..r....)...colle
-00001c30: 6374 696f 6e73 2e61 6263 7273 0000 0072  ctions.abcrs...r
-00001c40: 6500 0000 da06 7479 7069 6e67 7202 0000  e.....typingr...
-00001c50: 0072 0300 0000 7247 0000 00da 0573 6572  .r....rG.....ser
-00001c60: 6465 7205 0000 00da 0566 696c 6573 7207  der......filesr.
-00001c70: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00001c80: 0000 7239 0000 0072 0c00 0000 720d 0000  ..r9...r....r...
-00001c90: 0072 0e00 0000 720f 0000 0072 2200 0000  .r....r....r"...
-00001ca0: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00001cb0: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
-00001cc0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001cd0: 0073 1200 0000 0800 0801 1001 0802 0c02  .s..............
-00001ce0: 1801 1806 1006 1203                      ........
+00000320: 6424 8405 5a20 0903 0903 6430 641d 6507  d$..Z ....d0d.e.
+00000330: 6513 6510 1900 1900 641e 6507 6513 6510  e.e.....d.e.e.e.
+00000340: 1900 1900 640e 6516 6a17 6a18 6521 6403  ....d.e.j.j.e!d.
+00000350: 6403 6603 1900 6606 6425 6426 8405 5a22  d.f...f.d%d&..Z"
+00000360: 640e 6511 6510 6512 6602 1900 6602 6427  d.e.e.e.f...f.d'
+00000370: 6428 8404 5a23 0903 6431 6429 651b 6a1c  d(..Z#..d1d)e.j.
+00000380: 641e 6507 6513 6510 1900 1900 640e 6403  d.e.e.e.....d.d.
+00000390: 6606 642a 642b 8405 5a24 642c 651b 6a1c  f.d*d+..Z$d,e.j.
+000003a0: 642d 6510 640e 6403 6606 642e 642f 8404  d-e.d.d.f.d.d/..
+000003b0: 5a25 6403 5300 2932 da07 4461 7461 7365  Z%d.S.)2..Datase
+000003c0: 74da 125f 4461 7461 7365 745f 5f64 656c  t.._Dataset__del
+000003d0: 6567 6174 65da 105f 4461 7461 7365 745f  egate.._Dataset_
+000003e0: 5f72 6563 6f72 644e da18 5f44 6174 6173  _recordN.._Datas
+000003f0: 6574 5f5f 6669 6c65 735f 6465 6c65 6761  et__files_delega
+00000400: 7465 da1a 5f44 6174 6173 6574 5f5f 7465  te.._Dataset__te
+00000410: 6d70 5f63 7265 6465 6e74 6961 6c73 da10  mp_credentials..
+00000420: 6461 7461 7365 745f 6465 6c65 6761 7465  dataset_delegate
+00000430: da0d 6164 6d69 6e69 7374 7261 746f 72da  ..administrator.
+00000440: 1073 746f 7261 6765 5f6c 6f63 6174 696f  .storage_locatio
+00000450: 6eda 066f 7267 5f69 64da 0a63 7265 6174  n..org_id..creat
+00000460: 6564 5f62 79da 086d 6574 6164 6174 61da  ed_by..metadata.
+00000470: 0474 6167 73da 0e66 696c 6573 5f64 656c  .tags..files_del
+00000480: 6567 6174 65da 0672 6574 7572 6e63 0900  egate..returnc..
+00000490: 0000 0000 0000 0000 0000 0a00 0000 0800  ................
+000004a0: 0000 4300 0000 7320 0000 007c 01a0 007c  ..C...s ...|...|
+000004b0: 027c 067c 037c 077c 047c 05a1 067d 097c  .|.|.|.|.|...}.|
+000004c0: 007c 097c 017c 0883 0353 00a9 014e 2901  .|.|.|...S...N).
+000004d0: 5a0e 6372 6561 7465 5f64 6174 6173 6574  Z.create_dataset
+000004e0: 290a da03 636c 7372 1700 0000 7218 0000  )...clsr....r...
+000004f0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000500: 721c 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+00000510: 0672 6563 6f72 64a9 0072 2300 0000 faef  .record..r#.....
+00000520: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
+00000530: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000540: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
+00000550: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
+00000560: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+00000570: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
+00000580: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
+00000590: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
+000005a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
+000005b0: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
+000005c0: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
+000005d0: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
+000005e0: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
+000005f0: 5f73 646b 2f64 6f6d 6169 6e2f 6461 7461  _sdk/domain/data
+00000600: 7365 7473 2f64 6174 6173 6574 2e70 79da  sets/dataset.py.
+00000610: 0663 7265 6174 651d 0000 0073 0800 0000  .create....s....
+00000620: 040c 0c01 04ff 0c03 7a0e 4461 7461 7365  ........z.Datase
+00000630: 742e 6372 6561 7465 da0a 6461 7461 7365  t.create..datase
+00000640: 745f 6964 6305 0000 0000 0000 0000 0000  t_idc...........
+00000650: 0006 0000 0004 0000 0043 0000 0073 1800  .........C...s..
+00000660: 0000 7c02 a000 7c01 7c03 a102 7d05 7c00  ..|...|.|...}.|.
+00000670: 7c05 7c02 7c04 8303 5300 7220 0000 0029  |.|.|...S.r ...)
+00000680: 015a 1a67 6574 5f64 6174 6173 6574 5f62  .Z.get_dataset_b
+00000690: 795f 7072 696d 6172 795f 6b65 7929 0672  y_primary_key).r
+000006a0: 2100 0000 7226 0000 0072 1700 0000 721a  !...r&...r....r.
+000006b0: 0000 0072 1e00 0000 7222 0000 0072 2300  ...r....r"...r#.
+000006c0: 0000 7223 0000 0072 2400 0000 da07 6672  ..r#...r$.....fr
+000006d0: 6f6d 5f69 642e 0000 0073 0400 0000 0c08  om_id....s......
+000006e0: 0c01 7a0f 4461 7461 7365 742e 6672 6f6d  ..z.Dataset.from
+000006f0: 5f69 64da 0766 696c 7465 7273 2903 7212  _id..filters).r.
+00000700: 0000 004e 4e63 0500 0000 0000 0000 0000  ...NNc..........
+00000710: 0000 0c00 0000 0600 0000 6300 0000 73a2  ..........c...s.
+00000720: 0000 0081 0074 0074 016a 02a0 03a1 0083  .....t.t.j......
+00000730: 017d 0574 007c 01a0 03a1 0083 017d 067c  .}.t.|.......}.|
+00000740: 067c 0518 007d 077c 0772 2c74 047c 0783  .|...}.|.r,t.|..
+00000750: 0164 016b 047d 087c 0872 1e64 026e 0164  .d.k.}.|.r.d.n.d
+00000760: 037d 0974 057c 079b 0064 047c 099b 0064  .}.t.|...d.|...d
+00000770: 057c 059b 009d 0583 0182 017c 026a 067c  .|.........|.j.|
+00000780: 017c 0464 068d 027d 0a09 007c 0a6a 0744  .|.d...}...|.j.D
+00000790: 005d 097d 0b7c 007c 0b7c 027c 0383 0356  .].}.|.|.|.|...V
+000007a0: 0001 0071 377c 0a6a 0872 4e7c 026a 067c  ...q7|.j.rN|.j.|
+000007b0: 017c 047c 0a6a 0864 088d 037d 0a6e 0264  .|.|.j.d...}.n.d
+000007c0: 0053 0071 3429 094e 720b 0000 007a 2361  .S.q4).Nr....z#a
+000007d0: 7265 206e 6f74 206b 6e6f 776e 2061 7474  re not known att
+000007e0: 7269 6275 7465 7320 6f66 2044 6174 6173  ributes of Datas
+000007f0: 6574 7a23 6973 206e 6f74 2061 206b 6e6f  etz#is not a kno
+00000800: 776e 2061 7474 7269 6275 7465 206f 6620  wn attribute of 
+00000810: 4461 7461 7365 74da 0120 7a14 2e20 4b6e  Dataset.. z.. Kn
+00000820: 6f77 6e20 6174 7472 6962 7574 6573 3a20  own attributes: 
+00000830: 2901 721a 0000 0054 2902 721a 0000 00da  ).r....T).r.....
+00000840: 0a70 6167 655f 746f 6b65 6e29 09da 0373  .page_token)...s
+00000850: 6574 7211 0000 00da 0a5f 5f66 6965 6c64  etr......__field
+00000860: 735f 5fda 046b 6579 73da 036c 656e da0a  s__..keys..len..
+00000870: 5661 6c75 6545 7272 6f72 5a0e 7175 6572  ValueErrorZ.quer
+00000880: 795f 6461 7461 7365 7473 da05 6974 656d  y_datasets..item
+00000890: 73da 0a6e 6578 745f 746f 6b65 6e29 0c72  s..next_token).r
+000008a0: 2100 0000 7228 0000 0072 1700 0000 721e  !...r(...r....r.
+000008b0: 0000 0072 1a00 0000 da0a 6b6e 6f77 6e5f  ...r......known_
+000008c0: 6b65 7973 da0b 6163 7475 616c 5f6b 6579  keys..actual_key
+000008d0: 73da 0c75 6e6b 6e6f 776e 5f6b 6579 73da  s..unknown_keys.
+000008e0: 0670 6c75 7261 6cda 036d 7367 da11 7061  .plural..msg..pa
+000008f0: 6769 6e61 7465 645f 7265 7375 6c74 7372  ginated_resultsr
+00000900: 2200 0000 7223 0000 0072 2300 0000 7224  "...r#...r#...r$
+00000910: 0000 00da 0571 7565 7279 3900 0000 732a  .....query9...s*
+00000920: 0000 0002 800e 080c 0108 0104 010c 0102  ................
+00000930: 0306 ff02 0202 fd18 050e 0202 010a 0110  ................
+00000940: 0106 0104 0108 0108 ff04 0402 f87a 0d44  .............z.D
+00000950: 6174 6173 6574 2e71 7565 7279 7222 0000  ataset.queryr"..
+00000960: 00da 0864 656c 6567 6174 6563 0400 0000  ...delegatec....
+00000970: 0000 0000 0000 0000 0400 0000 0200 0000  ................
+00000980: 4300 0000 7316 0000 007c 027c 005f 007c  C...s....|.|._.|
+00000990: 037c 005f 017c 017c 005f 0264 0053 0072  .|._.|.|._.d.S.r
+000009a0: 2000 0000 2903 7213 0000 0072 1500 0000   ...).r....r....
+000009b0: 7214 0000 0029 04da 0473 656c 6672 2200  r....)...selfr".
+000009c0: 0000 7239 0000 0072 1e00 0000 7223 0000  ..r9...r....r#..
+000009d0: 0072 2300 0000 7224 0000 00da 085f 5f69  .r#...r$.....__i
+000009e0: 6e69 745f 5f58 0000 0073 0600 0000 0606  nit__X...s......
+000009f0: 0601 0a01 7a10 4461 7461 7365 742e 5f5f  ....z.Dataset.__
+00000a00: 696e 6974 5f5f da08 6f75 745f 7061 7468  init__..out_path
+00000a10: da10 696e 636c 7564 655f 7061 7474 6572  ..include_patter
+00000a20: 6e73 da10 6578 636c 7564 655f 7061 7474  ns..exclude_patt
+00000a30: 6572 6e73 6304 0000 0000 0000 0000 0000  ernsc...........
+00000a40: 0008 0000 0005 0000 0043 0000 0073 9000  .........C...s..
+00000a50: 0000 7c00 6a00 6a01 7402 6a03 6b03 730e  ..|.j.j.t.j.k.s.
+00000a60: 7c00 6a00 6a04 7405 6a06 6b03 7212 7407  |.j.j.t.j.k.r.t.
+00000a70: 6401 8301 8201 7c01 a008 a100 731c 7c01  d.....|.....s.|.
+00000a80: 6a09 6402 6403 8d01 0100 7c00 a00a 740b  j.d.d.....|...t.
+00000a90: 6a0c a101 7d04 7c00 6a0d 6404 7501 722a  j...}.|.j.d.u.r*
+00000aa0: 7c00 6a0d 6e06 740e 7c04 6a0f 7c04 6405  |.j.n.t.|.j.|.d.
+00000ab0: 8d02 7d05 7c00 a010 7c02 7c03 a102 4400  ..}.|...|.|...D.
+00000ac0: 5d0e 7d06 7c01 7c06 6a11 1b00 7d07 7c05  ].}.|.|.j...}.|.
+00000ad0: a012 7c06 6a13 7c07 a102 0100 7137 6404  ..|.j.|.....q7d.
+00000ae0: 5300 2906 613f 0200 000a 2020 2020 2020  S.).a?....      
+00000af0: 2020 446f 776e 6c6f 6164 2066 696c 6573    Download files
+00000b00: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00000b10: 2074 6869 7320 6461 7461 7365 7420 746f   this dataset to
+00000b20: 2074 6865 2067 6976 656e 2064 6972 6563   the given direc
+00000b30: 746f 7279 2e0a 2020 2020 2020 2020 4966  tory..        If
+00000b40: 2060 6f75 745f 7061 7468 6020 646f 6573   `out_path` does
+00000b50: 206e 6f74 2065 7869 7374 2c20 6974 2077   not exist, it w
+00000b60: 696c 6c20 6265 2063 7265 6174 6564 2e0a  ill be created..
+00000b70: 0a20 2020 2020 2020 2060 696e 636c 7564  .        `includ
+00000b80: 655f 7061 7474 6572 6e73 6020 616e 6420  e_patterns` and 
+00000b90: 6065 7863 6c75 6465 5f70 6174 7465 726e  `exclude_pattern
+00000ba0: 7360 2061 7265 206c 6973 7473 206f 6620  s` are lists of 
+00000bb0: 6769 7469 676e 6f72 652d 7374 796c 6520  gitignore-style 
+00000bc0: 7061 7474 6572 6e73 2e0a 2020 2020 2020  patterns..      
+00000bd0: 2020 5365 6520 6874 7470 733a 2f2f 6769    See https://gi
+00000be0: 742d 7363 6d2e 636f 6d2f 646f 6373 2f67  t-scm.com/docs/g
+00000bf0: 6974 6967 6e6f 7265 2e0a 0a20 2020 2020  itignore...     
+00000c00: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
+00000c10: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000c20: 6461 7461 7365 7420 3d20 6461 7461 7365  dataset = datase
+00000c30: 7473 2e44 6174 6173 6574 2e62 795f 6964  ts.Dataset.by_id
+00000c40: 2822 3c64 6174 6173 6574 5f69 643e 222c  ("<dataset_id>",
+00000c50: 2064 6174 6173 6574 5f64 656c 6567 6174   dataset_delegat
+00000c60: 6529 0a20 2020 2020 2020 2064 6174 6173  e).        datas
+00000c70: 6574 2e64 6f77 6e6c 6f61 645f 6669 6c65  et.download_file
+00000c80: 7328 0a20 2020 2020 2020 2020 2020 2070  s(.            p
+00000c90: 6174 686c 6962 2e50 6174 6828 222f 746d  athlib.Path("/tm
+00000ca0: 702f 746d 702e 6e56 3167 6457 3557 4856  p/tmp.nV1gdW5WHV
+00000cb0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00000cc0: 696e 636c 7564 655f 7061 7474 6572 6e73  include_patterns
+00000cd0: 3d5b 222a 2a2f 2a2e 6734 225d 2c0a 2020  =["**/*.g4"],.  
+00000ce0: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
+00000cf0: 655f 7061 7474 6572 6e73 3d5b 222a 2a2f  e_patterns=["**/
+00000d00: 7465 7374 2f2a 2a22 5d0a 2020 2020 2020  test/**"].      
+00000d10: 2020 290a 2020 2020 2020 2020 6060 600a    ).        ```.
+00000d20: 2020 2020 2020 2020 fa48 4f6e 6c79 2053          .HOnly S
+00000d30: 332d 6261 636b 6564 2073 746f 7261 6765  3-backed storage
+00000d40: 2061 646d 696e 6973 7465 7265 6420 6279   administered by
+00000d50: 2052 6f62 6f74 6f20 6973 2073 7570 706f   Roboto is suppo
+00000d60: 7274 6564 2061 7420 7468 6973 2074 696d  rted at this tim
+00000d70: 652e 5429 01da 0770 6172 656e 7473 4ea9  e.T)...parentsN.
+00000d80: 02da 0b62 7563 6b65 745f 6e61 6d65 da0b  ...bucket_name..
+00000d90: 6372 6564 656e 7469 616c 7329 1472 1400  credentials).r..
+00000da0: 0000 7219 0000 0072 0f00 0000 da02 5333  ..r....r......S3
+00000db0: 7218 0000 0072 1000 0000 da06 526f 626f  r....r......Robo
+00000dc0: 746f da13 4e6f 7449 6d70 6c65 6d65 6e74  to..NotImplement
+00000dd0: 6564 4572 726f 72da 0669 735f 6469 72da  edError..is_dir.
+00000de0: 056d 6b64 6972 da19 6765 745f 7465 6d70  .mkdir..get_temp
+00000df0: 6f72 6172 795f 6372 6564 656e 7469 616c  orary_credential
+00000e00: 7372 0c00 0000 da08 5265 6164 4f6e 6c79  sr......ReadOnly
+00000e10: 7215 0000 0072 0900 0000 da06 6275 636b  r....r......buck
+00000e20: 6574 da0a 6c69 7374 5f66 696c 6573 da0d  et..list_files..
+00000e30: 7265 6c61 7469 7665 5f70 6174 68da 0d64  relative_path..d
+00000e40: 6f77 6e6c 6f61 645f 6669 6c65 da03 6b65  ownload_file..ke
+00000e50: 7929 0872 3a00 0000 723c 0000 0072 3d00  y).r:...r<...r=.
+00000e60: 0000 723e 0000 0072 4300 0000 721e 0000  ..r>...rC...r...
+00000e70: 00da 0466 696c 655a 0a6c 6f63 616c 5f70  ...fileZ.local_p
+00000e80: 6174 6872 2300 0000 7223 0000 0072 2400  athr#...r#...r$.
+00000e90: 0000 da0e 646f 776e 6c6f 6164 5f66 696c  ....download_fil
+00000ea0: 6573 6200 0000 7326 0000 000e 180e 0102  esb...s&........
+00000eb0: 0202 0104 ff08 040c 010c 020a 0306 ff02  ................
+00000ec0: 0204 0102 0104 fe02 fd10 080a 0110 0104  ................
+00000ed0: fe7a 1644 6174 6173 6574 2e64 6f77 6e6c  .z.Dataset.downl
+00000ee0: 6f61 645f 6669 6c65 73da 046d 6f64 65da  oad_files..mode.
+00000ef0: 0663 616c 6c65 7263 0300 0000 0000 0000  .callerc........
+00000f00: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+00000f10: 732e 0000 007c 006a 0064 0075 0073 0a7c  s....|.j.d.u.s.|
+00000f20: 006a 00a0 01a1 0072 147c 006a 02a0 037c  .j.....r.|.j...|
+00000f30: 006a 047c 017c 02a1 037c 005f 007c 006a  .j.|.|...|._.|.j
+00000f40: 0053 0072 2000 0000 2905 7216 0000 00da  .S.r ...).r.....
+00000f50: 0a69 735f 6578 7069 7265 6472 1300 0000  .is_expiredr....
+00000f60: 7249 0000 0072 1400 0000 2903 723a 0000  rI...r....).r:..
+00000f70: 0072 5200 0000 7253 0000 0072 2300 0000  .rR...rS...r#...
+00000f80: 7223 0000 0072 2400 0000 7249 0000 0091  r#...r$...rI....
+00000f90: 0000 0073 0a00 0000 1405 0601 0801 06ff  ...s............
+00000fa0: 0603 7a21 4461 7461 7365 742e 6765 745f  ..z!Dataset.get_
+00000fb0: 7465 6d70 6f72 6172 795f 6372 6564 656e  temporary_creden
+00000fc0: 7469 616c 7363 0300 0000 0000 0000 0000  tialsc..........
+00000fd0: 0000 0800 0000 0500 0000 6300 0000 73ba  ..........c...s.
+00000fe0: 0000 0081 0064 017d 037c 0164 0175 0172  .....d.}.|.d.u.r
+00000ff0: 1074 006a 01a0 0274 006a 036a 047c 01a1  .t.j...t.j.j.|..
+00001000: 027d 0364 017d 047c 0264 0175 0172 1c74  .}.d.}.|.d.u.r.t
+00001010: 006a 05a0 027c 02a1 017d 047c 006a 06a0  .j...|...}.|.j..
+00001020: 077c 006a 086a 097c 006a 086a 0aa1 027d  .|.j.j.|.j.j...}
+00001030: 0509 007c 056a 0b44 005d 1d7d 0674 0c7c  ...|.j.D.].}.t.|
+00001040: 0683 017d 077c 0372 3b7c 03a0 0d7c 076a  ...}.|.r;|...|.j
+00001050: 0ea1 0173 3b09 0071 2b7c 0472 457c 04a0  ...s;..q+|.rE|..
+00001060: 0d7c 076a 0ea1 0172 4509 0071 2b7c 0756  .|.j...rE..q+|.V
+00001070: 0001 0071 2b7c 056a 0f72 5a7c 006a 06a0  ...q+|.j.rZ|.j..
+00001080: 077c 006a 086a 097c 006a 086a 0a7c 056a  .|.j.j.|.j.j.|.j
+00001090: 0fa1 037d 056e 0264 0153 0071 2829 027a  ...}.n.d.S.q().z
+000010a0: 920a 2020 2020 2020 2020 6069 6e63 6c75  ..        `inclu
+000010b0: 6465 5f70 6174 7465 726e 7360 2061 6e64  de_patterns` and
+000010c0: 2060 6578 636c 7564 655f 7061 7474 6572   `exclude_patter
+000010d0: 6e73 6020 6172 6520 6c69 7374 7320 6f66  ns` are lists of
+000010e0: 2067 6974 6967 6e6f 7265 2d73 7479 6c65   gitignore-style
+000010f0: 2070 6174 7465 726e 732e 0a20 2020 2020   patterns..     
+00001100: 2020 2053 6565 2068 7474 7073 3a2f 2f67     See https://g
+00001110: 6974 2d73 636d 2e63 6f6d 2f64 6f63 732f  it-scm.com/docs/
+00001120: 6769 7469 676e 6f72 652e 0a20 2020 2020  gitignore..     
+00001130: 2020 204e 2910 da08 7061 7468 7370 6563     N)...pathspec
+00001140: 5a08 5061 7468 5370 6563 da0a 6672 6f6d  Z.PathSpec..from
+00001150: 5f6c 696e 6573 da08 7061 7474 6572 6e73  _lines..patterns
+00001160: 5a13 4769 7457 696c 644d 6174 6368 5061  Z.GitWildMatchPa
+00001170: 7474 6572 6eda 0d47 6974 4967 6e6f 7265  ttern..GitIgnore
+00001180: 5370 6563 7213 0000 0072 4c00 0000 7214  Specr....rL...r.
+00001190: 0000 0072 2600 0000 721a 0000 0072 3000  ...r&...r....r0.
+000011a0: 0000 7207 0000 00da 0a6d 6174 6368 5f66  ..r......match_f
+000011b0: 696c 6572 4d00 0000 7231 0000 0029 0872  ilerM...r1...).r
+000011c0: 3a00 0000 723d 0000 0072 3e00 0000 5a14  :...r=...r>...Z.
+000011d0: 696e 636c 7564 655f 7061 7474 6572 6e5f  include_pattern_
+000011e0: 7370 6563 5a14 6578 636c 7564 655f 7061  specZ.exclude_pa
+000011f0: 7474 6572 6e5f 7370 6563 7237 0000 0072  ttern_specr7...r
+00001200: 2200 0000 7250 0000 0072 2300 0000 7223  "...rP...r#...r#
+00001210: 0000 0072 2400 0000 724c 0000 009c 0000  ...r$...rL......
+00001220: 0073 4400 0000 0280 0409 0801 0601 0801  .sD.............
+00001230: 04ff 0404 0801 0c01 0602 0c01 04ff 0203  ................
+00001240: 0a01 0801 0801 0401 04ff 0203 0201 0801  ................
+00001250: 0401 04ff 0203 0201 0801 0601 0601 0601  ................
+00001260: 0601 0401 06fd 0406 02eb 7a12 4461 7461  ..........z.Data
+00001270: 7365 742e 6c69 7374 5f66 696c 6573 6301  set.list_filesc.
+00001280: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00001290: 0000 0043 0000 0073 0a00 0000 7400 7c00  ...C...s....t.|.
+000012a0: 6a01 8301 5300 7220 0000 0029 0272 0500  j...S.r ...).r..
+000012b0: 0000 7214 0000 0029 0172 3a00 0000 7223  ..r....).r:...r#
+000012c0: 0000 0072 2300 0000 7224 0000 00da 0774  ...r#...r$.....t
+000012d0: 6f5f 6469 6374 c900 0000 7302 0000 000a  o_dict....s.....
+000012e0: 017a 0f44 6174 6173 6574 2e74 6f5f 6469  .z.Dataset.to_di
+000012f0: 6374 da0e 6469 7265 6374 6f72 795f 7061  ct..directory_pa
+00001300: 7468 6303 0000 0000 0000 0000 0000 0003  thc.............
+00001310: 0000 0006 0000 0003 0000 0073 5c00 0000  ...........s\...
+00001320: 7c01 a000 a100 730b 7401 7c01 9b00 6401  |.....s.t.|...d.
+00001330: 9d02 8301 8201 6402 8901 7c02 6402 7501  ......d...|.d.u.
+00001340: 7217 7402 6a03 a004 7c02 a101 8901 6403  r.t.j...|.....d.
+00001350: 7405 6a06 6404 7407 6405 6402 6606 8700  t.j.d.t.d.d.f...
+00001360: 8701 8702 6603 6406 6407 840c 8900 8800  ....f.d.d.......
+00001370: 7c01 6408 8302 0100 6402 5300 2909 6122  |.d.....d.S.).a"
+00001380: 0200 000a 2020 2020 2020 2020 5570 6c6f  ....        Uplo
+00001390: 6164 2065 7665 7279 7468 696e 672c 2072  ad everything, r
+000013a0: 6563 7572 7369 7665 6c79 2c20 696e 2064  ecursively, in d
+000013b0: 6972 6563 746f 7279 2c20 6967 6e6f 7269  irectory, ignori
+000013c0: 6e67 2066 696c 6573 2074 6861 7420 6d61  ng files that ma
+000013d0: 7463 6820 616e 7920 6f66 2074 6865 2069  tch any of the i
+000013e0: 676e 6f72 6520 7061 7474 6572 6e73 2e0a  gnore patterns..
+000013f0: 0a20 2020 2020 2020 2060 6578 636c 7564  .        `exclud
+00001400: 655f 7061 7474 6572 6e73 6020 6973 2061  e_patterns` is a
+00001410: 206c 6973 7420 6f66 2067 6974 6967 6e6f   list of gitigno
+00001420: 7265 2d73 7479 6c65 2070 6174 7465 726e  re-style pattern
+00001430: 732e 0a20 2020 2020 2020 2053 6565 2068  s..        See h
+00001440: 7474 7073 3a2f 2f67 6974 2d73 636d 2e63  ttps://git-scm.c
+00001450: 6f6d 2f64 6f63 732f 6769 7469 676e 6f72  om/docs/gitignor
+00001460: 6523 5f70 6174 7465 726e 5f66 6f72 6d61  e#_pattern_forma
+00001470: 742e 0a0a 2020 2020 2020 2020 4578 616d  t...        Exam
+00001480: 706c 653a 0a20 2020 2020 2020 2060 6060  ple:.        ```
+00001490: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
+000014a0: 2e75 706c 6f61 645f 6469 7265 6374 6f72  .upload_director
+000014b0: 7928 0a20 2020 2020 2020 2020 2020 2070  y(.            p
+000014c0: 6174 686c 6962 2e50 6174 6828 222f 7061  athlib.Path("/pa
+000014d0: 7468 2f74 6f2f 6469 7265 6374 6f72 7922  th/to/directory"
+000014e0: 292c 0a20 2020 2020 2020 2020 2020 2065  ),.            e
+000014f0: 7863 6c75 6465 5f70 6174 7465 726e 733d  xclude_patterns=
+00001500: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00001510: 2020 225f 5f70 7963 6163 6865 5f5f 2f22    "__pycache__/"
+00001520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001530: 2020 222a 2e70 7963 222c 0a20 2020 2020    "*.pyc",.     
+00001540: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
+00001550: 5f6d 6f64 756c 6573 2f22 2c0a 2020 2020  _modules/",.    
+00001560: 2020 2020 2020 2020 2020 2020 222a 2a2f              "**/
+00001570: 2a2e 6c6f 6722 2c0a 2020 2020 2020 2020  *.log",.        
+00001580: 2020 2020 5d2c 0a20 2020 2020 2020 2029      ],.        )
+00001590: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+000015a0: 2020 2020 207a 1320 6973 206e 6f74 2061       z. is not a
+000015b0: 2064 6972 6563 746f 7279 4e72 5b00 0000   directoryNr[...
+000015c0: da0a 6b65 795f 7072 6566 6978 721f 0000  ..key_prefixr...
+000015d0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+000015e0: 0000 0700 0000 1300 0000 735e 0000 007c  ..........s^...|
+000015f0: 00a0 00a1 0044 005d 287d 027c 02a0 01a1  .....D.](}.|....
+00001600: 0072 1688 007c 027c 019b 0064 017c 026a  .r...|.|...d.|.j
+00001610: 029b 009d 0383 0201 0071 0488 0164 0075  .........q...d.u
+00001620: 0172 2088 01a0 037c 02a1 0172 2071 0488  .r ....|...r q..
+00001630: 02a0 047c 027c 019b 0064 017c 026a 029b  ...|.|...d.|.j..
+00001640: 009d 03a1 0201 0071 0464 0053 0029 024e  .......q.d.S.).N
+00001650: fa01 2f29 05da 0769 7465 7264 6972 7247  ../)...iterdirrG
+00001660: 0000 00da 046e 616d 6572 5900 0000 da0b  .....namerY.....
+00001670: 7570 6c6f 6164 5f66 696c 6529 0372 5b00  upload_file).r[.
+00001680: 0000 725c 0000 00da 0470 6174 68a9 03da  ..r\.....path...
+00001690: 115f 7570 6c6f 6164 5f64 6972 6563 746f  ._upload_directo
+000016a0: 7279 5a0c 6578 636c 7564 655f 7370 6563  ryZ.exclude_spec
+000016b0: 723a 0000 0072 2300 0000 7224 0000 0072  r:...r#...r$...r
+000016c0: 6300 0000 ed00 0000 730e 0000 000c 0108  c.......s.......
+000016d0: 0118 0112 0202 011a 0104 fa7a 3344 6174  ...........z3Dat
+000016e0: 6173 6574 2e75 706c 6f61 645f 6469 7265  aset.upload_dire
+000016f0: 6374 6f72 792e 3c6c 6f63 616c 733e 2e5f  ctory.<locals>._
+00001700: 7570 6c6f 6164 5f64 6972 6563 746f 7279  upload_directory
+00001710: da00 2908 7247 0000 0072 2f00 0000 7255  ..).rG...r/...rU
+00001720: 0000 0072 5800 0000 7256 0000 00da 0770  ...rX...rV.....p
+00001730: 6174 686c 6962 da04 5061 7468 da03 7374  athlib..Path..st
+00001740: 7229 0372 3a00 0000 725b 0000 0072 3e00  r).r:...r[...r>.
+00001750: 0000 7223 0000 0072 6200 0000 7224 0000  ..r#...rb...r$..
+00001760: 00da 1075 706c 6f61 645f 6469 7265 6374  ...upload_direct
+00001770: 6f72 79cc 0000 0073 1200 0000 0818 0e01  ory....s........
+00001780: 0402 0801 0601 0201 04ff 2004 0e09 7a18  .......... ...z.
+00001790: 4461 7461 7365 742e 7570 6c6f 6164 5f64  Dataset.upload_d
+000017a0: 6972 6563 746f 7279 da0f 6c6f 6361 6c5f  irectory..local_
+000017b0: 6669 6c65 5f70 6174 6872 4f00 0000 6303  file_pathrO...c.
+000017c0: 0000 0000 0000 0000 0000 0005 0000 0009  ................
+000017d0: 0000 0043 0000 0073 aa00 0000 7c01 a000  ...C...s....|...
+000017e0: a100 730b 7401 7c01 9b00 6401 9d02 8301  ..s.t.|...d.....
+000017f0: 8201 7c00 6a02 6a03 7404 6a05 6b03 7319  ..|.j.j.t.j.k.s.
+00001800: 7c00 6a02 6a06 7407 6a08 6b03 721d 7409  |.j.j.t.j.k.r.t.
+00001810: 6402 8301 8201 7c00 a00a 740b 6a0c a101  d.....|...t.j...
+00001820: 7d03 7c00 6a0d 6403 7501 722b 7c00 6a0d  }.|.j.d.u.r+|.j.
+00001830: 6e06 740e 7c03 6a0f 7c03 6404 8d02 7d04  n.t.|.j.|.d...}.
+00001840: 7c03 6a10 9b00 6405 7c02 a011 6405 a101  |.j...d.|...d...
+00001850: 9b00 9d03 7d02 7c04 6a12 7c01 7c02 7413  ....}.|.j.|.|.t.
+00001860: 6a14 7c00 6a02 6a15 7413 6a16 7c00 6a02  j.|.j.j.t.j.|.j.
+00001870: 6a17 7413 6a18 7c03 6a10 6903 6406 8d03  j.t.j.|.j.i.d...
+00001880: 0100 6403 5300 2907 611c 0100 000a 2020  ..d.S.).a.....  
+00001890: 2020 2020 2020 5570 6c6f 6164 7320 6120        Uploads a 
+000018a0: 6669 6c65 2074 6f20 7468 6520 6461 7461  file to the data
+000018b0: 7365 7427 7320 7374 6f72 6167 6520 6c6f  set's storage lo
+000018c0: 6361 7469 6f6e 2e0a 0a20 2020 2020 2020  cation...       
+000018d0: 203a 7061 7261 6d20 6669 6c65 5f70 6174   :param file_pat
+000018e0: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
+000018f0: 6865 2066 696c 6520 746f 2075 706c 6f61  he file to uploa
+00001900: 642e 0a20 2020 2020 2020 203a 7061 7261  d..        :para
+00001910: 6d20 6b65 793a 2054 6865 206b 6579 2074  m key: The key t
+00001920: 6f20 7573 6520 666f 7220 7468 6520 6669  o use for the fi
+00001930: 6c65 2069 6e20 7468 6520 6461 7461 7365  le in the datase
+00001940: 7427 7320 7374 6f72 6167 6520 6c6f 6361  t's storage loca
+00001950: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+00001960: 2020 2020 2020 2020 2020 4974 2077 696c            It wil
+00001970: 6c20 6265 2070 7265 6669 7865 6420 7769  l be prefixed wi
+00001980: 7468 2074 6865 2064 6174 6173 6574 2773  th the dataset's
+00001990: 2073 746f 7261 6765 2070 7265 6669 782e   storage prefix.
+000019a0: 0a20 2020 2020 2020 207a 0e20 6973 206e  .        z. is n
+000019b0: 6f74 2061 2066 696c 6572 3f00 0000 4e72  ot a filer?...Nr
+000019c0: 4100 0000 725d 0000 0029 0172 1d00 0000  A...r]...).r....
+000019d0: 2919 da07 6973 5f66 696c 6572 2f00 0000  )...is_filer/...
+000019e0: 7214 0000 0072 1900 0000 720f 0000 0072  r....r....r....r
+000019f0: 4400 0000 7218 0000 0072 1000 0000 7245  D...r....r....rE
+00001a00: 0000 0072 4600 0000 7249 0000 0072 0c00  ...rF...rI...r..
+00001a10: 0000 5a09 5265 6164 5772 6974 6572 1500  ..Z.ReadWriter..
+00001a20: 0000 7209 0000 0072 4b00 0000 5a0f 7265  ..r....rK...Z.re
+00001a30: 7175 6972 6564 5f70 7265 6669 78da 066c  quired_prefix..l
+00001a40: 7374 7269 7072 6000 0000 720a 0000 005a  stripr`...r....Z
+00001a50: 0944 6174 6173 6574 4964 7226 0000 00da  .DatasetIdr&....
+00001a60: 054f 7267 4964 721a 0000 005a 0c43 6f6d  .OrgIdr....Z.Com
+00001a70: 6d6f 6e50 7265 6669 7829 0572 3a00 0000  monPrefix).r:...
+00001a80: 7269 0000 0072 4f00 0000 7243 0000 0072  ri...rO...rC...r
+00001a90: 1e00 0000 7223 0000 0072 2300 0000 7224  ....r#...r#...r$
+00001aa0: 0000 0072 6000 0000 f800 0000 7330 0000  ...r`.......s0..
+00001ab0: 0008 0c0e 010e 030e 0102 0202 0104 ff0c  ................
+00001ac0: 040a 0306 ff02 0204 0102 0104 fe02 fd16  ................
+00001ad0: 0804 0102 0102 010a 020a 0108 0102 fd0a  ................
+00001ae0: fd7a 1344 6174 6173 6574 2e75 706c 6f61  .z.Dataset.uploa
+00001af0: 645f 6669 6c65 2902 4e4e 7220 0000 0029  d_file).NNr ...)
+00001b00: 26da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  &..__name__..__m
+00001b10: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001b20: 616d 655f 5f72 0e00 0000 da0f 5f5f 616e  ame__r......__an
+00001b30: 6e6f 7461 7469 6f6e 735f 5f72 1100 0000  notations__r....
+00001b40: 7215 0000 0072 0300 0000 7208 0000 0072  r....r....r....r
+00001b50: 1600 0000 720d 0000 00da 0b63 6c61 7373  ....r......class
+00001b60: 6d65 7468 6f64 7210 0000 0072 4500 0000  methodr....rE...
+00001b70: 720f 0000 0072 4400 0000 7267 0000 00da  r....rD...rg....
+00001b80: 0464 6963 7472 0200 0000 da04 6c69 7374  .dictr......list
+00001b90: 7225 0000 0072 2700 0000 da0b 636f 6c6c  r%...r'.....coll
+00001ba0: 6563 7469 6f6e 73da 0361 6263 da09 4765  ections..abc..Ge
+00001bb0: 6e65 7261 746f 7272 3800 0000 723b 0000  neratorr8...r;..
+00001bc0: 0072 6500 0000 7266 0000 0072 5100 0000  .re...rf...rQ...
+00001bd0: 720c 0000 0072 4a00 0000 7249 0000 0072  r....rJ...rI...r
+00001be0: 0700 0000 724c 0000 0072 5a00 0000 7268  ....rL...rZ...rh
+00001bf0: 0000 0072 6000 0000 7223 0000 0072 2300  ...r`...r#...r#.
+00001c00: 0000 7223 0000 0072 2400 0000 7212 0000  ..r#...r$...r...
+00001c10: 0017 0000 0073 e600 0000 0a00 0801 0801  .....s..........
+00001c20: 1001 1001 0202 0404 0401 0201 0201 0201  ................
+00001c30: 0201 0201 04f7 0202 02fe 0203 02fd 0204  ................
+00001c40: 02fc 0605 02fb 0606 02fa 0e07 02f9 0a08  ................
+00001c50: 02f8 0609 02f7 020a 0cf6 0210 0205 0201  ................
+00001c60: 04fb 0202 02fe 0203 02fd 0604 02fc 0605  ................
+00001c70: 02fb 0206 0cfa 020a 0205 0201 04fb 0a02  ................
+00001c80: 02fe 0203 02fd 0604 02fc 0605 02fb 0a06  ................
+00001c90: 0cfa 0222 04fc 0202 02fe 0203 02fd 0604  ..."............
+00001ca0: 02fc 0205 0afb 020d 0201 04fc 0402 02fe  ................
+00001cb0: 0a03 02fd 0a04 02fc 0205 0afb 0431 0201  .............1..
+00001cc0: 04fd 0202 02fe 0603 02fd 0204 0afc 020d  ................
+00001cd0: 0201 04fd 0a02 02fe 0a03 02fd 1004 0afc  ................
+00001ce0: 162d 0206 04fd 0402 02fe 0a03 02fd 0204  .-..............
+00001cf0: 0afc 022c 0402 02fe 0203 02fd 0204 0efc  ...,............
+00001d00: 7212 0000 0029 17da 0f63 6f6c 6c65 6374  r....)...collect
+00001d10: 696f 6e73 2e61 6263 7274 0000 0072 6500  ions.abcrt...re.
+00001d20: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
+00001d30: 0300 0000 7255 0000 00da 0573 6572 6465  ....rU.....serde
+00001d40: 7205 0000 00da 0566 696c 6573 7207 0000  r......filesr...
+00001d50: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00001d60: 7239 0000 0072 0c00 0000 720d 0000 0072  r9...r....r....r
+00001d70: 0e00 0000 720f 0000 0072 2200 0000 7210  ....r....r"...r.
+00001d80: 0000 0072 1100 0000 7212 0000 0072 2300  ...r....r....r#.
+00001d90: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
+00001da0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001db0: 1200 0000 0800 0801 1001 0802 0c02 1801  ................
+00001dc0: 1806 1006 1203                           ......
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 4911 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 2f13 0000  o.......Ms.d/...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 2f13 0000  o.......1..d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a05 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6403 6405 6c0a 6d0b 5a0b 0100 6403  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6407 6408 6c0e  d.l.m.Z...d.d.l.
@@ -66,16 +66,16 @@
 00000410: 0000 0300 0000 731a 0000 0074 0083 00a0  ......s....t....
 00000420: 01a1 0001 007c 027c 005f 027c 017c 005f  .....|.|._.|.|._
 00000430: 0364 0053 00a9 014e 2904 da05 7375 7065  .d.S...N)...supe
 00000440: 72da 085f 5f69 6e69 745f 5f72 1500 0000  r..__init__r....
 00000450: 7216 0000 0029 03da 0473 656c 6672 1700  r....)...selfr..
 00000460: 0000 7218 0000 00a9 01da 095f 5f63 6c61  ..r........__cla
 00000470: 7373 5f5f a900 faf5 2f63 6f64 6562 7569  ss__..../codebui
-00000480: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
-00000490: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
+00000480: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+00000490: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
 000004a0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000004b0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000004c0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000004d0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000004e0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000004f0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000500: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 5401 0000  o.......Ms.dT...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 5401 0000  o.......1..dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6404 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6502 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 6402 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 0341 6e79 4ee9 0100 0000 2902 da0d  ...AnyN.....)...
@@ -26,15 +26,15 @@
 00000190: 5f72 0400 0000 da0f 5f5f 616e 6e6f 7461  _r......__annota
 000001a0: 7469 6f6e 735f 5f72 0500 0000 da08 7079  tions__r......py
 000001b0: 6461 6e74 6963 da05 4669 656c 64da 0464  dantic..Field..d
 000001c0: 6963 7472 0a00 0000 da03 7374 7272 0200  ictr......strr..
 000001d0: 0000 da04 6c69 7374 720b 0000 00a9 0072  ....listr......r
 000001e0: 1500 0000 7215 0000 00fa f62f 636f 6465  ....r....../code
 000001f0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000200: 3334 3937 3236 3836 3730 2f73 7263 2f63  3497268670/src/c
+00000200: 3136 3839 3135 3533 3939 2f73 7263 2f63  1689155399/src/c
 00000210: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 00000220: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000230: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000240: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 00000250: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 00000260: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000270: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 867 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 6303 0000  o.......Ms.dc...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 6303 0000  o.......1..dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6505 6501  Z.G.d.d...d.e.e.
 00000060: 6a06 8304 5a07 4700 6405 6406 8400 6406  j...Z.G.d.d...d.
 00000070: 6505 6501 6a06 8304 5a08 4700 6407 6408  e.e.j...Z.G.d.d.
@@ -13,15 +13,15 @@
 000000c0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
 000000d0: 0d41 646d 696e 6973 7472 6174 6f72 da06  .Administrator..
 000000e0: 526f 626f 746f 4e29 04da 085f 5f6e 616d  RobotoN)...__nam
 000000f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000100: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0500  .__qualname__r..
 00000110: 0000 a900 7209 0000 0072 0900 0000 faee  ....r....r......
 00000120: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000130: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+00000130: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 00000140: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000150: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000160: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000170: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000180: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000190: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,69 +122,77 @@
             self.__record.storage_location != StorageLocation.S3
             or self.__record.administrator != Administrator.Roboto
         ):
             raise NotImplementedError(
                 "Only S3-backed storage administered by Roboto is supported at this time."
             )
 
-        include_pattern_spec: Optional[pathspec.PathSpec] = None
-        if include_patterns is not None:
-            include_pattern_spec = pathspec.PathSpec.from_lines(
-                pathspec.patterns.GitWildMatchPattern, include_patterns
-            )
-
-        exclude_pattern_spec: Optional[pathspec.PathSpec] = None
-        if exclude_patterns is not None:
-            exclude_pattern_spec = pathspec.GitIgnoreSpec.from_lines(exclude_patterns)
-
         if not out_path.is_dir():
             out_path.mkdir(parents=True)
 
         credentials = self.get_temporary_credentials(AccessMode.ReadOnly)
         files_delegate = (
             self.__files_delegate
             if self.__files_delegate is not None
             else FileS3Delegate(
                 bucket_name=credentials.bucket,
                 credentials=credentials,
             )
         )
-        for file in self.list_files():
-            if include_pattern_spec and not include_pattern_spec.match_file(
-                file.relative_path
-            ):
-                """Given file does not match any of the include patterns."""
-                continue
-            if exclude_pattern_spec and exclude_pattern_spec.match_file(
-                file.relative_path
-            ):
-                """Given file matches one of the exclude patterns."""
-                continue
-
+        for file in self.list_files(include_patterns, exclude_patterns):
             local_path = out_path / file.relative_path
             files_delegate.download_file(file.key, local_path)
 
     def get_temporary_credentials(
         self,
         mode: AccessMode = AccessMode.ReadOnly,
         caller: Optional[str] = None,  # A Roboto user_id
     ) -> Credentials:
         if self.__temp_credentials is None or self.__temp_credentials.is_expired():
             self.__temp_credentials = self.__delegate.get_temporary_credentials(
                 self.__record, mode, caller
             )
         return self.__temp_credentials
 
-    def list_files(self) -> collections.abc.Generator[File, None, None]:
+    def list_files(
+        self,
+        include_patterns: Optional[list[str]] = None,
+        exclude_patterns: Optional[list[str]] = None,
+    ) -> collections.abc.Generator[File, None, None]:
+        """
+        `include_patterns` and `exclude_patterns` are lists of gitignore-style patterns.
+        See https://git-scm.com/docs/gitignore.
+        """
+        include_pattern_spec: Optional[pathspec.PathSpec] = None
+        if include_patterns is not None:
+            include_pattern_spec = pathspec.PathSpec.from_lines(
+                pathspec.patterns.GitWildMatchPattern, include_patterns
+            )
+
+        exclude_pattern_spec: Optional[pathspec.PathSpec] = None
+        if exclude_patterns is not None:
+            exclude_pattern_spec = pathspec.GitIgnoreSpec.from_lines(exclude_patterns)
+
         paginated_results = self.__delegate.list_files(
             self.__record.dataset_id, self.__record.org_id
         )
         while True:
             for record in paginated_results.items:
-                yield File(record)
+                file = File(record)
+                if include_pattern_spec and not include_pattern_spec.match_file(
+                    file.relative_path
+                ):
+                    """Given file does not match any of the include patterns."""
+                    continue
+                if exclude_pattern_spec and exclude_pattern_spec.match_file(
+                    file.relative_path
+                ):
+                    """Given file matches one of the exclude patterns."""
+                    continue
+                yield file
             if paginated_results.next_token:
                 paginated_results = self.__delegate.list_files(
                     self.__record.dataset_id,
                     self.__record.org_id,
                     paginated_results.next_token,
                 )
             else:
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 436 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 b401 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 b401 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
@@ -22,16 +22,16 @@
 00000150: 6572 0400 0000 da0d 6874 7470 5f64 656c  er......http_del
 00000160: 6567 6174 6572 0500 0000 da0e 6874 7470  egater......http
 00000170: 5f72 6573 6f75 7263 6573 7206 0000 0072  _resourcesr....r
 00000180: 0700 0000 da06 7265 636f 7264 7208 0000  ......recordr...
 00000190: 005a 0b73 335f 6465 6c65 6761 7465 7209  .Z.s3_delegater.
 000001a0: 0000 00da 075f 5f61 6c6c 5f5f a900 7210  .....__all__..r.
 000001b0: 0000 0072 1000 0000 faed 2f63 6f64 6562  ...r....../codeb
-000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
-000001d0: 3439 3732 3638 3637 302f 7372 632f 636f  497268670/src/co
+000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
+000001d0: 3638 3931 3535 3339 392f 7372 632f 636f  689155399/src/co
 000001e0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001f0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000200: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000210: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000220: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000230: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000240: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1181 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 9d04 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 9d04 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6501 6a07 8303 5a08  d.d...d.e.j...Z.
 00000070: 4700 6407 6408 8400 6408 6500 6a09 8303  G.d.d...d.e.j...
@@ -17,16 +17,16 @@
 00000100: 6964 5a0d 636f 6d6d 6f6e 5f70 7265 6669  idZ.common_prefi
 00000110: 784e 2906 da08 5f5f 6e61 6d65 5f5f da0a  xN)...__name__..
 00000120: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000130: 616c 6e61 6d65 5f5f da09 4461 7461 7365  alname__..Datase
 00000140: 7449 64da 054f 7267 4964 da0c 436f 6d6d  tId..OrgId..Comm
 00000150: 6f6e 5072 6566 6978 a900 720e 0000 0072  onPrefix..r....r
 00000160: 0e00 0000 faed 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000170: 2f6f 7574 7075 742f 7372 6333 3439 3732  /output/src34972
-00000180: 3638 3637 302f 7372 632f 636f 6465 7374  68670/src/codest
+00000170: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
+00000180: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
 00000190: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000001a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000001b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000001c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000001d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000001e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000001f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 802 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 2203 0000  o.......Ms.d"...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 2203 0000  o.......1..d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6403 6404 6c04 6d05 5a05 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 8302 5a06 6402 5300  d.d...d...Z.d.S.
 00000060: 2907 e900 0000 0029 01da 084f 7074 696f  )......)...Optio
 00000070: 6e61 6c4e e901 0000 0029 01da 0a46 696c  nalN.....)...Fil
@@ -21,15 +21,15 @@
 00000140: 4669 6c65 5f5f 7061 7273 6564 5f75 7269  File__parsed_uri
 00000150: da06 7265 636f 7264 6302 0000 0000 0000  ..recordc.......
 00000160: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000170: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
 00000180: a901 4e29 0172 0600 0000 2902 da04 7365  ..N).r....)...se
 00000190: 6c66 7208 0000 00a9 0072 0b00 0000 fae9  lfr......r......
 000001a0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001b0: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+000001b0: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 000001c0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 000001d0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000001e0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000001f0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000200: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000210: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000220: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 2166 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 7608 0000  o.......Ms.dv...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 7608 0000  o.......1..dv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6406 6408 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6406 6409 6c0d  m.Z.m.Z...d.d.l.
@@ -56,15 +56,15 @@
 00000370: 0000 0074 0083 00a0 01a1 0001 007c 027c  ...t.........|.|
 00000380: 005f 027c 017c 005f 0364 0053 00a9 014e  ._.|.|._.d.S...N
 00000390: 2904 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
 000003a0: 745f 5f72 0d00 0000 720e 0000 0029 03da  t__r....r....)..
 000003b0: 0473 656c 6672 0f00 0000 7210 0000 00a9  .selfr....r.....
 000003c0: 01da 095f 5f63 6c61 7373 5f5f a900 faf2  ...__class__....
 000003d0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000003e0: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+000003e0: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 000003f0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000400: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000410: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000420: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000430: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000440: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000450: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 a800 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 a800 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 4700 6404 6405 8400  e.j...Z.G.d.d...
 00000050: 6405 6500 6a01 8303 5a03 6401 5300 2906  d.e.j...Z.d.S.).
 00000060: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
 00000070: 0000 0000 0000 0003 0000 0040 0000 00f3  ...........@....
@@ -12,15 +12,15 @@
 000000b0: 5265 7175 6573 74da 0662 7563 6b65 74da  Request..bucket.
 000000c0: 036b 6579 4ea9 05da 085f 5f6e 616d 655f  .keyN....__name_
 000000d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 000000e0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 000000f0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000100: 5fa9 0072 0c00 0000 720c 0000 00fa f32f  _..r....r....../
 00000110: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000120: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
+00000120: 2f73 7263 3136 3839 3135 3533 3939 2f73  /src1689155399/s
 00000130: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000140: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000150: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000160: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000170: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000180: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000190: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 382 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 7e01 0000  o.......Ms.d~...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 7e01 0000  o.......1..d~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 4700  d.l.Z.d.d.l.Z.G.
 00000040: 6402 6403 8400 6403 6501 6a02 8303 5a03  d.d...d.e.j...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6300 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 0000 0000 0003 0000  ................
 00000070: 0040 0000 0073 4000 0000 6500 5a01 6400  .@...s@...e.Z.d.
@@ -17,15 +17,15 @@
 00000100: 0375 7269 4e29 07da 085f 5f6e 616d 655f  .uriN)...__name_
 00000110: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000120: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 00000130: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000140: 5fda 0864 6174 6574 696d 65da 0369 6e74  _..datetime..int
 00000150: a900 720f 0000 0072 0f00 0000 faeb 2f63  ..r....r....../c
 00000160: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000170: 7372 6333 3439 3732 3638 3637 302f 7372  src3497268670/sr
+00000170: 7372 6331 3638 3931 3535 3339 392f 7372  src1689155399/sr
 00000180: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000190: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000001a0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000001b0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000001c0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000001d0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000001e0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 2358 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 3609 0000  o.......Ms.d6...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 3609 0000  o.......1..d6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6400 6401 6c07 5a07 6403 6404 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6403 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
@@ -22,16 +22,16 @@
 00000150: 6563 7265 745f 6163 6365 7373 5f6b 6579  ecret_access_key
 00000160: da0d 7365 7373 696f 6e5f 746f 6b65 6e4e  ..session_tokenN
 00000170: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000180: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000190: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
 000001a0: 6e6e 6f74 6174 696f 6e73 5f5f a900 7212  nnotations__..r.
 000001b0: 0000 0072 1200 0000 faf0 2f63 6f64 6562  ...r....../codeb
-000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
-000001d0: 3439 3732 3638 3637 302f 7372 632f 636f  497268670/src/co
+000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
+000001d0: 3638 3931 3535 3339 392f 7372 632f 636f  689155399/src/co
 000001e0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001f0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000200: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000210: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000220: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000230: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000240: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/http_delegates.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/http_delegates.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from .delegate import OrgDelegate
 from .http_delegate import OrgHttpDelegate
 from .http_resources import (
     BindEmailDomainRequest,
     CreateOrgRequest,
     InviteUserRequest,
+    ModifyRoleForUserRequest,
+    RemoveUserFromOrgRequest,
 )
 from .org import Org
 from .org_invite import OrgInvite
 from .org_role import OrgRole
 from .record import (
     OrgInviteRecord,
     OrgRecord,
@@ -20,14 +22,16 @@
     OrgType,
 )
 
 __all__ = [
     "BindEmailDomainRequest",
     "CreateOrgRequest",
     "InviteUserRequest",
+    "RemoveUserFromOrgRequest",
+    "ModifyRoleForUserRequest",
     "Org",
     "OrgDelegate",
     "OrgHttpDelegate",
     "OrgInvite",
     "OrgInviteRecord",
     "OrgRecord",
     "OrgRole",
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1815 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,158 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 1707 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 2207 0000  o.......1..d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
+00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 6d09 5a09 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
-00000070: 8302 5a0a 6409 5300 290a e900 0000 0029  ..Z.d.S.)......)
-00000080: 02da 0341 6e79 da08 4f70 7469 6f6e 616c  ...Any..Optional
-00000090: e903 0000 0029 01da 1670 7964 616e 7469  .....)...pydanti
-000000a0: 635f 6a73 6f6e 6162 6c65 5f64 6963 74e9  c_jsonable_dict.
-000000b0: 0100 0000 2901 da0b 4f72 6744 656c 6567  ....)...OrgDeleg
-000000c0: 6174 6529 02da 094f 7267 5265 636f 7264  ate)...OrgRecord
-000000d0: da07 4f72 6754 7970 6563 0000 0000 0000  ..OrgTypec......
-000000e0: 0000 0000 0000 0000 0000 0c00 0000 4000  ..............@.
-000000f0: 0000 73d4 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-00000100: 0065 0365 0464 013c 0065 0565 0464 023c  .e.e.d.<.e.e.d.<
-00000110: 0065 0609 0364 1f64 0465 0765 0819 0064  .e...d.d.e.e...d
-00000120: 0565 0864 0665 0964 0765 0564 0865 0a66  .e.d.e.d.e.d.e.f
-00000130: 0a64 0964 0a84 0583 015a 0b65 0664 0b65  .d.d.....Z.e.d.e
-00000140: 0864 0765 0564 0c64 0066 0664 0d64 0e84  .d.e.d.d.f.d.d..
-00000150: 0483 015a 0c65 0664 0f65 0765 0819 0064  ...Z.e.d.e.e...d
-00000160: 0765 0564 0c65 0d64 0019 0066 0664 1064  .e.d.e.d...f.d.d
-00000170: 1184 0483 015a 0e64 2064 1364 1484 045a  .....Z.d d.d...Z
-00000180: 0f64 1565 0864 0c64 1266 0464 1664 1784  .d.e.d.d.f.d.d..
-00000190: 045a 1064 1865 0364 0765 0566 0464 1964  .Z.d.e.d.e.f.d.d
-000001a0: 1a84 045a 1164 0c65 1265 0865 1366 0219  ...Z.d.e.e.e.f..
-000001b0: 0066 0264 1b64 1c84 045a 1465 1564 1d64  .f.d.d...Z.e.d.d
-000001c0: 1e84 0083 015a 1664 1253 0029 21da 034f  .....Z.d.S.)!..O
-000001d0: 7267 da0c 5f4f 7267 5f5f 7265 636f 7264  rg.._Org__record
-000001e0: da12 5f4f 7267 5f5f 6f72 675f 6465 6c65  .._Org__org_dele
-000001f0: 6761 7465 46da 0f63 7265 6174 6f72 5f75  gateF..creator_u
-00000200: 7365 725f 6964 da04 6e61 6d65 da08 6f72  ser_id..name..or
-00000210: 675f 7479 7065 da0c 6f72 675f 6465 6c65  g_type..org_dele
-00000220: 6761 7465 da11 6269 6e64 5f65 6d61 696c  gate..bind_email
-00000230: 5f64 6f6d 6169 6e63 0600 0000 0000 0000  _domainc........
-00000240: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
-00000250: 731e 0000 007c 046a 007c 017c 027c 037c  s....|.j.|.|.|.|
-00000260: 0564 018d 047d 067c 007c 067c 0464 028d  .d...}.|.|.|.d..
-00000270: 0253 0029 034e 2904 720d 0000 0072 0e00  .S.).N).r....r..
-00000280: 0000 720f 0000 0072 1100 0000 a902 da06  ..r....r........
-00000290: 7265 636f 7264 7210 0000 0029 01da 0a63  recordr....)...c
-000002a0: 7265 6174 655f 6f72 6729 07da 0363 6c73  reate_org)...cls
-000002b0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-000002c0: 1000 0000 7211 0000 0072 1300 0000 a900  ....r....r......
-000002d0: 7216 0000 00fa e72f 636f 6465 6275 696c  r....../codebuil
-000002e0: 642f 6f75 7470 7574 2f73 7263 3334 3937  d/output/src3497
-000002f0: 3236 3836 3730 2f73 7263 2f63 6f64 6573  268670/src/codes
-00000300: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
-00000310: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
-00000320: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
-00000330: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
-00000340: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
-00000350: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
-00000360: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
-00000370: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
-00000380: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
-00000390: 732f 726f 626f 746f 5f73 646b 2f73 7263  s/roboto_sdk/src
-000003a0: 2f72 6f62 6f74 6f5f 7364 6b2f 646f 6d61  /roboto_sdk/doma
-000003b0: 696e 2f6f 7267 732f 6f72 672e 7079 da06  in/orgs/org.py..
-000003c0: 6372 6561 7465 0e00 0000 730e 0000 0004  create....s.....
-000003d0: 0902 0102 0102 0102 0106 fc0c 067a 0a4f  .............z.O
-000003e0: 7267 2e63 7265 6174 65da 066f 7267 5f69  rg.create..org_i
-000003f0: 64da 0672 6574 7572 6e63 0300 0000 0000  d..returnc......
-00000400: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-00000410: 0000 7318 0000 007c 026a 007c 0164 018d  ..s....|.j.|.d..
-00000420: 017d 037c 007c 037c 0264 028d 0253 0029  .}.|.|.|.d...S.)
-00000430: 034e a901 7219 0000 0072 1200 0000 2901  .N..r....r....).
-00000440: da0d 6765 745f 6f72 675f 6279 5f69 6429  ..get_org_by_id)
-00000450: 0472 1500 0000 7219 0000 0072 1000 0000  .r....r....r....
-00000460: 7213 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000470: 1700 0000 da09 6279 5f6f 7267 5f69 641f  ......by_org_id.
-00000480: 0000 0073 0400 0000 0c02 0c01 7a0d 4f72  ...s........z.Or
-00000490: 672e 6279 5f6f 7267 5f69 64da 0775 7365  g.by_org_id..use
-000004a0: 725f 6964 6303 0000 0000 0000 0000 0000  r_idc...........
-000004b0: 0004 0000 0003 0000 0003 0000 0073 2000  .............s .
-000004c0: 0000 8801 6a00 7c01 6401 8d01 7d03 8700  ....j.|.d...}...
-000004d0: 8701 6602 6402 6403 8408 7c03 4400 8301  ..f.d.d...|.D...
-000004e0: 5300 2904 4e29 0172 1e00 0000 6301 0000  S.).N).r....c...
-000004f0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00000500: 0013 0000 0073 1800 0000 6700 7c00 5d08  .....s....g.|.].
-00000510: 7d01 8800 7c01 8801 6400 8d02 9102 7102  }...|...d.....q.
-00000520: 5300 2901 7212 0000 0072 1600 0000 2902  S.).r....r....).
-00000530: da02 2e30 7213 0000 00a9 0272 1500 0000  ...0r......r....
-00000540: 7210 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00000550: 0a3c 6c69 7374 636f 6d70 3e29 0000 0073  .<listcomp>)...s
-00000560: 0200 0000 1800 7a22 4f72 672e 6279 5f75  ......z"Org.by_u
-00000570: 7365 725f 6964 2e3c 6c6f 6361 6c73 3e2e  ser_id.<locals>.
-00000580: 3c6c 6973 7463 6f6d 703e 2901 da0d 6f72  <listcomp>)...or
-00000590: 6773 5f66 6f72 5f75 7365 7229 0472 1500  gs_for_user).r..
-000005a0: 0000 721e 0000 0072 1000 0000 da07 7265  ..r....r......re
-000005b0: 636f 7264 7372 1600 0000 7220 0000 0072  cordsr....r ...r
-000005c0: 1700 0000 da0a 6279 5f75 7365 725f 6964  ......by_user_id
-000005d0: 2400 0000 7304 0000 000c 0414 017a 0e4f  $...s........z.O
-000005e0: 7267 2e62 795f 7573 6572 5f69 644e 6301  rg.by_user_idNc.
-000005f0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000600: 0000 0043 0000 0073 1400 0000 7c00 6a00  ...C...s....|.j.
-00000610: 6a01 7c00 6a02 6401 8d01 0100 6400 5300  j.|.j.d.....d.S.
-00000620: 2902 4e72 1b00 0000 2903 720c 0000 00da  ).Nr....).r.....
-00000630: 0a64 656c 6574 655f 6f72 6772 1900 0000  .delete_orgr....
-00000640: a901 da04 7365 6c66 7216 0000 0072 1600  ....selfr....r..
-00000650: 0000 7217 0000 00da 0664 656c 6574 652b  ..r......delete+
-00000660: 0000 0073 0200 0000 1401 7a0a 4f72 672e  ...s......z.Org.
-00000670: 6465 6c65 7465 da0c 656d 6169 6c5f 646f  delete..email_do
-00000680: 6d61 696e 6302 0000 0000 0000 0000 0000  mainc...........
-00000690: 0002 0000 0004 0000 0043 0000 0073 1800  .........C...s..
-000006a0: 0000 7c00 6a00 6a01 7c00 6a02 6a03 7c01  ..|.j.j.|.j.j.|.
-000006b0: 6401 8d02 0100 6400 5300 2902 4e29 0272  d.....d.S.).N).r
-000006c0: 1900 0000 7229 0000 0029 0472 0c00 0000  ....r)...).r....
-000006d0: 7211 0000 0072 0b00 0000 7219 0000 0029  r....r....r....)
-000006e0: 0272 2700 0000 7229 0000 0072 1600 0000  .r'...r)...r....
-000006f0: 7216 0000 0072 1700 0000 7211 0000 002e  r....r....r.....
-00000700: 0000 0073 0600 0000 0601 0801 0aff 7a15  ...s..........z.
-00000710: 4f72 672e 6269 6e64 5f65 6d61 696c 5f64  Org.bind_email_d
-00000720: 6f6d 6169 6e72 1300 0000 6303 0000 0000  omainr....c.....
-00000730: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000740: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
-00000750: 7c00 5f01 6400 5300 a901 4e29 0272 0b00  |._.d.S...N).r..
-00000760: 0000 720c 0000 0029 0372 2700 0000 7213  ..r....).r'...r.
-00000770: 0000 0072 1000 0000 7216 0000 0072 1600  ...r....r....r..
-00000780: 0000 7217 0000 00da 085f 5f69 6e69 745f  ..r......__init_
-00000790: 5f33 0000 0073 0400 0000 0601 0a01 7a0c  _3...s........z.
-000007a0: 4f72 672e 5f5f 696e 6974 5f5f 6301 0000  Org.__init__c...
-000007b0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000007c0: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-000007d0: 8301 5300 722a 0000 0029 0272 0500 0000  ..S.r*...).r....
-000007e0: 720b 0000 0072 2600 0000 7216 0000 0072  r....r&...r....r
-000007f0: 1600 0000 7217 0000 00da 0774 6f5f 6469  ....r......to_di
-00000800: 6374 3700 0000 7302 0000 000a 017a 0b4f  ct7...s......z.O
-00000810: 7267 2e74 6f5f 6469 6374 6301 0000 0000  rg.to_dictc.....
-00000820: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000830: 0000 0073 0800 0000 7c00 6a00 6a01 5300  ...s....|.j.j.S.
-00000840: 722a 0000 0029 0272 0b00 0000 7219 0000  r*...).r....r...
-00000850: 0072 2600 0000 7216 0000 0072 1600 0000  .r&...r....r....
-00000860: 7217 0000 0072 1900 0000 3a00 0000 7302  r....r....:...s.
-00000870: 0000 0008 027a 0a4f 7267 2e6f 7267 5f69  .....z.Org.org_i
-00000880: 6429 0146 2902 721a 0000 004e 2917 da08  d).F).r....N)...
-00000890: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000008a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000008b0: 5f5f 7208 0000 00da 0f5f 5f61 6e6e 6f74  __r......__annot
-000008c0: 6174 696f 6e73 5f5f 7207 0000 00da 0b63  ations__r......c
-000008d0: 6c61 7373 6d65 7468 6f64 7203 0000 00da  lassmethodr.....
-000008e0: 0373 7472 7209 0000 00da 0462 6f6f 6c72  .strr......boolr
-000008f0: 1800 0000 721d 0000 00da 046c 6973 7472  ....r......listr
-00000900: 2400 0000 7228 0000 0072 1100 0000 722b  $...r(...r....r+
-00000910: 0000 00da 0464 6963 7472 0200 0000 722c  .....dictr....r,
-00000920: 0000 00da 0870 726f 7065 7274 7972 1900  .....propertyr..
-00000930: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00000940: 0072 1700 0000 720a 0000 000a 0000 0073  .r....r........s
-00000950: 4000 0000 0a00 0801 0801 0202 0207 04fa  @...............
-00000960: 0602 02fe 0203 02fd 0204 02fc 0205 02fb  ................
-00000970: 0206 0cfa 0210 1801 0204 0201 0601 02ff  ................
-00000980: 0201 02ff 0602 0cfe 0a06 1203 1205 1604  ................
-00000990: 0203 0e01 720a 0000 004e 290b da06 7479  ....r....N)...ty
-000009a0: 7069 6e67 7202 0000 0072 0300 0000 da05  pingr....r......
-000009b0: 7365 7264 6572 0500 0000 da08 6465 6c65  serder......dele
-000009c0: 6761 7465 7207 0000 0072 1300 0000 7208  gater....r....r.
-000009d0: 0000 0072 0900 0000 720a 0000 0072 1600  ...r....r....r..
-000009e0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000009f0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000a00: 0a00 0000 1002 0c02 0c01 1001 1203       ..............
+00000060: 0100 4700 6407 6408 8400 6408 8302 5a09  ..G.d.d...d...Z.
+00000070: 6409 5300 290a e900 0000 0029 02da 0341  d.S.)......)...A
+00000080: 6e79 da08 4f70 7469 6f6e 616c e903 0000  ny..Optional....
+00000090: 0029 01da 1670 7964 616e 7469 635f 6a73  .)...pydantic_js
+000000a0: 6f6e 6162 6c65 5f64 6963 74e9 0100 0000  onable_dict.....
+000000b0: 2901 da0d 546f 6b65 6e44 656c 6567 6174  )...TokenDelegat
+000000c0: 6529 01da 0b54 6f6b 656e 5265 636f 7264  e)...TokenRecord
+000000d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000000e0: 000b 0000 0040 0000 0073 e000 0000 6500  .....@...s....e.
+000000f0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000100: 6505 6504 6402 3c00 6506 6403 6507 6404  e.e.d.<.e.d.e.d.
+00000110: 6505 6405 6400 6606 6406 6407 8404 8301  e.d.d.f.d.d.....
+00000120: 5a08 6506 6408 6509 6507 1900 6404 6505  Z.e.d.e.e...d.e.
+00000130: 6405 650a 6400 1900 6606 6409 640a 8404  d.e.d...f.d.d...
+00000140: 8301 5a0b 6506 6408 6509 6507 1900 640b  ..Z.e.d.e.e...d.
+00000150: 650c 640c 6507 640d 6509 6507 1900 6404  e.d.e.d.e.e...d.
+00000160: 6505 660a 640e 640f 8404 8301 5a0d 6410  e.f.d.d.....Z.d.
+00000170: 6411 8400 5a0e 6412 6503 6404 6505 6604  d...Z.d.e.d.e.f.
+00000180: 6413 6414 8404 5a0f 6405 6510 6507 6511  d.d...Z.d.e.e.e.
+00000190: 6602 1900 6602 6415 6416 8404 5a12 6513  f...f.d.d...Z.e.
+000001a0: 6405 6509 6507 1900 6602 6417 6418 8404  d.e.e...f.d.d...
+000001b0: 8301 5a14 6513 6405 6509 6507 1900 6602  ..Z.e.d.e.e...f.
+000001c0: 6419 641a 8404 8301 5a15 641b 5300 291c  d.d.....Z.d.S.).
+000001d0: da05 546f 6b65 6eda 0e5f 546f 6b65 6e5f  ..Token.._Token_
+000001e0: 5f72 6563 6f72 64da 165f 546f 6b65 6e5f  _record.._Token_
+000001f0: 5f74 6f6b 656e 5f64 656c 6567 6174 65da  _token_delegate.
+00000200: 0874 6f6b 656e 5f69 64da 0e74 6f6b 656e  .token_id..token
+00000210: 5f64 656c 6567 6174 65da 0672 6574 7572  _delegate..retur
+00000220: 6e63 0300 0000 0000 0000 0000 0000 0400  nc..............
+00000230: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
+00000240: 026a 007c 0164 018d 017d 037c 007c 037c  .j.|.d...}.|.|.|
+00000250: 0264 028d 0253 0029 034e a901 720c 0000  .d...S.).N..r...
+00000260: 00a9 02da 0672 6563 6f72 6472 0d00 0000  .....recordr....
+00000270: 2901 da15 6765 745f 746f 6b65 6e5f 6279  )...get_token_by
+00000280: 5f74 6f6b 656e 5f69 6429 04da 0363 6c73  _token_id)...cls
+00000290: 720c 0000 0072 0d00 0000 7211 0000 00a9  r....r....r.....
+000002a0: 0072 1400 0000 faeb 2f63 6f64 6562 7569  .r....../codebui
+000002b0: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+000002c0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+000002d0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
+000002e0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
+000002f0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
+00000300: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
+00000310: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
+00000320: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
+00000330: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
+00000340: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
+00000350: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
+00000360: 6573 2f72 6f62 6f74 6f5f 7364 6b2f 7372  es/roboto_sdk/sr
+00000370: 632f 726f 626f 746f 5f73 646b 2f64 6f6d  c/roboto_sdk/dom
+00000380: 6169 6e2f 746f 6b65 6e73 2f74 6f6b 656e  ain/tokens/token
+00000390: 2e70 79da 0766 726f 6d5f 6964 0e00 0000  .py..from_id....
+000003a0: 7304 0000 000c 020c 017a 0d54 6f6b 656e  s........z.Token
+000003b0: 2e66 726f 6d5f 6964 da07 7573 6572 5f69  .from_id..user_i
+000003c0: 6463 0300 0000 0000 0000 0000 0000 0400  dc..............
+000003d0: 0000 0300 0000 0300 0000 7320 0000 0088  ..........s ....
+000003e0: 016a 007c 0164 018d 017d 0387 0087 0166  .j.|.d...}.....f
+000003f0: 0264 0264 0384 087c 0344 0083 0153 0029  .d.d...|.D...S.)
+00000400: 044e 2901 7217 0000 0063 0100 0000 0000  .N).r....c......
+00000410: 0000 0000 0000 0200 0000 0600 0000 1300  ................
+00000420: 0000 7318 0000 0067 007c 005d 087d 0188  ..s....g.|.].}..
+00000430: 007c 0188 0164 008d 0291 0271 0253 0029  .|...d.....q.S.)
+00000440: 0172 1000 0000 7214 0000 0029 02da 022e  .r....r....)....
+00000450: 3072 1100 0000 a902 7213 0000 0072 0d00  0r......r....r..
+00000460: 0000 7214 0000 0072 1500 0000 da0a 3c6c  ..r....r......<l
+00000470: 6973 7463 6f6d 703e 1800 0000 7302 0000  istcomp>....s...
+00000480: 0018 007a 2254 6f6b 656e 2e66 6f72 5f75  ...z"Token.for_u
+00000490: 7365 722e 3c6c 6f63 616c 733e 2e3c 6c69  ser.<locals>.<li
+000004a0: 7374 636f 6d70 3e29 01da 1367 6574 5f74  stcomp>)...get_t
+000004b0: 6f6b 656e 735f 666f 725f 7573 6572 2904  okens_for_user).
+000004c0: 7213 0000 0072 1700 0000 720d 0000 00da  r....r....r.....
+000004d0: 0772 6563 6f72 6473 7214 0000 0072 1900  .recordsr....r..
+000004e0: 0000 7215 0000 00da 0866 6f72 5f75 7365  ..r......for_use
+000004f0: 7213 0000 0073 0400 0000 0c04 1401 7a0e  r....s........z.
+00000500: 546f 6b65 6e2e 666f 725f 7573 6572 da0b  Token.for_user..
+00000510: 6578 7069 7279 5f64 6179 73da 046e 616d  expiry_days..nam
+00000520: 65da 0b64 6573 6372 6970 7469 6f6e 6306  e..descriptionc.
+00000530: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+00000540: 0000 0043 0000 0073 1e00 0000 7c05 6a00  ...C...s....|.j.
+00000550: 7c01 7c02 7c03 7c04 6401 8d04 7d06 7c00  |.|.|.|.d...}.|.
+00000560: 7c06 7c05 6402 8d02 5300 2903 4e29 0472  |.|.d...S.).N).r
+00000570: 1700 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+00000580: 0000 0072 1000 0000 2901 da0c 6372 6561  ...r....)...crea
+00000590: 7465 5f74 6f6b 656e 2907 7213 0000 0072  te_token).r....r
+000005a0: 1700 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000005b0: 0000 0072 0d00 0000 7211 0000 0072 1400  ...r....r....r..
+000005c0: 0000 7214 0000 0072 1500 0000 da06 6372  ..r....r......cr
+000005d0: 6561 7465 1a00 0000 7308 0000 0004 0908  eate....s.......
+000005e0: 0106 ff0c 037a 0c54 6f6b 656e 2e63 7265  .....z.Token.cre
+000005f0: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
+00000600: 0100 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
+00000610: 007c 006a 006a 0164 0075 0173 084a 0082  .|.j.j.d.u.s.J..
+00000620: 017c 006a 026a 037c 006a 006a 016a 0464  .|.j.j.|.j.j.j.d
+00000630: 018d 0153 0029 024e 720f 0000 0029 0572  ...S.).Nr....).r
+00000640: 0a00 0000 da07 636f 6e74 6578 7472 0b00  ......contextr..
+00000650: 0000 da0c 6465 6c65 7465 5f74 6f6b 656e  ....delete_token
+00000660: 720c 0000 00a9 01da 0473 656c 6672 1400  r........selfr..
+00000670: 0000 7214 0000 0072 1500 0000 da06 6465  ..r....r......de
+00000680: 6c65 7465 2800 0000 7308 0000 0010 0106  lete(...s.......
+00000690: 0108 0106 ff7a 0c54 6f6b 656e 2e64 656c  .....z.Token.del
+000006a0: 6574 6572 1100 0000 6303 0000 0000 0000  eter....c.......
+000006b0: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+000006c0: 0073 1000 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
+000006d0: 5f01 6400 5300 a901 4e29 0272 0a00 0000  _.d.S...N).r....
+000006e0: 720b 0000 0029 0372 2600 0000 7211 0000  r....).r&...r...
+000006f0: 0072 0d00 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000700: 7215 0000 00da 085f 5f69 6e69 745f 5f2e  r......__init__.
+00000710: 0000 0073 0400 0000 0601 0a01 7a0e 546f  ...s........z.To
+00000720: 6b65 6e2e 5f5f 696e 6974 5f5f 6301 0000  ken.__init__c...
+00000730: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000740: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
+00000750: 8301 5300 7228 0000 0029 0272 0500 0000  ..S.r(...).r....
+00000760: 720a 0000 0072 2500 0000 7214 0000 0072  r....r%...r....r
+00000770: 1400 0000 7215 0000 00da 0774 6f5f 6469  ....r......to_di
+00000780: 6374 3200 0000 7302 0000 000a 017a 0d54  ct2...s......z.T
+00000790: 6f6b 656e 2e74 6f5f 6469 6374 6301 0000  oken.to_dictc...
+000007a0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+000007b0: 0043 0000 00f3 0800 0000 7c00 6a00 6a01  .C........|.j.j.
+000007c0: 5300 7228 0000 0029 0272 0a00 0000 da06  S.r(...).r......
+000007d0: 7365 6372 6574 7225 0000 0072 1400 0000  secretr%...r....
+000007e0: 7214 0000 0072 1500 0000 722c 0000 0035  r....r....r,...5
+000007f0: 0000 00f3 0200 0000 0802 7a0c 546f 6b65  ..........z.Toke
+00000800: 6e2e 7365 6372 6574 6301 0000 0000 0000  n.secretc.......
+00000810: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000820: 0072 2b00 0000 7228 0000 0029 0272 0a00  .r+...r(...).r..
+00000830: 0000 7217 0000 0072 2500 0000 7214 0000  ..r....r%...r...
+00000840: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
+00000850: 3900 0000 722d 0000 007a 0d54 6f6b 656e  9...r-...z.Token
+00000860: 2e75 7365 725f 6964 4e29 16da 085f 5f6e  .user_idN)...__n
+00000870: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000880: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000890: 0800 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
+000008a0: 6f6e 735f 5f72 0700 0000 da0b 636c 6173  ons__r......clas
+000008b0: 736d 6574 686f 64da 0373 7472 7216 0000  smethod..strr...
+000008c0: 0072 0300 0000 da04 6c69 7374 721d 0000  .r......listr...
+000008d0: 00da 0369 6e74 7222 0000 0072 2700 0000  ...intr"...r'...
+000008e0: 7229 0000 00da 0464 6963 7472 0200 0000  r).....dictr....
+000008f0: 722a 0000 00da 0870 726f 7065 7274 7972  r*.....propertyr
+00000900: 2c00 0000 7217 0000 0072 1400 0000 7214  ,...r....r....r.
+00000910: 0000 0072 1400 0000 7215 0000 0072 0900  ...r....r....r..
+00000920: 0000 0a00 0000 7340 0000 000a 0008 0108  ......s@........
+00000930: 0102 0218 0102 0402 0106 0102 ff02 0102  ................
+00000940: ff06 020c fe02 0602 0106 0202 fe02 0302  ................
+00000950: fd02 0402 fc06 0502 fb02 060c fa08 0d12  ................
+00000960: 0616 0402 0314 0102 0318 0172 0900 0000  ...........r....
+00000970: 4e29 0ada 0674 7970 696e 6772 0200 0000  N)...typingr....
+00000980: 7203 0000 00da 0573 6572 6465 7205 0000  r......serder...
+00000990: 00da 0864 656c 6567 6174 6572 0700 0000  ...delegater....
+000009a0: 7211 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+000009b0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+000009c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000009d0: 0073 0a00 0000 1002 0c02 0c01 0c01 1203  .s..............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1680 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,137 +1,146 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 9006 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 e806 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6408 6409 8400 6409 8302 5a0b 640a 5300  d.d...d...Z.d.S.
 00000080: 290b e900 0000 0029 02da 0341 6e79 da08  )......)...Any..
 00000090: 4f70 7469 6f6e 616c e903 0000 0029 01da  Optional.....)..
 000000a0: 1670 7964 616e 7469 635f 6a73 6f6e 6162  .pydantic_jsonab
 000000b0: 6c65 5f64 6963 74e9 0100 0000 2901 da0b  le_dict.....)...
 000000c0: 4f72 6744 656c 6567 6174 6529 01da 034f  OrgDelegate)...O
 000000d0: 7267 2901 da0f 4f72 6749 6e76 6974 6552  rg)...OrgInviteR
 000000e0: 6563 6f72 6463 0000 0000 0000 0000 0000  ecordc..........
-000000f0: 0000 0000 0000 0c00 0000 4000 0000 73be  ..........@...s.
+000000f0: 0000 0000 0000 0c00 0000 4000 0000 73d0  ..........@...s.
 00000100: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
 00000110: 0464 013c 0065 0565 0464 023c 0065 0665  .d.<.e.e.d.<.e.e
-00000120: 0464 033c 0065 0709 0464 1964 0565 0864  .d.<.e...d.d.e.d
+00000120: 0464 033c 0065 0709 0464 1b64 0565 0864  .d.<.e...d.d.e.d
 00000130: 0665 0864 0765 0364 0865 0965 0819 0064  .e.d.e.d.e.e...d
 00000140: 0964 0066 0a64 0a64 0b84 0583 015a 0a65  .d.f.d.d.....Z.e
-00000150: 0709 0464 1964 0c65 0864 0765 0364 0d65  ...d.d.e.d.e.d.e
+00000150: 0709 0464 1b64 0c65 0864 0765 0364 0d65  ...d.d.e.d.e.d.e
 00000160: 0965 0819 0066 0664 0e64 0f84 0583 015a  .e...f.d.d.....Z
 00000170: 0b64 0d65 0965 0819 0066 0264 1064 1184  .d.e.e...f.d.d..
 00000180: 045a 0c64 0d65 0965 0819 0066 0264 1264  .Z.d.e.e...f.d.d
-00000190: 1384 045a 0d64 1465 0664 0765 0366 0464  ...Z.d.e.d.e.f.d
-000001a0: 1564 1684 045a 0e64 0965 0f65 0865 1066  .d...Z.d.e.e.e.f
-000001b0: 0219 0066 0264 1764 1884 045a 1164 0453  ...f.d.d...Z.d.S
-000001c0: 0029 1ada 094f 7267 496e 7669 7465 da18  .)...OrgInvite..
-000001d0: 5f4f 7267 496e 7669 7465 5f5f 6f72 675f  _OrgInvite__org_
-000001e0: 6465 6c65 6761 7465 da0f 5f4f 7267 496e  delegate.._OrgIn
-000001f0: 7669 7465 5f5f 6f72 67da 125f 4f72 6749  vite__org.._OrgI
-00000200: 6e76 6974 655f 5f72 6563 6f72 644e da0f  nvite__recordN..
-00000210: 696e 7669 7465 645f 7573 6572 5f69 64da  invited_user_id.
-00000220: 066f 7267 5f69 64da 0c6f 7267 5f64 656c  .org_id..org_del
-00000230: 6567 6174 65da 1069 6e76 6974 696e 675f  egate..inviting_
-00000240: 7573 6572 5f69 64da 0672 6574 7572 6e63  user_id..returnc
-00000250: 0500 0000 0000 0000 0000 0000 0600 0000  ................
-00000260: 0500 0000 4300 0000 731c 0000 007c 036a  ....C...s....|.j
-00000270: 007c 017c 047c 0264 018d 037d 057c 007c  .|.|.|.d...}.|.|
-00000280: 057c 0364 028d 0253 0029 034e 2903 720e  .|.d...S.).N).r.
-00000290: 0000 0072 1100 0000 720f 0000 00a9 02da  ...r....r.......
-000002a0: 0672 6563 6f72 6472 1000 0000 2901 da12  .recordr....)...
-000002b0: 696e 7669 7465 5f75 7365 725f 746f 5f6f  invite_user_to_o
-000002c0: 7267 2906 da03 636c 7372 0e00 0000 720f  rg)...clsr....r.
-000002d0: 0000 0072 1000 0000 7211 0000 0072 1400  ...r....r....r..
-000002e0: 0000 a900 7217 0000 00fa ee2f 636f 6465  ....r....../code
-000002f0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000300: 3334 3937 3236 3836 3730 2f73 7263 2f63  3497268670/src/c
-00000310: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
-00000320: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
-00000330: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
-00000340: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
-00000350: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
-00000360: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
-00000370: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
-00000380: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
-00000390: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
-000003a0: 6b61 6765 732f 726f 626f 746f 5f73 646b  kages/roboto_sdk
-000003b0: 2f73 7263 2f72 6f62 6f74 6f5f 7364 6b2f  /src/roboto_sdk/
-000003c0: 646f 6d61 696e 2f6f 7267 732f 6f72 675f  domain/orgs/org_
-000003d0: 696e 7669 7465 2e70 79da 0663 7265 6174  invite.py..creat
-000003e0: 6510 0000 0073 0c00 0000 0408 0201 0201  e....s..........
-000003f0: 0201 06fd 0c05 7a10 4f72 6749 6e76 6974  ......z.OrgInvit
-00000400: 652e 6372 6561 7465 da09 696e 7669 7465  e.create..invite
-00000410: 5f69 64da 0775 7365 725f 6964 6304 0000  _id..user_idc...
-00000420: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00000430: 0043 0000 0073 1a00 0000 7c02 6a00 7c01  .C...s....|.j.|.
-00000440: 7c03 6401 8d02 7d04 7c00 7c04 7c02 6402  |.d...}.|.|.|.d.
-00000450: 8d02 5300 2903 4ea9 0272 1a00 0000 721b  ..S.).N..r....r.
-00000460: 0000 0072 1300 0000 2901 da0e 6765 745f  ...r....)...get_
-00000470: 6f72 675f 696e 7669 7465 2905 7216 0000  org_invite).r...
-00000480: 0072 1a00 0000 7210 0000 0072 1b00 0000  .r....r....r....
-00000490: 7214 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-000004a0: 1800 0000 da05 6279 5f69 641f 0000 0073  ......by_id....s
-000004b0: 0400 0000 0e04 0c01 7a0f 4f72 6749 6e76  ........z.OrgInv
-000004c0: 6974 652e 6279 5f69 6463 0200 0000 0000  ite.by_idc......
-000004d0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000004e0: 0000 f318 0000 007c 006a 006a 017c 006a  .......|.j.j.|.j
-000004f0: 026a 037c 0164 018d 0201 0064 0053 00a9  .j.|.d.....d.S..
-00000500: 024e 721c 0000 0029 0472 0b00 0000 da11  .Nr....).r......
-00000510: 6163 6365 7074 5f6f 7267 5f69 6e76 6974  accept_org_invit
-00000520: 6572 0d00 0000 721a 0000 00a9 02da 0473  er....r........s
-00000530: 656c 6672 1b00 0000 7217 0000 0072 1700  elfr....r....r..
-00000540: 0000 7218 0000 00da 0661 6363 6570 7426  ..r......accept&
-00000550: 0000 00f3 0600 0000 0601 0801 0aff 7a10  ..............z.
-00000560: 4f72 6749 6e76 6974 652e 6163 6365 7074  OrgInvite.accept
-00000570: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000580: 0004 0000 0043 0000 0072 1f00 0000 7220  .....C...r....r 
-00000590: 0000 0029 0472 0b00 0000 da12 6465 636c  ...).r......decl
-000005a0: 696e 655f 6f72 675f 696e 7669 7465 720d  ine_org_inviter.
-000005b0: 0000 0072 1a00 0000 7222 0000 0072 1700  ...r....r"...r..
-000005c0: 0000 7217 0000 0072 1800 0000 da07 6465  ..r....r......de
-000005d0: 636c 696e 652b 0000 0072 2500 0000 7a11  cline+...r%...z.
-000005e0: 4f72 6749 6e76 6974 652e 6465 636c 696e  OrgInvite.declin
-000005f0: 6572 1400 0000 6303 0000 0000 0000 0000  er....c.........
-00000600: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000610: 2000 0000 7c01 7c00 5f00 7c02 7c00 5f01   ...|.|._.|.|._.
-00000620: 7402 7c01 6a03 7c02 6401 8d02 7c00 5f04  t.|.j.|.d...|._.
-00000630: 6400 5300 2902 4e72 1300 0000 2905 720d  d.S.).Nr....).r.
-00000640: 0000 0072 0b00 0000 7208 0000 00da 036f  ...r....r......o
-00000650: 7267 720c 0000 0029 0372 2300 0000 7214  rgr....).r#...r.
-00000660: 0000 0072 1000 0000 7217 0000 0072 1700  ...r....r....r..
-00000670: 0000 7218 0000 00da 085f 5f69 6e69 745f  ..r......__init_
-00000680: 5f30 0000 0073 0600 0000 0601 0601 1401  _0...s..........
-00000690: 7a12 4f72 6749 6e76 6974 652e 5f5f 696e  z.OrgInvite.__in
-000006a0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-000006b0: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-000006c0: 0000 7400 7c00 6a01 8301 5300 a901 4e29  ..t.|.j...S...N)
-000006d0: 0272 0500 0000 720d 0000 0029 0172 2300  .r....r....).r#.
-000006e0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000006f0: 00da 0774 6f5f 6469 6374 3500 0000 7302  ...to_dict5...s.
-00000700: 0000 000a 017a 114f 7267 496e 7669 7465  .....z.OrgInvite
-00000710: 2e74 6f5f 6469 6374 722a 0000 0029 12da  .to_dictr*...)..
-00000720: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000730: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000740: 655f 5f72 0700 0000 da0f 5f5f 616e 6e6f  e__r......__anno
-00000750: 7461 7469 6f6e 735f 5f72 0800 0000 7209  tations__r....r.
-00000760: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
-00000770: da03 7374 7272 0300 0000 7219 0000 0072  ..strr....r....r
-00000780: 1e00 0000 7224 0000 0072 2700 0000 7229  ....r$...r'...r)
-00000790: 0000 00da 0464 6963 7472 0200 0000 722b  .....dictr....r+
-000007a0: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-000007b0: 0000 7218 0000 0072 0a00 0000 0b00 0000  ..r....r........
-000007c0: 733c 0000 000a 0008 0108 0108 0102 0202  s<..............
-000007d0: 0604 fb02 0202 fe02 0302 fd02 0402 fc06  ................
-000007e0: 0502 fb02 060c fa02 0e02 0204 ff02 0102  ................
-000007f0: ff02 0102 ff06 010c ff12 0612 0512 051a  ................
-00000800: 0572 0a00 0000 4e29 0cda 0674 7970 696e  .r....N)...typin
-00000810: 6772 0200 0000 7203 0000 00da 0573 6572  gr....r......ser
-00000820: 6465 7205 0000 00da 0864 656c 6567 6174  der......delegat
-00000830: 6572 0700 0000 7228 0000 0072 0800 0000  er....r(...r....
-00000840: 7214 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000850: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000860: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000870: 0073 0c00 0000 1002 0c02 0c01 0c01 0c01  .s..............
-00000880: 1203                                     ..
+00000190: 1384 045a 0d65 0e64 0965 0866 0264 1464  ...Z.e.d.e.f.d.d
+000001a0: 1584 0483 015a 0f64 1665 0664 0765 0366  .....Z.d.e.d.e.f
+000001b0: 0464 1764 1884 045a 1064 0965 1165 0865  .d.d...Z.d.e.e.e
+000001c0: 1266 0219 0066 0264 1964 1a84 045a 1364  .f...f.d.d...Z.d
+000001d0: 0453 0029 1cda 094f 7267 496e 7669 7465  .S.)...OrgInvite
+000001e0: da18 5f4f 7267 496e 7669 7465 5f5f 6f72  .._OrgInvite__or
+000001f0: 675f 6465 6c65 6761 7465 da0f 5f4f 7267  g_delegate.._Org
+00000200: 496e 7669 7465 5f5f 6f72 67da 125f 4f72  Invite__org.._Or
+00000210: 6749 6e76 6974 655f 5f72 6563 6f72 644e  gInvite__recordN
+00000220: da0f 696e 7669 7465 645f 7573 6572 5f69  ..invited_user_i
+00000230: 64da 066f 7267 5f69 64da 0c6f 7267 5f64  d..org_id..org_d
+00000240: 656c 6567 6174 65da 1069 6e76 6974 696e  elegate..invitin
+00000250: 675f 7573 6572 5f69 64da 0672 6574 7572  g_user_id..retur
+00000260: 6e63 0500 0000 0000 0000 0000 0000 0600  nc..............
+00000270: 0000 0500 0000 4300 0000 731c 0000 007c  ......C...s....|
+00000280: 036a 007c 017c 047c 0264 018d 037d 057c  .j.|.|.|.d...}.|
+00000290: 007c 057c 0364 028d 0253 0029 034e 2903  .|.|.d...S.).N).
+000002a0: 720e 0000 0072 1100 0000 720f 0000 00a9  r....r....r.....
+000002b0: 02da 0672 6563 6f72 6472 1000 0000 2901  ...recordr....).
+000002c0: da12 696e 7669 7465 5f75 7365 725f 746f  ..invite_user_to
+000002d0: 5f6f 7267 2906 da03 636c 7372 0e00 0000  _org)...clsr....
+000002e0: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000002f0: 1400 0000 a900 7217 0000 00fa ee2f 636f  ......r....../co
+00000300: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
+00000310: 7263 3136 3839 3135 3533 3939 2f73 7263  rc1689155399/src
+00000320: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
+00000330: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
+00000340: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
+00000350: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
+00000360: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
+00000370: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
+00000380: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
+00000390: 3964 2f72 6f62 6f74 6f2d 6169 2f72 6f62  9d/roboto-ai/rob
+000003a0: 6f74 6f2d 686f 7374 6564 2d61 7070 2f70  oto-hosted-app/p
+000003b0: 6163 6b61 6765 732f 726f 626f 746f 5f73  ackages/roboto_s
+000003c0: 646b 2f73 7263 2f72 6f62 6f74 6f5f 7364  dk/src/roboto_sd
+000003d0: 6b2f 646f 6d61 696e 2f6f 7267 732f 6f72  k/domain/orgs/or
+000003e0: 675f 696e 7669 7465 2e70 79da 0663 7265  g_invite.py..cre
+000003f0: 6174 6510 0000 0073 0c00 0000 0408 0201  ate....s........
+00000400: 0201 0201 06fd 0c05 7a10 4f72 6749 6e76  ........z.OrgInv
+00000410: 6974 652e 6372 6561 7465 da09 696e 7669  ite.create..invi
+00000420: 7465 5f69 64da 0775 7365 725f 6964 6304  te_id..user_idc.
+00000430: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00000440: 0000 0043 0000 0073 1a00 0000 7c02 6a00  ...C...s....|.j.
+00000450: 7c01 7c03 6401 8d02 7d04 7c00 7c04 7c02  |.|.d...}.|.|.|.
+00000460: 6402 8d02 5300 2903 4ea9 0272 1a00 0000  d...S.).N..r....
+00000470: 721b 0000 0072 1300 0000 2901 da0e 6765  r....r....)...ge
+00000480: 745f 6f72 675f 696e 7669 7465 2905 7216  t_org_invite).r.
+00000490: 0000 0072 1a00 0000 7210 0000 0072 1b00  ...r....r....r..
+000004a0: 0000 7214 0000 0072 1700 0000 7217 0000  ..r....r....r...
+000004b0: 0072 1800 0000 da07 6672 6f6d 5f69 641f  .r......from_id.
+000004c0: 0000 0073 0400 0000 0e04 0c01 7a11 4f72  ...s........z.Or
+000004d0: 6749 6e76 6974 652e 6672 6f6d 5f69 6463  gInvite.from_idc
+000004e0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000004f0: 0400 0000 4300 0000 f318 0000 007c 006a  ....C........|.j
+00000500: 006a 017c 006a 026a 037c 0164 018d 0201  .j.|.j.j.|.d....
+00000510: 0064 0053 00a9 024e 721c 0000 0029 0472  .d.S...Nr....).r
+00000520: 0b00 0000 da11 6163 6365 7074 5f6f 7267  ......accept_org
+00000530: 5f69 6e76 6974 6572 0d00 0000 721a 0000  _inviter....r...
+00000540: 00a9 02da 0473 656c 6672 1b00 0000 7217  .....selfr....r.
+00000550: 0000 0072 1700 0000 7218 0000 00da 0661  ...r....r......a
+00000560: 6363 6570 7426 0000 00f3 0600 0000 0601  ccept&..........
+00000570: 0801 0aff 7a10 4f72 6749 6e76 6974 652e  ....z.OrgInvite.
+00000580: 6163 6365 7074 6302 0000 0000 0000 0000  acceptc.........
+00000590: 0000 0002 0000 0004 0000 0043 0000 0072  ...........C...r
+000005a0: 1f00 0000 7220 0000 0029 0472 0b00 0000  ....r ...).r....
+000005b0: da12 6465 636c 696e 655f 6f72 675f 696e  ..decline_org_in
+000005c0: 7669 7465 720d 0000 0072 1a00 0000 7222  viter....r....r"
+000005d0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+000005e0: 0000 da07 6465 636c 696e 652b 0000 0072  ....decline+...r
+000005f0: 2500 0000 7a11 4f72 6749 6e76 6974 652e  %...z.OrgInvite.
+00000600: 6465 636c 696e 6563 0100 0000 0000 0000  declinec........
+00000610: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000620: 7308 0000 007c 006a 006a 0153 00a9 014e  s....|.j.j.S...N
+00000630: 2902 720d 0000 0072 1a00 0000 a901 7223  ).r....r......r#
+00000640: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000650: 0000 721a 0000 0030 0000 0073 0200 0000  ..r....0...s....
+00000660: 0802 7a13 4f72 6749 6e76 6974 652e 696e  ..z.OrgInvite.in
+00000670: 7669 7465 5f69 6472 1400 0000 6303 0000  vite_idr....c...
+00000680: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00000690: 0043 0000 0073 2000 0000 7c01 7c00 5f00  .C...s ...|.|._.
+000006a0: 7c02 7c00 5f01 7402 7c01 6a03 7c02 6401  |.|._.t.|.j.|.d.
+000006b0: 8d02 7c00 5f04 6400 5300 2902 4e72 1300  ..|._.d.S.).Nr..
+000006c0: 0000 2905 720d 0000 0072 0b00 0000 7208  ..).r....r....r.
+000006d0: 0000 00da 036f 7267 720c 0000 0029 0372  .....orgr....).r
+000006e0: 2300 0000 7214 0000 0072 1000 0000 7217  #...r....r....r.
+000006f0: 0000 0072 1700 0000 7218 0000 00da 085f  ...r....r......_
+00000700: 5f69 6e69 745f 5f34 0000 0073 0600 0000  _init__4...s....
+00000710: 0601 0601 1401 7a12 4f72 6749 6e76 6974  ......z.OrgInvit
+00000720: 652e 5f5f 696e 6974 5f5f 6301 0000 0000  e.__init__c.....
+00000730: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000740: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
+00000750: 5300 7228 0000 0029 0272 0500 0000 720d  S.r(...).r....r.
+00000760: 0000 0072 2900 0000 7217 0000 0072 1700  ...r)...r....r..
+00000770: 0000 7218 0000 00da 0774 6f5f 6469 6374  ..r......to_dict
+00000780: 3900 0000 7302 0000 000a 017a 114f 7267  9...s......z.Org
+00000790: 496e 7669 7465 2e74 6f5f 6469 6374 7228  Invite.to_dictr(
+000007a0: 0000 0029 14da 085f 5f6e 616d 655f 5fda  ...)...__name__.
+000007b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000007c0: 7561 6c6e 616d 655f 5f72 0700 0000 da0f  ualname__r......
+000007d0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+000007e0: 0800 0000 7209 0000 00da 0b63 6c61 7373  ....r......class
+000007f0: 6d65 7468 6f64 da03 7374 7272 0300 0000  method..strr....
+00000800: 7219 0000 0072 1e00 0000 7224 0000 0072  r....r....r$...r
+00000810: 2700 0000 da08 7072 6f70 6572 7479 721a  '.....propertyr.
+00000820: 0000 0072 2b00 0000 da04 6469 6374 7202  ...r+.....dictr.
+00000830: 0000 0072 2c00 0000 7217 0000 0072 1700  ...r,...r....r..
+00000840: 0000 7217 0000 0072 1800 0000 720a 0000  ..r....r....r...
+00000850: 000b 0000 0073 4000 0000 0a00 0801 0801  .....s@.........
+00000860: 0801 0202 0206 04fb 0202 02fe 0203 02fd  ................
+00000870: 0204 02fc 0605 02fb 0206 0cfa 020e 0202  ................
+00000880: 04ff 0201 02ff 0201 02ff 0601 0cff 1206  ................
+00000890: 1205 0205 1001 1203 1a05 720a 0000 004e  ..........r....N
+000008a0: 290c da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
+000008b0: 0300 0000 da05 7365 7264 6572 0500 0000  ......serder....
+000008c0: da08 6465 6c65 6761 7465 7207 0000 0072  ..delegater....r
+000008d0: 2a00 0000 7208 0000 0072 1400 0000 7209  *...r....r....r.
+000008e0: 0000 0072 0a00 0000 7217 0000 0072 1700  ...r....r....r..
+000008f0: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
+00000900: 6f64 756c 653e 0100 0000 730c 0000 0010  odule>....s.....
+00000910: 020c 020c 010c 010c 0112 03              ...........
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1432 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 9805 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 d706 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 8302 5a0c  ..G.d.d...d...Z.
@@ -10,142 +10,158 @@
 00000090: 6e79 da08 4f70 7469 6f6e 616c e903 0000  ny..Optional....
 000000a0: 0029 01da 1670 7964 616e 7469 635f 6a73  .)...pydantic_js
 000000b0: 6f6e 6162 6c65 5f64 6963 74e9 0100 0000  onable_dict.....
 000000c0: 2901 da0b 4f72 6744 656c 6567 6174 6529  )...OrgDelegate)
 000000d0: 01da 034f 7267 2902 da0b 4f72 6752 6f6c  ...Org)...OrgRol
 000000e0: 654e 616d 65da 0d4f 7267 526f 6c65 5265  eName..OrgRoleRe
 000000f0: 636f 7264 6300 0000 0000 0000 0000 0000  cordc...........
-00000100: 0000 0000 0008 0000 0040 0000 0073 cc00  .........@...s..
+00000100: 0000 0000 0009 0000 0040 0000 0073 f400  .........@...s..
 00000110: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
 00000120: 6401 3c00 6505 6504 6402 3c00 6506 6504  d.<.e.e.d.<.e.e.
 00000130: 6403 3c00 6507 6404 6508 6509 1900 6405  d.<.e.d.e.e...d.
 00000140: 6505 6406 650a 6400 1900 6606 6407 6408  e.d.e.d...f.d.d.
 00000150: 8404 8301 5a0b 6507 6409 6508 6509 1900  ....Z.e.d.e.e...
 00000160: 6405 6505 6406 650a 6400 1900 6606 640a  d.e.d.e.d...f.d.
-00000170: 640b 8404 8301 5a0c 640c 6503 6405 6505  d.....Z.d.e.d.e.
-00000180: 6604 640d 640e 8404 5a0d 6406 650e 6509  f.d.d...Z.d.e.e.
-00000190: 650f 6602 1900 6602 640f 6410 8404 5a10  e.f...f.d.d...Z.
-000001a0: 6511 6406 6509 6602 6411 6412 8404 8301  e.d.e.f.d.d.....
-000001b0: 5a12 6511 6406 6506 6602 6413 6414 8404  Z.e.d.e.f.d.d...
-000001c0: 8301 5a13 6511 6406 650a 6514 1900 6602  ..Z.e.d.e.e...f.
-000001d0: 6415 6416 8404 8301 5a15 6417 5300 2918  d.d.....Z.d.S.).
-000001e0: da07 4f72 6752 6f6c 65da 105f 4f72 6752  ..OrgRole.._OrgR
-000001f0: 6f6c 655f 5f72 6563 6f72 64da 165f 4f72  ole__record.._Or
-00000200: 6752 6f6c 655f 5f6f 7267 5f64 656c 6567  gRole__org_deleg
-00000210: 6174 65da 0d5f 4f72 6752 6f6c 655f 5f6f  ate.._OrgRole__o
-00000220: 7267 da07 7573 6572 5f69 64da 0c6f 7267  rg..user_id..org
-00000230: 5f64 656c 6567 6174 65da 0672 6574 7572  _delegate..retur
-00000240: 6e63 0300 0000 0000 0000 0000 0000 0400  nc..............
-00000250: 0000 0300 0000 0300 0000 f320 0000 0088  ........... ....
-00000260: 016a 007c 0164 018d 017d 0387 0087 0166  .j.|.d...}.....f
-00000270: 0264 0264 0384 087c 0344 0083 0153 0029  .d.d...|.D...S.)
-00000280: 044e 2901 720f 0000 0063 0100 0000 0000  .N).r....c......
-00000290: 0000 0000 0000 0200 0000 0600 0000 1300  ................
-000002a0: 0000 f318 0000 0067 007c 005d 087d 0188  .......g.|.].}..
-000002b0: 007c 0188 0164 008d 0291 0271 0253 00a9  .|...d.....q.S..
-000002c0: 01a9 02da 0672 6563 6f72 6472 1000 0000  .....recordr....
-000002d0: a900 a902 da02 2e30 7216 0000 00a9 02da  .......0r.......
-000002e0: 0363 6c73 7210 0000 0072 1700 0000 faec  .clsr....r......
-000002f0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000300: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
-00000310: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
-00000320: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
-00000330: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
-00000340: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
-00000350: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
-00000360: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
-00000370: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
-00000380: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
-00000390: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
-000003a0: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
-000003b0: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
-000003c0: 5f73 646b 2f64 6f6d 6169 6e2f 6f72 6773  _sdk/domain/orgs
-000003d0: 2f6f 7267 5f72 6f6c 652e 7079 da0a 3c6c  /org_role.py..<l
-000003e0: 6973 7463 6f6d 703e 1500 0000 f302 0000  istcomp>........
-000003f0: 0018 007a 264f 7267 526f 6c65 2e62 795f  ...z&OrgRole.by_
-00000400: 7573 6572 5f69 642e 3c6c 6f63 616c 733e  user_id.<locals>
-00000410: 2e3c 6c69 7374 636f 6d70 3e29 01da 126f  .<listcomp>)...o
-00000420: 7267 5f72 6f6c 6573 5f66 6f72 5f75 7365  rg_roles_for_use
-00000430: 7229 0472 1b00 0000 720f 0000 0072 1000  r).r....r....r..
-00000440: 0000 da07 7265 636f 7264 7372 1700 0000  ....recordsr....
-00000450: 721a 0000 0072 1c00 0000 da0a 6279 5f75  r....r......by_u
-00000460: 7365 725f 6964 1000 0000 f304 0000 000c  ser_id..........
-00000470: 0414 017a 124f 7267 526f 6c65 2e62 795f  ...z.OrgRole.by_
-00000480: 7573 6572 5f69 64da 066f 7267 5f69 6463  user_id..org_idc
-00000490: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-000004a0: 0300 0000 0300 0000 7212 0000 0029 044e  ........r....).N
-000004b0: 2901 7223 0000 0063 0100 0000 0000 0000  ).r#...c........
-000004c0: 0000 0000 0200 0000 0600 0000 1300 0000  ................
-000004d0: 7213 0000 0072 1400 0000 7217 0000 0072  r....r....r....r
-000004e0: 1800 0000 721a 0000 0072 1700 0000 721c  ....r....r....r.
-000004f0: 0000 0072 1d00 0000 1c00 0000 721e 0000  ...r........r...
-00000500: 007a 254f 7267 526f 6c65 2e62 795f 6f72  .z%OrgRole.by_or
-00000510: 675f 6964 2e3c 6c6f 6361 6c73 3e2e 3c6c  g_id.<locals>.<l
-00000520: 6973 7463 6f6d 703e 2901 da11 6f72 675f  istcomp>)...org_
-00000530: 726f 6c65 735f 666f 725f 6f72 6729 0472  roles_for_org).r
-00000540: 1b00 0000 7223 0000 0072 1000 0000 7220  ....r#...r....r 
-00000550: 0000 0072 1700 0000 721a 0000 0072 1c00  ...r....r....r..
-00000560: 0000 da09 6279 5f6f 7267 5f69 6417 0000  ....by_org_id...
-00000570: 0072 2200 0000 7a11 4f72 6752 6f6c 652e  .r"...z.OrgRole.
-00000580: 6279 5f6f 7267 5f69 6472 1600 0000 6303  by_org_idr....c.
-00000590: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000005a0: 0000 0043 0000 0073 2000 0000 7c01 7c00  ...C...s ...|.|.
-000005b0: 5f00 7c02 7c00 5f01 7402 7c01 6a03 7c02  _.|.|._.t.|.j.|.
-000005c0: 6401 8d02 7c00 5f04 6400 5300 2902 4e72  d...|._.d.S.).Nr
-000005d0: 1500 0000 2905 720c 0000 0072 0d00 0000  ....).r....r....
-000005e0: 7208 0000 00da 036f 7267 720e 0000 0029  r......orgr....)
-000005f0: 03da 0473 656c 6672 1600 0000 7210 0000  ...selfr....r...
-00000600: 0072 1700 0000 7217 0000 0072 1c00 0000  .r....r....r....
-00000610: da08 5f5f 696e 6974 5f5f 1e00 0000 7306  ..__init__....s.
-00000620: 0000 0006 0106 0114 017a 104f 7267 526f  .........z.OrgRo
-00000630: 6c65 2e5f 5f69 6e69 745f 5f63 0100 0000  le.__init__c....
-00000640: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000650: 4300 0000 730a 0000 0074 007c 006a 0183  C...s....t.|.j..
-00000660: 0153 00a9 014e 2902 7205 0000 0072 0c00  .S...N).r....r..
-00000670: 0000 a901 7227 0000 0072 1700 0000 7217  ....r'...r....r.
-00000680: 0000 0072 1c00 0000 da07 746f 5f64 6963  ...r......to_dic
-00000690: 7423 0000 0073 0200 0000 0a01 7a0f 4f72  t#...s......z.Or
-000006a0: 6752 6f6c 652e 746f 5f64 6963 7463 0100  gRole.to_dictc..
-000006b0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000006c0: 0000 4300 0000 730a 0000 007c 006a 006a  ..C...s....|.j.j
-000006d0: 016a 0253 0072 2900 0000 2903 720c 0000  .j.S.r)...).r...
-000006e0: 0072 2600 0000 7223 0000 0072 2a00 0000  .r&...r#...r*...
-000006f0: 7217 0000 0072 1700 0000 721c 0000 0072  r....r....r....r
-00000700: 2300 0000 2600 0000 7302 0000 000a 027a  #...&...s......z
-00000710: 0e4f 7267 526f 6c65 2e6f 7267 5f69 6463  .OrgRole.org_idc
-00000720: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000730: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
-00000740: 0053 0072 2900 0000 2901 720e 0000 0072  .S.r)...).r....r
-00000750: 2a00 0000 7217 0000 0072 1700 0000 721c  *...r....r....r.
-00000760: 0000 0072 2600 0000 2a00 0000 7302 0000  ...r&...*...s...
-00000770: 0006 027a 0b4f 7267 526f 6c65 2e6f 7267  ...z.OrgRole.org
-00000780: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000790: 0001 0000 0043 0000 0073 0800 0000 7c00  .....C...s....|.
-000007a0: 6a00 6a01 5300 7229 0000 0029 0272 0c00  j.j.S.r)...).r..
-000007b0: 0000 da05 726f 6c65 7372 2a00 0000 7217  ....rolesr*...r.
-000007c0: 0000 0072 1700 0000 721c 0000 0072 2c00  ...r....r....r,.
-000007d0: 0000 2e00 0000 7302 0000 0008 027a 0d4f  ......s......z.O
-000007e0: 7267 526f 6c65 2e72 6f6c 6573 4e29 16da  rgRole.rolesN)..
-000007f0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000800: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000810: 655f 5f72 0a00 0000 da0f 5f5f 616e 6e6f  e__r......__anno
-00000820: 7461 7469 6f6e 735f 5f72 0700 0000 7208  tations__r....r.
-00000830: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
-00000840: 7203 0000 00da 0373 7472 da04 6c69 7374  r......str..list
-00000850: 7221 0000 0072 2500 0000 7228 0000 00da  r!...r%...r(....
-00000860: 0464 6963 7472 0200 0000 722b 0000 00da  .dictr....r+....
-00000870: 0870 726f 7065 7274 7972 2300 0000 7226  .propertyr#...r&
-00000880: 0000 0072 0900 0000 722c 0000 0072 1700  ...r....r,...r..
-00000890: 0000 7217 0000 0072 1700 0000 721c 0000  ..r....r....r...
-000008a0: 0072 0b00 0000 0b00 0000 7338 0000 000a  .r........s8....
-000008b0: 0008 0108 0108 0102 0202 0106 0102 ff02  ................
-000008c0: 0102 ff06 020c fe02 0602 0106 0102 ff02  ................
-000008d0: 0102 ff06 020c fe12 0616 0502 0310 0102  ................
-000008e0: 0310 0102 0318 0172 0b00 0000 4e29 0dda  .......r....N)..
-000008f0: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-00000900: 00da 0573 6572 6465 7205 0000 00da 0864  ...serder......d
-00000910: 656c 6567 6174 6572 0700 0000 7226 0000  elegater....r&..
-00000920: 0072 0800 0000 7216 0000 0072 0900 0000  .r....r....r....
-00000930: 720a 0000 0072 0b00 0000 7217 0000 0072  r....r....r....r
-00000940: 1700 0000 7217 0000 0072 1c00 0000 da08  ....r....r......
-00000950: 3c6d 6f64 756c 653e 0100 0000 730c 0000  <module>....s...
-00000960: 0010 020c 020c 010c 0110 0112 03         .............
+00000170: 640b 8404 8301 5a0c 6507 090c 090c 641a  d.....Z.e.....d.
+00000180: 6405 6505 6404 6508 6509 1900 6409 6508  d.e.d.e.e...d.e.
+00000190: 6509 1900 6606 640d 640e 8405 8301 5a0d  e...f.d.d.....Z.
+000001a0: 640f 6503 6405 6505 6604 6410 6411 8404  d.e.d.e.f.d.d...
+000001b0: 5a0e 6406 650f 6509 6510 6602 1900 6602  Z.d.e.e.e.f...f.
+000001c0: 6412 6413 8404 5a11 6512 6406 6509 6602  d.d...Z.e.d.e.f.
+000001d0: 6414 6415 8404 8301 5a13 6512 6406 6506  d.d.....Z.e.d.e.
+000001e0: 6602 6416 6417 8404 8301 5a14 6512 6406  f.d.d.....Z.e.d.
+000001f0: 650a 6515 1900 6602 6418 6419 8404 8301  e.e...f.d.d.....
+00000200: 5a16 640c 5300 291b da07 4f72 6752 6f6c  Z.d.S.)...OrgRol
+00000210: 65da 105f 4f72 6752 6f6c 655f 5f72 6563  e.._OrgRole__rec
+00000220: 6f72 64da 165f 4f72 6752 6f6c 655f 5f6f  ord.._OrgRole__o
+00000230: 7267 5f64 656c 6567 6174 65da 0d5f 4f72  rg_delegate.._Or
+00000240: 6752 6f6c 655f 5f6f 7267 da07 7573 6572  gRole__org..user
+00000250: 5f69 64da 0c6f 7267 5f64 656c 6567 6174  _id..org_delegat
+00000260: 65da 0672 6574 7572 6e63 0300 0000 0000  e..returnc......
+00000270: 0000 0000 0000 0400 0000 0300 0000 0300  ................
+00000280: 0000 f320 0000 0088 016a 007c 0164 018d  ... .....j.|.d..
+00000290: 017d 0387 0087 0166 0264 0264 0384 087c  .}.....f.d.d...|
+000002a0: 0344 0083 0153 0029 044e 2901 720f 0000  .D...S.).N).r...
+000002b0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+000002c0: 0000 0600 0000 1300 0000 f318 0000 0067  ...............g
+000002d0: 007c 005d 087d 0188 007c 0188 0164 008d  .|.].}...|...d..
+000002e0: 0291 0271 0253 00a9 01a9 02da 0672 6563  ...q.S.......rec
+000002f0: 6f72 6472 1000 0000 a900 a902 da02 2e30  ordr...........0
+00000300: 7216 0000 00a9 02da 0363 6c73 7210 0000  r........clsr...
+00000310: 0072 1700 0000 faec 2f63 6f64 6562 7569  .r....../codebui
+00000320: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+00000330: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+00000340: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
+00000350: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
+00000360: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
+00000370: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
+00000380: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
+00000390: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
+000003a0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
+000003b0: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
+000003c0: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
+000003d0: 6573 2f72 6f62 6f74 6f5f 7364 6b2f 7372  es/roboto_sdk/sr
+000003e0: 632f 726f 626f 746f 5f73 646b 2f64 6f6d  c/roboto_sdk/dom
+000003f0: 6169 6e2f 6f72 6773 2f6f 7267 5f72 6f6c  ain/orgs/org_rol
+00000400: 652e 7079 da0a 3c6c 6973 7463 6f6d 703e  e.py..<listcomp>
+00000410: 1500 0000 f302 0000 0018 007a 244f 7267  ...........z$Org
+00000420: 526f 6c65 2e66 6f72 5f75 7365 722e 3c6c  Role.for_user.<l
+00000430: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000440: 3e29 01da 126f 7267 5f72 6f6c 6573 5f66  >)...org_roles_f
+00000450: 6f72 5f75 7365 7229 0472 1b00 0000 720f  or_user).r....r.
+00000460: 0000 0072 1000 0000 da07 7265 636f 7264  ...r......record
+00000470: 7372 1700 0000 721a 0000 0072 1c00 0000  sr....r....r....
+00000480: da08 666f 725f 7573 6572 1000 0000 f304  ..for_user......
+00000490: 0000 000c 0414 017a 104f 7267 526f 6c65  .......z.OrgRole
+000004a0: 2e66 6f72 5f75 7365 72da 066f 7267 5f69  .for_user..org_i
+000004b0: 6463 0300 0000 0000 0000 0000 0000 0400  dc..............
+000004c0: 0000 0300 0000 0300 0000 7212 0000 0029  ..........r....)
+000004d0: 044e 2901 7223 0000 0063 0100 0000 0000  .N).r#...c......
+000004e0: 0000 0000 0000 0200 0000 0600 0000 1300  ................
+000004f0: 0000 7213 0000 0072 1400 0000 7217 0000  ..r....r....r...
+00000500: 0072 1800 0000 721a 0000 0072 1700 0000  .r....r....r....
+00000510: 721c 0000 0072 1d00 0000 1c00 0000 721e  r....r........r.
+00000520: 0000 007a 234f 7267 526f 6c65 2e66 6f72  ...z#OrgRole.for
+00000530: 5f6f 7267 2e3c 6c6f 6361 6c73 3e2e 3c6c  _org.<locals>.<l
+00000540: 6973 7463 6f6d 703e 2901 da11 6f72 675f  istcomp>)...org_
+00000550: 726f 6c65 735f 666f 725f 6f72 6729 0472  roles_for_org).r
+00000560: 1b00 0000 7223 0000 0072 1000 0000 7220  ....r#...r....r 
+00000570: 0000 0072 1700 0000 721a 0000 0072 1c00  ...r....r....r..
+00000580: 0000 da07 666f 725f 6f72 6717 0000 0072  ....for_org....r
+00000590: 2200 0000 7a0f 4f72 6752 6f6c 652e 666f  "...z.OrgRole.fo
+000005a0: 725f 6f72 674e 6304 0000 0000 0000 0000  r_orgNc.........
+000005b0: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
+000005c0: 1a00 0000 7c01 6a00 7c02 7c03 6401 8d02  ....|.j.|.|.d...
+000005d0: 7d04 7c00 7c04 7c01 6402 8d02 5300 2903  }.|.|.|.d...S.).
+000005e0: 4e29 0272 0f00 0000 7223 0000 0072 1500  N).r....r#...r..
+000005f0: 0000 2901 da18 6f72 675f 726f 6c65 5f66  ..)...org_role_f
+00000600: 6f72 5f75 7365 725f 696e 5f6f 7267 2905  or_user_in_org).
+00000610: 721b 0000 0072 1000 0000 720f 0000 0072  r....r....r....r
+00000620: 2300 0000 7216 0000 0072 1700 0000 7217  #...r....r....r.
+00000630: 0000 0072 1c00 0000 da0f 666f 725f 7573  ...r......for_us
+00000640: 6572 5f69 6e5f 6f72 671e 0000 0073 0400  er_in_org....s..
+00000650: 0000 0e07 0c01 7a17 4f72 6752 6f6c 652e  ......z.OrgRole.
+00000660: 666f 725f 7573 6572 5f69 6e5f 6f72 6772  for_user_in_orgr
+00000670: 1600 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00000680: 0003 0000 0004 0000 0043 0000 0073 2000  .........C...s .
+00000690: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7402  ..|.|._.|.|._.t.
+000006a0: 7c01 6a03 7c02 6401 8d02 7c00 5f04 6400  |.j.|.d...|._.d.
+000006b0: 5300 2902 4e72 1500 0000 2905 720c 0000  S.).Nr....).r...
+000006c0: 0072 0d00 0000 7208 0000 00da 036f 7267  .r....r......org
+000006d0: 720e 0000 0029 03da 0473 656c 6672 1600  r....)...selfr..
+000006e0: 0000 7210 0000 0072 1700 0000 7217 0000  ..r....r....r...
+000006f0: 0072 1c00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+00000700: 2800 0000 7306 0000 0006 0106 0114 017a  (...s..........z
+00000710: 104f 7267 526f 6c65 2e5f 5f69 6e69 745f  .OrgRole.__init_
+00000720: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000730: 0000 0200 0000 4300 0000 730a 0000 0074  ......C...s....t
+00000740: 007c 006a 0183 0153 00a9 014e 2902 7205  .|.j...S...N).r.
+00000750: 0000 0072 0c00 0000 a901 7229 0000 0072  ...r......r)...r
+00000760: 1700 0000 7217 0000 0072 1c00 0000 da07  ....r....r......
+00000770: 746f 5f64 6963 742d 0000 0073 0200 0000  to_dict-...s....
+00000780: 0a01 7a0f 4f72 6752 6f6c 652e 746f 5f64  ..z.OrgRole.to_d
+00000790: 6963 7463 0100 0000 0000 0000 0000 0000  ictc............
+000007a0: 0100 0000 0100 0000 4300 0000 730a 0000  ........C...s...
+000007b0: 007c 006a 006a 016a 0253 0072 2b00 0000  .|.j.j.j.S.r+...
+000007c0: 2903 720c 0000 0072 2800 0000 7223 0000  ).r....r(...r#..
+000007d0: 0072 2c00 0000 7217 0000 0072 1700 0000  .r,...r....r....
+000007e0: 721c 0000 0072 2300 0000 3000 0000 7302  r....r#...0...s.
+000007f0: 0000 000a 027a 0e4f 7267 526f 6c65 2e6f  .....z.OrgRole.o
+00000800: 7267 5f69 6463 0100 0000 0000 0000 0000  rg_idc..........
+00000810: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00000820: 0000 007c 006a 0053 0072 2b00 0000 2901  ...|.j.S.r+...).
+00000830: 720e 0000 0072 2c00 0000 7217 0000 0072  r....r,...r....r
+00000840: 1700 0000 721c 0000 0072 2800 0000 3400  ....r....r(...4.
+00000850: 0000 7302 0000 0006 027a 0b4f 7267 526f  ..s......z.OrgRo
+00000860: 6c65 2e6f 7267 6301 0000 0000 0000 0000  le.orgc.........
+00000870: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
+00000880: 0800 0000 7c00 6a00 6a01 5300 722b 0000  ....|.j.j.S.r+..
+00000890: 0029 0272 0c00 0000 da05 726f 6c65 7372  .).r......rolesr
+000008a0: 2c00 0000 7217 0000 0072 1700 0000 721c  ,...r....r....r.
+000008b0: 0000 0072 2e00 0000 3800 0000 7302 0000  ...r....8...s...
+000008c0: 0008 027a 0d4f 7267 526f 6c65 2e72 6f6c  ...z.OrgRole.rol
+000008d0: 6573 2902 4e4e 2917 da08 5f5f 6e61 6d65  es).NN)...__name
+000008e0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000008f0: 5f5f 7175 616c 6e61 6d65 5f5f 720a 0000  __qualname__r...
+00000900: 00da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  ...__annotations
+00000910: 5f5f 7207 0000 0072 0800 0000 da0b 636c  __r....r......cl
+00000920: 6173 736d 6574 686f 6472 0300 0000 da03  assmethodr......
+00000930: 7374 72da 046c 6973 7472 2100 0000 7225  str..listr!...r%
+00000940: 0000 0072 2700 0000 722a 0000 00da 0464  ...r'...r*.....d
+00000950: 6963 7472 0200 0000 722d 0000 00da 0870  ictr....r-.....p
+00000960: 726f 7065 7274 7972 2300 0000 7228 0000  ropertyr#...r(..
+00000970: 0072 0900 0000 722e 0000 0072 1700 0000  .r....r....r....
+00000980: 7217 0000 0072 1700 0000 721c 0000 0072  r....r....r....r
+00000990: 0b00 0000 0b00 0000 734c 0000 000a 0008  ........sL......
+000009a0: 0108 0108 0102 0202 0106 0102 ff02 0102  ................
+000009b0: ff06 020c fe02 0602 0106 0102 ff02 0102  ................
+000009c0: ff06 020c fe02 0602 0402 0104 fc02 0202  ................
+000009d0: fe06 0302 fd06 040c fc12 0916 0502 0310  ................
+000009e0: 0102 0310 0102 0318 0172 0b00 0000 4e29  .........r....N)
+000009f0: 0dda 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+00000a00: 0000 00da 0573 6572 6465 7205 0000 00da  .....serder.....
+00000a10: 0864 656c 6567 6174 6572 0700 0000 7228  .delegater....r(
+00000a20: 0000 0072 0800 0000 7216 0000 0072 0900  ...r....r....r..
+00000a30: 0000 720a 0000 0072 0b00 0000 7217 0000  ..r....r....r...
+00000a40: 0072 1700 0000 7217 0000 0072 1c00 0000  .r....r....r....
+00000a50: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
+00000a60: 0000 0010 020c 020c 010c 0110 0112 03    ...............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 722 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 d202 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 d602 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6504 6500 6a05 8304 5a06 4700  ..d.e.e.j...Z.G.
 00000060: 6406 6407 8400 6407 6504 6500 6a05 8304  d.d...d.e.e.j...
 00000070: 5a07 4700 6408 6409 8400 6409 6501 6a08  Z.G.d.d...d.e.j.
@@ -17,16 +17,16 @@
 00000100: 0264 015a 0364 025a 0464 0353 0029 04da  .d.Z.d.Z.d.S.)..
 00000110: 074f 7267 5479 7065 da0a 696e 6469 7669  .OrgType..indivi
 00000120: 6475 616c da04 7465 616d 4e29 05da 085f  dual..teamN)..._
 00000130: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000140: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000150: 5f72 0600 0000 7207 0000 00a9 0072 0b00  _r....r......r..
 00000160: 0000 720b 0000 00fa ea2f 636f 6465 6275  ..r....../codebu
-00000170: 696c 642f 6f75 7470 7574 2f73 7263 3334  ild/output/src34
-00000180: 3937 3236 3836 3730 2f73 7263 2f63 6f64  97268670/src/cod
+00000170: 696c 642f 6f75 7470 7574 2f73 7263 3136  ild/output/src16
+00000180: 3839 3135 3533 3939 2f73 7263 2f63 6f64  89155399/src/cod
 00000190: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 000001a0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000001b0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000001c0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000001d0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 000001e0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000001f0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
@@ -71,37 +71,37 @@
 00000460: 0000 720c 0000 0072 1900 0000 1c00 0000  ..r....r........
 00000470: 7308 0000 0008 0004 0104 0108 0172 1900  s............r..
 00000480: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000490: 0000 0003 0000 0040 0000 0073 2a00 0000  .......@...s*...
 000004a0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 000004b0: 3c00 6505 6504 6402 3c00 6506 6507 1900  <.e.e.d.<.e.e...
 000004c0: 6504 6403 3c00 6404 5300 2905 da0d 4f72  e.d.<.d.S.)...Or
-000004d0: 6752 6f6c 6552 6563 6f72 64da 0775 7365  gRoleRecord..use
-000004e0: 725f 6964 da03 6f72 675a 0572 6f6c 6573  r_id..orgZ.roles
-000004f0: 4e29 0872 0800 0000 7209 0000 0072 0a00  N).r....r....r..
-00000500: 0000 7216 0000 0072 1700 0000 7211 0000  ..r....r....r...
-00000510: 00da 046c 6973 7472 1900 0000 720b 0000  ...listr....r...
-00000520: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000530: 721d 0000 0022 0000 0073 0800 0000 0a00  r...."...s......
-00000540: 0801 0801 1001 721d 0000 0063 0000 0000  ......r....c....
-00000550: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000560: 4000 0000 732e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000570: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
-00000580: 023c 0065 0565 0464 033c 0065 0665 0464  .<.e.e.d.<.e.e.d
-00000590: 043c 0064 0553 0029 06da 0f4f 7267 496e  .<.d.S.)...OrgIn
-000005a0: 7669 7465 5265 636f 7264 da09 696e 7669  viteRecord..invi
-000005b0: 7465 5f69 6472 1e00 0000 5a0a 696e 7669  te_idr....Z.invi
-000005c0: 7465 645f 6279 721f 0000 004e 2907 7208  ted_byr....N).r.
+000004d0: 6752 6f6c 6552 6563 6f72 6472 1a00 0000  gRoleRecordr....
+000004e0: da03 6f72 675a 0572 6f6c 6573 4e29 0872  ..orgZ.rolesN).r
+000004f0: 0800 0000 7209 0000 0072 0a00 0000 7203  ....r....r....r.
+00000500: 0000 0072 1700 0000 7211 0000 00da 046c  ...r....r......l
+00000510: 6973 7472 1900 0000 720b 0000 0072 0b00  istr....r....r..
+00000520: 0000 720b 0000 0072 0c00 0000 721d 0000  ..r....r....r...
+00000530: 0022 0000 0073 0800 0000 0a00 0801 0801  ."...s..........
+00000540: 1001 721d 0000 0063 0000 0000 0000 0000  ..r....c........
+00000550: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000560: 732e 0000 0065 005a 0164 005a 0255 0065  s....e.Z.d.Z.U.e
+00000570: 0365 0464 013c 0065 0365 0464 023c 0065  .e.d.<.e.e.d.<.e
+00000580: 0565 0464 033c 0065 0665 0464 043c 0064  .e.d.<.e.e.d.<.d
+00000590: 0553 0029 06da 0f4f 7267 496e 7669 7465  .S.)...OrgInvite
+000005a0: 5265 636f 7264 da09 696e 7669 7465 5f69  Record..invite_i
+000005b0: 64da 0775 7365 725f 6964 5a0a 696e 7669  d..user_idZ.invi
+000005c0: 7465 645f 6279 721e 0000 004e 2907 7208  ted_byr....N).r.
 000005d0: 0000 0072 0900 0000 720a 0000 0072 1600  ...r....r....r..
 000005e0: 0000 7217 0000 0072 0300 0000 7211 0000  ..r....r....r...
 000005f0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000600: 720c 0000 0072 2100 0000 2800 0000 730a  r....r!...(...s.
-00000610: 0000 000a 0008 0108 0108 010c 0172 2100  .............r!.
+00000600: 720c 0000 0072 2000 0000 2800 0000 730a  r....r ...(...s.
+00000610: 0000 000a 0008 0108 0108 010c 0172 2000  .............r .
 00000620: 0000 290d da04 656e 756d da08 7079 6461  ..)...enum..pyda
 00000630: 6e74 6963 da05 7573 6572 7372 0300 0000  ntic..usersr....
 00000640: 7216 0000 00da 0445 6e75 6d72 0500 0000  r......Enumr....
 00000650: 720e 0000 00da 0942 6173 654d 6f64 656c  r......BaseModel
 00000660: 7211 0000 0072 1900 0000 721d 0000 0072  r....r....r....r
-00000670: 2100 0000 720b 0000 0072 0b00 0000 720b  !...r....r....r.
+00000670: 2000 0000 720b 0000 0072 0b00 0000 720b   ...r....r....r.
 00000680: 0000 0072 0c00 0000 da08 3c6d 6f64 756c  ...r......<modul
 00000690: 653e 0100 0000 7312 0000 0008 0208 020c  e>....s.........
 000006a0: 0214 0314 0512 0514 0812 0616 06         .............
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import abc
 from typing import Optional
 
 from .record import (
     OrgInviteRecord,
     OrgRecord,
+    OrgRoleName,
     OrgRoleRecord,
     OrgType,
 )
 
 
 class OrgDelegate(abc.ABC):
     @abc.abstractmethod
@@ -31,14 +32,36 @@
         raise NotImplementedError("org_roles_for_user")
 
     @abc.abstractmethod
     def org_roles_for_org(self, org_id: Optional[str]) -> list[OrgRoleRecord]:
         raise NotImplementedError("org_roles_for_org")
 
     @abc.abstractmethod
+    def org_role_for_user_in_org(
+        self, user_id: Optional[str] = None, org_id: Optional[str] = None
+    ) -> OrgRoleRecord:
+        raise NotImplementedError("org_role_for_user_in_org")
+
+    @abc.abstractmethod
+    def add_role_for_user(
+        self, user_id: str, role_name: OrgRoleName, org_id: Optional[str] = None
+    ):
+        raise NotImplementedError("add_role_for_user")
+
+    @abc.abstractmethod
+    def remove_role_from_user(
+        self, user_id: str, role_name: OrgRoleName, org_id: Optional[str] = None
+    ):
+        raise NotImplementedError("remove_role_for_user")
+
+    @abc.abstractmethod
+    def remove_user_from_org(self, user_id: str, org_id: Optional[str] = None) -> None:
+        raise NotImplementedError("remove_user_from_org")
+
+    @abc.abstractmethod
     def get_org_by_id(self, org_id: str) -> OrgRecord:
         raise NotImplementedError("get_org_by_id")
 
     @abc.abstractmethod
     def delete_org(self, org_id: str):
         raise NotImplementedError("delete_org")
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_invite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .delegate import OrgDelegate
-from .record import OrgRecord, OrgType
+from .org import Org
+from .record import OrgInviteRecord
 
 
-class Org:
-    __record: OrgRecord
+class OrgInvite:
     __org_delegate: OrgDelegate
+    __org: Org
+    __record: OrgInviteRecord
 
     @classmethod
     def create(
         cls,
-        creator_user_id: Optional[str],
-        name: str,
-        org_type: OrgType,
+        invited_user_id: str,
+        org_id: str,
         org_delegate: OrgDelegate,
-        bind_email_domain: bool = False,
-    ):
-        record = org_delegate.create_org(
-            creator_user_id=creator_user_id,
-            name=name,
-            org_type=org_type,
-            bind_email_domain=bind_email_domain,
+        inviting_user_id: Optional[str] = None,
+    ) -> "OrgInvite":
+        record = org_delegate.invite_user_to_org(
+            invited_user_id=invited_user_id,
+            inviting_user_id=inviting_user_id,
+            org_id=org_id,
         )
         return cls(record=record, org_delegate=org_delegate)
 
     @classmethod
-    def by_org_id(cls, org_id: str, org_delegate: OrgDelegate) -> "Org":
-        record = org_delegate.get_org_by_id(org_id=org_id)
+    def from_id(
+        cls, invite_id: str, org_delegate: OrgDelegate, user_id: Optional[str] = None
+    ):
+        record = org_delegate.get_org_invite(invite_id=invite_id, user_id=user_id)
         return cls(record=record, org_delegate=org_delegate)
 
-    @classmethod
-    def by_user_id(
-        cls, user_id: Optional[str], org_delegate: OrgDelegate
-    ) -> list["Org"]:
-        records = org_delegate.orgs_for_user(user_id=user_id)
-        return [cls(record=record, org_delegate=org_delegate) for record in records]
-
-    def delete(self) -> None:
-        self.__org_delegate.delete_org(org_id=self.org_id)
-
-    def bind_email_domain(self, email_domain: str) -> None:
-        self.__org_delegate.bind_email_domain(
-            org_id=self.__record.org_id, email_domain=email_domain
+    def accept(self, user_id: Optional[str]):
+        self.__org_delegate.accept_org_invite(
+            invite_id=self.__record.invite_id, user_id=user_id
+        )
+
+    def decline(self, user_id: Optional[str]):
+        self.__org_delegate.decline_org_invite(
+            invite_id=self.__record.invite_id, user_id=user_id
         )
 
-    def __init__(self, record: OrgRecord, org_delegate: OrgDelegate):
+    @property
+    def invite_id(self) -> str:
+        return self.__record.invite_id
+
+    def __init__(self, record: OrgInviteRecord, org_delegate: OrgDelegate):
         self.__record = record
         self.__org_delegate = org_delegate
+        self.__org = Org(record=record.org, org_delegate=org_delegate)
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
-
-    @property
-    def org_id(self):
-        return self.__record.org_id
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_invite.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .delegate import OrgDelegate
 from .org import Org
-from .record import OrgInviteRecord
+from .record import OrgRoleName, OrgRoleRecord
 
 
-class OrgInvite:
+class OrgRole:
+    __record: OrgRoleRecord
     __org_delegate: OrgDelegate
     __org: Org
-    __record: OrgInviteRecord
 
     @classmethod
-    def create(
-        cls,
-        invited_user_id: str,
-        org_id: str,
-        org_delegate: OrgDelegate,
-        inviting_user_id: Optional[str] = None,
-    ) -> "OrgInvite":
-        record = org_delegate.invite_user_to_org(
-            invited_user_id=invited_user_id,
-            inviting_user_id=inviting_user_id,
-            org_id=org_id,
-        )
-        return cls(record=record, org_delegate=org_delegate)
+    def for_user(
+        cls, user_id: Optional[str], org_delegate: OrgDelegate
+    ) -> list["OrgRole"]:
+        records = org_delegate.org_roles_for_user(user_id=user_id)
+        return [cls(record=record, org_delegate=org_delegate) for record in records]
+
+    @classmethod
+    def for_org(
+        cls, org_id: Optional[str], org_delegate: OrgDelegate
+    ) -> list["OrgRole"]:
+        records = org_delegate.org_roles_for_org(org_id=org_id)
+        return [cls(record=record, org_delegate=org_delegate) for record in records]
 
     @classmethod
-    def by_id(
-        cls, invite_id: str, org_delegate: OrgDelegate, user_id: Optional[str] = None
+    def for_user_in_org(
+        cls,
+        org_delegate: OrgDelegate,
+        user_id: Optional[str] = None,
+        org_id: Optional[str] = None,
     ):
-        record = org_delegate.get_org_invite(invite_id=invite_id, user_id=user_id)
+        record = org_delegate.org_role_for_user_in_org(user_id=user_id, org_id=org_id)
         return cls(record=record, org_delegate=org_delegate)
 
-    def accept(self, user_id: Optional[str]):
-        self.__org_delegate.accept_org_invite(
-            invite_id=self.__record.invite_id, user_id=user_id
-        )
-
-    def decline(self, user_id: Optional[str]):
-        self.__org_delegate.decline_org_invite(
-            invite_id=self.__record.invite_id, user_id=user_id
-        )
-
-    def __init__(self, record: OrgInviteRecord, org_delegate: OrgDelegate):
+    def __init__(self, record: OrgRoleRecord, org_delegate: OrgDelegate):
         self.__record = record
         self.__org_delegate = org_delegate
         self.__org = Org(record=record.org, org_delegate=org_delegate)
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
+
+    @property
+    def org_id(self) -> str:
+        return self.__record.org.org_id
+
+    @property
+    def org(self) -> Org:
+        return self.__org
+
+    @property
+    def roles(self) -> list[OrgRoleName]:
+        return self.__record.roles
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class OrgRoleName(str, enum.Enum):
     user = "user"
     admin = "admin"
     owner = "owner"
 
 
 class OrgRoleRecord(pydantic.BaseModel):
-    user_id: str
+    user: UserRecord
     org: OrgRecord
     roles: list[OrgRoleName]
 
 
 class OrgInviteRecord(pydantic.BaseModel):
     invite_id: str
     user_id: str
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 387 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 8301 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 8301 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6700  ..d.d.l.m.Z...g.
 00000070: 6406 a201 5a0b 6407 5300 2908 e901 0000  d...Z.d.S.).....
@@ -18,16 +18,16 @@
 00000110: 7202 0000 00da 0d68 7474 705f 6465 6c65  r......http_dele
 00000120: 6761 7465 7203 0000 00da 0e68 7474 705f  gater......http_
 00000130: 7265 736f 7572 6365 7372 0400 0000 da06  resourcesr......
 00000140: 7265 636f 7264 7205 0000 0072 0600 0000  recordr....r....
 00000150: da05 746f 6b65 6e72 0700 0000 da07 5f5f  ..tokenr......__
 00000160: 616c 6c5f 5fa9 0072 0e00 0000 720e 0000  all__..r....r...
 00000170: 00fa ee2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000180: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
-00000190: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
+00000180: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
+00000190: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
 000001a0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001b0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001c0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001d0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000001e0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000001f0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000200: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 888 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 7803 0000  o.......Ms.dx...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 7803 0000  o.......1..dx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000070: 4f70 7469 6f6e 616c e901 0000 0029 01da  Optional.....)..
@@ -22,15 +22,15 @@
 00000150: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
 00000160: 0100 0000 0200 0000 0300 0000 730e 0000  ............s...
 00000170: 0074 0083 00a0 01a1 0001 0064 0053 0029  .t.........d.S.)
 00000180: 014e 2902 da05 7375 7065 72da 085f 5f69  .N)...super..__i
 00000190: 6e69 745f 5f29 01da 0473 656c 66a9 01da  nit__)...self...
 000001a0: 095f 5f63 6c61 7373 5f5f a900 faee 2f63  .__class__..../c
 000001b0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-000001c0: 7372 6333 3439 3732 3638 3637 302f 7372  src3497268670/sr
+000001c0: 7372 6331 3638 3931 3535 3339 392f 7372  src1689155399/sr
 000001d0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000001e0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000001f0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000200: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000210: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000220: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000230: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 2038 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 f607 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 f607 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6402 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 4700 6409 640a  d.l.m.Z...G.d.d.
@@ -35,15 +35,15 @@
 00000220: 0002 0000 0003 0000 0073 1400 0000 7400  .........s....t.
 00000230: 8300 a001 a100 0100 7c01 7c00 5f02 6400  ........|.|._.d.
 00000240: 5300 2901 4e29 03da 0573 7570 6572 da08  S.).N)...super..
 00000250: 5f5f 696e 6974 5f5f 720c 0000 0029 02da  __init__r....)..
 00000260: 0473 656c 6672 0d00 0000 a901 da09 5f5f  .selfr........__
 00000270: 636c 6173 735f 5fa9 00fa f32f 636f 6465  class__..../code
 00000280: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000290: 3334 3937 3236 3836 3730 2f73 7263 2f63  3497268670/src/c
+00000290: 3136 3839 3135 3533 3939 2f73 7263 2f63  1689155399/src/c
 000002a0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 000002b0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 000002c0: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 000002d0: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 000002e0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 000002f0: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000300: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 216 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 d800 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 d800 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6502 6a03  Z.G.d.d...d.e.j.
 00000050: 8303 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 084f 7074 696f 6e61 6c4e 6300 0000  ...OptionalNc...
 00000070: 0000 0000 0000 0000 0000 0000 0003 0000  ................
@@ -15,16 +15,16 @@
 000000e0: 654e da0b 6465 7363 7269 7074 696f 6e29  eN..description)
 000000f0: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00000100: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 00000110: 616d 655f 5fda 0369 6e74 da0f 5f5f 616e  ame__..int..__an
 00000120: 6e6f 7461 7469 6f6e 735f 5fda 0373 7472  notations__..str
 00000130: 7206 0000 0072 0200 0000 a900 720d 0000  r....r......r...
 00000140: 0072 0d00 0000 faf4 2f63 6f64 6562 7569  .r....../codebui
-00000150: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
-00000160: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
+00000150: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+00000160: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
 00000170: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000180: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000190: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000001a0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000001b0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000001c0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000001d0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 455 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 c701 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 c701 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6503 6a04 8303 5a05 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6503 6a04 8303 5a06 6401  d...d.e.j...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da08 4f70  S.)......N)...Op
@@ -20,16 +20,16 @@
 00000130: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000140: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000150: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
 00000160: 6e6e 6f74 6174 696f 6e73 5f5f 7206 0000  nnotations__r...
 00000170: 0072 0200 0000 da08 6461 7465 7469 6d65  .r......datetime
 00000180: 7208 0000 00a9 0072 0f00 0000 720f 0000  r......r....r...
 00000190: 00fa ec2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000001a0: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
-000001b0: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
+000001a0: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
+000001b0: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
 000001c0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001d0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001e0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001f0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000200: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000210: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000220: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/token.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 class Token:
     __record: TokenRecord
     __token_delegate: TokenDelegate
 
     @classmethod
-    def by_token_id(cls, token_id: str, token_delegate: TokenDelegate) -> "Token":
+    def from_id(cls, token_id: str, token_delegate: TokenDelegate) -> "Token":
         record = token_delegate.get_token_by_token_id(token_id=token_id)
         return cls(record=record, token_delegate=token_delegate)
 
     @classmethod
-    def by_user_id(
+    def for_user(
         cls, user_id: Optional[str], token_delegate: TokenDelegate
     ) -> list["Token"]:
         records = token_delegate.get_tokens_for_user(user_id=user_id)
         return [cls(record=record, token_delegate=token_delegate) for record in records]
 
     @classmethod
     def create(
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 391 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 8701 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 8701 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6700 6406 a201  d.l.m.Z...g.d...
 00000070: 5a0a 6407 5300 2908 e901 0000 0029 01da  Z.d.S.)......)..
@@ -18,16 +18,16 @@
 00000110: 7474 705f 7265 736f 7572 6365 7372 0300  ttp_resourcesr..
 00000120: 0000 5a07 7472 6967 6765 7272 0400 0000  ..Z.triggerr....
 00000130: 5a10 7472 6967 6765 725f 6465 6c65 6761  Z.trigger_delega
 00000140: 7465 7205 0000 005a 0e74 7269 6767 6572  ter....Z.trigger
 00000150: 5f72 6563 6f72 6472 0600 0000 da07 5f5f  _recordr......__
 00000160: 616c 6c5f 5fa9 0072 0a00 0000 720a 0000  all__..r....r...
 00000170: 00fa f02f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000180: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
-00000190: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
+00000180: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
+00000190: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
 000001a0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001b0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001c0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001d0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000001e0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000001f0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000200: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 2280 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 e808 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 e808 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6402  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6402 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6406 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6406 6408 6c0c 6d0d 5a0d 0100 6406  ..d.d.l.m.Z...d.
@@ -39,15 +39,15 @@
 00000260: 0000 0200 0000 0300 0000 7314 0000 0074  ..........s....t
 00000270: 0083 00a0 01a1 0001 007c 017c 005f 0264  .........|.|._.d
 00000280: 0053 00a9 014e 2903 da05 7375 7065 72da  .S...N)...super.
 00000290: 085f 5f69 6e69 745f 5f72 0e00 0000 2902  .__init__r....).
 000002a0: da04 7365 6c66 720f 0000 00a9 01da 095f  ..selfr........_
 000002b0: 5f63 6c61 7373 5f5f a900 faf5 2f63 6f64  _class__..../cod
 000002c0: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000002d0: 6333 3439 3732 3638 3637 302f 7372 632f  c3497268670/src/
+000002d0: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
 000002e0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 000002f0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000300: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000310: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000320: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000330: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000340: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 205 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 cd00 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 cd00 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0003 0000 0040 0000 0073 2a00  .........@...s*.
 00000070: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
@@ -15,15 +15,15 @@
 000000e0: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000000f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000100: 6e61 6d65 5f5f da08 7079 6461 6e74 6963  name__..pydantic
 00000110: da05 4669 656c 6472 0400 0000 da03 7374  ..Fieldr......st
 00000120: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
 00000130: 5f5f a900 720d 0000 0072 0d00 0000 faf6  __..r....r......
 00000140: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000150: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+00000150: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 00000160: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000170: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000180: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000190: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 000001a0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 000001b0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001c0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 2683 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 7b0a 0000  o.......Ms.d{...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 7d0a 0000  o.......1..d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6405 6c07 6d08 5a08 0100 6406  ..d.d.l.m.Z...d.
 00000060: 6407 6c09 6d0a 5a0a 0100 6406 6408 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
@@ -46,16 +46,16 @@
 000002d0: 720e 0000 0072 0f00 0000 7210 0000 00a9  r....r....r.....
 000002e0: 03da 0672 6563 6f72 6472 1100 0000 7212  ...recordr....r.
 000002f0: 0000 0029 01da 0e63 7265 6174 655f 7472  ...)...create_tr
 00000300: 6967 6765 7229 07da 0363 6c73 720e 0000  igger)...clsr...
 00000310: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
 00000320: 7212 0000 0072 1500 0000 a900 7218 0000  r....r......r...
 00000330: 00fa ef2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000340: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
-00000350: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
+00000340: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
+00000350: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
 00000360: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 00000370: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 00000380: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000390: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000003a0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000003b0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 000003c0: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
@@ -72,79 +72,79 @@
 00000470: 007c 046a 007c 017c 0264 018d 027d 057c  .|.j.|.|.d...}.|
 00000480: 007c 057c 037c 0464 028d 0353 0029 034e  .|.|.|.d...S.).N
 00000490: 2902 720e 0000 0072 0f00 0000 7214 0000  ).r....r....r...
 000004a0: 0029 01da 1a67 6574 5f74 7269 6767 6572  .)...get_trigger
 000004b0: 5f62 795f 7072 696d 6172 795f 6b65 7929  _by_primary_key)
 000004c0: 0672 1700 0000 720e 0000 0072 0f00 0000  .r....r....r....
 000004d0: 7211 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
-000004e0: 1800 0000 7218 0000 0072 1900 0000 da07  ....r....r......
-000004f0: 6279 5f6e 616d 6524 0000 0073 0c00 0000  by_name$...s....
-00000500: 0e08 0201 0201 0201 0201 06fd 7a0f 5472  ............z.Tr
-00000510: 6967 6765 722e 6279 5f6e 616d 65da 0766  igger.by_name..f
-00000520: 696c 7465 7273 2903 720a 0000 004e 4e63  ilters).r....NNc
-00000530: 0500 0000 0000 0000 0000 0000 0700 0000  ................
-00000540: 0600 0000 6300 0000 734e 0000 0081 007c  ....c...sN.....|
-00000550: 046a 007c 017c 0264 018d 027d 0509 007c  .j.|.|.d...}...|
-00000560: 056a 0144 005d 0a7d 067c 007c 067c 037c  .j.D.].}.|.|.|.|
-00000570: 0464 038d 0356 0001 0071 0c7c 056a 0272  .d...V...q.|.j.r
-00000580: 247c 046a 007c 017c 027c 056a 0264 048d  $|.j.|.|.|.j.d..
-00000590: 037d 056e 0264 0053 0071 0929 054e 2902  .}.n.d.S.q.).N).
-000005a0: 721d 0000 0072 0f00 0000 5472 1400 0000  r....r....Tr....
-000005b0: 2903 721d 0000 0072 0f00 0000 da0a 7061  ).r....r......pa
-000005c0: 6765 5f74 6f6b 656e 2903 da0e 7175 6572  ge_token)...quer
-000005d0: 795f 7472 6967 6765 7273 da05 6974 656d  y_triggers..item
-000005e0: 73da 0a6e 6578 745f 746f 6b65 6e29 0772  s..next_token).r
-000005f0: 1700 0000 721d 0000 0072 0f00 0000 7211  ....r....r....r.
-00000600: 0000 0072 1200 0000 da11 7061 6769 6e61  ...r......pagina
-00000610: 7465 645f 7265 7375 6c74 7372 1500 0000  ted_resultsr....
-00000620: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000630: 0571 7565 7279 3300 0000 7326 0000 0002  .query3...s&....
-00000640: 8004 0804 0106 ff02 030a 0102 0102 0102  ................
-00000650: 0102 010a fd06 0504 0102 0102 0104 0108  ................
-00000660: fd04 0602 f27a 0d54 7269 6767 6572 2e71  .....z.Trigger.q
-00000670: 7565 7279 7215 0000 0063 0400 0000 0000  ueryr....c......
-00000680: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
-00000690: 0000 7316 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
-000006a0: 005f 017c 037c 005f 0264 0053 00a9 014e  ._.|.|._.d.S...N
-000006b0: 2903 720b 0000 0072 0c00 0000 720d 0000  ).r....r....r...
-000006c0: 0029 04da 0473 656c 6672 1500 0000 7211  .)...selfr....r.
-000006d0: 0000 0072 1200 0000 7218 0000 0072 1800  ...r....r....r..
-000006e0: 0000 7219 0000 00da 085f 5f69 6e69 745f  ..r......__init_
-000006f0: 5f4e 0000 0073 0600 0000 0606 0601 0a01  _N...s..........
-00000700: 7a10 5472 6967 6765 722e 5f5f 696e 6974  z.Trigger.__init
-00000710: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00000720: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00000730: 7400 7c00 6a01 8301 5300 7224 0000 0029  t.|.j...S.r$...)
-00000740: 0272 0600 0000 720b 0000 0029 0172 2500  .r....r....).r%.
-00000750: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000760: 00da 0774 6f5f 6469 6374 5800 0000 7302  ...to_dictX...s.
-00000770: 0000 000a 017a 0f54 7269 6767 6572 2e74  .....z.Trigger.t
-00000780: 6f5f 6469 6374 4e29 14da 085f 5f6e 616d  o_dictN)...__nam
-00000790: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000007a0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0900  .__qualname__r..
-000007b0: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
-000007c0: 735f 5f72 0500 0000 7208 0000 00da 0b63  s__r....r......c
-000007d0: 6c61 7373 6d65 7468 6f64 da03 7374 7272  lassmethod..strr
-000007e0: 0300 0000 721a 0000 0072 1c00 0000 da04  ....r....r......
-000007f0: 6469 6374 7202 0000 00da 0b63 6f6c 6c65  dictr......colle
-00000800: 6374 696f 6e73 da03 6162 63da 0947 656e  ctions..abc..Gen
-00000810: 6572 6174 6f72 7223 0000 0072 2600 0000  eratorr#...r&...
-00000820: 7227 0000 0072 1800 0000 7218 0000 0072  r'...r....r....r
-00000830: 1800 0000 7219 0000 0072 0a00 0000 0c00  ....r....r......
-00000840: 0000 7364 0000 000a 0008 0108 0108 0102  ..sd............
-00000850: 0202 0102 0202 fe06 0302 fd02 0402 fc02  ................
-00000860: 0502 fb02 0602 fa02 070c f902 1202 0102  ................
-00000870: 0202 fe06 0302 fd02 0402 fc02 0502 fb02  ................
-00000880: 060c fa02 0e02 010e 0202 fe06 0302 fd02  ................
-00000890: 0402 fc02 0502 fb0a 060c fa02 1a02 0202  ................
-000008a0: fe02 0302 fd02 040a fc1a 0a72 0a00 0000  ...........r....
-000008b0: 290e da0f 636f 6c6c 6563 7469 6f6e 732e  )...collections.
-000008c0: 6162 6372 2f00 0000 da06 7479 7069 6e67  abcr/.....typing
-000008d0: 7202 0000 0072 0300 0000 5a0e 646f 6d61  r....r....Z.doma
-000008e0: 696e 2e61 6374 696f 6e73 7205 0000 00da  in.actionsr.....
-000008f0: 0573 6572 6465 7206 0000 0072 1200 0000  .serder....r....
-00000900: 7208 0000 00da 0e74 7269 6767 6572 5f72  r......trigger_r
-00000910: 6563 6f72 6472 0900 0000 720a 0000 0072  ecordr....r....r
-00000920: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-00000930: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000940: 0073 0e00 0000 0802 1001 0c02 0c01 0c01  .s..............
-00000950: 0c01 1203                                ....
+000004e0: 1800 0000 7218 0000 0072 1900 0000 da09  ....r....r......
+000004f0: 6672 6f6d 5f6e 616d 6524 0000 0073 0c00  from_name$...s..
+00000500: 0000 0e08 0201 0201 0201 0201 06fd 7a11  ..............z.
+00000510: 5472 6967 6765 722e 6672 6f6d 5f6e 616d  Trigger.from_nam
+00000520: 65da 0766 696c 7465 7273 2903 720a 0000  e..filters).r...
+00000530: 004e 4e63 0500 0000 0000 0000 0000 0000  .NNc............
+00000540: 0700 0000 0600 0000 6300 0000 734e 0000  ........c...sN..
+00000550: 0081 007c 046a 007c 017c 0264 018d 027d  ...|.j.|.|.d...}
+00000560: 0509 007c 056a 0144 005d 0a7d 067c 007c  ...|.j.D.].}.|.|
+00000570: 067c 037c 0464 038d 0356 0001 0071 0c7c  .|.|.d...V...q.|
+00000580: 056a 0272 247c 046a 007c 017c 027c 056a  .j.r$|.j.|.|.|.j
+00000590: 0264 048d 037d 056e 0264 0053 0071 0929  .d...}.n.d.S.q.)
+000005a0: 054e 2902 721d 0000 0072 0f00 0000 5472  .N).r....r....Tr
+000005b0: 1400 0000 2903 721d 0000 0072 0f00 0000  ....).r....r....
+000005c0: da0a 7061 6765 5f74 6f6b 656e 2903 da0e  ..page_token)...
+000005d0: 7175 6572 795f 7472 6967 6765 7273 da05  query_triggers..
+000005e0: 6974 656d 73da 0a6e 6578 745f 746f 6b65  items..next_toke
+000005f0: 6e29 0772 1700 0000 721d 0000 0072 0f00  n).r....r....r..
+00000600: 0000 7211 0000 0072 1200 0000 da11 7061  ..r....r......pa
+00000610: 6769 6e61 7465 645f 7265 7375 6c74 7372  ginated_resultsr
+00000620: 1500 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+00000630: 0000 00da 0571 7565 7279 3300 0000 7326  .....query3...s&
+00000640: 0000 0002 8004 0804 0106 ff02 030a 0102  ................
+00000650: 0102 0102 0102 010a fd06 0504 0102 0102  ................
+00000660: 0104 0108 fd04 0602 f27a 0d54 7269 6767  .........z.Trigg
+00000670: 6572 2e71 7565 7279 7215 0000 0063 0400  er.queryr....c..
+00000680: 0000 0000 0000 0000 0000 0400 0000 0200  ................
+00000690: 0000 4300 0000 7316 0000 007c 017c 005f  ..C...s....|.|._
+000006a0: 007c 027c 005f 017c 037c 005f 0264 0053  .|.|._.|.|._.d.S
+000006b0: 00a9 014e 2903 720b 0000 0072 0c00 0000  ...N).r....r....
+000006c0: 720d 0000 0029 04da 0473 656c 6672 1500  r....)...selfr..
+000006d0: 0000 7211 0000 0072 1200 0000 7218 0000  ..r....r....r...
+000006e0: 0072 1800 0000 7219 0000 00da 085f 5f69  .r....r......__i
+000006f0: 6e69 745f 5f4e 0000 0073 0600 0000 0606  nit__N...s......
+00000700: 0601 0a01 7a10 5472 6967 6765 722e 5f5f  ....z.Trigger.__
+00000710: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000720: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000730: 0a00 0000 7400 7c00 6a01 8301 5300 7224  ....t.|.j...S.r$
+00000740: 0000 0029 0272 0600 0000 720b 0000 0029  ...).r....r....)
+00000750: 0172 2500 0000 7218 0000 0072 1800 0000  .r%...r....r....
+00000760: 7219 0000 00da 0774 6f5f 6469 6374 5800  r......to_dictX.
+00000770: 0000 7302 0000 000a 017a 0f54 7269 6767  ..s......z.Trigg
+00000780: 6572 2e74 6f5f 6469 6374 4e29 14da 085f  er.to_dictN)..._
+00000790: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000007a0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000007b0: 5f72 0900 0000 da0f 5f5f 616e 6e6f 7461  _r......__annota
+000007c0: 7469 6f6e 735f 5f72 0500 0000 7208 0000  tions__r....r...
+000007d0: 00da 0b63 6c61 7373 6d65 7468 6f64 da03  ...classmethod..
+000007e0: 7374 7272 0300 0000 721a 0000 0072 1c00  strr....r....r..
+000007f0: 0000 da04 6469 6374 7202 0000 00da 0b63  ....dictr......c
+00000800: 6f6c 6c65 6374 696f 6e73 da03 6162 63da  ollections..abc.
+00000810: 0947 656e 6572 6174 6f72 7223 0000 0072  .Generatorr#...r
+00000820: 2600 0000 7227 0000 0072 1800 0000 7218  &...r'...r....r.
+00000830: 0000 0072 1800 0000 7219 0000 0072 0a00  ...r....r....r..
+00000840: 0000 0c00 0000 7364 0000 000a 0008 0108  ......sd........
+00000850: 0108 0102 0202 0102 0202 fe06 0302 fd02  ................
+00000860: 0402 fc02 0502 fb02 0602 fa02 070c f902  ................
+00000870: 1202 0102 0202 fe06 0302 fd02 0402 fc02  ................
+00000880: 0502 fb02 060c fa02 0e02 010e 0202 fe06  ................
+00000890: 0302 fd02 0402 fc02 0502 fb0a 060c fa02  ................
+000008a0: 1a02 0202 fe02 0302 fd02 040a fc1a 0a72  ...............r
+000008b0: 0a00 0000 290e da0f 636f 6c6c 6563 7469  ....)...collecti
+000008c0: 6f6e 732e 6162 6372 2f00 0000 da06 7479  ons.abcr/.....ty
+000008d0: 7069 6e67 7202 0000 0072 0300 0000 5a0e  pingr....r....Z.
+000008e0: 646f 6d61 696e 2e61 6374 696f 6e73 7205  domain.actionsr.
+000008f0: 0000 00da 0573 6572 6465 7206 0000 0072  .....serder....r
+00000900: 1200 0000 7208 0000 00da 0e74 7269 6767  ....r......trigg
+00000910: 6572 5f72 6563 6f72 6472 0900 0000 720a  er_recordr....r.
+00000920: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
+00000930: 0000 7219 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000940: 3e01 0000 0073 0e00 0000 0802 1001 0c02  >....s..........
+00000950: 0c01 0c01 0c01 1203                      ........
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 7203 0000  o.......Ms.dr...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 7203 0000  o.......1..dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6407 6408 8400 6408 6500 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6401 5300 2909 e900 0000 004e 2902 da03  d.S.)......N)...
@@ -28,15 +28,15 @@
 000001b0: 0000 0200 0000 4300 0000 f308 0000 0074  ......C........t
 000001c0: 0064 0183 0182 0129 024e da0e 6372 6561  .d.....).N..crea
 000001d0: 7465 5f74 7269 6767 6572 a901 da13 4e6f  te_trigger....No
 000001e0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
 000001f0: 7229 04da 0473 656c 6672 0900 0000 720a  r)...selfr....r.
 00000200: 0000 0072 0b00 0000 a900 7212 0000 00fa  ...r......r.....
 00000210: f82f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-00000220: 7574 2f73 7263 3334 3937 3236 3836 3730  ut/src3497268670
+00000220: 7574 2f73 7263 3136 3839 3135 3533 3939  ut/src1689155399
 00000230: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000240: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000250: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000260: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000270: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000280: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000290: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 f900 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 f900 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
 00000070: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
@@ -12,15 +12,15 @@
 000000b0: 066f 7267 5f69 64da 0b61 6374 696f 6e5f  .org_id..action_
 000000c0: 6e61 6d65 4e29 05da 085f 5f6e 616d 655f  nameN)...__name_
 000000d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 000000e0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 000000f0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000100: 5fa9 0072 0b00 0000 720b 0000 00fa f62f  _..r....r....../
 00000110: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000120: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
+00000120: 2f73 7263 3136 3839 3135 3533 3939 2f73  /src1689155399/s
 00000130: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000140: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000150: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000160: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000170: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000180: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000190: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             record=record,
             action_delegate=action_delegate,
             trigger_delegate=trigger_delegate,
         )
 
     # And version?
     @classmethod
-    def by_name(
+    def from_name(
         cls,
         name: str,
         org_id: Optional[str],
         action_delegate: ActionDelegate,
         trigger_delegate: TriggerDelegate,
     ) -> "Trigger":
         record = trigger_delegate.get_trigger_by_primary_key(name=name, org_id=org_id)
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 262 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 0601 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 0601 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6700  ..d.d.l.m.Z...g.
 00000060: 6405 a201 5a08 6406 5300 2907 e901 0000  d...Z.d.S.).....
 00000070: 0029 01da 1055 7365 7248 7474 7044 656c  .)...UserHttpDel
@@ -13,15 +13,15 @@
 000000c0: 004e 2909 da0d 6874 7470 5f64 656c 6567  .N)...http_deleg
 000000d0: 6174 6572 0200 0000 da04 7573 6572 7203  ater......userr.
 000000e0: 0000 005a 0d75 7365 725f 6465 6c65 6761  ...Z.user_delega
 000000f0: 7465 7204 0000 005a 0b75 7365 725f 7265  ter....Z.user_re
 00000100: 636f 7264 7205 0000 00da 075f 5f61 6c6c  cordr......__all
 00000110: 5f5f a900 7209 0000 0072 0900 0000 faed  __..r....r......
 00000120: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000130: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+00000130: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 00000140: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000150: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000160: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000170: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000180: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000190: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1051 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 1b04 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 1b04 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6404 6405 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6407 6408 8400 6408 6506 8303  ..G.d.d...d.e...
 00000070: 5a09 6409 5300 290a e900 0000 0029 01da  Z.d.S.)......)..
@@ -26,16 +26,16 @@
 00000190: 0000 0000 0000 0000 0002 0000 0002 0000  ................
 000001a0: 0003 0000 0073 1400 0000 7400 8300 a001  .....s....t.....
 000001b0: a100 0100 7c01 7c00 5f02 6400 5300 2901  ....|.|._.d.S.).
 000001c0: 4e29 03da 0573 7570 6572 da08 5f5f 696e  N)...super..__in
 000001d0: 6974 5f5f 720a 0000 0029 02da 0473 656c  it__r....)...sel
 000001e0: 6672 0b00 0000 a901 da09 5f5f 636c 6173  fr........__clas
 000001f0: 735f 5fa9 00fa f22f 636f 6465 6275 696c  s__..../codebuil
-00000200: 642f 6f75 7470 7574 2f73 7263 3334 3937  d/output/src3497
-00000210: 3236 3836 3730 2f73 7263 2f63 6f64 6573  268670/src/codes
+00000200: 642f 6f75 7470 7574 2f73 7263 3136 3839  d/output/src1689
+00000210: 3135 3533 3939 2f73 7263 2f63 6f64 6573  155399/src/codes
 00000220: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000230: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 00000240: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 00000250: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000260: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000270: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000280: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1213 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,139 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 bd04 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 8005 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6407 6408 8400 6408 8302 5a09  ..G.d.d...d...Z.
 00000070: 6409 5300 290a e900 0000 0029 02da 0341  d.S.)......)...A
 00000080: 6e79 da08 4f70 7469 6f6e 616c e903 0000  ny..Optional....
 00000090: 0029 01da 1670 7964 616e 7469 635f 6a73  .)...pydantic_js
 000000a0: 6f6e 6162 6c65 5f64 6963 74e9 0100 0000  onable_dict.....
 000000b0: 2901 da0c 5573 6572 4465 6c65 6761 7465  )...UserDelegate
 000000c0: 2901 da0a 5573 6572 5265 636f 7264 6300  )...UserRecordc.
-000000d0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000000e0: 0000 0040 0000 0073 a000 0000 6500 5a01  ...@...s....e.Z.
+000000d0: 0000 0000 0000 0000 0000 0000 0000 0007  ................
+000000e0: 0000 0040 0000 0073 ce00 0000 6500 5a01  ...@...s....e.Z.
 000000f0: 6400 5a02 5500 6503 6504 6401 3c00 6505  d.Z.U.e.e.d.<.e.
-00000100: 6504 6402 3c00 6506 6403 6507 6508 1900  e.d.<.e.d.e.e...
-00000110: 6404 6505 6604 6405 6406 8404 8301 5a09  d.e.f.d.d.....Z.
-00000120: 6407 6503 6404 6505 6604 6408 6409 8404  d.e.d.e.f.d.d...
-00000130: 5a0a 640a 650b 6508 650c 6602 1900 6602  Z.d.e.e.e.f...f.
-00000140: 640b 640c 8404 5a0d 6416 640e 640f 8404  d.d...Z.d.d.d...
-00000150: 5a0e 650f 640a 6508 6602 6410 6411 8404  Z.e.d.e.f.d.d...
-00000160: 8301 5a10 650f 640a 6508 6602 6412 6413  ..Z.e.d.e.f.d.d.
-00000170: 8404 8301 5a11 650f 640a 6512 6602 6414  ....Z.e.d.e.f.d.
-00000180: 6415 8404 8301 5a13 640d 5300 2917 da04  d.....Z.d.S.)...
-00000190: 5573 6572 da0d 5f55 7365 725f 5f72 6563  User.._User__rec
-000001a0: 6f72 64da 145f 5573 6572 5f5f 7573 6572  ord.._User__user
-000001b0: 5f64 656c 6567 6174 65da 0775 7365 725f  _delegate..user_
-000001c0: 6964 da0d 7573 6572 5f64 656c 6567 6174  id..user_delegat
-000001d0: 6563 0300 0000 0000 0000 0000 0000 0400  ec..............
-000001e0: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
-000001f0: 026a 007c 0164 018d 017d 037c 007c 037c  .j.|.d...}.|.|.|
-00000200: 0264 028d 0253 0029 034e a901 720c 0000  .d...S.).N..r...
-00000210: 0029 02da 0672 6563 6f72 6472 0d00 0000  .)...recordr....
-00000220: 2901 da0e 6765 745f 7573 6572 5f62 795f  )...get_user_by_
-00000230: 6964 2904 da03 636c 7372 0c00 0000 720d  id)...clsr....r.
-00000240: 0000 0072 0f00 0000 a900 7212 0000 00fa  ...r......r.....
-00000250: e92f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-00000260: 7574 2f73 7263 3334 3937 3236 3836 3730  ut/src3497268670
-00000270: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
-00000280: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
-00000290: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
-000002a0: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
-000002b0: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
-000002c0: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
-000002d0: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
-000002e0: 3933 3639 3964 2f72 6f62 6f74 6f2d 6169  93699d/roboto-ai
-000002f0: 2f72 6f62 6f74 6f2d 686f 7374 6564 2d61  /roboto-hosted-a
-00000300: 7070 2f70 6163 6b61 6765 732f 726f 626f  pp/packages/robo
-00000310: 746f 5f73 646b 2f73 7263 2f72 6f62 6f74  to_sdk/src/robot
-00000320: 6f5f 7364 6b2f 646f 6d61 696e 2f75 7365  o_sdk/domain/use
-00000330: 7273 2f75 7365 722e 7079 da05 6279 5f69  rs/user.py..by_i
-00000340: 640e 0000 0073 0400 0000 0c02 0c01 7a0a  d....s........z.
-00000350: 5573 6572 2e62 795f 6964 720f 0000 0063  User.by_idr....c
-00000360: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000370: 0200 0000 4300 0000 7310 0000 007c 017c  ....C...s....|.|
-00000380: 005f 007c 027c 005f 0164 0053 00a9 014e  ._.|.|._.d.S...N
-00000390: 2902 720a 0000 0072 0b00 0000 2903 da04  ).r....r....)...
-000003a0: 7365 6c66 720f 0000 0072 0d00 0000 7212  selfr....r....r.
-000003b0: 0000 0072 1200 0000 7213 0000 00da 085f  ...r....r......_
-000003c0: 5f69 6e69 745f 5f13 0000 0073 0400 0000  _init__....s....
-000003d0: 0601 0a01 7a0d 5573 6572 2e5f 5f69 6e69  ....z.User.__ini
-000003e0: 745f 5fda 0672 6574 7572 6e63 0100 0000  t__..returnc....
-000003f0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000400: 4300 0000 730a 0000 0074 007c 006a 0183  C...s....t.|.j..
-00000410: 0153 0072 1500 0000 2902 7205 0000 0072  .S.r....).r....r
-00000420: 0a00 0000 a901 7216 0000 0072 1200 0000  ......r....r....
-00000430: 7212 0000 0072 1300 0000 da07 746f 5f64  r....r......to_d
-00000440: 6963 7417 0000 0073 0200 0000 0a01 7a0c  ict....s......z.
-00000450: 5573 6572 2e74 6f5f 6469 6374 4e63 0100  User.to_dictNc..
-00000460: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000470: 0000 4300 0000 7312 0000 007c 006a 006a  ..C...s....|.j.j
-00000480: 017c 006a 026a 0364 018d 0153 0029 024e  .|.j.j.d...S.).N
-00000490: 720e 0000 0029 0472 0b00 0000 da0b 6465  r....).r......de
-000004a0: 6c65 7465 5f75 7365 7272 0a00 0000 720c  lete_userr....r.
-000004b0: 0000 0072 1900 0000 7212 0000 0072 1200  ...r....r....r..
-000004c0: 0000 7213 0000 00da 0664 656c 6574 651a  ..r......delete.
-000004d0: 0000 0073 0200 0000 1201 7a0b 5573 6572  ...s......z.User
-000004e0: 2e64 656c 6574 6563 0100 0000 0000 0000  .deletec........
-000004f0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000500: f308 0000 007c 006a 006a 0153 0072 1500  .....|.j.j.S.r..
-00000510: 0000 a902 720a 0000 0072 0c00 0000 7219  ....r....r....r.
-00000520: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000530: 0000 720c 0000 001d 0000 00f3 0200 0000  ..r.............
-00000540: 0802 7a0c 5573 6572 2e75 7365 725f 6964  ..z.User.user_id
-00000550: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000560: 0001 0000 0043 0000 0072 1d00 0000 7215  .....C...r....r.
-00000570: 0000 0072 1e00 0000 7219 0000 0072 1200  ...r....r....r..
-00000580: 0000 7212 0000 0072 1300 0000 da08 7573  ..r....r......us
-00000590: 6572 6e61 6d65 2100 0000 721f 0000 007a  ername!...r....z
-000005a0: 0d55 7365 722e 7573 6572 6e61 6d65 6301  .User.usernamec.
-000005b0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-000005c0: 0000 0043 0000 0073 1800 0000 7c00 6a00  ...C...s....|.j.
-000005d0: 6a01 6400 7501 720a 7c00 6a00 6a01 5300  j.d.u.r.|.j.j.S.
-000005e0: 6401 5300 2902 4e46 2902 720a 0000 00da  d.S.).NF).r.....
-000005f0: 0e69 735f 7379 7374 656d 5f75 7365 7272  .is_system_userr
-00000600: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000610: 0000 0072 2100 0000 2500 0000 730a 0000  ...r!...%...s...
-00000620: 000c 0406 ff02 ff02 0302 fd7a 1355 7365  ...........z.Use
-00000630: 722e 6973 5f73 7973 7465 6d5f 7573 6572  r.is_system_user
-00000640: 2902 7218 0000 004e 2914 da08 5f5f 6e61  ).r....N)...__na
-00000650: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000660: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7208  ..__qualname__r.
-00000670: 0000 00da 0f5f 5f61 6e6e 6f74 6174 696f  .....__annotatio
-00000680: 6e73 5f5f 7207 0000 00da 0b63 6c61 7373  ns__r......class
-00000690: 6d65 7468 6f64 7203 0000 00da 0373 7472  methodr......str
-000006a0: 7214 0000 0072 1700 0000 da04 6469 6374  r....r......dict
-000006b0: 7202 0000 0072 1a00 0000 721c 0000 00da  r....r....r.....
-000006c0: 0870 726f 7065 7274 7972 0c00 0000 7220  .propertyr....r 
-000006d0: 0000 00da 0462 6f6f 6c72 2100 0000 7212  .....boolr!...r.
-000006e0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-000006f0: 0000 7209 0000 000a 0000 0073 1c00 0000  ..r........s....
-00000700: 0a00 0801 0801 0202 1801 1204 1604 0a03  ................
-00000710: 0203 1001 0203 1001 0203 1401 7209 0000  ............r...
-00000720: 004e 290a da06 7479 7069 6e67 7202 0000  .N)...typingr...
-00000730: 0072 0300 0000 da05 7365 7264 6572 0500  .r......serder..
-00000740: 0000 720d 0000 0072 0700 0000 da0b 7573  ..r....r......us
-00000750: 6572 5f72 6563 6f72 6472 0800 0000 7209  er_recordr....r.
-00000760: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00000770: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000780: 3e01 0000 0073 0a00 0000 1002 0c02 0c01  >....s..........
-00000790: 0c01 1203                                ....
+00000100: 6504 6402 3c00 6506 641a 6404 6505 6405  e.d.<.e.d.d.e.d.
+00000110: 6507 6508 1900 6604 6406 6407 8405 8301  e.e...f.d.d.....
+00000120: 5a09 6408 6503 6404 6505 6604 6409 640a  Z.d.e.d.e.f.d.d.
+00000130: 8404 5a0a 640b 650b 6508 650c 6602 1900  ..Z.d.e.e.e.f...
+00000140: 6602 640c 640d 8404 5a0d 641b 640e 640f  f.d.d...Z.d.d.d.
+00000150: 8404 5a0e 650f 640b 6508 6602 6410 6411  ..Z.e.d.e.f.d.d.
+00000160: 8404 8301 5a10 650f 640b 6508 6602 6412  ....Z.e.d.e.f.d.
+00000170: 6413 8404 8301 5a11 650f 640b 6512 6602  d.....Z.e.d.e.f.
+00000180: 6414 6415 8404 8301 5a13 650f 640b 6507  d.d.....Z.e.d.e.
+00000190: 6508 1900 6602 6416 6417 8404 8301 5a14  e...f.d.d.....Z.
+000001a0: 650f 640b 6507 6508 1900 6602 6418 6419  e.d.e.e...f.d.d.
+000001b0: 8404 8301 5a15 6403 5300 291c da04 5573  ....Z.d.S.)...Us
+000001c0: 6572 da0d 5f55 7365 725f 5f72 6563 6f72  er.._User__recor
+000001d0: 64da 145f 5573 6572 5f5f 7573 6572 5f64  d.._User__user_d
+000001e0: 656c 6567 6174 654e da0d 7573 6572 5f64  elegateN..user_d
+000001f0: 656c 6567 6174 65da 0775 7365 725f 6964  elegate..user_id
+00000200: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00000210: 0004 0000 0043 0000 0073 1800 0000 7c01  .....C...s....|.
+00000220: 6a00 7c02 6401 8d01 7d03 7c00 7c03 7c01  j.|.d...}.|.|.|.
+00000230: 6402 8d02 5300 2903 4ea9 0172 0d00 0000  d...S.).N..r....
+00000240: 2902 da06 7265 636f 7264 720c 0000 0029  )...recordr....)
+00000250: 01da 0e67 6574 5f75 7365 725f 6279 5f69  ...get_user_by_i
+00000260: 6429 04da 0363 6c73 720c 0000 0072 0d00  d)...clsr....r..
+00000270: 0000 720f 0000 00a9 0072 1200 0000 fae9  ..r......r......
+00000280: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
+00000290: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+000002a0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
+000002b0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
+000002c0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+000002d0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
+000002e0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
+000002f0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
+00000300: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
+00000310: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
+00000320: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
+00000330: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
+00000340: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
+00000350: 5f73 646b 2f64 6f6d 6169 6e2f 7573 6572  _sdk/domain/user
+00000360: 732f 7573 6572 2e70 79da 0766 726f 6d5f  s/user.py..from_
+00000370: 6964 0e00 0000 7304 0000 000c 020c 017a  id....s........z
+00000380: 0c55 7365 722e 6672 6f6d 5f69 6472 0f00  .User.from_idr..
+00000390: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+000003a0: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
+000003b0: 7c01 7c00 5f00 7c02 7c00 5f01 6400 5300  |.|._.|.|._.d.S.
+000003c0: a901 4e29 0272 0a00 0000 720b 0000 0029  ..N).r....r....)
+000003d0: 03da 0473 656c 6672 0f00 0000 720c 0000  ...selfr....r...
+000003e0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+000003f0: da08 5f5f 696e 6974 5f5f 1300 0000 7304  ..__init__....s.
+00000400: 0000 0006 010a 017a 0d55 7365 722e 5f5f  .......z.User.__
+00000410: 696e 6974 5f5f da06 7265 7475 726e 6301  init__..returnc.
+00000420: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000430: 0000 0043 0000 0073 0a00 0000 7400 7c00  ...C...s....t.|.
+00000440: 6a01 8301 5300 7215 0000 0029 0272 0500  j...S.r....).r..
+00000450: 0000 720a 0000 00a9 0172 1600 0000 7212  ..r......r....r.
+00000460: 0000 0072 1200 0000 7213 0000 00da 0774  ...r....r......t
+00000470: 6f5f 6469 6374 1700 0000 7302 0000 000a  o_dict....s.....
+00000480: 017a 0c55 7365 722e 746f 5f64 6963 7463  .z.User.to_dictc
+00000490: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000004a0: 0300 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
+000004b0: 006a 017c 006a 026a 0364 018d 0153 0029  .j.|.j.j.d...S.)
+000004c0: 024e 720e 0000 0029 0472 0b00 0000 da0b  .Nr....).r......
+000004d0: 6465 6c65 7465 5f75 7365 7272 0a00 0000  delete_userr....
+000004e0: 720d 0000 0072 1900 0000 7212 0000 0072  r....r....r....r
+000004f0: 1200 0000 7213 0000 00da 0664 656c 6574  ....r......delet
+00000500: 651a 0000 0073 0200 0000 1201 7a0b 5573  e....s......z.Us
+00000510: 6572 2e64 656c 6574 6563 0100 0000 0000  er.deletec......
+00000520: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000530: 0000 f308 0000 007c 006a 006a 0153 0072  .......|.j.j.S.r
+00000540: 1500 0000 a902 720a 0000 0072 0d00 0000  ......r....r....
+00000550: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000560: 1300 0000 720d 0000 001d 0000 00f3 0200  ....r...........
+00000570: 0000 0802 7a0c 5573 6572 2e75 7365 725f  ....z.User.user_
+00000580: 6964 6301 0000 0000 0000 0000 0000 0001  idc.............
+00000590: 0000 0001 0000 0043 0000 0072 1d00 0000  .......C...r....
+000005a0: 7215 0000 0072 1e00 0000 7219 0000 0072  r....r....r....r
+000005b0: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
+000005c0: 7573 6572 6e61 6d65 2100 0000 721f 0000  username!...r...
+000005d0: 007a 0d55 7365 722e 7573 6572 6e61 6d65  .z.User.username
+000005e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000005f0: 0002 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
+00000600: 6a00 6a01 6400 7501 720a 7c00 6a00 6a01  j.j.d.u.r.|.j.j.
+00000610: 5300 6401 5300 2902 4e46 2902 720a 0000  S.d.S.).NF).r...
+00000620: 00da 0e69 735f 7379 7374 656d 5f75 7365  ...is_system_use
+00000630: 7272 1900 0000 7212 0000 0072 1200 0000  rr....r....r....
+00000640: 7213 0000 0072 2100 0000 2500 0000 730a  r....r!...%...s.
+00000650: 0000 000c 0406 ff02 ff02 0302 fd7a 1355  .............z.U
+00000660: 7365 722e 6973 5f73 7973 7465 6d5f 7573  ser.is_system_us
+00000670: 6572 6301 0000 0000 0000 0000 0000 0001  erc.............
+00000680: 0000 0001 0000 0043 0000 0072 1d00 0000  .......C...r....
+00000690: 7215 0000 0029 0272 0a00 0000 da04 6e61  r....).r......na
+000006a0: 6d65 7219 0000 0072 1200 0000 7212 0000  mer....r....r...
+000006b0: 0072 1300 0000 7222 0000 002d 0000 0072  .r....r"...-...r
+000006c0: 1f00 0000 7a09 5573 6572 2e6e 616d 6563  ....z.User.namec
+000006d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000006e0: 0100 0000 4300 0000 721d 0000 0072 1500  ....C...r....r..
+000006f0: 0000 2902 720a 0000 00da 0b70 6963 7475  ..).r......pictu
+00000700: 7265 5f75 726c 7219 0000 0072 1200 0000  re_urlr....r....
+00000710: 7212 0000 0072 1300 0000 7223 0000 0031  r....r....r#...1
+00000720: 0000 0072 1f00 0000 7a10 5573 6572 2e70  ...r....z.User.p
+00000730: 6963 7475 7265 5f75 726c 7215 0000 0029  icture_urlr....)
+00000740: 0272 1800 0000 4e29 16da 085f 5f6e 616d  .r....N)...__nam
+00000750: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000760: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0800  .__qualname__r..
+00000770: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
+00000780: 735f 5f72 0700 0000 da0b 636c 6173 736d  s__r......classm
+00000790: 6574 686f 6472 0300 0000 da03 7374 7272  ethodr......strr
+000007a0: 1400 0000 7217 0000 00da 0464 6963 7472  ....r......dictr
+000007b0: 0200 0000 721a 0000 0072 1c00 0000 da08  ....r....r......
+000007c0: 7072 6f70 6572 7479 720d 0000 0072 2000  propertyr....r .
+000007d0: 0000 da04 626f 6f6c 7221 0000 0072 2200  ....boolr!...r".
+000007e0: 0000 7223 0000 0072 1200 0000 7212 0000  ..r#...r....r...
+000007f0: 0072 1200 0000 7213 0000 0072 0900 0000  .r....r....r....
+00000800: 0a00 0000 7324 0000 000a 0008 0108 0102  ....s$..........
+00000810: 021a 0112 0416 040a 0302 0310 0102 0310  ................
+00000820: 0102 0310 0102 0714 0102 0318 0172 0900  .............r..
+00000830: 0000 4e29 0ada 0674 7970 696e 6772 0200  ..N)...typingr..
+00000840: 0000 7203 0000 00da 0573 6572 6465 7205  ..r......serder.
+00000850: 0000 0072 0c00 0000 7207 0000 00da 0b75  ...r....r......u
+00000860: 7365 725f 7265 636f 7264 7208 0000 0072  ser_recordr....r
+00000870: 0900 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
+00000880: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000890: 653e 0100 0000 730a 0000 0010 020c 020c  e>....s.........
+000008a0: 010c 0112 03                             .....
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 485 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 e501 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 e501 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000070: 4f70 7469 6f6e 616c e901 0000 0029 01da  Optional.....)..
@@ -17,16 +17,16 @@
 00000100: 0c55 7365 7244 656c 6567 6174 6563 0100  .UserDelegatec..
 00000110: 0000 0000 0000 0000 0000 0100 0000 0200  ................
 00000120: 0000 0300 0000 730e 0000 0074 0083 00a0  ......s....t....
 00000130: 01a1 0001 0064 0053 0029 014e 2902 da05  .....d.S.).N)...
 00000140: 7375 7065 72da 085f 5f69 6e69 745f 5f29  super..__init__)
 00000150: 01da 0473 656c 66a9 01da 095f 5f63 6c61  ...self....__cla
 00000160: 7373 5f5f a900 faf2 2f63 6f64 6562 7569  ss__..../codebui
-00000170: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
-00000180: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
+00000170: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
+00000180: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
 00000190: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000001a0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000001b0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000001c0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000001d0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000001e0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000001f0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class User:
     __record: UserRecord
     __user_delegate: UserDelegate
 
     @classmethod
-    def by_id(cls, user_id: Optional[str], user_delegate: UserDelegate):
+    def from_id(cls, user_delegate: UserDelegate, user_id: Optional[str] = None):
         record = user_delegate.get_user_by_id(user_id=user_id)
         return cls(record=record, user_delegate=user_delegate)
 
     def __init__(self, record: UserRecord, user_delegate: UserDelegate):
         self.__record = record
         self.__user_delegate = user_delegate
 
@@ -37,7 +37,15 @@
     @property
     def is_system_user(self) -> bool:
         return (
             self.__record.is_system_user
             if self.__record.is_system_user is not None
             else False
         )
+
+    @property
+    def name(self) -> Optional[str]:
+        return self.__record.name
+
+    @property
+    def picture_url(self) -> Optional[str]:
+        return self.__record.picture_url
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.6/src/roboto_sdk/http/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from .constants import (
     ORG_OVERRIDE_HEADER,
     ORG_OVERRIDE_QUERY_PARAM,
     USER_OVERRIDE_HEADER,
     USER_OVERRIDE_QUERY_PARAM,
 )
+from .headers import headers_for_org_and_user
 from .http_client import (
     ClientError,
     HttpClient,
     HttpError,
     ServerError,
 )
 from .request_decorators import (
     LocalAuthDecorator,
     PATAuthDecorator,
     SigV4AuthDecorator,
 )
 from .testing_util import FakeHttpResponseFactory
 
 __all__ = (
+    "headers_for_org_and_user",
     "ClientError",
     "FakeHttpResponseFactory",
     "HttpClient",
     "HttpError",
     "LocalAuthDecorator",
     "PATAuthDecorator",
     "ServerError",
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 704 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 c002 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 0e03 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
+00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6400  m.Z.m.Z.m.Z...d.
-00000060: 6403 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
-00000070: 0100 6400 6404 6c0e 6d0f 5a0f 0100 6405  ..d.d.l.m.Z...d.
-00000080: 5a10 6406 5300 2907 e901 0000 0029 04da  Z.d.S.)......)..
-00000090: 134f 5247 5f4f 5645 5252 4944 455f 4845  .ORG_OVERRIDE_HE
-000000a0: 4144 4552 da18 4f52 475f 4f56 4552 5249  ADER..ORG_OVERRI
-000000b0: 4445 5f51 5545 5259 5f50 4152 414d da14  DE_QUERY_PARAM..
-000000c0: 5553 4552 5f4f 5645 5252 4944 455f 4845  USER_OVERRIDE_HE
-000000d0: 4144 4552 da19 5553 4552 5f4f 5645 5252  ADER..USER_OVERR
-000000e0: 4944 455f 5155 4552 595f 5041 5241 4d29  IDE_QUERY_PARAM)
-000000f0: 04da 0b43 6c69 656e 7445 7272 6f72 da0a  ...ClientError..
-00000100: 4874 7470 436c 6965 6e74 da09 4874 7470  HttpClient..Http
-00000110: 4572 726f 72da 0b53 6572 7665 7245 7272  Error..ServerErr
-00000120: 6f72 2903 da12 4c6f 6361 6c41 7574 6844  or)...LocalAuthD
-00000130: 6563 6f72 6174 6f72 da10 5041 5441 7574  ecorator..PATAut
-00000140: 6844 6563 6f72 6174 6f72 da12 5369 6756  hDecorator..SigV
-00000150: 3441 7574 6844 6563 6f72 6174 6f72 2901  4AuthDecorator).
-00000160: da17 4661 6b65 4874 7470 5265 7370 6f6e  ..FakeHttpRespon
-00000170: 7365 4661 6374 6f72 7929 0c72 0600 0000  seFactory).r....
-00000180: 720d 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000190: 0a00 0000 720b 0000 0072 0900 0000 720c  ....r....r....r.
-000001a0: 0000 0072 0200 0000 7203 0000 0072 0400  ...r....r....r..
-000001b0: 0000 7205 0000 004e 2911 da09 636f 6e73  ..r....N)...cons
-000001c0: 7461 6e74 7372 0200 0000 7203 0000 0072  tantsr....r....r
-000001d0: 0400 0000 7205 0000 00da 0b68 7474 705f  ....r......http_
-000001e0: 636c 6965 6e74 7206 0000 0072 0700 0000  clientr....r....
-000001f0: 7208 0000 0072 0900 0000 5a12 7265 7175  r....r....Z.requ
-00000200: 6573 745f 6465 636f 7261 746f 7273 720a  est_decoratorsr.
-00000210: 0000 0072 0b00 0000 720c 0000 005a 0c74  ...r....r....Z.t
-00000220: 6573 7469 6e67 5f75 7469 6c72 0d00 0000  esting_utilr....
-00000230: da07 5f5f 616c 6c5f 5fa9 0072 1100 0000  ..__all__..r....
-00000240: 7211 0000 00fa e52f 636f 6465 6275 696c  r....../codebuil
-00000250: 642f 6f75 7470 7574 2f73 7263 3334 3937  d/output/src3497
-00000260: 3236 3836 3730 2f73 7263 2f63 6f64 6573  268670/src/codes
-00000270: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
-00000280: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
-00000290: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
-000002a0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
-000002b0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
-000002c0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
-000002d0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
-000002e0: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
-000002f0: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
-00000300: 732f 726f 626f 746f 5f73 646b 2f73 7263  s/roboto_sdk/src
-00000310: 2f72 6f62 6f74 6f5f 7364 6b2f 6874 7470  /roboto_sdk/http
-00000320: 2f5f 5f69 6e69 745f 5f2e 7079 da08 3c6d  /__init__.py..<m
-00000330: 6f64 756c 653e 0100 0000 730a 0000 0018  odule>....s.....
-00000340: 0018 0614 060c 0508 02                   .........
+00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
+00000060: 6d0a 5a0a 6d0b 5a0b 0100 6400 6404 6c0c  m.Z.m.Z...d.d.l.
+00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400  m.Z.m.Z.m.Z...d.
+00000080: 6405 6c10 6d11 5a11 0100 6406 5a12 6407  d.l.m.Z...d.Z.d.
+00000090: 5300 2908 e901 0000 0029 04da 134f 5247  S.)......)...ORG
+000000a0: 5f4f 5645 5252 4944 455f 4845 4144 4552  _OVERRIDE_HEADER
+000000b0: da18 4f52 475f 4f56 4552 5249 4445 5f51  ..ORG_OVERRIDE_Q
+000000c0: 5545 5259 5f50 4152 414d da14 5553 4552  UERY_PARAM..USER
+000000d0: 5f4f 5645 5252 4944 455f 4845 4144 4552  _OVERRIDE_HEADER
+000000e0: da19 5553 4552 5f4f 5645 5252 4944 455f  ..USER_OVERRIDE_
+000000f0: 5155 4552 595f 5041 5241 4d29 01da 1868  QUERY_PARAM)...h
+00000100: 6561 6465 7273 5f66 6f72 5f6f 7267 5f61  eaders_for_org_a
+00000110: 6e64 5f75 7365 7229 04da 0b43 6c69 656e  nd_user)...Clien
+00000120: 7445 7272 6f72 da0a 4874 7470 436c 6965  tError..HttpClie
+00000130: 6e74 da09 4874 7470 4572 726f 72da 0b53  nt..HttpError..S
+00000140: 6572 7665 7245 7272 6f72 2903 da12 4c6f  erverError)...Lo
+00000150: 6361 6c41 7574 6844 6563 6f72 6174 6f72  calAuthDecorator
+00000160: da10 5041 5441 7574 6844 6563 6f72 6174  ..PATAuthDecorat
+00000170: 6f72 da12 5369 6756 3441 7574 6844 6563  or..SigV4AuthDec
+00000180: 6f72 6174 6f72 2901 da17 4661 6b65 4874  orator)...FakeHt
+00000190: 7470 5265 7370 6f6e 7365 4661 6374 6f72  tpResponseFactor
+000001a0: 7929 0d72 0600 0000 7207 0000 0072 0e00  y).r....r....r..
+000001b0: 0000 7208 0000 0072 0900 0000 720b 0000  ..r....r....r...
+000001c0: 0072 0c00 0000 720a 0000 0072 0d00 0000  .r....r....r....
+000001d0: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+000001e0: 0500 0000 4e29 13da 0963 6f6e 7374 616e  ....N)...constan
+000001f0: 7473 7202 0000 0072 0300 0000 7204 0000  tsr....r....r...
+00000200: 0072 0500 0000 da07 6865 6164 6572 7372  .r......headersr
+00000210: 0600 0000 da0b 6874 7470 5f63 6c69 656e  ......http_clien
+00000220: 7472 0700 0000 7208 0000 0072 0900 0000  tr....r....r....
+00000230: 720a 0000 005a 1272 6571 7565 7374 5f64  r....Z.request_d
+00000240: 6563 6f72 6174 6f72 7372 0b00 0000 720c  ecoratorsr....r.
+00000250: 0000 0072 0d00 0000 5a0c 7465 7374 696e  ...r....Z.testin
+00000260: 675f 7574 696c 720e 0000 00da 075f 5f61  g_utilr......__a
+00000270: 6c6c 5f5f a900 7213 0000 0072 1300 0000  ll__..r....r....
+00000280: fae5 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
+00000290: 7075 742f 7372 6331 3638 3931 3535 3339  put/src168915539
+000002a0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000002b0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
+000002c0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
+000002d0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
+000002e0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
+000002f0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
+00000300: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
+00000310: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
+00000320: 692f 726f 626f 746f 2d68 6f73 7465 642d  i/roboto-hosted-
+00000330: 6170 702f 7061 636b 6167 6573 2f72 6f62  app/packages/rob
+00000340: 6f74 6f5f 7364 6b2f 7372 632f 726f 626f  oto_sdk/src/robo
+00000350: 746f 5f73 646b 2f68 7474 702f 5f5f 696e  to_sdk/http/__in
+00000360: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
+00000370: 3e01 0000 0073 0c00 0000 1800 0c06 1801  >....s..........
+00000380: 1406 0c05 0802                           ......
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 9060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 6423 0000  o.......Ms.dd#..
+00000000: 6f0d 0d0a 0000 0000 3192 a764 6423 0000  o.......1..dd#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a07 6400 6401 6c08 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c09 5a07 6400 6401 6c0a 5a07 6400  d.l.Z.d.d.l.Z.d.
@@ -42,15 +42,15 @@
 00000290: 0463 6f64 655a 1154 4f4f 5f4d 414e 595f  .codeZ.TOO_MANY_
 000002a0: 5245 5155 4553 5453 5a13 5345 5256 4943  REQUESTSZ.SERVIC
 000002b0: 455f 554e 4156 4149 4c41 424c 45da 0a56  E_UNAVAILABLE..V
 000002c0: 616c 7565 4572 726f 72da 0855 524c 4572  alueError..URLEr
 000002d0: 726f 72da 0373 7472 da06 7265 6173 6f6e  ror..str..reason
 000002e0: 2901 7205 0000 00a9 0072 1300 0000 fae8  ).r......r......
 000002f0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000300: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+00000300: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
 00000310: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000320: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000330: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000340: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000350: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000360: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000370: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 3161 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 590c 0000  o.......Ms.dY...
+00000000: 6f0d 0d0a 0000 0000 3192 a764 590c 0000  o.......1..dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -33,16 +33,16 @@
 00000200: 7574 6844 6563 6f72 6174 6f72 5f5f 7573  uthDecorator__us
 00000210: 6572 5f69 64da 0775 7365 725f 6964 6302  er_id..user_idc.
 00000220: 0000 0000 0000 0000 0000 0002 0000 0002  ................
 00000230: 0000 0043 0000 00f3 0a00 0000 7c01 7c00  ...C........|.|.
 00000240: 5f00 6400 5300 a901 4e29 0172 0e00 0000  _.d.S...N).r....
 00000250: 2902 da04 7365 6c66 720f 0000 00a9 0072  )...selfr......r
 00000260: 1300 0000 faef 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000270: 2f6f 7574 7075 742f 7372 6333 3439 3732  /output/src34972
-00000280: 3638 3637 302f 7372 632f 636f 6465 7374  68670/src/codest
+00000270: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
+00000280: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
 00000290: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000002a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000002b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000002c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000002d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000002e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000002f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 1004 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 ec03 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 ec03 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6402 6403 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6404 6405 8400 6405 8302 5a08  ..G.d.d...d...Z.
 00000070: 6401 5300 2906 e900 0000 004e e901 0000  d.S.)......N....
@@ -36,16 +36,16 @@
 00000230: 5f00 7c04 7007 7401 8300 7c00 5f02 7c02  _.|.p.t...|._.|.
 00000240: 7c00 5f03 7c01 7c00 5f04 6400 5300 a901  |._.|.|._.d.S...
 00000250: 4e29 0572 0700 0000 da04 6469 6374 7205  N).r......dictr.
 00000260: 0000 0072 0600 0000 7208 0000 0029 05da  ...r....r....)..
 00000270: 0473 656c 6672 0a00 0000 720b 0000 0072  .selfr....r....r
 00000280: 0c00 0000 720d 0000 00a9 0072 1200 0000  ....r......r....
 00000290: fae9 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000002a0: 7075 742f 7372 6333 3439 3732 3638 3637  put/src349726867
-000002b0: 302f 7372 632f 636f 6465 7374 6172 2d63  0/src/codestar-c
+000002a0: 7075 742f 7372 6331 3638 3931 3535 3339  put/src168915539
+000002b0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
 000002c0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000002d0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000002e0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000002f0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000300: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000310: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000320: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.6/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.6/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.6/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc` & `roboto_sdk-0.1.6/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 01:18:05 2023 UTC, .py size: 2977 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4d73 a364 a10b 0000  o.......Ms.d....
+00000000: 6f0d 0d0a 0000 0000 3192 a764 a10b 0000  o.......1..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c07 5a07 6403 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6509 8300 5a0a 6405 5a0b 6406 5a0c  ..e...Z.d.Z.d.Z.
@@ -35,16 +35,16 @@
 00000220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000230: 5f5f da03 7374 72da 0f5f 5f61 6e6e 6f74  __..str..__annot
 00000240: 6174 696f 6e73 5f5f da0d 5052 4f44 5f45  ations__..PROD_E
 00000250: 4e44 504f 494e 5472 0a00 0000 da18 5052  NDPOINTr......PR
 00000260: 4f44 5f55 5345 525f 504f 4f4c 5f43 4c49  OD_USER_POOL_CLI
 00000270: 454e 545f 4944 720b 0000 00a9 0072 1300  ENT_IDr......r..
 00000280: 0000 7213 0000 00fa e72f 636f 6465 6275  ..r....../codebu
-00000290: 696c 642f 6f75 7470 7574 2f73 7263 3334  ild/output/src34
-000002a0: 3937 3236 3836 3730 2f73 7263 2f63 6f64  97268670/src/cod
+00000290: 696c 642f 6f75 7470 7574 2f73 7263 3136  ild/output/src16
+000002a0: 3839 3135 3533 3939 2f73 7263 2f63 6f64  89155399/src/cod
 000002b0: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 000002c0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000002d0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000002e0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000002f0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000300: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 00000310: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.6/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.6/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.5/PKG-INFO` & `roboto_sdk-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

