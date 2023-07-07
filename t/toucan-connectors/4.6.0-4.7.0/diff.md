# Comparing `tmp/toucan_connectors-4.6.0.tar.gz` & `tmp/toucan_connectors-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_connectors-4.6.0.tar", max compression
+gzip compressed data, was "toucan_connectors-4.7.0.tar", max compression
```

## Comparing `toucan_connectors-4.6.0.tar` & `toucan_connectors-4.7.0.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1510 2023-06-02 09:26:49.571571 toucan_connectors-4.6.0/LICENSE
--rw-r--r--   0        0        0     9969 2023-06-02 09:26:49.571571 toucan_connectors-4.6.0/README.md
--rw-r--r--   0        0        0     5573 2023-06-02 09:26:49.575571 toucan_connectors-4.6.0/pyproject.toml
--rw-r--r--   0        0        0    10795 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/__init__.py
--rw-r--r--   0        0        0    13648 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe-analytics.png
--rw-r--r--   0        0        0     1740 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/anaplan/__init__.py
--rw-r--r--   0        0        0     7277 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan.png
--rw-r--r--   0        0        0     7005 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan_connector.py
--rw-r--r--   0        0        0     4622 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/auth.py
--rw-r--r--   0        0        0    61900 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/aws/aws.png
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/awsathena/__init__.py
--rw-r--r--   0        0        0     2524 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/awsathena/athena.png
--rw-r--r--   0        0        0     8464 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/awsathena/awsathena_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/azure_mssql/__init__.py
--rw-r--r--   0        0        0     2404 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/azure_mssql/azure_mssql_connector.py
--rw-r--r--   0        0        0    24249 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/azure_mssql/sql-azure.png
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/clickhouse/__init__.py
--rw-r--r--   0        0        0     1780 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse.png
--rw-r--r--   0        0        0     4541 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse_connector.py
--rw-r--r--   0        0        0    15322 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/common.py
--rw-r--r--   0        0        0     5549 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/condition_translator.py
--rw-r--r--   0        0        0     8162 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/connection_manager.py
--rw-r--r--   0        0        0     3534 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/databricks/databricks.png
--rw-r--r--   0        0        0     5236 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/databricks/databricks_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/dataiku/__init__.py
--rw-r--r--   0        0        0    10971 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku.png
--rw-r--r--   0        0        0     1100 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku_connector.py
--rwxr-xr-x   0        0        0      235 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/default-logo.png
--rw-r--r--   0        0        0     3331 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/denodo/denodo.png
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/elasticsearch/__init__.py
--rw-r--r--   0        0        0    29549 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch.png
--rw-r--r--   0        0        0     5118 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/__init__.py
--rw-r--r--   0        0        0      452 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/doc.md
--rw-r--r--   0        0        0      183 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/enums.py
--rw-r--r--   0        0        0     5283 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_ads_connector.py
--rw-r--r--   0        0        0    27755 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_logo.png
--rw-r--r--   0        0        0      126 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/helpers.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_insights/__init__.py
--rw-r--r--   0        0        0    38402 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook-insights.png
--rw-r--r--   0        0        0     3985 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook_insights_connector.py
--rw-r--r--   0        0        0    13001 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/GitHub_Logo.png
--rw-r--r--   0        0        0      412 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/doc.md
--rw-r--r--   0        0        0    17081 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/github_connector.py
--rw-r--r--   0        0        0    15902 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/helpers.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/__init__.py
--rw-r--r--   0        0        0      469 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/doc.md
--rw-r--r--   0        0        0    68711 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords.jpg
--rw-r--r--   0        0        0     9049 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords_connector.py
--rw-r--r--   0        0        0      834 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/helpers.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_analytics/__init__.py
--rw-r--r--   0        0        0     6243 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_analytics/google-analytics.png
--rw-r--r--   0        0        0     6799 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_analytics/google_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_big_query/__init__.py
--rw-r--r--   0        0        0    17667 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_big_query/google-bigquery.png
--rw-r--r--   0        0        0    12920 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_big_query/google_big_query_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/__init__.py
--rw-r--r--   0        0        0    24008 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
--rw-r--r--   0        0        0     2488 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
--rw-r--r--   0        0        0     2473 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_credentials.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_my_business/__init__.py
--rw-r--r--   0        0        0     4045 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_my_business/google-my-business.png
--rw-r--r--   0        0        0     3024 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_my_business/google_my_business_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets/__init__.py
--rw-r--r--   0        0        0    14238 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets/google-sheets.png
--rw-r--r--   0        0        0     9061 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets/google_sheets_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/__init__.py
--rw-r--r--   0        0        0      361 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/doc.md
--rw-r--r--   0        0        0     9559 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/__init__.py
--rw-r--r--   0        0        0    14238 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png
--rw-r--r--   0        0        0     2986 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/http_api/__init__.py
--rw-r--r--   0        0        0    19694 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/http_api/http-api.png
--rw-r--r--   0        0        0     7584 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/http_api/http_api_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/__init__.py
--rw-r--r--   0        0        0      380 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/doc.md
--rw-r--r--   0        0        0      294 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/enums.py
--rw-r--r--   0        0        0      173 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/helpers.py
--rw-r--r--   0        0        0    33203 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot.png
--rw-r--r--   0        0        0     5738 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot_private_app/__init__.py
--rw-r--r--   0        0        0     5197 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot_private_app/hubspot_connector.py
--rw-r--r--   0        0        0      140 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/__init__.py
--rwxr-xr-x   0        0        0      726 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/databricks.sh
--rwxr-xr-x   0        0        0      509 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/mssql.sh
--rwxr-xr-x   0        0        0      926 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
--rwxr-xr-x   0        0        0      908 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/odbc.sh
--rwxr-xr-x   0        0        0      706 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/oracle.sh
--rw-r--r--   0        0        0     3285 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/json_wrapper.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/__init__.py
--rw-r--r--   0        0        0      365 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/doc.md
--rw-r--r--   0        0        0     9990 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads.png
--rw-r--r--   0        0        0     7544 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/__init__.py
--rw-r--r--   0        0        0     1853 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/client.py
--rw-r--r--   0        0        0     4454 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/data.py
--rw-r--r--   0        0        0     4664 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/micro_strategy_connector.py
--rw-r--r--   0        0        0    13133 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/microstrategy.png
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/__init__.py
--rw-r--r--   0        0        0    26880 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/mongo-db.png
--rw-r--r--   0        0        0    17096 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_connector.py
--rw-r--r--   0        0        0     1822 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_translator.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql/__init__.py
--rw-r--r--   0        0        0    26319 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql/mssql.png
--rw-r--r--   0        0        0     4673 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/__init__.py
--rw-r--r--   0        0        0    26319 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql.png
--rw-r--r--   0        0        0     4893 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mysql/__init__.py
--rw-r--r--   0        0        0     3761 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mysql/mysql.png
--rw-r--r--   0        0        0    14656 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mysql/mysql_connector.py
--rw-r--r--   0        0        0     2401 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer.png
--rwxr-xr-x   0        0        0     3536 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oauth2_connector/__init__.py
--rw-r--r--   0        0        0     6028 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oauth2_connector/oauth2connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odata/__init__.py
--rw-r--r--   0        0        0    31781 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odata/odata.png
--rw-r--r--   0        0        0     2047 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odata/odata_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odbc/__init__.py
--rw-r--r--   0        0        0     3141 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odbc/odbc.png
--rw-r--r--   0        0        0     1298 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odbc/odbc_connector.py
--rw-r--r--   0        0        0    10551 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive.png
--rwxr-xr-x   0        0        0    12312 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oracle_sql/__init__.py
--rw-r--r--   0        0        0    12887 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle-sql.png
--rw-r--r--   0        0        0     3375 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle_sql_connector.py
--rw-r--r--   0        0        0     3948 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/pagination.py
--rw-r--r--   0        0        0     2638 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/pandas_translator.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/peakina/__init__.py
--rw-r--r--   0        0        0     1377 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/peakina/peakina.png
--rw-r--r--   0        0        0      509 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/peakina/peakina_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/__init__.py
--rw-r--r--   0        0        0    28440 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/postgres.png
--rw-r--r--   0        0        0    10400 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/postgresql_connector.py
--rw-r--r--   0        0        0    17824 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/utils.py
--rw-r--r--   0        0        0     1498 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/query_manager.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/__init__.py
--rw-r--r--   0        0        0     8867 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/redshift.png
--rw-r--r--   0        0        0    16551 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/redshift_database_connector.py
--rw-r--r--   0        0        0     1850 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/utils.py
--rw-r--r--   0        0        0      410 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/salesforce/doc.md
--rw-r--r--   0        0        0   165347 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce.jpg
--rw-r--r--   0        0        0     7429 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce_connector.py
--rw-r--r--   0        0        0      410 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/doc.md
--rw-r--r--   0        0        0   165347 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce.jpg
--rw-r--r--   0        0        0       84 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sap_hana/__init__.py
--rw-r--r--   0        0        0    20257 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap-hana.png
--rw-r--r--   0        0        0     1264 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap_hana_connector.py
--rw-r--r--   0        0        0    20013 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/share_point/share_point.png
--rw-r--r--   0        0        0      143 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake/__init__.py
--rw-r--r--   0        0        0    15417 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake.png
--rw-r--r--   0        0        0    18251 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake_connector.py
--rw-r--r--   0        0        0    12795 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_common.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/__init__.py
--rw-r--r--   0        0        0    15417 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake.png
--rw-r--r--   0        0        0    12246 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/__init__.py
--rw-r--r--   0        0        0      609 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/helpers.py
--rw-r--r--   0        0        0    42145 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/soap.png
--rw-r--r--   0        0        0     4325 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/soap_connector.py
--rw-r--r--   0        0        0     3080 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sql_query_helper.py
--rw-r--r--   0        0        0    21205 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_toco/__init__.py
--rwxr-xr-x   0        0        0     4372 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan.png
--rw-r--r--   0        0        0     1289 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan_toco_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/trello/__init__.py
--rw-r--r--   0        0        0     3966 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/trello/trello.png
--rw-r--r--   0        0        0     6603 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/trello/trello_connector.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/utils/__init__.py
--rw-r--r--   0        0        0      492 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/utils/datetime.py
--rw-r--r--   0        0        0      629 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/utils/pem.py
--rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/wootric/__init__.py
--rw-r--r--   0        0        0     8734 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/wootric/wootric.png
--rw-r--r--   0        0        0     5228 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/wootric/wootric_connector.py
--rw-r--r--   0        0        0    14616 1970-01-01 00:00:00.000000 toucan_connectors-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-07-07 14:31:29.960840 toucan_connectors-4.7.0/LICENSE
+-rw-r--r--   0        0        0     9969 2023-07-07 14:31:29.960840 toucan_connectors-4.7.0/README.md
+-rw-r--r--   0        0        0     5586 2023-07-07 14:31:29.964839 toucan_connectors-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10795 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/adobe_analytics/__init__.py
+-rw-r--r--   0        0        0    13648 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/adobe_analytics/adobe-analytics.png
+-rw-r--r--   0        0        0     1740 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/anaplan/__init__.py
+-rw-r--r--   0        0        0     7277 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/anaplan/anaplan.png
+-rw-r--r--   0        0        0     7005 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/anaplan/anaplan_connector.py
+-rw-r--r--   0        0        0     4622 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/auth.py
+-rw-r--r--   0        0        0    61900 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/aws/aws.png
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/awsathena/__init__.py
+-rw-r--r--   0        0        0     2524 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/awsathena/athena.png
+-rw-r--r--   0        0        0     8464 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/awsathena/awsathena_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/azure_mssql/__init__.py
+-rw-r--r--   0        0        0     2404 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/azure_mssql/azure_mssql_connector.py
+-rw-r--r--   0        0        0    24249 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/azure_mssql/sql-azure.png
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1780 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/clickhouse/clickhouse.png
+-rw-r--r--   0        0        0     4541 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/clickhouse/clickhouse_connector.py
+-rw-r--r--   0        0        0    15322 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/common.py
+-rw-r--r--   0        0        0     5549 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/condition_translator.py
+-rw-r--r--   0        0        0     8162 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/connection_manager.py
+-rw-r--r--   0        0        0     3534 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/databricks/databricks.png
+-rw-r--r--   0        0        0     5236 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/databricks/databricks_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/dataiku/__init__.py
+-rw-r--r--   0        0        0    10971 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/dataiku/dataiku.png
+-rw-r--r--   0        0        0     1100 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/dataiku/dataiku_connector.py
+-rwxr-xr-x   0        0        0      235 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/default-logo.png
+-rw-r--r--   0        0        0     3331 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/denodo/denodo.png
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    29549 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/elasticsearch/elasticsearch.png
+-rw-r--r--   0        0        0     5118 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/elasticsearch/elasticsearch_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/facebook_ads/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/facebook_ads/doc.md
+-rw-r--r--   0        0        0      183 2023-07-07 14:31:29.976835 toucan_connectors-4.7.0/toucan_connectors/facebook_ads/enums.py
+-rw-r--r--   0        0        0     5283 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/facebook_ads/facebook_ads_connector.py
+-rw-r--r--   0        0        0    27755 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/facebook_ads/facebook_logo.png
+-rw-r--r--   0        0        0      126 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/facebook_ads/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/facebook_insights/__init__.py
+-rw-r--r--   0        0        0    38402 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/facebook_insights/facebook-insights.png
+-rw-r--r--   0        0        0     3985 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/facebook_insights/facebook_insights_connector.py
+-rw-r--r--   0        0        0    13001 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/github/GitHub_Logo.png
+-rw-r--r--   0        0        0      412 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/github/doc.md
+-rw-r--r--   0        0        0    17081 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/github/github_connector.py
+-rw-r--r--   0        0        0    15902 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/github/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_adwords/__init__.py
+-rw-r--r--   0        0        0      469 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_adwords/doc.md
+-rw-r--r--   0        0        0    68711 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_adwords/google_adwords.jpg
+-rw-r--r--   0        0        0     9049 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_adwords/google_adwords_connector.py
+-rw-r--r--   0        0        0      834 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_adwords/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_analytics/__init__.py
+-rw-r--r--   0        0        0     6243 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_analytics/google-analytics.png
+-rw-r--r--   0        0        0     6799 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_analytics/google_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_big_query/__init__.py
+-rw-r--r--   0        0        0    17667 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_big_query/google-bigquery.png
+-rw-r--r--   0        0        0    14501 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_big_query/google_big_query_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_cloud_mysql/__init__.py
+-rw-r--r--   0        0        0    24008 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
+-rw-r--r--   0        0        0     2488 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
+-rw-r--r--   0        0        0     2473 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_credentials.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_my_business/__init__.py
+-rw-r--r--   0        0        0     4045 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_my_business/google-my-business.png
+-rw-r--r--   0        0        0     3024 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_my_business/google_my_business_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_sheets/__init__.py
+-rw-r--r--   0        0        0    14238 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_sheets/google-sheets.png
+-rw-r--r--   0        0        0     9061 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_sheets/google_sheets_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_sheets_2/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_sheets_2/doc.md
+-rw-r--r--   0        0        0     9559 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_spreadsheet/__init__.py
+-rw-r--r--   0        0        0    14238 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png
+-rw-r--r--   0        0        0     2986 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/http_api/__init__.py
+-rw-r--r--   0        0        0    19694 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/http_api/http-api.png
+-rw-r--r--   0        0        0     8020 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/http_api/http_api_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot/doc.md
+-rw-r--r--   0        0        0      294 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot/enums.py
+-rw-r--r--   0        0        0      173 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot/helpers.py
+-rw-r--r--   0        0        0    33203 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot/hubspot.png
+-rw-r--r--   0        0        0     5738 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot/hubspot_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot_private_app/__init__.py
+-rw-r--r--   0        0        0     5197 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/hubspot_private_app/hubspot_connector.py
+-rw-r--r--   0        0        0      140 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/install_scripts/__init__.py
+-rwxr-xr-x   0        0        0      726 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/install_scripts/databricks.sh
+-rwxr-xr-x   0        0        0      509 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/install_scripts/mssql.sh
+-rwxr-xr-x   0        0        0      926 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
+-rwxr-xr-x   0        0        0      908 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/install_scripts/odbc.sh
+-rwxr-xr-x   0        0        0      706 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/install_scripts/oracle.sh
+-rw-r--r--   0        0        0     3285 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/json_wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/linkedinads/__init__.py
+-rw-r--r--   0        0        0      365 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/linkedinads/doc.md
+-rw-r--r--   0        0        0     9990 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/linkedinads/linkedinads.png
+-rw-r--r--   0        0        0     7544 2023-07-07 14:31:29.980834 toucan_connectors-4.7.0/toucan_connectors/linkedinads/linkedinads_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/micro_strategy/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/micro_strategy/client.py
+-rw-r--r--   0        0        0     4454 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/micro_strategy/data.py
+-rw-r--r--   0        0        0     4664 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/micro_strategy/micro_strategy_connector.py
+-rw-r--r--   0        0        0    13133 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/micro_strategy/microstrategy.png
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mongo/__init__.py
+-rw-r--r--   0        0        0    26880 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mongo/mongo-db.png
+-rw-r--r--   0        0        0    17096 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mongo/mongo_connector.py
+-rw-r--r--   0        0        0     1822 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mongo/mongo_translator.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mssql/__init__.py
+-rw-r--r--   0        0        0    26319 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mssql/mssql.png
+-rw-r--r--   0        0        0     4673 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mssql/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mssql_TLSv1_0/__init__.py
+-rw-r--r--   0        0        0    26319 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mssql_TLSv1_0/mssql.png
+-rw-r--r--   0        0        0     4893 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mysql/__init__.py
+-rw-r--r--   0        0        0     3761 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mysql/mysql.png
+-rw-r--r--   0        0        0    14692 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/mysql/mysql_connector.py
+-rw-r--r--   0        0        0     2401 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/net_explorer/net_explorer.png
+-rwxr-xr-x   0        0        0     3536 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/net_explorer/net_explorer_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/oauth2_connector/__init__.py
+-rw-r--r--   0        0        0     6028 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/oauth2_connector/oauth2connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/odata/__init__.py
+-rw-r--r--   0        0        0    31781 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/odata/odata.png
+-rw-r--r--   0        0        0     2047 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/odata/odata_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/odbc/__init__.py
+-rw-r--r--   0        0        0     3141 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/odbc/odbc.png
+-rw-r--r--   0        0        0     1298 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/odbc/odbc_connector.py
+-rw-r--r--   0        0        0    10551 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/one_drive/one_drive.png
+-rwxr-xr-x   0        0        0    12312 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/one_drive/one_drive_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/oracle_sql/__init__.py
+-rw-r--r--   0        0        0    12887 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/oracle_sql/oracle-sql.png
+-rw-r--r--   0        0        0     3375 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/oracle_sql/oracle_sql_connector.py
+-rw-r--r--   0        0        0     3948 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/pagination.py
+-rw-r--r--   0        0        0     2638 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/pandas_translator.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/peakina/__init__.py
+-rw-r--r--   0        0        0     1377 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/peakina/peakina.png
+-rw-r--r--   0        0        0      509 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/peakina/peakina_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/postgres/__init__.py
+-rw-r--r--   0        0        0    28440 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/postgres/postgres.png
+-rw-r--r--   0        0        0    10400 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/postgres/postgresql_connector.py
+-rw-r--r--   0        0        0    17824 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/postgres/utils.py
+-rw-r--r--   0        0        0     1498 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/query_manager.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/redshift/__init__.py
+-rw-r--r--   0        0        0     8867 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/redshift/redshift.png
+-rw-r--r--   0        0        0    16551 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/redshift/redshift_database_connector.py
+-rw-r--r--   0        0        0     1850 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/redshift/utils.py
+-rw-r--r--   0        0        0      410 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/salesforce/doc.md
+-rw-r--r--   0        0        0   165347 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/salesforce/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/salesforce/salesforce.jpg
+-rw-r--r--   0        0        0     7429 2023-07-07 14:31:29.984833 toucan_connectors-4.7.0/toucan_connectors/salesforce/salesforce_connector.py
+-rw-r--r--   0        0        0      410 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/salesforce_sandbox/doc.md
+-rw-r--r--   0        0        0   165347 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/salesforce_sandbox/salesforce.jpg
+-rw-r--r--   0        0        0       84 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/sap_hana/__init__.py
+-rw-r--r--   0        0        0    20257 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/sap_hana/sap-hana.png
+-rw-r--r--   0        0        0     1264 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/sap_hana/sap_hana_connector.py
+-rw-r--r--   0        0        0    20013 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/share_point/share_point.png
+-rw-r--r--   0        0        0      143 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    15417 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake/snowflake.png
+-rw-r--r--   0        0        0    18251 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake/snowflake_connector.py
+-rw-r--r--   0        0        0    12795 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake_common.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake_oauth2/__init__.py
+-rw-r--r--   0        0        0    15417 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake_oauth2/snowflake.png
+-rw-r--r--   0        0        0    12246 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/soap/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/soap/helpers.py
+-rw-r--r--   0        0        0    42145 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/soap/soap.png
+-rw-r--r--   0        0        0     4325 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/soap/soap_connector.py
+-rw-r--r--   0        0        0     3080 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/sql_query_helper.py
+-rw-r--r--   0        0        0    21205 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/toucan_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/toucan_toco/__init__.py
+-rwxr-xr-x   0        0        0     4372 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/toucan_toco/toucan.png
+-rw-r--r--   0        0        0     1289 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/toucan_toco/toucan_toco_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/trello/__init__.py
+-rw-r--r--   0        0        0     3966 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/trello/trello.png
+-rw-r--r--   0        0        0     6603 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/trello/trello_connector.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/utils/__init__.py
+-rw-r--r--   0        0        0      492 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/utils/datetime.py
+-rw-r--r--   0        0        0      629 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/utils/pem.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/wootric/__init__.py
+-rw-r--r--   0        0        0     8734 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/wootric/wootric.png
+-rw-r--r--   0        0        0     5228 2023-07-07 14:31:29.988832 toucan_connectors-4.7.0/toucan_connectors/wootric/wootric_connector.py
+-rw-r--r--   0        0        0    14612 1970-01-01 00:00:00.000000 toucan_connectors-4.7.0/PKG-INFO
```

### Comparing `toucan_connectors-4.6.0/LICENSE` & `toucan_connectors-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/README.md` & `toucan_connectors-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/pyproject.toml` & `toucan_connectors-4.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 profile = "black"
 include_trailing_comma = true
 line_length = 100
 multi_line_output = 3
 
 [tool.poetry]
 name = "toucan-connectors"
