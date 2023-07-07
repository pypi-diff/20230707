# Comparing `tmp/influxdb3-python-cli-0.3.0.tar.gz` & `tmp/influxdb3-python-cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.3.0.tar", last modified: Tue Jul  4 15:23:42 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.3.1.tar", last modified: Fri Jul  7 09:45:22 2023, max compression
```

## Comparing `influxdb3-python-cli-0.3.0.tar` & `influxdb3-python-cli-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11720 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/influx3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/openai_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:23:42.672693 influxdb3-python-cli-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:22.536999 influxdb3-python-cli-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-07 09:45:22.536999 influxdb3-python-cli-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:22.536999 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-07 09:45:22.000000 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-07 09:45:22.000000 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:45:22.000000 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 09:45:22.000000 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 09:45:22.000000 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 09:45:22.000000 influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:22.536999 influxdb3-python-cli-0.3.1/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/influxdb_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/influxdb_cli/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12288 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/influxdb_cli/openai_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:45:22.536999 influxdb3-python-cli-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-07 09:45:07.000000 influxdb3-python-cli-0.3.1/setup.py
```

### Comparing `influxdb3-python-cli-0.3.0/LICENSE` & `influxdb3-python-cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.3.0/PKG-INFO` & `influxdb3-python-cli-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -139,31 +139,31 @@
 home,room=kitchen temp=70.5,hum=80
 ```
 
 To exit a prompt, enter `exit`.
 
 ## Write from a file
 
-The InfluxDB CLI and client library can write data from a CSV file.
+The InfluxDB CLI and client library can write data from CSV, JSON, ORC, Parquet and Feather files.
 The CSV file must contain the following:
 
 - A header row with column names
 - A column that contains a timestamp for each row
 
 The following CLI options specify how data is parsed:
 
-* `--file` - The path to the csv file.
+* `--file` - The path to the file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
-* `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
+* `--measurement` - The name of the measurement to store the data under. (Optional, will look for a measurement column in data otherwise).
+* `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user-specified strings) for example: `--tags=host,region`
 
 The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
 
 ```bash
-influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
+influx3 write_file --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 ## Config Commands
 
 The `config` command allows you to manage configurations for your application. It has the following subcommands: `create`, `update`, `use`, `delete`, and `list`.
 
 ### Create
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.3.1 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -41,51 +41,51 @@
 >) select * from home ``` The `influx3` CLI displays query results in Markdown
 table format--for example: ``` | | co | hum | room | temp | time | |----:|----
 -:|------:|:------------|-------:|:------------------------------| | 0 | 0 |
 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 |
 2023-03-09 08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>)
 write ``` At the `(write >)` prompt, enter line protocol data. ``` (>) write
 home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
