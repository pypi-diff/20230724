# Comparing `tmp/financetoolkit-1.1.1.tar.gz` & `tmp/financetoolkit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.1.1.tar", max compression
+gzip compressed data, was "financetoolkit-1.1.2.tar", max compression
```

## Comparing `financetoolkit-1.1.1.tar` & `financetoolkit-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0    15047 2023-07-20 09:08:23.484138 financetoolkit-1.1.1/README.md
--rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.1.1/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.1.1/financetoolkit/base/__init__.py
--rw-r--r--   0        0        0     3305 2023-07-20 08:13:34.949877 financetoolkit-1.1.1/financetoolkit/base/helpers.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.1.1/financetoolkit/base/models/__init__.py
--rw-r--r--   0        0        0    12891 2023-07-20 10:32:01.892332 financetoolkit-1.1.1/financetoolkit/base/models/fundamentals_model.py
--rw-r--r--   0        0        0     5680 2023-07-20 08:02:31.857798 financetoolkit-1.1.1/financetoolkit/base/models/historical_model.py
--rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.1.1/financetoolkit/base/models/normalization/README.md
--rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.1.1/financetoolkit/base/models/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.1.1/financetoolkit/base/models/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.1.1/financetoolkit/base/models/normalization/income.csv
--rw-r--r--   0        0        0     4126 2023-07-20 07:02:40.987492 financetoolkit-1.1.1/financetoolkit/base/models/normalization_model.py
--rw-r--r--   0        0        0     2751 2023-06-11 10:10:27.009590 financetoolkit-1.1.1/financetoolkit/base/models_controller.py
--rw-r--r--   0        0        0    53788 2023-07-20 07:14:06.784762 financetoolkit-1.1.1/financetoolkit/base/ratios_controller.py
--rw-r--r--   0        0        0    23583 2023-07-20 08:09:34.192259 financetoolkit-1.1.1/financetoolkit/base/toolkit_controller.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.1.1/financetoolkit/historical/__init__.py
--rw-r--r--   0        0        0     2804 2023-06-11 10:10:27.010650 financetoolkit-1.1.1/financetoolkit/historical/price.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.1.1/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     5436 2023-06-11 10:10:27.011152 financetoolkit-1.1.1/financetoolkit/models/dupont.py
--rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.1.1/financetoolkit/portfolio/__init__.py
--rw-r--r--   0        0        0     5958 2023-06-11 10:10:27.011432 financetoolkit-1.1.1/financetoolkit/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.1.1/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9590 2023-06-11 10:10:27.011837 financetoolkit-1.1.1/financetoolkit/ratios/efficiency.py
--rw-r--r--   0        0        0     5236 2023-06-11 10:10:27.012162 financetoolkit-1.1.1/financetoolkit/ratios/liquidity.py
--rw-r--r--   0        0        0    12600 2023-06-11 10:10:27.012508 financetoolkit-1.1.1/financetoolkit/ratios/profitability.py
--rw-r--r--   0        0        0     7090 2023-06-11 10:10:27.012732 financetoolkit-1.1.1/financetoolkit/ratios/solvency.py
--rw-r--r--   0        0        0    15285 2023-07-20 07:06:05.477276 financetoolkit-1.1.1/financetoolkit/ratios/valuation.py
--rw-r--r--   0        0        0     2023 2023-07-20 10:36:32.444640 financetoolkit-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    15896 1970-01-01 00:00:00.000000 financetoolkit-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2023-07-24 07:40:15.294645 financetoolkit-1.1.2/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.295650 financetoolkit-1.1.2/financetoolkit/base/__init__.py
+-rw-r--r--   0        0        0     3305 2023-07-24 07:40:15.296647 financetoolkit-1.1.2/financetoolkit/base/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.298642 financetoolkit-1.1.2/financetoolkit/base/models/__init__.py
+-rw-r--r--   0        0        0    13677 2023-07-24 10:10:48.464634 financetoolkit-1.1.2/financetoolkit/base/models/fundamentals_model.py
+-rw-r--r--   0        0        0     5548 2023-07-24 10:11:04.654704 financetoolkit-1.1.2/financetoolkit/base/models/historical_model.py
+-rw-r--r--   0        0        0     1813 2023-07-24 07:40:15.304647 financetoolkit-1.1.2/financetoolkit/base/models/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-07-24 07:40:15.305647 financetoolkit-1.1.2/financetoolkit/base/models/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-07-24 07:40:15.306647 financetoolkit-1.1.2/financetoolkit/base/models/normalization/income.csv
+-rw-r--r--   0        0        0     4267 2023-07-24 07:40:15.303656 financetoolkit-1.1.2/financetoolkit/base/models/normalization/README.md
+-rw-r--r--   0        0        0     4126 2023-07-24 07:40:15.307643 financetoolkit-1.1.2/financetoolkit/base/models/normalization_model.py
+-rw-r--r--   0        0        0     2751 2023-07-24 07:40:15.309645 financetoolkit-1.1.2/financetoolkit/base/models_controller.py
+-rw-r--r--   0        0        0    53788 2023-07-24 07:40:15.310644 financetoolkit-1.1.2/financetoolkit/base/ratios_controller.py
+-rw-r--r--   0        0        0    24679 2023-07-24 10:12:00.322591 financetoolkit-1.1.2/financetoolkit/base/toolkit_controller.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.313644 financetoolkit-1.1.2/financetoolkit/historical/__init__.py
+-rw-r--r--   0        0        0     2804 2023-07-24 07:40:15.314643 financetoolkit-1.1.2/financetoolkit/historical/price.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.316652 financetoolkit-1.1.2/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     5436 2023-07-24 07:40:15.317645 financetoolkit-1.1.2/financetoolkit/models/dupont.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.319646 financetoolkit-1.1.2/financetoolkit/portfolio/__init__.py
+-rw-r--r--   0        0        0     5958 2023-07-24 07:40:15.320645 financetoolkit-1.1.2/financetoolkit/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.321646 financetoolkit-1.1.2/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     9590 2023-07-24 07:40:15.323645 financetoolkit-1.1.2/financetoolkit/ratios/efficiency.py
+-rw-r--r--   0        0        0     5236 2023-07-24 07:40:15.324648 financetoolkit-1.1.2/financetoolkit/ratios/liquidity.py
+-rw-r--r--   0        0        0    12600 2023-07-24 07:40:15.326647 financetoolkit-1.1.2/financetoolkit/ratios/profitability.py
+-rw-r--r--   0        0        0     7090 2023-07-24 07:40:15.327648 financetoolkit-1.1.2/financetoolkit/ratios/solvency.py
+-rw-r--r--   0        0        0    15285 2023-07-24 07:40:15.328647 financetoolkit-1.1.2/financetoolkit/ratios/valuation.py
+-rw-r--r--   0        0        0     1069 2023-07-24 07:40:15.153513 financetoolkit-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2028 2023-07-24 10:14:25.119555 financetoolkit-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15047 2023-07-24 07:40:15.154509 financetoolkit-1.1.2/README.md
+-rw-r--r--   0        0        0    15896 1970-01-01 00:00:00.000000 financetoolkit-1.1.2/PKG-INFO
```

### Comparing `financetoolkit-1.1.1/LICENSE.txt` & `financetoolkit-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/README.md` & `financetoolkit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/helpers.py` & `financetoolkit-1.1.2/financetoolkit/base/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/fundamentals_model.py` & `financetoolkit-1.1.2/financetoolkit/base/models/fundamentals_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 """Fundamentals Module"""
 __docformat__ = "numpy"
 
 