-version = "4.6.0"
+version = "4.7.0"
 description = "Toucan Toco Connectors"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 license = "BSD"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -32,15 +32,15 @@
 adobe-analytics = {version = "^1.2.3", optional = true}
 bearer = {version = "3.1.0", optional = true}
 oauthlib = {version = "3.2.2", optional = true}
 requests-oauthlib = {version = "1.3.1", optional = true}
 awswrangler = {version = "^3.0.0", optional = true}
 pyodbc = {version = "^4", optional = true}
 clickhouse-driver = {version = ">=0.2.3,<1.0", optional = true}
-dataiku-api-client = {version = "^9.0.1", optional = true}
+dataiku-api-client = {version = ">=9.0.1,<13.0.0", optional = true}
 elasticsearch = {version = ">=7.11.0,<8", optional = true}
 facebook-sdk = {version = "^3.1.0", optional = true}
 python-graphql-client = {version = ">=0.4.3,<1.0", optional = true}
 google-api-python-client = {version = "^2", optional = true}
 oauth2client = {version = "^4.1.3", optional = true}
 googleads = {version = ">=32,<34", optional = true}
 google-cloud-bigquery = {version = ">=3,<4", extras = ["bqstorage", "pandas"], optional = true}
@@ -58,49 +58,49 @@
 simplejson = {version = "^3.17.6", optional = true}
 pyhdb = {version = ">=0.3.4,<1.0", optional = true}
 zeep = {version = "^4.1.0", optional = true}
 snowflake-connector-python = {version = ">=2.7.12,<4.0.0", optional = true}
 pyarrow = {version = "<12", optional = true}
 toucan-client = {version = "^1.0.1", optional = true}
 peakina = {version = "^0.11.0", optional = true}
