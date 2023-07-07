# Comparing `tmp/finops-0.2.2.tar.gz` & `tmp/finops-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.2.2.tar", last modified: Thu Jul  6 21:44:01 2023, max compression
+gzip compressed data, was "finops-0.2.3.tar", last modified: Fri Jul  7 20:19:42 2023, max compression
```

## Comparing `finops-0.2.2.tar` & `finops-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-06 21:43:50.000000 finops-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 21:44:01.854472 finops-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-06 21:43:50.000000 finops-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.850472 finops-0.2.2/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 21:43:50.000000 finops-0.2.2/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-06 21:43:50.000000 finops-0.2.2/finops/codal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-06 21:43:50.000000 finops-0.2.2/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-06 21:43:50.000000 finops-0.2.2/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-06 21:43:50.000000 finops-0.2.2/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-06 21:43:50.000000 finops-0.2.2/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:44:01.854472 finops-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 21:43:50.000000 finops-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:43:50.000000 finops-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_utils/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:42.673632 finops-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-07 20:19:34.000000 finops-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:19:42.673632 finops-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 20:19:34.000000 finops-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:42.673632 finops-0.2.3/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 20:19:34.000000 finops-0.2.3/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-07 20:19:34.000000 finops-0.2.3/finops/codal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-07 20:19:34.000000 finops-0.2.3/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-07 20:19:34.000000 finops-0.2.3/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-07 20:19:34.000000 finops-0.2.3/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-07 20:19:34.000000 finops-0.2.3/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:42.673632 finops-0.2.3/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:34.000000 finops-0.2.3/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 20:19:34.000000 finops-0.2.3/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-07 20:19:34.000000 finops-0.2.3/finops/utils/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-07 20:19:34.000000 finops-0.2.3/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 20:19:34.000000 finops-0.2.3/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:42.673632 finops-0.2.3/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:19:42.000000 finops-0.2.3/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-07 20:19:42.000000 finops-0.2.3/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:19:42.000000 finops-0.2.3/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 20:19:42.000000 finops-0.2.3/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 20:19:42.000000 finops-0.2.3/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:19:42.673632 finops-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-07 20:19:34.000000 finops-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:42.673632 finops-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:34.000000 finops-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-07 20:19:34.000000 finops-0.2.3/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-07 20:19:34.000000 finops-0.2.3/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:42.673632 finops-0.2.3/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:19:34.000000 finops-0.2.3/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-07 20:19:34.000000 finops-0.2.3/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-07 20:19:34.000000 finops-0.2.3/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.2.2/LICENSE` & `finops-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/PKG-INFO` & `finops-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.2.2/README.md` & `finops-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/finops/codal.py` & `finops-0.2.3/finops/codal.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     CODAL_SEARCH_BASE_URL,
     CODAL_LETTERS_LIST_COLUMNS,
     BALANCE_SHEET_ID,
     PNL_SHEET_ID,
     CASH_FLOW_SHEET_ID,
     BALANCE_SHEET_COLUMNS,
     PNL_SHEET_COLUMNS,
-    CODAL_BASIC_INFO_COLUMNS,
     CASH_FLOW_SHEET_COLUMNS,
 )
 from finops.logger import logger
 
 
 class Codal(Scraper, Preprocessor):
     def __init__(self, store_path, driver_path="selenium/chromedriver"):
@@ -67,22 +66,28 @@
         search_url = self._create_search_url(**search_params)
         response = self._download(search_url)
         parsed_response = self._parse_json_response(response)
         letters_list_df = self._preprocess_letters_list(parsed_response)
         return letters_list_df
 
     def scrap_letters_list(
-        self, search_params, start_page_number=None, stocks=None, verbose=True
+        self,
+        search_params,
+        start_page_number=None,
+        stocks=None,
+        n_threads=1,
+        verbose=True,
     ):
         letters_list = self._load_or_create_csv(
             self.letters_list_path, CODAL_LETTERS_LIST_COLUMNS
         )
         scraped_letters = self._get_scraped_ids(letters_list, "tracing_id")
         n_pages = self._get_letters_list_pages_number(search_params)
-        for page_number in range(start_page_number or 1, n_pages + 1):
+
+        def scrap_page(page_number):
             letters_list_one_page = self._scrap_letters_list_one_page(
                 search_params, page_number
             )
             if stocks is not None:
                 letters_list_one_page = letters_list_one_page[
                     letters_list_one_page.symbol.isin(stocks)
                 ]