-from urllib.error import HTTPError
-
 import numpy as np
 import pandas as pd
+import requests
 
 from financetoolkit.base.models.normalization_model import (
     convert_financial_statements,
 )
 
-# pylint: disable=no-member
+# pylint: disable=no-member,too-many-locals
 
 
 def get_financial_statements(
     tickers: str | list[str],
     statement: str = "",
     api_key: str = "",
     quarter: bool = False,
+    start_date: str | None = None,
+    end_date: str | None = None,
     limit: int = 100,
     statement_format: pd.DataFrame = pd.DataFrame(),
 ):
     """
     Retrieves financial statements (balance, income, or cash flow statements) for one or multiple companies,
     and returns a DataFrame containing the data.
 
     Args:
         tickers (List[str]): List of company tickers.
         statement (str): The type of financial statement to retrieve. Can be "balance", "income", or "cash-flow".
         api_key (str): API key for the financial data provider.
         quarter (bool): Whether to retrieve quarterly data. Defaults to False (annual data).
+        start_date (str): The start date to filter data with.
+        end_date (str): The end date to filter data with.
         statement_format (pd.DataFrame): Optional DataFrame containing the names of the financial
             statement line items to include in the output. Rows should contain the original name
             of the line item, and columns should contain the desired name for that line item.
 
     Returns:
         pd.DataFrame: A DataFrame containing the financial statement data. If only one ticker is provided, the
                       returned DataFrame will have a single column containing the data for that ticker. If multiple
@@ -68,28 +71,25 @@
 
     period = "quarter" if quarter else "annual"
 
     financial_statement_dict: dict = {}
     invalid_tickers = []
     for ticker in ticker_list:
         try:
-            financial_statement = pd.read_json(
+            response = requests.get(
                 f"https://financialmodelingprep.com/api/v3/{location}/"
-                f"{ticker}?period={period}&apikey={api_key}&limit={limit}"
-            )
-        except HTTPError:
-            print(
-                f"No financial statement data found for {ticker}. "
-                "This is usually due to data not available with "
-                "your current FMP plan."
+                f"{ticker}?period={period}&apikey={api_key}&limit={limit}",
+                timeout=60,
             )
+            response.raise_for_status()
+            financial_statement = pd.read_json(response.text)
+        except requests.exceptions.HTTPError:
+            print(f"{response.json()['Error Message']} (ticker: {ticker})")
             invalid_tickers.append(ticker)
             continue
-        except Exception as error:
-            raise ValueError(error) from error
 
         try:
             financial_statement = financial_statement.drop("symbol", axis=1)
         except KeyError:
             print(f"No financial statement data found for {ticker}")
             invalid_tickers.append(ticker)
             continue
@@ -115,18 +115,22 @@
         )
 
         try:
             financial_statement_total = financial_statement_total.astype(np.float64)
         except ValueError as error:
             print(
                 f"Not able to convert DataFrame to float64 due to {error}. This could result in"
-                "issues when values are zero and is prodominently relevant for "
+                "issues when values are zero and is predominently relevant for "
                 "ratio calculations."
             )
 
+        financial_statement_total = financial_statement_total.sort_index(
+            axis=1
+        ).truncate(before=start_date, after=end_date, axis=1)
+
         if quarter:
             financial_statement_total.columns = pd.PeriodIndex(
                 financial_statement_total.columns, freq="M"
             )
         else:
             financial_statement_total.columns = pd.PeriodIndex(
                 financial_statement_total.columns, freq="Y"
@@ -216,15 +220,18 @@
         except Exception as error:
             raise ValueError(error) from error
 
     return quote_dataframe, invalid_tickers
 
 
 def get_enterprise(
-    tickers: list[str] | str, api_key: str, quarter: bool = False, limit: int = 100
+    tickers: list[str] | str,
+    api_key: str,
+    quarter: bool = False,
+    limit: int = 100,
 ):
     """
     Description
     ----
     Gives information about the enterprise value of a company which includes
     i.a. market capitalisation, Cash & Cash Equivalents, total debt and enterprise value.
     Input