-hubspot-api-client = {version = "^7.4.0", optional = true}
+hubspot-api-client = {version = ">=7.4,<9.0", optional = true}
 aiohttp = "^3.8.4"
 
 [tool.poetry.dev-dependencies]
 Authlib = "^1.0.1"
 aioresponses = ">=0.7.3,<1.0"
 black = "^23.3.0"
-click = "^8.1.3"
+click = "^8.1.4"
 cryptography = ">=40.0.2"
 docker = "^6.1.3"
 flake8 = "^6.0.0"
 flake8-quotes = "^3.3.2"
 isort = "^5.12.0"
 mock = "^5.0.2"
 pytest-aiohttp = "^1.0.4"
 pytest-asyncio = ">=0.19.0,<1"
 pytest-cov = "^4.1.0"
-pytest = "^7.3.1"
-pytest-mock = "^3.10.0"
-pytest-rerunfailures = "^11.1"
+pytest = "^7.4.0"
+pytest-mock = "^3.11.1"
+pytest-rerunfailures = "^12.0"
 python-slugify = "<7"
 PyYAML = "<6"
 responses = ">=0.21.0,<1"
 psycopg2 = "^2.9.3"
 xmltodict = ">=0.13.0,<1"
 python-graphql-client = ">=0.4.3,<1"
 clickhouse-driver = ">=0.2.3,<1"
 lxml = "4.9.1"
 zeep = "^4.1.0"