@@ -90,14 +95,17 @@
                 ~letters_list_one_page.tracing_id.isin(scraped_letters)
             ]
             self._save_csv(letters_list_one_page, self.letters_list_path)
             time.sleep(1)
             if verbose:
                 logger.info(f"Page {page_number} of {n_pages} is scrapped.")
 
+        with concurrent.futures.ThreadPoolExecutor(max_workers=n_threads) as executor:
+            executor.map(scrap_page, range(start_page_number or 1, n_pages + 1))
+
     @retry(max_retries=3, wait_time=1)
     def _scrap_letter(self, driver, letter_url):
         driver.get(letter_url)
         response = WebDriverWait(driver, 10, 1).until(
             EC.presence_of_element_located(
                 (By.CSS_SELECTOR, ".table_wrapper, .rayanDynamicStatement")
             )
@@ -106,14 +114,27 @@
             response.get_attribute("innerHTML"), "html.parser"
         )
         letter = []
         for row in parsed_response.find_all("tr"):
             letter.append([cell.text for cell in row.find_all("td")])
         return pd.DataFrame(letter)
 
+    def _scrap_sheet(
+        self, driver, url, sheet_id, tracing_id, sheet_df, preprocess_func, path
+    ):
+        if tracing_id not in sheet_df.tracing_id.values:
+            try:
+                sheet_url = url + f"&sheetId={sheet_id}"
+                letter_df = preprocess_func(self._scrap_letter(driver, sheet_url))
+                letter_df["tracing_id"] = tracing_id
+                self._save_csv(letter_df, path)
+            except Exception as e:
+                print(e)
+                print(sheet_url)
+
     def _scrap_letter_wrapper(
         self,
         drivers,
         row,
         is_scrap_balance_sheets,
         is_scrap_pnl_sheets,
         is_scrap_cash_flow,
@@ -121,70 +142,62 @@
         pnl_sheets,
         cash_flow_sheets,
     ):
         url = row["url"]
         tracing_id = row["tracing_id"]
         driver = drivers.get()
 
-        if (
-            is_scrap_balance_sheets
-            and tracing_id not in balance_sheets.tracing_id.values
-        ):
-            try:
-                balance_sheet_url = url + f"&sheetId={BALANCE_SHEET_ID}"
-                letter_df = self._preprocess_balance_sheet_df(
-                    self._scrap_letter(driver, balance_sheet_url)
-                )
-                self._add_basic_letter_info(letter_df, row)
-                self._save_csv(letter_df, self.balance_sheets_path)
-            except Exception as e:
-                print(e)
-                print(balance_sheet_url)
+        if is_scrap_balance_sheets:
+            self._scrap_sheet(
+                driver,
+                url,
+                BALANCE_SHEET_ID,
+                tracing_id,
+                balance_sheets,
+                self._preprocess_balance_sheet_df,
+                self.balance_sheets_path,
+            )
 
-        if is_scrap_pnl_sheets and tracing_id not in pnl_sheets.tracing_id.values:
-            try:
-                pnl_sheet_url = url + f"&sheetId={PNL_SHEET_ID}"
-                letter_df = self._preprocess_pnl_df(
-                    self._scrap_letter(driver, pnl_sheet_url)
-                )
-                self._add_basic_letter_info(letter_df, row)
-                self._save_csv(letter_df, self.pnl_path)
-            except Exception as e:
-                print(e)
-                print(pnl_sheet_url)
+        if is_scrap_pnl_sheets:
+            self._scrap_sheet(
+                driver,
+                url,
+                PNL_SHEET_ID,
+                tracing_id,
+                pnl_sheets,
+                self._preprocess_pnl_df,
+                self.pnl_path,
+            )
 
