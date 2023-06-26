# Comparing `tmp/cgt_calc-1.9.0.tar.gz` & `tmp/cgt_calc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgt_calc-1.9.0.tar", max compression
+gzip compressed data, was "cgt_calc-1.9.1.tar", max compression
```

## Comparing `cgt_calc-1.9.0.tar` & `cgt_calc-1.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1075 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/LICENSE
--rw-r--r--   0        0        0     4711 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/README.md
--rw-r--r--   0        0        0       32 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/__init__.py
--rw-r--r--   0        0        0     3119 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/args_parser.py
--rw-r--r--   0        0        0      973 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/const.py
--rw-r--r--   0        0        0     4387 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/currency_converter.py
--rw-r--r--   0        0        0      624 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/dates.py
--rw-r--r--   0        0        0     2960 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/exceptions.py
--rw-r--r--   0        0        0      701 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/initial_prices.py
--rwxr-xr-x   0        0        0    30758 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/main.py
--rw-r--r--   0        0        0     4785 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/model.py
--rw-r--r--   0        0        0     3882 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/parsers/__init__.py
--rw-r--r--   0        0        0     5359 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/parsers/mssb.py
--rw-r--r--   0        0        0     8776 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/parsers/schwab.py
--rw-r--r--   0        0        0    10919 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/parsers/schwab_equity_award_json.py
--rw-r--r--   0        0        0     9606 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/parsers/sharesight.py
--rw-r--r--   0        0        0     5459 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/parsers/trading212.py
--rw-r--r--   0        0        0        0 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/py.typed
--rw-r--r--   0        0        0     1905 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/render_latex.py
--rw-r--r--   0        0        0       99 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/resources/__init__.py
--rw-r--r--   0        0        0      498 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/resources/initial_prices.csv
--rw-r--r--   0        0        0     5022 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/resources/template.tex.j2
--rw-r--r--   0        0        0     1225 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/transaction_log.py
--rw-r--r--   0        0        0      445 2023-02-01 18:22:24.617001 cgt_calc-1.9.0/cgt_calc/util.py
--rw-r--r--   0        0        0     2297 2023-02-01 18:23:04.022026 cgt_calc-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 cgt_calc-1.9.0/setup.py
--rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 cgt_calc-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/LICENSE
+-rw-r--r--   0        0        0     4711 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/README.md
+-rw-r--r--   0        0        0       32 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/__init__.py
+-rw-r--r--   0        0        0     3119 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/args_parser.py
+-rw-r--r--   0        0        0      972 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/const.py
+-rw-r--r--   0        0        0     4388 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/currency_converter.py
+-rw-r--r--   0        0        0      624 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/dates.py
+-rw-r--r--   0        0        0     2960 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/exceptions.py
+-rw-r--r--   0        0        0      701 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/initial_prices.py
+-rwxr-xr-x   0        0        0    30758 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/main.py
+-rw-r--r--   0        0        0     4785 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/model.py
+-rw-r--r--   0        0        0     3882 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/parsers/__init__.py
+-rw-r--r--   0        0        0     5359 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/parsers/mssb.py
+-rw-r--r--   0        0        0     8774 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/parsers/schwab.py
+-rw-r--r--   0        0        0    10919 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/parsers/schwab_equity_award_json.py
+-rw-r--r--   0        0        0     9606 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/parsers/sharesight.py
+-rw-r--r--   0        0        0     5459 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/parsers/trading212.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/py.typed
+-rw-r--r--   0        0        0     1905 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/render_latex.py
+-rw-r--r--   0        0        0       99 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/resources/__init__.py
+-rw-r--r--   0        0        0      498 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/resources/initial_prices.csv
+-rw-r--r--   0        0        0     5022 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/resources/template.tex.j2
+-rw-r--r--   0        0        0     1225 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/transaction_log.py
+-rw-r--r--   0        0        0      445 2023-05-19 11:19:53.717376 cgt_calc-1.9.1/cgt_calc/util.py
+-rw-r--r--   0        0        0     2295 2023-05-19 11:20:36.177666 cgt_calc-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 cgt_calc-1.9.1/setup.py
+-rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 cgt_calc-1.9.1/PKG-INFO
```

### Comparing `cgt_calc-1.9.0/LICENSE` & `cgt_calc-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/README.md` & `cgt_calc-1.9.1/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# UK capital gains calculator
-
 [![CI](https://github.com/KapJI/capital-gains-calculator/actions/workflows/ci.yml/badge.svg)](https://github.com/KapJI/capital-gains-calculator/actions)
 [![PyPI version](https://img.shields.io/pypi/v/cgt-calc)](https://pypi.org/project/cgt-calc/)
 
+# UK capital gains calculator
+
 Calculate capital gains tax by transaction history exported from Charles Schwab, Trading 212 and Morgan Stanley. Generate PDF report with calculations.
 
 Automatically convert all prices to GBP and apply HMRC rules to calculate capital gains tax: "same day" rule, "bed and breakfast" rule, section 104 holding.
 
 ## Report example
 
 [calculations_example.pdf](https://github.com/KapJI/capital-gains-calculator/blob/main/calculations_example.pdf)
```

### Comparing `cgt_calc-1.9.0/cgt_calc/args_parser.py` & `cgt_calc-1.9.1/cgt_calc/args_parser.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/const.py` & `cgt_calc-1.9.1/cgt_calc/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     2016: 11100,
     2017: 11300,
     2018: 11700,
     2019: 12000,
     2020: 12300,
     2021: 12300,
     2022: 12300,
-    2023: 12300,
+    2023: 6000,
 }
 
 DEFAULT_REPORT_PATH: Final = "calculations.pdf"
 
 INTERNAL_START_DATE: Final = datetime.date(2010, 1, 1)
 
 # Resources
```

### Comparing `cgt_calc-1.9.0/cgt_calc/currency_converter.py` & `cgt_calc-1.9.1/cgt_calc/currency_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .exceptions import ExchangeRateMissingError, ParsingError
 from .model import BrokerTransaction
 
 EXCHANGE_RATES_HEADER: Final = ["month", "currency", "rate"]
 
 
 class CurrencyConverter:
-    """Coverter which holds rate history."""
+    """Converter which holds rate history."""
 
     def __init__(
         self,
         exchange_rates_file: str | None = None,
         initial_data: dict[str, dict[str, Decimal]] | None = None,
     ):
         """Load data from exchange_rates_file and optionally from initial_data."""
```

### Comparing `cgt_calc-1.9.0/cgt_calc/dates.py` & `cgt_calc-1.9.1/cgt_calc/dates.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/exceptions.py` & `cgt_calc-1.9.1/cgt_calc/exceptions.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/initial_prices.py` & `cgt_calc-1.9.1/cgt_calc/initial_prices.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/main.py` & `cgt_calc-1.9.1/cgt_calc/main.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/model.py` & `cgt_calc-1.9.1/cgt_calc/model.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/parsers/__init__.py` & `cgt_calc-1.9.1/cgt_calc/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/parsers/mssb.py` & `cgt_calc-1.9.1/cgt_calc/parsers/mssb.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/parsers/schwab.py` & `cgt_calc-1.9.1/cgt_calc/parsers/schwab.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         return ActionType.SELL
 
     if label in [
         "MoneyLink Transfer",
         "Misc Cash Entry",
         "Service Fee",
         "Wire Funds",
+        "Wire Sent",
         "Funds Received",
         "Journal",
         "Cash In Lieu",
     ]:
         return ActionType.TRANSFER
 
     if label == "Stock Plan Activity":
@@ -257,9 +258,9 @@
             date = datetime.datetime.strptime(date_str, "%Y/%m/%d").date()
         except ValueError:
             date = datetime.datetime.strptime(date_str, "%m/%d/%Y").date()
         symbol = lapse_main[2] if lapse_main[2] != "" else None
         price = Decimal(lapse_data[3].replace("$", "")) if lapse_data[3] != "" else None
         if symbol is not None and price is not None:
             symbol = TICKER_RENAMES.get(symbol, symbol)
-            initial_prices[date][symbol] = price  # type: ignore[index]
+            initial_prices[date][symbol] = price
     return AwardPrices(award_prices=dict(initial_prices))
```

### Comparing `cgt_calc-1.9.0/cgt_calc/parsers/schwab_equity_award_json.py` & `cgt_calc-1.9.1/cgt_calc/parsers/schwab_equity_award_json.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/parsers/sharesight.py` & `cgt_calc-1.9.1/cgt_calc/parsers/sharesight.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/parsers/trading212.py` & `cgt_calc-1.9.1/cgt_calc/parsers/trading212.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/render_latex.py` & `cgt_calc-1.9.1/cgt_calc/render_latex.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/resources/template.tex.j2` & `cgt_calc-1.9.1/cgt_calc/resources/template.tex.j2`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/cgt_calc/transaction_log.py` & `cgt_calc-1.9.1/cgt_calc/transaction_log.py`

 * *Files identical despite different names*

### Comparing `cgt_calc-1.9.0/pyproject.toml` & `cgt_calc-1.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgt-calc"
-version = "1.9.0"
+version = "1.9.1"
 description = "UK capital gains tax calculator for Charles Schwab and Trading 212 accounts"
 authors = ["Ruslan Sayfutdinov <ruslan@sayfutdinov.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/KapJI/capital-gains-calculator"
 repository = "https://github.com/KapJI/capital-gains-calculator"
 classifiers = [
@@ -27,29 +27,29 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 Jinja2 = ">=2.11.3,<4.0.0"
 requests = "^2.27.1"
 types-requests = "^2.27.7"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
-codespell = "^2.2.2"
+black = "^23.3"
+codespell = "^2.2.4"
 flake8 = "^5.0.4"
-flake8-bugbear = "^23.1.20"
-flake8-comprehensions = "^3.10.1"
+flake8-bugbear = "^23.3.12"
+flake8-comprehensions = "^3.12.0"
 flake8-docstrings = "^1.7.0"
-flake8-simplify = "^0.19.3"
+flake8-simplify = "^0.20.0"
 flake8-use-fstring = "^1.4"
 flake8-use-pathlib = "^0.3.0"
 isort = "^5.12.0"
-mypy = "^0.991"
-pandas = "^1.5.3"
-pre-commit = "^3.0.2"
-pylint = "^2.16.0"
-pytest = "^7.2.1"
+mypy = "^1.3"
+pandas = "^2.0.1"
+pre-commit = "^3.3.2"
+pylint = "^2.17.4"
+pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 cgt-calc = 'cgt_calc.main:init'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cgt_calc-1.9.0/setup.py` & `cgt_calc-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'types-requests>=2.27.7,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['cgt-calc = cgt_calc.main:init']}
 
 setup_kwargs = {
     'name': 'cgt-calc',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'UK capital gains tax calculator for Charles Schwab and Trading 212 accounts',
-    'long_description': '# UK capital gains calculator\n\n[![CI](https://github.com/KapJI/capital-gains-calculator/actions/workflows/ci.yml/badge.svg)](https://github.com/KapJI/capital-gains-calculator/actions)\n[![PyPI version](https://img.shields.io/pypi/v/cgt-calc)](https://pypi.org/project/cgt-calc/)\n\nCalculate capital gains tax by transaction history exported from Charles Schwab, Trading 212 and Morgan Stanley. Generate PDF report with calculations.\n\nAutomatically convert all prices to GBP and apply HMRC rules to calculate capital gains tax: "same day" rule, "bed and breakfast" rule, section 104 holding.\n\n## Report example\n\n[calculations_example.pdf](https://github.com/KapJI/capital-gains-calculator/blob/main/calculations_example.pdf)\n\n## Installation\n\nInstall it with [pipx](https://pypa.github.io/pipx/) (or regular pip):\n\n```shell\npipx install cgt-calc\n```\n\n## Prerequisites\n\n-   Python 3.8 or above.\n-   `pdflatex` is required to generate the report.\n\n## Install LaTeX\n\n### MacOS\n\n```shell\nbrew install --cask mactex-no-gui\n```\n\n### Debian based\n\n```shell\napt install texlive-latex-base\n```\n\n### Windows\n\n[Install MiKTeX.](https://miktex.org/download)\n\n## Usage\n\nYou will need several input files:\n\n-   Exported transaction history from Schwab in CSV format since the beginning.\n    Or at least since you first acquired the shares, which you were holding during the tax year. Schwab only allows to download transaction for the last 4 years so keep it safe. After that you may need to restore transactions from PDF statements.\n    [See example](https://github.com/KapJI/capital-gains-calculator/blob/main/tests/test_data/schwab_transactions.csv).\n-   Exported transaction history from Schwab Equity Awards (e.g. for Alphabet/Google employees) since the beginning. These are to be downloaded in JSON format. Instructions are available at the top of the [parser file](../main/cgt_calc/parsers/schwab_equity_award_json.py).\n-   Exported transaction history from Trading 212.\n    You can use several files here since Trading 212 limit the statements to 1 year periods.\n    [See example](https://github.com/KapJI/capital-gains-calculator/tree/main/tests/test_data/trading212).\n-   Exported transaction history from Morgan Stanley.\n    Since Morgan Stanley generates multiple files in a single report, please specify a directory produced from the report download page.\n-   Exported transaction history from Sharesight\n    Sharesight is a portfolio tracking tool with support for multiple brokers.\n\n    You will need the "All Trades" and "Taxable Income" reports since the beginning.\n    Make sure to select "Since Inception" for the period, and "Not Grouping".\n    Export both reports to Excel or Google Sheets, save as CSV, and place them in the same folder.\n\n    Sharesight aggregates transactions from multiple brokers, but doesn\'t necessarily have balance information.\n    Use the `--no-balance-check` flag to avoid spurious errors.\n\n    Since there is no direct support for equity grants, add `Stock Activity` as part of the comment associated with any vesting transactions - making sure they have the grant price filled.\n\n    [See example](https://github.com/KapJI/capital-gains-calculator/tree/main/tests/test_data/sharesight).\n\n-   CSV file with initial stock prices in USD at the moment of vesting, split, etc.\n    [`initial_prices.csv`](https://github.com/KapJI/capital-gains-calculator/blob/main/cgt_calc/resources/initial_prices.csv) comes pre-packaged, you need to use the same format.\n-   (Optional) Monthly exchange rates prices from [gov.uk](https://www.gov.uk/government/collections/exchange-rates-for-customs-and-vat).\n    `exchange_rates.csv` gets generated automatically using HMRC API, you need to use the same format if you want to override it.\n\nThen run (you can omit the brokers you don\'t use):\n\n```shell\ncgt-calc --year 2020 --schwab schwab_transactions.csv --trading212 trading212/ --mssb mmsb_report/\n```\n\nSee `cgt-calc --help` for the full list of settings.\n\n## Disclaimer\n\nPlease be aware that I\'m not a tax adviser so use this data at your own risk.\n\n## Contribute\n\nAll contributions are highly welcomed.\nIf you notice any bugs please open an issue or send a PR to fix it.\n\nFeel free to add new parsers to support transaction history from more brokers.\n\n## Testing\n\nThis project uses [Poetry](https://python-poetry.org/) for managing dependencies.\n\n-   For local testing you need to [install it](https://python-poetry.org/docs/#installation).\n-   After that run `poetry install` to install all dependencies.\n-   Then activate `pre-commit` hook: `poetry run pre-commit install`\n\nYou can also run all linters and tests manually with this command:\n\n```shell\npoetry run pre-commit run --all-files\n```\n',
+    'long_description': '[![CI](https://github.com/KapJI/capital-gains-calculator/actions/workflows/ci.yml/badge.svg)](https://github.com/KapJI/capital-gains-calculator/actions)\n[![PyPI version](https://img.shields.io/pypi/v/cgt-calc)](https://pypi.org/project/cgt-calc/)\n\n# UK capital gains calculator\n\nCalculate capital gains tax by transaction history exported from Charles Schwab, Trading 212 and Morgan Stanley. Generate PDF report with calculations.\n\nAutomatically convert all prices to GBP and apply HMRC rules to calculate capital gains tax: "same day" rule, "bed and breakfast" rule, section 104 holding.\n\n## Report example\n\n[calculations_example.pdf](https://github.com/KapJI/capital-gains-calculator/blob/main/calculations_example.pdf)\n\n## Installation\n\nInstall it with [pipx](https://pypa.github.io/pipx/) (or regular pip):\n\n```shell\npipx install cgt-calc\n```\n\n## Prerequisites\n\n-   Python 3.8 or above.\n-   `pdflatex` is required to generate the report.\n\n## Install LaTeX\n\n### MacOS\n\n```shell\nbrew install --cask mactex-no-gui\n```\n\n### Debian based\n\n```shell\napt install texlive-latex-base\n```\n\n### Windows\n\n[Install MiKTeX.](https://miktex.org/download)\n\n## Usage\n\nYou will need several input files:\n\n-   Exported transaction history from Schwab in CSV format since the beginning.\n    Or at least since you first acquired the shares, which you were holding during the tax year. Schwab only allows to download transaction for the last 4 years so keep it safe. After that you may need to restore transactions from PDF statements.\n    [See example](https://github.com/KapJI/capital-gains-calculator/blob/main/tests/test_data/schwab_transactions.csv).\n-   Exported transaction history from Schwab Equity Awards (e.g. for Alphabet/Google employees) since the beginning. These are to be downloaded in JSON format. Instructions are available at the top of the [parser file](../main/cgt_calc/parsers/schwab_equity_award_json.py).\n-   Exported transaction history from Trading 212.\n    You can use several files here since Trading 212 limit the statements to 1 year periods.\n    [See example](https://github.com/KapJI/capital-gains-calculator/tree/main/tests/test_data/trading212).\n-   Exported transaction history from Morgan Stanley.\n    Since Morgan Stanley generates multiple files in a single report, please specify a directory produced from the report download page.\n-   Exported transaction history from Sharesight\n    Sharesight is a portfolio tracking tool with support for multiple brokers.\n\n    You will need the "All Trades" and "Taxable Income" reports since the beginning.\n    Make sure to select "Since Inception" for the period, and "Not Grouping".\n    Export both reports to Excel or Google Sheets, save as CSV, and place them in the same folder.\n\n    Sharesight aggregates transactions from multiple brokers, but doesn\'t necessarily have balance information.\n    Use the `--no-balance-check` flag to avoid spurious errors.\n\n    Since there is no direct support for equity grants, add `Stock Activity` as part of the comment associated with any vesting transactions - making sure they have the grant price filled.\n\n    [See example](https://github.com/KapJI/capital-gains-calculator/tree/main/tests/test_data/sharesight).\n\n-   CSV file with initial stock prices in USD at the moment of vesting, split, etc.\n    [`initial_prices.csv`](https://github.com/KapJI/capital-gains-calculator/blob/main/cgt_calc/resources/initial_prices.csv) comes pre-packaged, you need to use the same format.\n-   (Optional) Monthly exchange rates prices from [gov.uk](https://www.gov.uk/government/collections/exchange-rates-for-customs-and-vat).\n    `exchange_rates.csv` gets generated automatically using HMRC API, you need to use the same format if you want to override it.\n\nThen run (you can omit the brokers you don\'t use):\n\n```shell\ncgt-calc --year 2020 --schwab schwab_transactions.csv --trading212 trading212/ --mssb mmsb_report/\n```\n\nSee `cgt-calc --help` for the full list of settings.\n\n## Disclaimer\n\nPlease be aware that I\'m not a tax adviser so use this data at your own risk.\n\n## Contribute\n\nAll contributions are highly welcomed.\nIf you notice any bugs please open an issue or send a PR to fix it.\n\nFeel free to add new parsers to support transaction history from more brokers.\n\n## Testing\n\nThis project uses [Poetry](https://python-poetry.org/) for managing dependencies.\n\n-   For local testing you need to [install it](https://python-poetry.org/docs/#installation).\n-   After that run `poetry install` to install all dependencies.\n-   Then activate `pre-commit` hook: `poetry run pre-commit install`\n\nYou can also run all linters and tests manually with this command:\n\n```shell\npoetry run pre-commit run --all-files\n```\n',
     'author': 'Ruslan Sayfutdinov',
     'author_email': 'ruslan@sayfutdinov.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/KapJI/capital-gains-calculator',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cgt_calc-1.9.0/PKG-INFO` & `cgt_calc-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt-calc
-Version: 1.9.0
+Version: 1.9.1
 Summary: UK capital gains tax calculator for Charles Schwab and Trading 212 accounts
 Home-page: https://github.com/KapJI/capital-gains-calculator
 License: MIT
 Keywords: capital gain,schwab,trading 212
 Author: Ruslan Sayfutdinov
 Author-email: ruslan@sayfutdinov.com
 Requires-Python: >=3.8,<4.0
@@ -22,19 +22,19 @@
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: types-requests (>=2.27.7,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/KapJI/capital-gains-calculator/issues
 Project-URL: Repository, https://github.com/KapJI/capital-gains-calculator
 Project-URL: Release Notes, https://github.com/KapJI/capital-gains-calculator/releases
 Description-Content-Type: text/markdown
 
-# UK capital gains calculator
-
 [![CI](https://github.com/KapJI/capital-gains-calculator/actions/workflows/ci.yml/badge.svg)](https://github.com/KapJI/capital-gains-calculator/actions)
 [![PyPI version](https://img.shields.io/pypi/v/cgt-calc)](https://pypi.org/project/cgt-calc/)
 
+# UK capital gains calculator
+
 Calculate capital gains tax by transaction history exported from Charles Schwab, Trading 212 and Morgan Stanley. Generate PDF report with calculations.
 
 Automatically convert all prices to GBP and apply HMRC rules to calculate capital gains tax: "same day" rule, "bed and breakfast" rule, section 104 holding.
 
 ## Report example
 
 [calculations_example.pdf](https://github.com/KapJI/capital-gains-calculator/blob/main/calculations_example.pdf)
```