-mypy = "^1.3"
-pandas-stubs = "^2.0.1.230501"
+mypy = "^1.4"
+pandas-stubs = "^2.0.2.230605"
 types-requests = "^2.31.0.1"
 types-simplejson = "^3.19.0.1"
 types-python-slugify = "^8.0.0.2"
-types-pyopenssl = "^23.2.0.0"
+types-pyopenssl = "^23.2.0.1"
 
 [tool.poetry.extras]
 adobe = ["adobe-analytics"]
 awsathena = ["awswrangler"]
 azure_mssql = ["pyodbc"]
 clickhouse = ["clickhouse-driver"]
 dataiku = ["dataiku-api-client"]
```

### Comparing `toucan_connectors-4.6.0/toucan_connectors/__init__.py` & `toucan_connectors-4.7.0/toucan_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe-analytics.png` & `toucan_connectors-4.7.0/toucan_connectors/adobe_analytics/adobe-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan.png` & `toucan_connectors-4.7.0/toucan_connectors/anaplan/anaplan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/anaplan/anaplan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/auth.py` & `toucan_connectors-4.7.0/toucan_connectors/auth.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/aws/aws.png` & `toucan_connectors-4.7.0/toucan_connectors/aws/aws.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/awsathena/athena.png` & `toucan_connectors-4.7.0/toucan_connectors/awsathena/athena.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/awsathena/awsathena_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/awsathena/awsathena_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/azure_mssql/azure_mssql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/azure_mssql/azure_mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/azure_mssql/sql-azure.png` & `toucan_connectors-4.7.0/toucan_connectors/azure_mssql/sql-azure.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse.png` & `toucan_connectors-4.7.0/toucan_connectors/clickhouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/common.py` & `toucan_connectors-4.7.0/toucan_connectors/common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/condition_translator.py` & `toucan_connectors-4.7.0/toucan_connectors/condition_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/connection_manager.py` & `toucan_connectors-4.7.0/toucan_connectors/connection_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/databricks/databricks.png` & `toucan_connectors-4.7.0/toucan_connectors/databricks/databricks.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/databricks/databricks_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/databricks/databricks_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku.png` & `toucan_connectors-4.7.0/toucan_connectors/dataiku/dataiku.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/dataiku/dataiku_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/denodo/denodo.png` & `toucan_connectors-4.7.0/toucan_connectors/denodo/denodo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch.png` & `toucan_connectors-4.7.0/toucan_connectors/elasticsearch/elasticsearch.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/elasticsearch/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_ads_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/facebook_ads/facebook_ads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_logo.png` & `toucan_connectors-4.7.0/toucan_connectors/facebook_ads/facebook_logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook-insights.png` & `toucan_connectors-4.7.0/toucan_connectors/facebook_insights/facebook-insights.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook_insights_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/facebook_insights/facebook_insights_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/github/GitHub_Logo.png` & `toucan_connectors-4.7.0/toucan_connectors/github/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/github/github_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/github/github_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/github/helpers.py` & `toucan_connectors-4.7.0/toucan_connectors/github/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords.jpg` & `toucan_connectors-4.7.0/toucan_connectors/google_adwords/google_adwords.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_adwords/google_adwords_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_adwords/helpers.py` & `toucan_connectors-4.7.0/toucan_connectors/google_adwords/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_analytics/google-analytics.png` & `toucan_connectors-4.7.0/toucan_connectors/google_analytics/google-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_analytics/google_analytics_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_analytics/google_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_big_query/google-bigquery.png` & `toucan_connectors-4.7.0/toucan_connectors/google_big_query/google-bigquery.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_big_query/google_big_query_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_big_query/google_big_query_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import logging
 from enum import Enum
 from functools import cached_property
 from itertools import groupby
 from timeit import default_timer as timer
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Generator, Iterable, List, Union
 