-from a file The InfluxDB CLI and client library can write data from a CSV file.
-The CSV file must contain the following: - A header row with column names - A
-column that contains a timestamp for each row The following CLI options specify
-how data is parsed: * `--file` - The path to the csv file. * `--time` - The
-name of the column containing the timestamp. * `--measurement` - The name of
-the measurment to store the CSV data under. (Currently only supports user
-specified string) * `--tags` - (optional) Specify an array of column names to
-use as tags. (Currently only supports user specified strings) for example: `--
-tags=host,region` The following example shows how to write CSV data from the
-[`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-
-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol): ```bash
-influx3 write_csv --file ./Examples/example.csv --measurement table2 --time
-Date --tags host,region ``` ## Config Commands The `config` command allows you
-to manage configurations for your application. It has the following
-subcommands: `create`, `update`, `use`, `delete`, and `list`. ### Create The
-`create` subcommand creates a new configuration. It requires the `--name`, `--
-host`, `--token`, `--database`, and `--org` parameters. The `--active`
-parameter is optional and can be used to set the new configuration as the
-active one. Example usage: ```bash influx3.py config create --name="my-config"
---host="us-east-1-1.aws.cloud2.influxdata.com" --token="" --database="" --
-org="" --active ``` ### Update The `update` subcommand updates an existing
-configuration. The `--name` parameter is required to specify which
-configuration to update. All other parameters (`--host`, `--token`, `--
-database`, `--org`, `--active`) are optional. Example usage: ```bash influx3.py
-config update --name="my-config" --host="new-host.com" ``` ### Use The `use`
-subcommand sets a specific configuration as the active one. The `--name`
-parameter is required to specify which configuration to use. Example usage:
-```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
-subcommand deletes a configuration. The `--name` parameter is required to
-specify which configuration to delete. Example usage: ```bash influx3.py config
-delete --name="my-config" ``` ### List The `list` subcommand lists all the
-configurations. Example usage: ```bash influx3.py config list ``` Please
-replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
-and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The CLI
-also contians a beta feature that allows you to query your data using OpenAI's
-ChatGPT. To use this feature, you must have an OpenAI API key. You can get one
-by signing up for the [OpenAI waitlist](https://share.hsforms.com/
+from a file The InfluxDB CLI and client library can write data from CSV, JSON,
+ORC, Parquet and Feather files. The CSV file must contain the following: - A
+header row with column names - A column that contains a timestamp for each row
+The following CLI options specify how data is parsed: * `--file` - The path to
+the file. * `--time` - The name of the column containing the timestamp. * `--
+measurement` - The name of the measurement to store the data under. (Optional,
+will look for a measurement column in data otherwise). * `--tags` - (optional)
+Specify an array of column names to use as tags. (Currently only supports user-
+specified strings) for example: `--tags=host,region` The following example
+shows how to write CSV data from the [`./Examples/example.csv` file](https://
+github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to
+InfluxDB (as line protocol): ```bash influx3 write_file --file ./Examples/
+example.csv --measurement table2 --time Date --tags host,region ``` ## Config
+Commands The `config` command allows you to manage configurations for your
+application. It has the following subcommands: `create`, `update`, `use`,
+`delete`, and `list`. ### Create The `create` subcommand creates a new
+configuration. It requires the `--name`, `--host`, `--token`, `--database`, and
+`--org` parameters. The `--active` parameter is optional and can be used to set
+the new configuration as the active one. Example usage: ```bash influx3.py
+config create --name="my-config" --host="us-east-1-1.aws.cloud2.influxdata.com"
+--token="" --database="" --org="" --active ``` ### Update The `update`
+subcommand updates an existing configuration. The `--name` parameter is
+required to specify which configuration to update. All other parameters (`--
+host`, `--token`, `--database`, `--org`, `--active`) are optional. Example
+usage: ```bash influx3.py config update --name="my-config" --host="new-
+host.com" ``` ### Use The `use` subcommand sets a specific configuration as the
+active one. The `--name` parameter is required to specify which configuration
+to use. Example usage: ```bash influx3.py config use --name="my-config" ``` ###
+Delete The `delete` subcommand deletes a configuration. The `--name` parameter
+is required to specify which configuration to delete. Example usage: ```bash
+influx3.py config delete --name="my-config" ``` ### List The `list` subcommand
+lists all the configurations. Example usage: ```bash influx3.py config list ```
+Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`,
+`""`, and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The
+CLI also contians a beta feature that allows you to query your data using
+OpenAI's ChatGPT. To use this feature, you must have an OpenAI API key. You can
+get one by signing up for the [OpenAI waitlist](https://share.hsforms.com/
 1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an
 environment variable called `OPENAI_API_KEY`. To use this feature, you can use
 the `chatgpt` command: ``` export OPENAI_API_KEY=sk-o2Sbq3aVBp influx3 chatgpt
 get average vibration grouped by machineID from machine_data Run InfluxQL
 query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY
 machineID | | iox::measurement | time | machineID | avg_vibration | |---:|:----
 ---------------|:--------------------|:------------|----------------:| | 0 |
```

### Comparing `influxdb3-python-cli-0.3.0/README.md` & `influxdb3-python-cli-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,31 +120,31 @@
 home,room=kitchen temp=70.5,hum=80
 ```
 
 To exit a prompt, enter `exit`.
 
 ## Write from a file
 
-The InfluxDB CLI and client library can write data from a CSV file.
+The InfluxDB CLI and client library can write data from CSV, JSON, ORC, Parquet and Feather files.
 The CSV file must contain the following:
 
 - A header row with column names
 - A column that contains a timestamp for each row
 
 The following CLI options specify how data is parsed:
 
-* `--file` - The path to the csv file.
+* `--file` - The path to the file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
-* `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
+* `--measurement` - The name of the measurement to store the data under. (Optional, will look for a measurement column in data otherwise).
+* `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user-specified strings) for example: `--tags=host,region`
 
 The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
 
 ```bash
-influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
+influx3 write_file --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 ## Config Commands
 
 The `config` command allows you to manage configurations for your application. It has the following subcommands: `create`, `update`, `use`, `delete`, and `list`.
 
 ### Create
```

#### html2text {}

```diff
@@ -31,51 +31,51 @@
 >) select * from home ``` The `influx3` CLI displays query results in Markdown
 table format--for example: ``` | | co | hum | room | temp | time | |----:|----
 -:|------:|:------------|-------:|:------------------------------| | 0 | 0 |
 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 |
 2023-03-09 08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>)
 write ``` At the `(write >)` prompt, enter line protocol data. ``` (>) write
 home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
-from a file The InfluxDB CLI and client library can write data from a CSV file.
-The CSV file must contain the following: - A header row with column names - A
-column that contains a timestamp for each row The following CLI options specify
-how data is parsed: * `--file` - The path to the csv file. * `--time` - The
-name of the column containing the timestamp. * `--measurement` - The name of
-the measurment to store the CSV data under. (Currently only supports user
-specified string) * `--tags` - (optional) Specify an array of column names to
-use as tags. (Currently only supports user specified strings) for example: `--
-tags=host,region` The following example shows how to write CSV data from the
-[`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-
-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol): ```bash
-influx3 write_csv --file ./Examples/example.csv --measurement table2 --time
-Date --tags host,region ``` ## Config Commands The `config` command allows you
-to manage configurations for your application. It has the following
-subcommands: `create`, `update`, `use`, `delete`, and `list`. ### Create The
-`create` subcommand creates a new configuration. It requires the `--name`, `--
-host`, `--token`, `--database`, and `--org` parameters. The `--active`
-parameter is optional and can be used to set the new configuration as the
-active one. Example usage: ```bash influx3.py config create --name="my-config"
---host="us-east-1-1.aws.cloud2.influxdata.com" --token="" --database="" --
-org="" --active ``` ### Update The `update` subcommand updates an existing
-configuration. The `--name` parameter is required to specify which
-configuration to update. All other parameters (`--host`, `--token`, `--
-database`, `--org`, `--active`) are optional. Example usage: ```bash influx3.py
-config update --name="my-config" --host="new-host.com" ``` ### Use The `use`
-subcommand sets a specific configuration as the active one. The `--name`
-parameter is required to specify which configuration to use. Example usage:
-```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
-subcommand deletes a configuration. The `--name` parameter is required to
-specify which configuration to delete. Example usage: ```bash influx3.py config
-delete --name="my-config" ``` ### List The `list` subcommand lists all the
-configurations. Example usage: ```bash influx3.py config list ``` Please
-replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
-and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The CLI
-also contians a beta feature that allows you to query your data using OpenAI's
-ChatGPT. To use this feature, you must have an OpenAI API key. You can get one
-by signing up for the [OpenAI waitlist](https://share.hsforms.com/
+from a file The InfluxDB CLI and client library can write data from CSV, JSON,
+ORC, Parquet and Feather files. The CSV file must contain the following: - A
+header row with column names - A column that contains a timestamp for each row
+The following CLI options specify how data is parsed: * `--file` - The path to
+the file. * `--time` - The name of the column containing the timestamp. * `--
+measurement` - The name of the measurement to store the data under. (Optional,
+will look for a measurement column in data otherwise). * `--tags` - (optional)
+Specify an array of column names to use as tags. (Currently only supports user-
+specified strings) for example: `--tags=host,region` The following example
+shows how to write CSV data from the [`./Examples/example.csv` file](https://
+github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to
+InfluxDB (as line protocol): ```bash influx3 write_file --file ./Examples/
+example.csv --measurement table2 --time Date --tags host,region ``` ## Config
+Commands The `config` command allows you to manage configurations for your
+application. It has the following subcommands: `create`, `update`, `use`,
+`delete`, and `list`. ### Create The `create` subcommand creates a new
+configuration. It requires the `--name`, `--host`, `--token`, `--database`, and
+`--org` parameters. The `--active` parameter is optional and can be used to set
+the new configuration as the active one. Example usage: ```bash influx3.py
+config create --name="my-config" --host="us-east-1-1.aws.cloud2.influxdata.com"
+--token="" --database="" --org="" --active ``` ### Update The `update`
+subcommand updates an existing configuration. The `--name` parameter is
+required to specify which configuration to update. All other parameters (`--
+host`, `--token`, `--database`, `--org`, `--active`) are optional. Example
+usage: ```bash influx3.py config update --name="my-config" --host="new-
+host.com" ``` ### Use The `use` subcommand sets a specific configuration as the
+active one. The `--name` parameter is required to specify which configuration
+to use. Example usage: ```bash influx3.py config use --name="my-config" ``` ###
+Delete The `delete` subcommand deletes a configuration. The `--name` parameter
+is required to specify which configuration to delete. Example usage: ```bash
+influx3.py config delete --name="my-config" ``` ### List The `list` subcommand
+lists all the configurations. Example usage: ```bash influx3.py config list ```
+Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`,
+`""`, and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The
+CLI also contians a beta feature that allows you to query your data using
+OpenAI's ChatGPT. To use this feature, you must have an OpenAI API key. You can
+get one by signing up for the [OpenAI waitlist](https://share.hsforms.com/
 1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an
 environment variable called `OPENAI_API_KEY`. To use this feature, you can use
 the `chatgpt` command: ``` export OPENAI_API_KEY=sk-o2Sbq3aVBp influx3 chatgpt
 get average vibration grouped by machineID from machine_data Run InfluxQL
 query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY
 machineID | | iox::measurement | time | machineID | avg_vibration | |---:|:----
 ---------------|:--------------------|:------------|----------------:| | 0 |
```

### Comparing `influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.3.1/influxdb3_python_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -139,31 +139,31 @@
 home,room=kitchen temp=70.5,hum=80
 ```
 
 To exit a prompt, enter `exit`.
 
 ## Write from a file
 
-The InfluxDB CLI and client library can write data from a CSV file.
+The InfluxDB CLI and client library can write data from CSV, JSON, ORC, Parquet and Feather files.
 The CSV file must contain the following:
 
 - A header row with column names
 - A column that contains a timestamp for each row
 
 The following CLI options specify how data is parsed:
 
-* `--file` - The path to the csv file.
+* `--file` - The path to the file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
-* `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
+* `--measurement` - The name of the measurement to store the data under. (Optional, will look for a measurement column in data otherwise).
+* `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user-specified strings) for example: `--tags=host,region`
 
 The following example shows how to write CSV data from the [`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol):
 
 ```bash
-influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
+influx3 write_file --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 ## Config Commands
 
 The `config` command allows you to manage configurations for your application. It has the following subcommands: `create`, `update`, `use`, `delete`, and `list`.
 
 ### Create
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.3.1 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -41,51 +41,51 @@
 >) select * from home ``` The `influx3` CLI displays query results in Markdown
 table format--for example: ``` | | co | hum | room | temp | time | |----:|----
 -:|------:|:------------|-------:|:------------------------------| | 0 | 0 |
 35.9 | Kitchen | 21 | 2023-03-09 08:00:00 | | 1 | 0 | 35.9 | Kitchen | 21 |
 2023-03-09 08:00:50 | ``` To write, type `write` at the `(>)` prompt. ``` (>)
 write ``` At the `(write >)` prompt, enter line protocol data. ``` (>) write
 home,room=kitchen temp=70.5,hum=80 ``` To exit a prompt, enter `exit`. ## Write
-from a file The InfluxDB CLI and client library can write data from a CSV file.
-The CSV file must contain the following: - A header row with column names - A
-column that contains a timestamp for each row The following CLI options specify
-how data is parsed: * `--file` - The path to the csv file. * `--time` - The
-name of the column containing the timestamp. * `--measurement` - The name of
-the measurment to store the CSV data under. (Currently only supports user
-specified string) * `--tags` - (optional) Specify an array of column names to
-use as tags. (Currently only supports user specified strings) for example: `--
-tags=host,region` The following example shows how to write CSV data from the
-[`./Examples/example.csv` file](https://github.com/InfluxCommunity/influxdb3-
-python/blob/main/Examples/example.csv) to InfluxDB (as line protocol): ```bash
-influx3 write_csv --file ./Examples/example.csv --measurement table2 --time
-Date --tags host,region ``` ## Config Commands The `config` command allows you
-to manage configurations for your application. It has the following
-subcommands: `create`, `update`, `use`, `delete`, and `list`. ### Create The
-`create` subcommand creates a new configuration. It requires the `--name`, `--
-host`, `--token`, `--database`, and `--org` parameters. The `--active`
-parameter is optional and can be used to set the new configuration as the
-active one. Example usage: ```bash influx3.py config create --name="my-config"
---host="us-east-1-1.aws.cloud2.influxdata.com" --token="" --database="" --
-org="" --active ``` ### Update The `update` subcommand updates an existing
-configuration. The `--name` parameter is required to specify which
-configuration to update. All other parameters (`--host`, `--token`, `--
-database`, `--org`, `--active`) are optional. Example usage: ```bash influx3.py
-config update --name="my-config" --host="new-host.com" ``` ### Use The `use`
-subcommand sets a specific configuration as the active one. The `--name`
-parameter is required to specify which configuration to use. Example usage:
-```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
-subcommand deletes a configuration. The `--name` parameter is required to
-specify which configuration to delete. Example usage: ```bash influx3.py config
-delete --name="my-config" ``` ### List The `list` subcommand lists all the
-configurations. Example usage: ```bash influx3.py config list ``` Please
-replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
-and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The CLI
-also contians a beta feature that allows you to query your data using OpenAI's
-ChatGPT. To use this feature, you must have an OpenAI API key. You can get one
-by signing up for the [OpenAI waitlist](https://share.hsforms.com/
+from a file The InfluxDB CLI and client library can write data from CSV, JSON,
+ORC, Parquet and Feather files. The CSV file must contain the following: - A
+header row with column names - A column that contains a timestamp for each row
+The following CLI options specify how data is parsed: * `--file` - The path to
+the file. * `--time` - The name of the column containing the timestamp. * `--
+measurement` - The name of the measurement to store the data under. (Optional,
+will look for a measurement column in data otherwise). * `--tags` - (optional)
+Specify an array of column names to use as tags. (Currently only supports user-
+specified strings) for example: `--tags=host,region` The following example
+shows how to write CSV data from the [`./Examples/example.csv` file](https://
+github.com/InfluxCommunity/influxdb3-python/blob/main/Examples/example.csv) to
+InfluxDB (as line protocol): ```bash influx3 write_file --file ./Examples/
+example.csv --measurement table2 --time Date --tags host,region ``` ## Config
+Commands The `config` command allows you to manage configurations for your
+application. It has the following subcommands: `create`, `update`, `use`,
+`delete`, and `list`. ### Create The `create` subcommand creates a new
+configuration. It requires the `--name`, `--host`, `--token`, `--database`, and
+`--org` parameters. The `--active` parameter is optional and can be used to set
+the new configuration as the active one. Example usage: ```bash influx3.py
+config create --name="my-config" --host="us-east-1-1.aws.cloud2.influxdata.com"
+--token="" --database="" --org="" --active ``` ### Update The `update`
+subcommand updates an existing configuration. The `--name` parameter is
+required to specify which configuration to update. All other parameters (`--
+host`, `--token`, `--database`, `--org`, `--active`) are optional. Example
+usage: ```bash influx3.py config update --name="my-config" --host="new-
+host.com" ``` ### Use The `use` subcommand sets a specific configuration as the
+active one. The `--name` parameter is required to specify which configuration
+to use. Example usage: ```bash influx3.py config use --name="my-config" ``` ###
+Delete The `delete` subcommand deletes a configuration. The `--name` parameter
+is required to specify which configuration to delete. Example usage: ```bash
+influx3.py config delete --name="my-config" ``` ### List The `list` subcommand
+lists all the configurations. Example usage: ```bash influx3.py config list ```
+Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`,
+`""`, and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The
+CLI also contians a beta feature that allows you to query your data using
+OpenAI's ChatGPT. To use this feature, you must have an OpenAI API key. You can
+get one by signing up for the [OpenAI waitlist](https://share.hsforms.com/
 1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an
 environment variable called `OPENAI_API_KEY`. To use this feature, you can use
 the `chatgpt` command: ``` export OPENAI_API_KEY=sk-o2Sbq3aVBp influx3 chatgpt
 get average vibration grouped by machineID from machine_data Run InfluxQL
 query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY
 machineID | | iox::measurement | time | machineID | avg_vibration | |---:|:----
 ---------------|:--------------------|:------------|----------------:| | 0 |
```

### Comparing `influxdb3-python-cli-0.3.0/influxdb_cli/helper.py` & `influxdb3-python-cli-0.3.1/influxdb_cli/helper.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.3.0/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.3.1/influxdb_cli/influx3.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import cmd
 import argparse
 from prompt_toolkit import PromptSession
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.lexers import PygmentsLexer
 from pygments.lexers import SqlLexer
 from influxdb_client_3 import InfluxDBClient3
-from .helper import config_helper
-from .openai_helper import OpenAIHelper
+from helper import config_helper
+from openai_helper import OpenAIHelper
 
 _usage_string = """
 to write data use influxdb line protocol:
 > influx3 write testmes,tag1=tagvalue field1=0.0 <optional timestamp>
 
 to read data with sql:
 > influx3 sql select * from testmes where time > now() - interval'1 minute'
@@ -103,35 +103,50 @@
             return
         if arg == "":
             print("can't write, no line protocol supplied")
             return
         
         self.influxdb_client.write(record=arg)
     
-    def do_write_csv(self, args):
+    def do_write_file(self, args):
         if self.active_config == {}:
             print("can't write, no active configs")
             return
 
         temp = {}
         attributes = ['file', 'measurement', 'time', 'tags']
         temp['tags'] = []
 
         for attribute in attributes:
             arg_value = getattr(args, attribute)
             if arg_value is not None:
                 temp[attribute] = arg_value
         if isinstance(temp['tags'], str):
             temp['tags'] =  temp['tags'].split(',')
+        
 
-
-        self.influxdb_client.write_csv(csv_file=temp['file'], 
+        if 'measurement' in temp:
+            try:
+                self.influxdb_client.write_file(file=temp['file'], 
                                        measurement_name=temp['measurement'], 
                                        timestamp_column=temp['time'], 
                                        tag_columns=temp['tags'])
+                
+            except Exception as e:
+                print(e)
+        else:
+            print("measurement not specified. Attempting to find measurement in file...")
+            try:
+                self.influxdb_client.write_file(file=temp['file'], 
+                                       timestamp_column=temp['time'], 
+                                       tag_columns=temp['tags'])
+                
+            except Exception as e:
+                print(e)
+                
 
     def do_exit(self, arg):
         'Exit the shell: exit'
         print('\nExiting ...')
         return True
 
     def do_EOF(self, arg):
@@ -229,19 +244,19 @@
 
     chatgpt_parser = subparsers.add_parser('chatgpt', help='execute the given chatgpt statement')
     chatgpt_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the chatgpt query to execute')
 
     write_parser = subparsers.add_parser('write', help='write line protocol to InfluxDB')
     write_parser.add_argument('line_protocol', metavar='LINE PROTOCOL',  nargs='*', action=StoreRemainingInput, help='the data to write')
 
-    write_csv_parser = subparsers.add_parser('write_csv', help='write CSV data to InfluxDB')
-    write_csv_parser.add_argument('--file', help='the CSV file to import', required=True)
-    write_csv_parser.add_argument('--measurement', help='Define the name of the measurement', required=True)
-    write_csv_parser.add_argument('--time', help='Define the name of the time column with the csv file', required=True)
-    write_csv_parser.add_argument('--tags', help='(optional) array of column names which are tags. Format should be: ["tag1", "tag2"]', required=False)
+    write_file_parser = subparsers.add_parser('write_file', help='write data from file to InfluxDB')
+    write_file_parser.add_argument('--file', help='the file to import', required=True)
+    write_file_parser.add_argument('--measurement', help='Define the name of the measurement', required=False)
+    write_file_parser.add_argument('--time', help='Define the name of the time column within the file', required=True)
+    write_file_parser.add_argument('--tags', help='(optional) array of column names which are tags. Format should be: ["tag1", "tag2"]', required=False)
 
     config_parser = subparsers.add_parser("config", help="configure the application")
     config_subparsers = config_parser.add_subparsers(dest='config_command')
 
     create_parser = config_subparsers.add_parser("create", help="create a new configuration")
     create_parser.add_argument("--name", help="Configuration name", required=True)
     create_parser.add_argument("--host", help="Host string", required=True)
@@ -281,16 +296,16 @@
         app.do_query(args.query, language='sql')
     if args.command == 'influxql':
         app.do_query(args.query, language='influxql')
     if args.command == 'chatgpt':
         app.do_chatgpt(args.query)
     if args.command == 'write':
         app.do_write(args.line_protocol)
-    if args.command == 'write_csv':
-        app.do_write_csv(args)
+    if args.command == 'write_file':
+        app.do_write_file(args)
     if args.command == 'config':
         if args.config_command == 'create':
             app.create_config(args)
         elif args.config_command == 'delete':
             app.delete_config(args)
         elif args.config_command == 'list':
             app.list_config(args)
```

### Comparing `influxdb3-python-cli-0.3.0/influxdb_cli/openai_helper.py` & `influxdb3-python-cli-0.3.1/influxdb_cli/openai_helper.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.3.0/setup.py` & `influxdb3-python-cli-0.3.1/setup.py`

 * *Files identical despite different names*