-        if is_scrap_cash_flow and tracing_id not in cash_flow_sheets.tracing_id.values:
-            try:
-                cash_flow_url = url + f"&sheetId={CASH_FLOW_SHEET_ID}"
-                letter_df = self._preprocess_cash_flow_df(
-                    self._scrap_letter(driver, cash_flow_url)
-                )
-                self._add_basic_letter_info(letter_df, row)
-                self._save_csv(letter_df, self.cash_flow_path)
-            except Exception as e:
-                print(e)
-                print(cash_flow_url)
+        if is_scrap_cash_flow:
+            self._scrap_sheet(
+                driver,
+                url,
+                CASH_FLOW_SHEET_ID,
+                tracing_id,
+                cash_flow_sheets,
+                self._preprocess_cash_flow_df,
+                self.cash_flow_path,
+            )
 
         drivers.put(driver)
 
     def scrap_letters(
         self,
         is_scrap_balance_sheets=True,
         is_scrap_pnl_sheets=True,
         is_scrap_cash_flow=True,
         n_threads=5,
     ):
         balance_sheets = self._load_or_create_csv(
-            self.balance_sheets_path, BALANCE_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
-        )
-        pnl_sheets = self._load_or_create_csv(
-            self.pnl_path, PNL_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
+            self.balance_sheets_path, BALANCE_SHEET_COLUMNS
         )
+        pnl_sheets = self._load_or_create_csv(self.pnl_path, PNL_SHEET_COLUMNS)
         cash_flow_sheets = self._load_or_create_csv(
-            self.cash_flow_path, CASH_FLOW_SHEET_COLUMNS + CODAL_BASIC_INFO_COLUMNS
+            self.cash_flow_path, CASH_FLOW_SHEET_COLUMNS
         )
         letters_list = self._load_csv(self.letters_list_path)
 
         drivers = queue.Queue()
         for _ in range(n_threads):
             drivers.put(self._create_driver(self.driver_path))
```

### Comparing `finops-0.2.2/finops/config.py` & `finops-0.2.3/finops/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,71 +19,74 @@
     "value",
     "volume",
     "open_int",
     "per",
     "open",
     "last",
 ]
+
 SHAREHOLDER_DATA_COLUMNS = [
     "shareholder_id",
     "shareholder_name",
     "isin",
     "date",
     "n_shares",
     "per_shares",
     "ticker_index",
     "req_date",
 ]
+
 CODAL_LETTERS_LIST_COLUMNS = [
     "tracing_id",
     "symbol",
     "letter_title",
+    "is_audited",
+    "is_correction",
+    "is_consolidated",
+    "period_type",
+    "period_length",
+    "period_end_date",
     "url",
 ]
+
 PNL_SHEET_COLUMNS = [
     "gross_profit",
     "operating_profit",
     "pre_tax_profit",
     "net_profit",
     "basic_earnings_per_share",
     "net_earnings_per_share",
     "capital",
+    "tracing_id",
 ]
+
 BALANCE_SHEET_COLUMNS = [
     "total_current_assets",
     "total_noncurrent_assets",
     "total_assets",
     "total_current_liabilities",
     "total_noncurrent_liabilities",
     "total_liabilities",
     "total_equity",
     "total_liabilities_and_equity",
+    "tracing_id",
 ]
 
 CASH_FLOW_SHEET_COLUMNS = [
     "net_cash_flow_operational",
     "net_cash_flow_investment",
     "net_cash_flow_financing",
     "net_change_in_cash",
     "cash_balance_beginning_year",
     "cash_balance_end_year",
     "effect_exchange_rate_changes",
     "non_cash_transactions",
-]
-
-CODAL_BASIC_INFO_COLUMNS = [
     "tracing_id",
-    "symbol",
-    "is_audited",
-    "is_correction",
-    "is_consolidated",
-    "period_type",
-    "period_length",
-    "period_end_date",
 ]