-import pandas
 import pandas as pd
 from google.api_core.exceptions import GoogleAPIError
 from google.cloud import bigquery
 from google.cloud.bigquery.dbapi import _helpers as bigquery_helpers
+from google.cloud.bigquery.job import QueryJob
 from google.oauth2.service_account import Credentials
 from pydantic import Field, create_model
 
 from toucan_connectors.common import sanitize_query
 from toucan_connectors.google_credentials import GoogleCredentials, get_google_oauth2_credentials
 from toucan_connectors.toucan_connector import (
     DiscoverableConnector,
     TableInfo,
     ToucanConnector,
     ToucanDataSource,
+    strlist_to_enum,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
+_PAGE_SIZE = 50
+_MAXIMUM_RESULTS_FETCHED = 2000
+
 
 class Dialect(str, Enum):
     legacy = 'legacy'
     standard = 'standard'
 
 
 class GoogleBigQueryDataSource(ToucanDataSource):
@@ -39,23 +43,26 @@
     )
     query_object: Dict = Field(
         None,
         description='An object describing a simple select query This field is used internally',
         **{'ui.hidden': True},
     )
     language: str = Field('sql', **{'ui.hidden': True})
-    database: str = Field(None)  # Needed for graphical selection in frontend but not used
-
-    class Config:
-        extra = 'ignore'
+    database: str = Field(None, **{'ui.hidden': True})
+    db_schema: str = Field(None, description='The name of the db_schema you want to query.')
 
     @classmethod
     def get_form(cls, connector: 'GoogleBigQueryConnector', current_config: dict[str, Any]):