@@ -252,31 +259,44 @@
     enterprise_value_dict = {}
 
     period = "quarter" if quarter else "annual"
 
     invalid_tickers = []
     for ticker in ticker_list:
         try:
-            enterprise_values = pd.read_json(
+            response = requests.get(
                 f"https://financialmodelingprep.com/api/v3/enterprise-values/{ticker}"
-                f"?period={period}&limit={limit}&apikey={api_key}"
+                f"?period={period}&limit={limit}&apikey={api_key}",
+                timeout=60,
             )
-        except Exception as error:
-            raise ValueError(error) from error
+            response.raise_for_status()
+            enterprise_values = pd.read_json(response.text)
+        except requests.exceptions.HTTPError:
+            print(f"{response.json()['Error Message']} (ticker: {ticker})")
+            invalid_tickers.append(ticker)
+            continue
 
         try:
             enterprise_values = enterprise_values.drop("symbol", axis=1).sort_values(
                 by="date", ascending=True
             )
         except KeyError:
             print(f"No historical data found for {ticker}.")
             invalid_tickers.append(ticker)
             continue
 
-        enterprise_values["date"] = pd.to_datetime(enterprise_values["date"]).dt.year
+        if quarter:
+            enterprise_values["date"] = pd.PeriodIndex(
+                enterprise_values["date"], freq="M"
+            )
+        else:
+            enterprise_values["date"] = pd.PeriodIndex(
+                enterprise_values["date"], freq="Y"
+            )
+
         enterprise_values = enterprise_values.set_index("date")
 
         enterprise_values = enterprise_values.rename(
             columns={
                 "stockPrice": "Stock Price",
                 "numberOfShares": "Number of Shares",
                 "marketCapitalization": "Market Capitalization",
@@ -284,20 +304,23 @@
                 "addTotalDebt": "Total Debt",
                 "enterpriseValue": "Enterprise Value",
             }
         )
 
         enterprise_value_dict[ticker] = enterprise_values
 
-    enterprise_dataframe = pd.concat(enterprise_value_dict, axis=0).dropna()
+    if enterprise_value_dict:
+        enterprise_dataframe = pd.concat(enterprise_value_dict, axis=0).dropna()
 
-    if len(ticker_list) == 1:
-        enterprise_dataframe = enterprise_dataframe.loc[ticker_list[0]]
+        if len(ticker_list) == 1:
+            enterprise_dataframe = enterprise_dataframe.loc[ticker_list[0]]
 
-    return enterprise_dataframe, invalid_tickers
+        return enterprise_dataframe, invalid_tickers
+
+    return pd.DataFrame(), invalid_tickers
 
 
 def get_rating(tickers: list[str] | str, api_key: str, limit: int = 100):
     """
     Description
     ----
     Gives information about the rating of a company which includes i.a. the company
```

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/historical_model.py` & `financetoolkit-1.1.2/financetoolkit/base/models/historical_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,43 +61,36 @@
         if start_date > end_date:
             start_date = end_date - timedelta(days=10 * 365)
 
         start_timestamp = int(start_date.timestamp())
 
     historical_data_dict: dict = {}
 
-    if interval == "yearly":
-        yearly = True
+    if interval in ["yearly", "quarterly"]:
         interval = "1d"
-    else:
-        yearly = False
 
     invalid_tickers = []
     for ticker in ticker_list:
         url = (
             f"https://query1.finance.yahoo.com/v7/finance/download/{ticker}?"
             f"interval={interval}&period1={start_timestamp}&period2={end_timestamp}"
             "&events=history&includeAdjustedClose=true"
         )
-
         try:
             historical_data_dict[ticker] = pd.read_csv(url, index_col="Date")
         except HTTPError:
             print(f"No historical data found for {ticker}")
             invalid_tickers.append(ticker)
             continue
 
     if historical_data_dict:
         historical_data = pd.concat(historical_data_dict, axis=1)
         historical_data.columns = historical_data.columns.swaplevel(0, 1)
         historical_data = historical_data.sort_index(axis=1)
 
-        if yearly:
-            historical_data = convert_daily_to_yearly(historical_data)
-
         return historical_data, invalid_tickers
 
     return pd.DataFrame(), invalid_tickers
 
 
 def convert_daily_to_yearly(daily_historical_data: pd.DataFrame):
     """
```

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/normalization/README.md` & `financetoolkit-1.1.2/financetoolkit/base/models/normalization/README.md`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/normalization/balance.csv` & `financetoolkit-1.1.2/financetoolkit/base/models/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/normalization/cash.csv` & `financetoolkit-1.1.2/financetoolkit/base/models/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/normalization/income.csv` & `financetoolkit-1.1.2/financetoolkit/base/models/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models/normalization_model.py` & `financetoolkit-1.1.2/financetoolkit/base/models/normalization_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/models_controller.py` & `financetoolkit-1.1.2/financetoolkit/base/models_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/ratios_controller.py` & `financetoolkit-1.1.2/financetoolkit/base/ratios_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/base/toolkit_controller.py` & `financetoolkit-1.1.2/financetoolkit/base/toolkit_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Toolkit Module"""
 __docformat__ = "numpy"
 
 
+import re
+
 import pandas as pd
 
 from financetoolkit.base.models.fundamentals_model import (
     get_enterprise as _get_enterprise,
     get_financial_statements as _get_financial_statements,
     get_profile as _get_profile,
     get_quote as _get_quote,
@@ -36,20 +38,22 @@
     from other providers and, given a financial statement, allow for efficient manual
     calculations. This leads to one uniform method of calculation being applied that
     is available and understood by everyone.
     """
 
     def __init__(
         self,
-        tickers,
+        tickers: list | str,
         api_key: str = "",
         historical: pd.DataFrame = pd.DataFrame(),
         balance: pd.DataFrame = pd.DataFrame(),
         income: pd.DataFrame = pd.DataFrame(),
         cash: pd.DataFrame = pd.DataFrame(),
+        start_date: str | None = None,
+        end_date: str | None = None,
         quarterly: bool = False,
         format_location: str = "",
         reverse_dates: bool = False,
         remove_invalid_tickers: bool = True,
     ):
         """
         Initializes an Toolkit object with a ticker or a list of tickers.
@@ -67,15 +71,30 @@
         if isinstance(tickers, str):
             self._tickers = [tickers.upper()]
         elif isinstance(tickers, list):
             self._tickers = [ticker.upper() for ticker in tickers]
         else:
             raise TypeError("Tickers must be a string or a list of strings.")
 
+        if start_date and re.match(r"^\d{4}-\d{2}-\d{2}$", start_date) is None:
+            raise ValueError(
+                "Please input a valid start date (%Y-%m-%d) like '2010-01-01'"
+            )
+        if end_date and re.match(r"^\d{4}-\d{2}-\d{2}$", end_date) is None:
+            raise ValueError(
+                "Please input a valid end date (%Y-%m-%d) like '2020-01-01'"
+            )
+        if start_date and end_date and start_date > end_date:
+            raise ValueError(
+                f"Please ensure the start date {start_date} is before the end date {end_date}"
+            )
+
         self._api_key = api_key
+        self._start_date = start_date
+        self._end_date = end_date
         self._quarterly = quarterly
         self._remove_invalid_tickers = remove_invalid_tickers
         self._invalid_tickers: list = []
 
         if self._api_key:
             # Initialization of FinancialModelingPrep Variables
             self._profile: pd.DataFrame = pd.DataFrame()
@@ -166,29 +185,35 @@
             and self._income_statement.empty
             and self._cash_flow_statement.empty
         ):
             raise ValueError(
                 "The datasets could not be populated and therefore the Ratios class cannot be initialized."
             )
 
-        start = f"{self._balance_sheet_statement.columns[0].year - 5}-01-01"
-        end = f"{self._balance_sheet_statement.columns[-1].year + 5}-01-01"
+        if not self._start_date:
+            self._start_date = (
+                f"{self._balance_sheet_statement.columns[0].year - 5}-01-01"
+            )
+        if not self._end_date:
+            self._end_date = (
+                f"{self._balance_sheet_statement.columns[-1].year + 5}-01-01"
+            )
 
         if self._quarterly:
             if (
                 self._quarterly_historical_data.empty
                 and not self._balance_sheet_statement.empty
             ):
-                self.get_historical_data(period="quarterly", start=start, end=end)
+                self.get_historical_data(period="quarterly")
         elif not self._quarterly:
             if (
                 self._yearly_historical_data.empty
                 and not self._balance_sheet_statement.empty
             ):
-                self.get_historical_data(period="yearly", start=start, end=end)
+                self.get_historical_data(period="yearly")
         else:
             raise ValueError("Invalid value for the quarterly parameter.")
 
         if empty_data:
             print(
                 "The following data was not provided within the Toolkit class and "
                 f"thus was retrieved from FinancialModelingPrep: {', '.join(empty_data)}."
@@ -329,15 +354,18 @@
         if not self._api_key:
             return print(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._enterprise.empty:
             self._enterprise, self._invalid_tickers = _get_enterprise(
-                self._tickers, self._api_key, self._quarterly, limit
+                self._tickers,
+                self._api_key,
+                self._quarterly,
+                limit,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
                 for ticker in self._tickers
                 if ticker not in self._invalid_tickers
@@ -373,15 +401,15 @@
                 ticker
                 for ticker in self._tickers
                 if ticker not in self._invalid_tickers
             ]
 
         return self._rating
 
-    def get_historical_data(self, start=None, end=None, period: str = "daily"):
+    def get_historical_data(self, period: str = "daily"):
         """
         Returns a pandas dataframe containing the historical data for the specified tickers.
 
         Args:
             start (str): The start date for the historical data. Defaults to None.
             end (str): The end date for the historical data. Defaults to None.
             period (str): The interval at which the historical data should be
@@ -391,15 +419,15 @@
             ValueError: If an invalid value is specified for period.
 
         Returns:
             pandas.DataFrame: The historical data for the specified tickers.
         """
         if period == "daily":
             self._daily_historical_data, self._invalid_tickers = _get_historical_data(
-                self._tickers, start, end, interval="1d"
+                self._tickers, self._start_date, self._end_date, interval="1d"
             )
 
             if self._remove_invalid_tickers:
                 self._tickers = [
                     ticker
                     for ticker in self._tickers
                     if ticker not in self._invalid_tickers
@@ -412,15 +440,15 @@
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._daily_historical_data
 
         if period == "weekly":
             self._weekly_historical_data, self._invalid_tickers = _get_historical_data(
-                self._tickers, start, end, interval="1wk"
+                self._tickers, self._start_date, self._end_date, interval="1wk"
             )
 
             if self._remove_invalid_tickers:
                 self._tickers = [
                     ticker
                     for ticker in self._tickers
                     if ticker not in self._invalid_tickers
@@ -433,15 +461,15 @@
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._weekly_historical_data
 
         if period == "monthly":
             self._monthly_historical_data, self._invalid_tickers = _get_historical_data(
-                self._tickers, start, end, interval="1mo"
+                self._tickers, self._start_date, self._end_date, interval="1mo"
             )
 
             if self._remove_invalid_tickers:
                 self._tickers = [
                     ticker
                     for ticker in self._tickers
                     if ticker not in self._invalid_tickers
@@ -457,44 +485,44 @@
             return self._monthly_historical_data
 
         if period == "quarterly":
             if self._daily_historical_data.empty:
                 (
                     self._daily_historical_data,
                     self._invalid_tickers,
-                ) = _get_historical_data(self._tickers, start, end, interval="1d")
+                ) = _get_historical_data(
+                    self._tickers, self._start_date, self._end_date, interval="1d"
+                )
 
             self._quarterly_historical_data = _convert_daily_to_quarterly(
                 self._daily_historical_data
             )
 
             if self._remove_invalid_tickers:
                 self._tickers = [
                     ticker
                     for ticker in self._tickers
                     if ticker not in self._invalid_tickers
                 ]
 
-            self._quarterly_historical_data = (
-                self._quarterly_historical_data.sort_index()
-            )
-
             if len(self._tickers) == 1:
                 return self._quarterly_historical_data.xs(
                     self._tickers[0], level=1, axis="columns"
                 )
 
             return self._quarterly_historical_data
 
         if period == "yearly":
             if self._daily_historical_data.empty:
                 (
                     self._daily_historical_data,
                     self._invalid_tickers,
-                ) = _get_historical_data(self._tickers, start, end, interval="1d")
+                ) = _get_historical_data(
+                    self._tickers, self._start_date, self._end_date, interval="1d"
+                )
 
             self._yearly_historical_data = _convert_daily_to_yearly(
                 self._daily_historical_data
             )
 
             if self._remove_invalid_tickers:
                 self._tickers = [
@@ -521,15 +549,15 @@
         limit: int = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the balance sheet statement financial data for the company(s) from the specified source.
 
         Args:
-            quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
+            limit (int): Defines the maximum years or quarters to obtain.
 
         Returns:
             pd.DataFrame: A pandas DataFrame with the retrieved balance sheet statement data.
         """
         if not self._api_key and self._balance_sheet_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
@@ -540,14 +568,16 @@
                 self._balance_sheet_statement,
                 self._invalid_tickers,
             ) = _get_financial_statements(
                 self._tickers,
                 "balance",
                 self._api_key,
                 self._quarterly,
+                self._start_date,
+                self._end_date,
                 limit,
                 self._balance_sheet_statement_generic,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
@@ -565,15 +595,15 @@
         limit: int = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the income statement financial data for the company(s) from the specified source.
 
         Args:
-            quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
+            limit (int): Defines the maximum years or quarters to obtain.
 
         Returns:
             pd.DataFrame: A pandas DataFrame with the retrieved income statement data.
         """
         if not self._api_key and self._income_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
@@ -581,14 +611,16 @@
 
         if self._income_statement.empty or overwrite:
             self._income_statement, self._invalid_tickers = _get_financial_statements(
                 self._tickers,
                 "income",
                 self._api_key,
                 self._quarterly,
+                self._start_date,
+                self._end_date,
                 limit,
                 self._income_statement_generic,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
@@ -606,15 +638,15 @@
         limit: int = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the cash flow statement financial data for the company(s) from the specified source.
 
         Args:
-            quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
+            limit (int): Defines the maximum years or quarters to obtain.
 
         Returns:
             pd.DataFrame: A pandas DataFrame with the retrieved cash flow statement data.
         """
         if not self._api_key and self._cash_flow_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
@@ -625,14 +657,16 @@
                 self._cash_flow_statement,
                 self._invalid_tickers,
             ) = _get_financial_statements(
                 self._tickers,
                 "cashflow",
                 self._api_key,
                 self._quarterly,
+                self._start_date,
+                self._end_date,
                 limit,
                 self._cash_flow_statement_generic,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
```

### Comparing `financetoolkit-1.1.1/financetoolkit/historical/price.py` & `financetoolkit-1.1.2/financetoolkit/historical/price.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/models/dupont.py` & `financetoolkit-1.1.2/financetoolkit/models/dupont.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/portfolio/portfolio.py` & `financetoolkit-1.1.2/financetoolkit/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/ratios/efficiency.py` & `financetoolkit-1.1.2/financetoolkit/ratios/efficiency.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/ratios/liquidity.py` & `financetoolkit-1.1.2/financetoolkit/ratios/liquidity.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/ratios/profitability.py` & `financetoolkit-1.1.2/financetoolkit/ratios/profitability.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/ratios/solvency.py` & `financetoolkit-1.1.2/financetoolkit/ratios/solvency.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/financetoolkit/ratios/valuation.py` & `financetoolkit-1.1.2/financetoolkit/ratios/valuation.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.1/pyproject.toml` & `financetoolkit-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.1.1"
+version = "1.1.2"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
@@ -60,14 +60,14 @@
 [tool.isort]
 profile = "black"
 line_length = 122
 skip_gitignore = true
 combine_as_imports = true
 
 [tool.codespell]
-ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue,nd,fo,nWe,nwe,0t,Ot,ot'
+ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue,nd,fo,nWe,nwe,0t,Ot,ot,juNI'
 skip = '*.json,./.git,pyproject.toml,poetry.lock'
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::pytest.PytestAssertRewriteWarning:",
 ]
```

### Comparing `financetoolkit-1.1.1/PKG-INFO` & `financetoolkit-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Transparent and Efficient Financial Analysis
 Home-page: https://www.jeroenbouma.com/
 License: MIT
 Author: Jeroen Bouma
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