+
 LOG_COLUMNS = [
     "id",
     "date",
 ]
 
 # Field maps
 PRICE_HISTORY_FIELD_MAP = {
```

### Comparing `finops-0.2.2/finops/tehran_stock_exchange.py` & `finops-0.2.3/finops/tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/finops/ticker.py` & `finops-0.2.3/finops/ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/finops/utils/downloader.py` & `finops-0.2.3/finops/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/finops/utils/preprocessor.py` & `finops-0.2.3/finops/utils/preprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -211,49 +211,58 @@
         df = df.drop_duplicates(subset=["title"], keep="first")
         df = df[df["title"].isin(CASH_FLOW_SHEET_COLUMNS)]
         df = df.set_index("title").T.reset_index(drop=True)
         df = self.safe_select_columns(df, CASH_FLOW_SHEET_COLUMNS)
         return df
 
     @staticmethod
-    def _preprocess_letters_list(parsed_response):
+    def _extract_period_type(letter_title):
+        period_type = re.search(r"(سال مالی|میاندوره‌ای|میاندوره ای)", letter_title)
+        if period_type is None:
+            return None
+        else:
+            period_type = "annual" if period_type.group() == "سال مالی" else "interim"
+        return period_type
+
+    def _extract_period_length(self, letter_title):
+        period_length = re.search(r"\d+(?= ماهه)", letter_title)
+        if period_length is None:
+            return None
+        else:
+            period_length = int(self._preprocess_persian_text(period_length.group()))
+        return period_length
+
+    @staticmethod
+    def _extract_period_end_date(letter_title):
+        period_end_date = re.search(r"\d{4}/\d{2}/\d{2}", letter_title)
+        if period_end_date is None:
+            return None
+        else:
+            period_end_date = (
+                jdatetime.datetime.strptime(
+                    period_end_date.group(),
+                    "%Y/%m/%d",
+                )
+                .date()
+                .togregorian()
+            )
+        return period_end_date
+
+    def _preprocess_letters_list(self, parsed_response):
         letters = parsed_response["Letters"]
         letters_list = []
         for letter in letters:
-            letters_list.append(
-                {
-                    "tracing_id": letter["TracingNo"],
-                    "symbol": letter["Symbol"],
-                    "letter_title": letter["Title"],
-                    "url": "https://www.codal.ir" + letter["Url"],
-                }
-            )
+            preprocessed_letter_info = {
+                "tracing_id": letter["TracingNo"],
+                "symbol": letter["Symbol"],
+                "letter_title": letter["Title"],
+                "is_audited": "حسابرسی شده" in letter["Title"],
+                "is_correction": "اصلاحیه" in letter["Title"],
+                "is_consolidated": "تلفیقی" in letter["Title"],
+                "period_type": self._extract_period_type(letter["Title"]),
+                "period_length": self._extract_period_length(letter["Title"]),
+                "period_end_date": self._extract_period_end_date(letter["Title"]),
+                "url": "https://www.codal.ir" + letter["Url"],
+            }
+            letters_list.append(preprocessed_letter_info)
         letters_list_df = pd.DataFrame(letters_list)
         return letters_list_df
-
-    def _add_basic_letter_info(self, letter_df, info):
-        letter_df["tracing_id"] = info["tracing_id"]
-        letter_df["symbol"] = info["symbol"]
-        letter_df["is_audited"] = "حسابرسی شده" in info["letter_title"]
-        letter_df["is_correction"] = "اصلاحیه" in info["letter_title"]
-        letter_df["is_consolidated"] = "تلفیقی" in info["letter_title"]
-        period_type = re.search(r"(سال مالی|میاندوره‌ای)", info["letter_title"])
-        if period_type is not None:
-            letter_df["period_type"] = "annual" if period_type.group() == "سال مالی" else "interim"
-        letter_df["period_length"] = (
-            int(
-                self._preprocess_persian_text(
-                    re.search(r"\d+(?= ماهه)", info["letter_title"]).group()
-                )
-            )
-            if re.search(r"\d+(?= ماهه)", info["letter_title"])
-            else 12
-        )
-        letter_df["period_end_date"] = (
-            jdatetime.datetime.strptime(
-                re.search(r"\d{4}/\d{2}/\d{2}", info["letter_title"]).group(),
-                "%Y/%m/%d",
-            )
-            .date()
-            .togregorian()
-        )
-        return letter_df
```

### Comparing `finops-0.2.2/finops/utils/scraper.py` & `finops-0.2.3/finops/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/finops/utils/wrappers.py` & `finops-0.2.3/finops/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/finops.egg-info/PKG-INFO` & `finops-0.2.3/finops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.2.2/finops.egg-info/SOURCES.txt` & `finops-0.2.3/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/setup.py` & `finops-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.2.2',
+    version='0.2.3',
     description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `finops-0.2.2/tests/test_tehran_stock_exchange.py` & `finops-0.2.3/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/tests/test_ticker.py` & `finops-0.2.3/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/tests/test_utils/test_downloader.py` & `finops-0.2.3/tests/test_utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.2/tests/test_utils/test_scraper.py` & `finops-0.2.3/tests/test_utils/test_scraper.py`

 * *Files identical despite different names*