-        schema = create_model('FormSchema', __base__=cls).schema()
+        schema = create_model(
+            'FormSchema',
+            db_schema=strlist_to_enum('db_schema', connector._available_schs),
+            __base__=cls,
+        ).schema()
         schema['properties']['database']['default'] = connector.credentials.project_id
+
         return schema
 
 
 BigQueryParam = Union[bigquery.ScalarQueryParameter, bigquery.ArrayQueryParameter]
 
 
 def _define_query_param(name: str, value: Any) -> BigQueryParam:
@@ -119,19 +126,16 @@
                     'execution_time': end - start,
                     'connector': 'google_big_query',
                 }
             },
         )
         return client
 
-    def project_tree(self) -> list[TableInfo]:
-        return self._get_project_structure()
-
     @staticmethod
-    def _execute_query(client: bigquery.Client, query: str, parameters: list) -> pandas.DataFrame:
+    def _execute_query(client: bigquery.Client, query: str, parameters: list) -> pd.DataFrame:
         try:
             start = timer()
 
             # Ugly but the select query generated by frontend adds '"'
             query = query.replace('"', '`')
 
             # Since the interpolated variable is given the exact value and we
@@ -222,38 +226,67 @@
             .apply(list)
             .reset_index()
             .to_dict(orient='records')
         )
 
     @staticmethod
     def _build_dataset_info_query_for_ds(dataset_id: str, db_name: str | None) -> str:
-        output = f"""
-SELECT C.table_name AS name, C.table_schema AS schema, T.table_catalog AS database,
-T.table_type AS type, C.column_name, C.data_type FROM {dataset_id}.INFORMATION_SCHEMA.COLUMNS C
-JOIN {dataset_id}.INFORMATION_SCHEMA.TABLES T ON C.table_name = T.table_name
-WHERE IS_SYSTEM_DEFINED='NO' AND IS_PARTITIONING_COLUMN='NO' AND IS_HIDDEN='NO'
+        query = f"""
+SELECT
+    C.table_name AS name,
+    C.table_schema AS schema,
+    T.table_catalog AS database,
+    T.table_type AS type,
+    C.column_name,
+    C.data_type
+FROM
+    {dataset_id}.INFORMATION_SCHEMA.COLUMNS C
+    JOIN {dataset_id}.INFORMATION_SCHEMA.TABLES T
+        ON C.table_name = T.table_name
+WHERE
+    IS_SYSTEM_DEFINED = 'NO'
+    AND IS_PARTITIONING_COLUMN = 'NO'
+    AND IS_HIDDEN = 'NO'
 """
+
         if db_name is not None:
-            output += f"AND T.table_catalog = '{db_name}'\n"
-        return output
+            query += f"AND T.table_catalog = '{db_name}'\n"
+
+        return query
 
     def _build_dataset_info_query(self, dataset_ids: Iterable[str], db_name: str | None) -> str:
         return '\nUNION ALL\n'.join(
             self._build_dataset_info_query_for_ds(dataset_id, db_name) for dataset_id in dataset_ids
         )
 
+    def _fetch_query_results(
+        self, query_job: QueryJob
+    ) -> Generator[Any, Any, Any]:  # pragma: no cover
+        """Fetches query results in a paginated manner using a generator."""
+        row_iterator = query_job.result(page_size=_PAGE_SIZE, max_results=_MAXIMUM_RESULTS_FETCHED)
+
+        while rows := next(row_iterator.pages, None):
+            yield rows.to_dataframe()
+
     def _get_project_structure_fast(
         self, client: bigquery.Client, db_name: str | None, dataset_ids: Iterable[str]
     ) -> pd.DataFrame:
         """Retrieves the project structure in a single query.
 
         Only works if all datasets are in the same location.
         """
         query = self._build_dataset_info_query(dataset_ids, db_name)
-        return client.query(query).to_dataframe()
+
+        try:
+            query_job = client.query(query)
+            # Fetch pages of results using the generator
+            # and Concatenate all dataframes into a single one
+            return pd.concat((df for df in self._fetch_query_results(query_job)), ignore_index=True)
+        except Exception as exc:
+            raise GoogleAPIError(f'An error occurred while executing the query: {exc}') from exc
 
     def _get_project_structure_slow(
         self, client: bigquery.Client, db_name: str | None, dataset_ids: Iterable[str]
     ) -> pd.DataFrame:
         """Retrieves the project structure in multiple queries.
 
         Works even if the project's datasets are in different locations.
@@ -272,32 +305,47 @@
                 (ds.dataset_id for ds in datasets_for_region), db_name
             )
             dfs.append(client.query(query, location=location).to_dataframe())
 
         # Then, we returning a single dataframe containing all results
         return pd.concat(dfs)
 
-    def _get_project_structure(self, db_name: str | None = None) -> List[TableInfo]:
+    @cached_property
+    def _available_schs(self) -> list[str]:  # pragma: no cover
+        credentials = self._get_google_credentials(self.credentials, self.scopes)
+        client = bigquery.Client(location=None, credentials=credentials)
+
+        return pd.Series((ds.dataset_id for ds in client.list_datasets())).values
+
+    def _get_project_structure(
+        self, db_name: str | None = None, schema_name: str | None = None
+    ) -> List[TableInfo]:
         creds = self._get_google_credentials(self.credentials, self.scopes)
         client = self._connect(creds)
-        datasets = list(client.list_datasets())
-        # Here, we're trying to retrieve table info for all datasets at once. However, this will
-        # only work if all datasets are in same location. Unfortunately, there is no way to
-        # retrieve the location along with the dataset list, so we're optimistic here.
+
+        # Either the schema_name is not specified
+        if schema_name is None:
+            dataset_ids = [ds.dataset_id for ds in list(client.list_datasets())]
+        else:
+            # if we already now the dataset/schema, we should be able to just
+            # fetch it instead of all of them
+            dataset_ids = [schema_name]
+
         try:
-            df = self._get_project_structure_fast(
-                client, db_name, (ds.dataset_id for ds in datasets)
-            )
+            # Here, we're trying to retrieve table info for all datasets at once. However, this will
+            # only work if all datasets are in same location. Unfortunately, there is no way to
+            # retrieve the location along with the dataset list, so we're optimistic here.
+            df = self._get_project_structure_fast(client, db_name, dataset_ids)
         except GoogleAPIError as exc:
             _LOGGER.info(
                 f'Got an exception when trying to retrieve domains for project: {exc}. '
                 'Falling back on listing by location...'
             )
-            df = self._get_project_structure_slow(
-                client, db_name, (ds.dataset_id for ds in datasets)
-            )
+            df = self._get_project_structure_slow(client, db_name, dataset_ids)
 
         return self._format_db_model(df)
 
-    def get_model(self, db_name: str | None = None) -> list[TableInfo]:
+    def get_model(
+        self, db_name: str | None = None, schema_name: str | None = None
+    ) -> list[TableInfo]:
         """Retrieves the database tree structure using current connection"""
-        return self._get_project_structure(db_name)
+        return self._get_project_structure(db_name, schema_name)
```

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png` & `toucan_connectors-4.7.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_credentials.py` & `toucan_connectors-4.7.0/toucan_connectors/google_credentials.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_my_business/google-my-business.png` & `toucan_connectors-4.7.0/toucan_connectors/google_my_business/google-my-business.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_my_business/google_my_business_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_my_business/google_my_business_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_sheets/google-sheets.png` & `toucan_connectors-4.7.0/toucan_connectors/google_sheets/google-sheets.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_sheets/google_sheets_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_sheets/google_sheets_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png` & `toucan_connectors-4.7.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/http_api/http-api.png` & `toucan_connectors-4.7.0/toucan_connectors/http_api/http-api.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/http_api/http_api_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/http_api/http_api_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,15 +139,21 @@
         query = {k: v for k, v in query.items() if k in available_params}
         query['url'] = '/'.join([self.baseroute.rstrip('/'), query['url'].lstrip('/')])
 
         if self.cert:
             # `cert` is a list of PosixPath. `request` needs a list of strings for certificates
             query['cert'] = [str(c) for c in self.cert]
 
+        HttpAPIConnector.logger.debug(
+            f'>> Request:  method={query.get("method")} url={query.get("url")}'
+        )
         res = session.request(**query)
+        HttpAPIConnector.logger.debug(
+            f'<< Response: status_code={res.status_code} reason={res.reason}'
+        )
 
         if self.responsetype == 'xml':
             try:
                 data = fromstring(res.content)
                 data = parse(tostring(data.find(xpath), method='xml'), attr_prefix='')
             except ParseError:
                 HttpAPIConnector.logger.error(f'Could not decode {res.content!r}')
@@ -158,15 +164,17 @@
                 data = res.json()
             except ValueError:
                 HttpAPIConnector.logger.error('Could not decode content using response.json()')
                 try:
                     # sometimes when the content is too big res.json() fails but json.loads works
                     data = json.loads(res.content)
                 except ValueError:
-                    HttpAPIConnector.logger.error('Cannot decode response content')
+                    HttpAPIConnector.logger.error(
+                        f'Cannot decode response content from query: method={query.get("method")} url={query.get("url")} response_status_code={res.status_code} response_reason=${res.reason}'
+                    )
                     raise
         try:
             return transform_with_jq(data, jq_filter)
         except ValueError:
             HttpAPIConnector.logger.error(f'Could not transform {data} using {jq_filter}')
             raise
```

### Comparing `toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot.png` & `toucan_connectors-4.7.0/toucan_connectors/hubspot/hubspot.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/hubspot/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/hubspot_private_app/hubspot_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/hubspot_private_app/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/install_scripts/databricks.sh` & `toucan_connectors-4.7.0/toucan_connectors/install_scripts/databricks.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh` & `toucan_connectors-4.7.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/install_scripts/odbc.sh` & `toucan_connectors-4.7.0/toucan_connectors/install_scripts/odbc.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/install_scripts/oracle.sh` & `toucan_connectors-4.7.0/toucan_connectors/install_scripts/oracle.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/json_wrapper.py` & `toucan_connectors-4.7.0/toucan_connectors/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads.png` & `toucan_connectors-4.7.0/toucan_connectors/linkedinads/linkedinads.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/linkedinads/linkedinads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/client.py` & `toucan_connectors-4.7.0/toucan_connectors/micro_strategy/client.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/data.py` & `toucan_connectors-4.7.0/toucan_connectors/micro_strategy/data.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/micro_strategy_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/micro_strategy/micro_strategy_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/microstrategy.png` & `toucan_connectors-4.7.0/toucan_connectors/micro_strategy/microstrategy.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mongo/mongo-db.png` & `toucan_connectors-4.7.0/toucan_connectors/mongo/mongo-db.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/mongo/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_translator.py` & `toucan_connectors-4.7.0/toucan_connectors/mongo/mongo_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mssql/mssql.png` & `toucan_connectors-4.7.0/toucan_connectors/mssql/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mssql/mssql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql.png` & `toucan_connectors-4.7.0/toucan_connectors/mssql_TLSv1_0/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mysql/mysql.png` & `toucan_connectors-4.7.0/toucan_connectors/mysql/mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/mysql/mysql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/mysql/mysql_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     # https://dba.stackexchange.com/questions/3774/what-is-the-point-of-the-table-catalog-column-in-information-schema-tables
     "SELECT t.table_schema AS 'database', t.table_schema AS 'schema', "
     # Table type and name
     "CASE WHEN t.table_type = 'BASE TABLE' THEN 'table' ELSE LOWER(t.table_type) END AS table_type, t.table_name, "
     # Columns from the columns table
     'c.column_name, c.data_type FROM information_schema.tables t INNER JOIN information_schema.columns c '
     # Inner join on table name
-    'ON t.table_name = c.table_name '
+    'ON t.table_name = c.table_name AND t.table_schema = c.table_schema '
     # Filtering on concrete tables/views
     "WHERE t.table_type in ('BASE TABLE', 'VIEW') AND t.table_schema NOT IN ('mysql', 'information_schema', 'performance_schema', 'sys') "
 )
 
 
 class SSLMode(str, Enum):
     VERIFY_IDENTITY = 'VERIFY_IDENTITY'
```

### Comparing `toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer.png` & `toucan_connectors-4.7.0/toucan_connectors/net_explorer/net_explorer.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/net_explorer/net_explorer_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/oauth2_connector/oauth2connector.py` & `toucan_connectors-4.7.0/toucan_connectors/oauth2_connector/oauth2connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/odata/odata.png` & `toucan_connectors-4.7.0/toucan_connectors/odata/odata.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/odata/odata_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/odata/odata_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/odbc/odbc.png` & `toucan_connectors-4.7.0/toucan_connectors/odbc/odbc.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/odbc/odbc_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/odbc/odbc_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive.png` & `toucan_connectors-4.7.0/toucan_connectors/one_drive/one_drive.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/one_drive/one_drive_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle-sql.png` & `toucan_connectors-4.7.0/toucan_connectors/oracle_sql/oracle-sql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle_sql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/oracle_sql/oracle_sql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/pagination.py` & `toucan_connectors-4.7.0/toucan_connectors/pagination.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/pandas_translator.py` & `toucan_connectors-4.7.0/toucan_connectors/pandas_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/peakina/peakina.png` & `toucan_connectors-4.7.0/toucan_connectors/peakina/peakina.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/postgres/postgres.png` & `toucan_connectors-4.7.0/toucan_connectors/postgres/postgres.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/postgres/postgresql_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/postgres/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/postgres/utils.py` & `toucan_connectors-4.7.0/toucan_connectors/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/query_manager.py` & `toucan_connectors-4.7.0/toucan_connectors/query_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/redshift/redshift.png` & `toucan_connectors-4.7.0/toucan_connectors/redshift/redshift.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/redshift/redshift_database_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/redshift/redshift_database_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/redshift/utils.py` & `toucan_connectors-4.7.0/toucan_connectors/redshift/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce-service-cloud.png` & `toucan_connectors-4.7.0/toucan_connectors/salesforce/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce.jpg` & `toucan_connectors-4.7.0/toucan_connectors/salesforce/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/salesforce/salesforce_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png` & `toucan_connectors-4.7.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce.jpg` & `toucan_connectors-4.7.0/toucan_connectors/salesforce_sandbox/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap-hana.png` & `toucan_connectors-4.7.0/toucan_connectors/sap_hana/sap-hana.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap_hana_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/sap_hana/sap_hana_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/share_point/share_point.png` & `toucan_connectors-4.7.0/toucan_connectors/share_point/share_point.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake.png` & `toucan_connectors-4.7.0/toucan_connectors/snowflake/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/snowflake/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/snowflake_common.py` & `toucan_connectors-4.7.0/toucan_connectors/snowflake_common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake.png` & `toucan_connectors-4.7.0/toucan_connectors/snowflake_oauth2/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/soap/helpers.py` & `toucan_connectors-4.7.0/toucan_connectors/soap/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/soap/soap.png` & `toucan_connectors-4.7.0/toucan_connectors/soap/soap.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/soap/soap_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/sql_query_helper.py` & `toucan_connectors-4.7.0/toucan_connectors/sql_query_helper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/toucan_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/toucan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan.png` & `toucan_connectors-4.7.0/toucan_connectors/toucan_toco/toucan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan_toco_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/toucan_toco/toucan_toco_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/trello/trello.png` & `toucan_connectors-4.7.0/toucan_connectors/trello/trello.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/trello/trello_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/trello/trello_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/utils/pem.py` & `toucan_connectors-4.7.0/toucan_connectors/utils/pem.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/wootric/wootric.png` & `toucan_connectors-4.7.0/toucan_connectors/wootric/wootric.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/toucan_connectors/wootric/wootric_connector.py` & `toucan_connectors-4.7.0/toucan_connectors/wootric/wootric_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.6.0/PKG-INFO` & `toucan_connectors-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toucan-connectors
-Version: 4.6.0
+Version: 4.7.0
 Summary: Toucan Toco Connectors
 License: BSD
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -49,22 +49,22 @@
 Requires-Dist: adobe-analytics (>=1.2.3,<2.0.0) ; extra == "adobe" or extra == "all"
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: awswrangler (>=3.0.0,<4.0.0) ; extra == "awsathena" or extra == "all"
 Requires-Dist: bearer (==3.1.0) ; extra == "all"
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: clickhouse-driver (>=0.2.3,<1.0) ; extra == "clickhouse" or extra == "all"
 Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0) ; extra == "oracle-sql" or extra == "all"
-Requires-Dist: dataiku-api-client (>=9.0.1,<10.0.0) ; extra == "dataiku" or extra == "all"
+Requires-Dist: dataiku-api-client (>=9.0.1,<13.0.0) ; extra == "dataiku" or extra == "all"
 Requires-Dist: elasticsearch (>=7.11.0,<8) ; extra == "elasticsearch" or extra == "all"
 Requires-Dist: facebook-sdk (>=3.1.0,<4.0.0) ; extra == "facebook" or extra == "all"
 Requires-Dist: google-api-python-client (>=2,<3) ; extra == "google-analytics" or extra == "google-my-business" or extra == "google-sheets" or extra == "all"
 Requires-Dist: google-cloud-bigquery[bqstorage,pandas] (>=3,<4) ; extra == "google-big-query" or extra == "all"
 Requires-Dist: googleads (>=32,<34) ; extra == "all"
 Requires-Dist: gspread (>=5.4.0,<6.0.0) ; extra == "google-spreadsheet" or extra == "all"
-Requires-Dist: hubspot-api-client (>=7.4.0,<8.0.0) ; extra == "hubspot" or extra == "all"
+Requires-Dist: hubspot-api-client (>=7.4,<9.0) ; extra == "hubspot" or extra == "all"
 Requires-Dist: jq (>=1.2.2,<2.0.0)
 Requires-Dist: lxml (>=4.6.5,<5.0.0) ; extra == "redshift" or extra == "soap" or extra == "all"
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0) ; extra == "google-analytics" or extra == "google-spreadsheet" or extra == "all"
 Requires-Dist: oauthlib (==3.2.2) ; extra == "http-api" or extra == "odata" or extra == "all"
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0) ; extra == "net-explorer" or extra == "all"
 Requires-Dist: peakina (>=0.11.0,<0.12.0) ; extra == "all"
 Requires-Dist: psycopg2 (>=2.7.4,<3.0.0) ; extra == "postgres" or extra == "all"
```

