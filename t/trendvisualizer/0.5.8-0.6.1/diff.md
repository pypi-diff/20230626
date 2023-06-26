# Comparing `tmp/trendvisualizer-0.5.8-py3-none-any.whl.zip` & `tmp/trendvisualizer-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33356 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat       31 b- defN 23-Jan-05 18:08 trendvisualizer/__init__.py
--rw-rw-rw-  2.0 fat    23176 b- defN 22-Mar-07 16:55 trendvisualizer/chart_display.py
--rw-rw-rw-  2.0 fat    19799 b- defN 22-Mar-07 16:36 trendvisualizer/chart_prep.py
--rw-rw-rw-  2.0 fat    16670 b- defN 21-Dec-14 18:51 trendvisualizer/marketdata.py
--rw-rw-rw-  2.0 fat    16964 b- defN 22-Mar-07 16:51 trendvisualizer/pie_charts.py
+Zip file size: 33787 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Jun-26 18:59 trendvisualizer/__init__.py
+-rw-rw-rw-  2.0 fat    24163 b- defN 23-Jun-26 18:53 trendvisualizer/chart_display.py
+-rw-rw-rw-  2.0 fat    20547 b- defN 23-Jun-26 16:50 trendvisualizer/chart_prep.py
+-rw-rw-rw-  2.0 fat    17097 b- defN 23-Jun-26 16:53 trendvisualizer/marketdata.py
+-rw-rw-rw-  2.0 fat    17319 b- defN 23-Jun-26 17:02 trendvisualizer/pie_charts.py
 -rw-rw-rw-  2.0 fat    56266 b- defN 21-Dec-14 19:25 trendvisualizer/sector_mappings.py
--rw-rw-rw-  2.0 fat    10921 b- defN 22-Mar-07 16:55 trendvisualizer/trend.py
+-rw-rw-rw-  2.0 fat    11178 b- defN 23-Jun-26 17:24 trendvisualizer/trend.py
 -rw-rw-rw-  2.0 fat     6068 b- defN 21-Dec-14 18:22 trendvisualizer/trend_params.py
--rw-rw-rw-  2.0 fat    21705 b- defN 21-Dec-14 19:13 trendvisualizer/trenddata.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jan-05 18:19 trendvisualizer-0.5.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      980 b- defN 23-Jan-05 18:19 trendvisualizer-0.5.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-05 18:19 trendvisualizer-0.5.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jan-05 18:19 trendvisualizer-0.5.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1206 b- defN 23-Jan-05 18:19 trendvisualizer-0.5.8.dist-info/RECORD
-14 files, 174983 bytes uncompressed, 31346 bytes compressed:  82.1%
+-rw-rw-rw-  2.0 fat    22695 b- defN 23-Jun-26 17:12 trendvisualizer/trenddata.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-26 19:00 trendvisualizer-0.6.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      766 b- defN 23-Jun-26 19:00 trendvisualizer-0.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 19:00 trendvisualizer-0.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-26 19:00 trendvisualizer-0.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1206 b- defN 23-Jun-26 19:00 trendvisualizer-0.6.1.dist-info/RECORD
+14 files, 178533 bytes uncompressed, 31777 bytes compressed:  82.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: trendvisualizer/trend_params.py
 Comment: 
 
 Filename: trendvisualizer/trenddata.py
 Comment: 
 
-Filename: trendvisualizer-0.5.8.dist-info/LICENSE
+Filename: trendvisualizer-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: trendvisualizer-0.5.8.dist-info/METADATA
+Filename: trendvisualizer-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: trendvisualizer-0.5.8.dist-info/WHEEL
+Filename: trendvisualizer-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: trendvisualizer-0.5.8.dist-info/top_level.txt
+Filename: trendvisualizer-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: trendvisualizer-0.5.8.dist-info/RECORD
+Filename: trendvisualizer-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trendvisualizer/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.5.8"
+__version__ = "0.6.1"
```

## trendvisualizer/chart_display.py

```diff
@@ -2,28 +2,33 @@
 Display various charts of Trend Strength
 
 """
 import warnings
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 import seaborn as sns
+from matplotlib import axes, cm
 from matplotlib.dates import MO, WeekdayLocator, MonthLocator
 from matplotlib.ticker import MaxNLocator, AutoMinorLocator, PercentFormatter
 from trendvisualizer.chart_prep import Formatting
 
 
 class Graphs():
     """
     Barchart, Line Graph, Summary Charts,Piecharts displaying trend strength
     of various markets
 
     """
     @classmethod
-    def trendbarchart(cls, params, barometer):
+    def trendbarchart(
+        cls,
+        params: dict,
+        barometer: pd.DataFrame) -> None:
         """
         Create a barchart of the most or least trending markets.
 
         Parameters
         ----------
         params : Dict
             mkts : Int
@@ -103,54 +108,63 @@
                      style='italic',
                      y=1.04)
 
         plt.show()
 
 
     @staticmethod
-    def _bar_up(ax1, params, barometer):
+    def _bar_up(
+        ax1: axes.Axes,
+        params: dict,
+        barometer: pd.DataFrame) -> tuple[axes.Axes, str]:
 
         # Set the x-axis range
-        ax1.set_xlim([0,1])
+        ax1.set_xlim(left=0, right=1)
 
         # Sort by Trend Strength
         barometer = barometer.sort_values(
             by=['Trend Strength %'], ascending=True)
 
         plt.barh(barometer['Short_name'][-params['mkts']:],
                  barometer['Trend Strength %'][-params['mkts']:],
                  color=list(barometer['Trend Color'][-params['mkts']:]))
         titlestr = 'Up'
 
         return ax1, titlestr
 
 
     @staticmethod
-    def _bar_down(ax1, params, barometer):
+    def _bar_down(
+        ax1: axes.Axes,
+        params: dict,
+        barometer: pd.DataFrame) -> tuple[axes.Axes, str]:
 
         # Set the x-axis range
-        ax1.set_xlim([-1,0])
+        ax1.set_xlim(left=-1, right=0)
 
         # Sort by Trend Strength
         barometer = barometer.sort_values(
             by=['Trend Strength %'], ascending=False)
 
         plt.barh(barometer['Short_name'][-params['mkts']:],
                  barometer['Trend Strength %'][-params['mkts']:],
                  color=list(barometer['Trend Color'][-params['mkts']:]))
         titlestr = 'Down'
 
         return ax1, titlestr
 
 
     @staticmethod
-    def _bar_neutral(ax1, params, barometer):
+    def _bar_neutral(
+        ax1: axes.Axes,
+        params: dict,
+        barometer: pd.DataFrame) -> tuple[axes.Axes, str]:
 
         # Set the x-axis range
-        ax1.set_xlim([-1,1])
+        ax1.set_xlim(left=-1, right=1)
 
         # Sort by Absolute Trend Strength
         barometer = barometer.sort_values(
             by=['Absolute Trend Strength %'], ascending=True)
 
         plt.barh(barometer['Short_name'][:params['mkts']],
                  barometer['Trend Strength %'][:params['mkts']],
@@ -159,33 +173,39 @@
                  )
         titlestr = 'Neutral'
 
         return ax1, titlestr
 
 
     @staticmethod
-    def _bar_strong(ax1, params, barometer):
+    def _bar_strong(
+        ax1: axes.Axes,
+        params: dict,
+        barometer: pd.DataFrame) -> tuple[axes.Axes, str]:
 
         # Set the x-axis range
-        ax1.set_xlim([-1,1])
+        ax1.set_xlim(left=-1, right=1)
 
         # Sort by Absolute Trend Strength
         barometer = barometer.sort_values(
             by=['Absolute Trend Strength %'], ascending=True)
 
         plt.barh(barometer['Short_name'][-params['mkts']:],
                  barometer['Trend Strength %'][-params['mkts']:],
                  color=list(barometer['Trend Color'][-params['mkts']:]))
         titlestr = 'Strongly'
 
         return ax1, titlestr
 
 
     @classmethod
-    def returnsgraph(cls, params, tables):
+    def returnsgraph(
+        cls,
+        params: dict,
+        tables: dict) -> None:
         """
         Create a line graph of normalised price history
 
         Parameters
         ----------
         params : Dict
             mkts : Int
@@ -272,15 +292,17 @@
                      style='italic',
                      y=dynamic_y) #1.08) #0.98)
 
         plt.show()
 
 
     @staticmethod
-    def _returns_ticks(ax1, tenor):
+    def _returns_ticks(
+        ax1: axes.Axes,
+        tenor: pd.DataFrame) -> axes.Axes:
 
         # create a variable to choose interval between xticks based on
         # length of history
         week_scaler = int(round(len(tenor) / 30))
         month_scaler = int(round(len(tenor) / 120))
 
         # Set major xticks as every 4th Monday or monthly at a specified
@@ -311,15 +333,15 @@
         # Set size of ticks
         ax1.tick_params(which='both', width=1)
         ax1.tick_params(which='major', length=8)
         ax1.tick_params(which='minor', length=4)
 
         # Set prices to the right as we are concerned with the current
         # level
-        ax1.yaxis.set_major_locator(plt.MaxNLocator(11))
+        ax1.yaxis.set_major_locator(MaxNLocator(11))
         ax1.yaxis.set_label_position('right')
         ax1.yaxis.tick_right()
 
         # Set ytick labels
         yticklabels = (
             int(round(tenor.min().min(), -1)),
             100 - int((abs(100 - round(tenor.min().min(), -1))) / 2),
@@ -329,15 +351,18 @@
 
         ax1.set_yticks(yticklabels)
 
         return ax1
 
 
     @classmethod
-    def marketchart(cls, params, tables):
+    def marketchart(
+        cls,
+        params: dict,
+        tables: dict) -> dict:
         """
         Create a chart showing the top and bottom 20 trending markets.
 
         Parameters
         ----------
         params : Dict
             days : Int
@@ -378,15 +403,15 @@
             num_charts=params['num_charts'])
 
         # Set style
         plt.style.use('seaborn-darkgrid')
         plt.rcParams.update(params['mpl_chart_params'])
 
         # create a color palette
-        palette = plt.get_cmap('tab20')
+        palette = cm.get_cmap('tab20')
 
         # Initialize the figure
         fig, ax1 = plt.subplots(figsize=(int(params['chart_dimensions'][1]*3),
                                         int(params['chart_dimensions'][0]*2)))
         fig.subplots_adjust(top=0.85)
         fig.tight_layout()
 
@@ -460,15 +485,17 @@
                      style='italic',
                      y=1.05)
 
         return params
 
 
     @staticmethod
-    def _market_ticks(ax1, params):
+    def _market_ticks(
+        ax1: axes.Axes,
+        params: dict) -> axes.Axes:
 
         # create a variable to choose interval between xticks based
         # on length of history
         week_scaler = int(round(params['days'] / 30))
         month_scaler = int(round(params['days'] / 120))
 
         # Set major xticks as every 4th Monday or monthly at a
@@ -507,15 +534,18 @@
         ax1.yaxis.set_label_position('right')
         ax1.yaxis.tick_right()
 
         return ax1
 
 
     @classmethod
-    def summaryplot(cls, params, tables):
+    def summaryplot(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Plot a summary of the strength of trend across markets
 
         Parameters
         ----------
         params : Dict
             sector_level : Int, optional
@@ -586,15 +616,18 @@
         # Return warnings to default setting
         warnings.filterwarnings("default", category=UserWarning)
 
         return params, tables
 
 
     @staticmethod
-    def _create_swarm(ax1, params, tables):
+    def _create_swarm(
+        ax1: axes.Axes,
+        params: dict,
+        tables: dict) -> axes.Axes:
 
         ax1 = sns.swarmplot(data=tables['chart_barometer'],
                             x=params['trend_type'],
                             y="Trend",
                             hue=params['sector_name'],
                             hue_order=params['sector_list'],
                             dodge=params['dodge'],
@@ -620,34 +653,39 @@
                   frameon=True,
                   facecolor='white')
 
         return ax1
 
 
     @staticmethod
-    def _create_strip(ax1, params, tables):
+    def _create_strip(
+        ax1: axes.Axes,
+        params: dict,
+        tables: dict) -> axes.Axes:
 
         if params['violin']:
             ax1 = sns.violinplot(x=params['trend_type'],
                                 y=params['sector_name'],
                                 data=tables['chart_barometer'],
                                 inner='quartile',
                                 #color=".8",
                                 linewidth=1,
                                 palette="coolwarm",
+                                hue=params['sector_name'],
                                 scale='count')
         ax1 = sns.stripplot(x=params['trend_type'],
                            y=params['sector_name'],
                            data=tables['chart_barometer'],
                            dodge=True,
                            alpha=0.5,
                            jitter=0.2,
                            order=params['sector_list'],
                            marker=params['marker'],
                            palette='viridis',
+                           hue=params['sector_name'],
                            s=params['marker_size'])
 
         ax1.set_title('Trend Strength by Sector'
                       +' - '
                       +params['end_date'],
                       fontsize=18, y=1)
         ax1.xaxis.set_major_formatter(PercentFormatter(1))
```

## trendvisualizer/chart_prep.py

```diff
@@ -9,15 +9,15 @@
 
 class Formatting():
     """
     Various data formatting methods for graphing
 
     """
     @staticmethod
-    def get_charttitle(params):
+    def get_charttitle(params: dict) -> dict:
         """
         Create title label for market chart
 
         Parameters
         ----------
         norm : Bool
             Whether the prices have been normalised.
@@ -92,15 +92,15 @@
 
         charttitle = charttitle+' - '+params['end_date']
 
         return charttitle
 
 
     @staticmethod
-    def mkt_dims(params):
+    def mkt_dims(params: dict) -> dict:
         """
         Create a tuple giving the height and width of the market chart
 
         Parameters
         ----------
         mkts : Int
             Number of markets to chart.
@@ -137,15 +137,18 @@
         height = math.ceil(mkts/width)
         params['chart_dimensions'] = (height, width)
 
         return params
 
 
     @classmethod
-    def normdata(cls, params, tables):
+    def normdata(
+        cls,
+        params: dict,
+        tables: dict) -> pd.DataFrame:
         """
         Create a subset of chart_prep dataset normalized to start from
         100 for the specified history window
 
         Parameters
         ----------
         params : Dict
@@ -184,15 +187,18 @@
         for ticker in tenor.columns:
             tenor[ticker] = tenor[ticker].div(tenor[ticker].iloc[0]).mul(100)
 
         return tenor
 
 
     @classmethod
-    def _chartdata(cls, params, tables):
+    def _chartdata(
+        cls,
+        params: dict,
+        tables: dict) -> pd.DataFrame:
         """
         Create a time series of closing prices for selected markets.
 
         Parameters
         ----------
         params : Dict
             mkts : Int
@@ -234,15 +240,20 @@
             columns=params['ticker_short_name_dict'])
         chart_data = chart_data.fillna(method='ffill')
 
         return chart_data
 
 
     @classmethod
-    def datalist(cls, params, barometer, market_chart, num_charts):
+    def datalist(
+        cls,
+        params: dict,
+        barometer: pd.DataFrame,
+        market_chart: bool,
+        num_charts: int) -> list:
         """
         Create a list of the most / least trending markets.
 
         Parameters
         ----------
         params : Dict
             mkts : Int
@@ -311,15 +322,19 @@
                 barometer=barometer, market_chart=market_chart,
                 num_charts=num_charts, mkts=mkts)
 
         return data_list
 
 
     @staticmethod
-    def _uptrend(barometer, market_chart, num_charts, mkts):
+    def _uptrend(
+        barometer: pd.DataFrame,
+        market_chart: bool,
+        num_charts: int,
+        mkts: int) -> list:
 
         # Sort by Trend Strength
         barometer = barometer.sort_values(
             by=['Trend Strength'], ascending=False)
 
         if market_chart:
             # Select the specified number of highest values
@@ -329,15 +344,19 @@
             # Select the highest values
             data_list = list(barometer['Ticker'][:mkts])
 
         return data_list
 
 
     @staticmethod
-    def _downtrend(barometer, market_chart, num_charts, mkts):
+    def _downtrend(
+        barometer: pd.DataFrame,
+        market_chart: bool,
+        num_charts: int,
+        mkts: int) -> list:
 
         # Sort by Trend Strength
         barometer = barometer.sort_values(
             by=['Trend Strength'], ascending=False)
 
         if market_chart:
             # Select the specified number of lowest values
@@ -347,15 +366,19 @@
             # Select the lowest values
             data_list = list(barometer['Ticker'][-mkts:])
 
         return data_list
 
 
     @staticmethod
-    def _neutraltrend(barometer, market_chart, num_charts, mkts):
+    def _neutraltrend(
+        barometer: pd.DataFrame,
+        market_chart: bool,
+        num_charts: int,
+        mkts: int) -> list:
 
         # Sort by Absolute Trend Strength
         barometer = barometer.sort_values(
             by=['Absolute Trend Strength'], ascending=False)
 
         if market_chart:
             # Select the specified number of lowest values
@@ -365,15 +388,19 @@
             # Select the lowest values
             data_list = list(barometer['Ticker'][-mkts:])
 
         return data_list
 
 
     @staticmethod
-    def _strongtrend(barometer, market_chart, num_charts, mkts):
+    def _strongtrend(
+        barometer: pd.DataFrame,
+        market_chart: bool,
+        num_charts: int,
+        mkts: int) -> list:
 
         # Sort by Trend Strength
         barometer = barometer.sort_values(
             by=['Trend Strength'], ascending=False)
 
         if market_chart:
             # Select the specified number of highest values
@@ -394,15 +421,19 @@
         # Combine this data
         data_list = top + bottom
 
         return data_list
 
 
     @staticmethod
-    def _mixedtrend(barometer, market_chart, num_charts, mkts):
+    def _mixedtrend(
+        barometer: pd.DataFrame,
+        market_chart: bool,
+        num_charts: int,
+        mkts: int) -> list:
 
         # Sort by Trend Strength
         barometer = barometer.sort_values(
             by=['Trend Strength'], ascending=False)
 
         if market_chart:
             # Select 1/3 of the specified number of highest values
@@ -437,15 +468,18 @@
         # Combine this data
         data_list = top + bottom + neutral
 
         return data_list
 
 
     @classmethod
-    def summary_config(cls, params, barometer):
+    def summary_config(
+        cls,
+        params: dict,
+        barometer: pd.DataFrame) -> tuple[dict, pd.DataFrame]:
         """
         Configure inputs for Trend Summary plots
 
         Parameters
         ----------
         params : Dict
             sector_level : Int, optional
@@ -555,15 +589,18 @@
         chart_barometer = chart_barometer.sort_values(
             by=[params['trend_type']], ascending=True)
 
         return params, chart_barometer
 
 
     @staticmethod
-    def _setheight(params, chart_barometer, trend_sector_group):
+    def _setheight(
+        params: dict,
+        chart_barometer: pd.DataFrame,
+        trend_sector_group: pd.DataFrame) -> float:
 
         max_bucket = chart_barometer[params['trend_type']].value_counts().max()
 
         max_bucket_per_sector = trend_sector_group.groupby(
             trend_sector_group.columns.tolist()).size().max()
 
         num_sectors = len(chart_barometer[params['sector_name']].unique())
```

## trendvisualizer/marketdata.py

```diff
@@ -12,15 +12,15 @@
 
 class NorgateExtract():
     """
     Functions to extract data from Norgate Data
 
     """
     @staticmethod
-    def get_norgate_tickers(params):
+    def get_norgate_tickers(params: dict) -> dict:
         """
         Create list of all available Norgate Commodity tickers
 
         Returns
         -------
         tickers : List
             Returns a list of ticker codes.
@@ -73,15 +73,19 @@
         params['tickers'] = tickers
         params['init_ticker_dict'] = init_ticker_dict
 
         return params
 
 
     @classmethod
-    def importnorgate(cls, params, tables, mappings):
+    def importnorgate(
+        cls,
+        params: dict,
+        tables: dict,
+        mappings: dict) -> tuple[dict, dict, dict]:
         """
         Return dictionary of price histories from Norgate Data.
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -154,15 +158,17 @@
         mappings['sector_mappings_df'] = cls._commodity_sector_mappings(
             params, mappings)
 
         return params, tables, mappings
 
 
     @staticmethod
-    def _commodity_sector_mappings(params, mappings):
+    def _commodity_sector_mappings(
+        params: dict,
+        mappings: dict) -> pd.DataFrame:
         """
         Create sector mappings DataFrame
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -206,15 +212,17 @@
 
 class YahooExtract():
     """
     Functions to extract data from Yahoo Finance
 
     """
     @staticmethod
-    def tickerextract(params, mappings):
+    def tickerextract(
+        params: dict,
+        mappings: dict) -> tuple[dict, dict]:
         """
         Extract list of S&P 500 Companies from Wikipedia.
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -232,15 +240,15 @@
         mappings : Dict
             Dictionary of sector mappings.
 
         """
 
         # Extract data from the Wikipedia SPX page
         url = 'https://en.wikipedia.org/wiki/List_of_S%26P_500_companies'
-        req = requests.get(url)
+        req = requests.get(url, timeout=10)
         html_doc = req.text
         spx_list = pd.read_html(html_doc)
 
         # the first table on the page contains the stock data
         spx_table = spx_list[0]
 
         # create a list of the tickers from the 'Symbol' column
@@ -280,15 +288,18 @@
             ['Sector', 'Industry Group', 'Industry', 'Sub-Industry',
              'Security']]
 
         return params, mappings
 
 
     @classmethod
-    def importyahoo(cls, params, tables):
+    def importyahoo(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Return dictionary of price histories from Yahoo Finance.
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -333,21 +344,23 @@
                     params['exceptions'].append(sym)
                     continue
 
         return params, tables
 
 
     @staticmethod
-    def _returndata(ticker, params):
+    def _returndata(
+        ticker: str,
+        params: dict) -> tuple[pd.DataFrame, dict]:
         """
         Create DataFrame of historic prices for specified ticker.
 
         Parameters
         ----------
-        ticker : Int
+        ticker : Str
             Stock to be returned in the form of Reuters RIC code as a
             string.
         params : Dict
             start_date : Str
                 Start Date represented as a string in the
                 format 'YYYY-MM-DD'.
             end_date : Str
@@ -395,15 +408,17 @@
 
 class MktUtils():
     """
     Various market data cleaning utilities
 
     """
     @staticmethod
-    def ticker_clean(params, tables):
+    def ticker_clean(
+        params: dict,
+        tables: dict) -> dict:
         """
         Remove tickers with incomplete history
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -436,15 +451,17 @@
             # Delete the ticker from the dictionary
             del tables['raw_ticker_dict'][ticker]
 
         return tables
 
 
     @staticmethod
-    def window_set(frame, params):
+    def window_set(
+        frame: pd.DataFrame,
+        params: dict) -> dict:
         """
         Set the correct length of the selected data
 
         Parameters
         ----------
         frame : DataFrame
             The historical prices.
@@ -469,15 +486,15 @@
                 # Set the window length to the length of the DataFrame
                 params['window'] = len(frame)
 
         return params
 
 
     @staticmethod
-    def date_set(params):
+    def date_set(params: dict) -> dict:
         """
         Create start and end dates if not supplied
 
         Parameters
         ----------
         params : Dict
             start_date : Str, optional
```

## trendvisualizer/pie_charts.py

```diff
@@ -2,24 +2,27 @@
 Display pie charts of trend strength
 
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from matplotlib import axes
 from matplotlib import font_manager as fm
-
+# pylint: disable=consider-using-f-string
 
 class PieCharts():
     """
     Summary and breakdown pie charts of trend strength
 
     """
     @staticmethod
-    def pie_summary(params, barometer):
+    def pie_summary(
+        params: dict,
+        barometer: pd.DataFrame) -> dict:
         """
         Plot pie charts for each of the 6 tenors: 10D, 20D, 30D, 50D, 100D
         and 200D for the chosen trend indicator.
 
         Parameters
         ----------
         params : Dict
@@ -172,15 +175,18 @@
                      style='italic',
                      y=1)
 
         return params
 
 
     @classmethod
-    def pie_breakdown(cls, params, tables):
+    def pie_breakdown(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Chart showing the proportions of long, short and neutral signals for a
         given indicator and tenor and the breakdown of these by sector
 
         Parameters
         ----------
         params : Dict
@@ -299,15 +305,17 @@
 
         plt.show()
 
         return params, tables
 
 
     @staticmethod
-    def _init_pie_params(params, barometer):
+    def _init_pie_params(
+        params: dict,
+        barometer: pd.DataFrame) -> dict:
 
         # Dictionary to store piechart parameters
         params['pie_params'] = {}
 
         params['pie_params']['indicator_type_ref'] = params[
             'indicator_name_dict'][params['indicator_type']][0]
 
@@ -348,15 +356,17 @@
         params['pie_params']['bottom'] = 0
         params['pie_params']['width'] = .2
 
         return params
 
 
     @staticmethod
-    def _sector_split(params, tables):
+    def _sector_split(
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
 
         # Suppress SettingWithCopyWarning caused by slicing DataFrame
         pd.options.mode.chained_assignment = None
 
         tables['sector_split'] = pd.crosstab(
             index=tables['barometer'][params['pie_params']['sector_name']],
             columns=(tables['barometer'][
@@ -410,19 +420,23 @@
         # Suppress SettingWithCopyWarning caused by slicing DataFrame
         pd.options.mode.chained_assignment = "warn"
 
         return params, tables
 
 
     @staticmethod
-    def _breakdown(axx, params, tables, direction):
+    def _breakdown(
+        axx: axes.Axes,
+        params: dict,
+        tables: dict,
+        direction: str) -> axes.Axes:
 
         ratios = params['pie_params']['ratios_'+direction]
-        for j, _ in enumerate(ratios):
-            height = ratios[j]
+        for j, value in enumerate(ratios):
+            height = value
             axx.bar(params['pie_params']['xpos'],
                     height=height,
                     width=params['pie_params']['width'],
                     edgecolor='black',
                     bottom=params['pie_params']['bottom'])
 
             params['pie_params']['ypos'] = params[
```

## trendvisualizer/trend.py

```diff
@@ -78,15 +78,15 @@
         and down-trending markets.
 
     Returns
     -------
     None.
 
     """
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
 
         # Import dictionary of default parameters
         self.default_dict = copy.deepcopy(trend_params_dict)
 
         # Import dictionary of sector mappings
         mappings = copy.deepcopy(sectmap)
 
@@ -119,15 +119,15 @@
         self.top_trends = top_trends
         self.tables = tables
         self.params = params
         self.mappings = mappings
 
 
     @staticmethod
-    def _init_params(inputs):
+    def _init_params(inputs: dict) -> dict:
         """
         Initialise parameter dictionary
         Parameters
         ----------
         inputs : Dict
             Dictionary of parameters supplied to the function.
 
@@ -145,15 +145,17 @@
             # Replace the default parameter with that provided
             params[key] = value
 
         return params
 
 
     @staticmethod
-    def prepnorgate(params, mappings):
+    def prepnorgate(
+        params: dict,
+        mappings: dict) -> tuple[dict, dict, dict]:
         """
         Create dataframes of prices, extracting data from Norgate Data.
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -192,15 +194,17 @@
         # Remove tickers with short history
         tables = MktUtils.ticker_clean(params=params, tables=tables)
 
         return params, tables, mappings
 
 
     @staticmethod
-    def prepyahoo(params, mappings):
+    def prepyahoo(
+        params: dict,
+        mappings: dict) -> tuple[dict, dict, dict]:
         """
         Create dataframes of prices, extracting data from Yahoo Finance.
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -241,15 +245,18 @@
         # Remove tickers with short history
         tables = MktUtils.ticker_clean(params=params, tables=tables)
 
         return params, tables, mappings
 
 
     @staticmethod
-    def trendcalc(params, tables, mappings):
+    def trendcalc(
+        params: dict,
+        tables: dict,
+        mappings: dict) -> dict:
         """
         Calculate the technical indicator fields and Trend Strength table
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -273,15 +280,17 @@
             params=params, ticker_dict=tables['ticker_dict'],
             sector_mappings_df=mappings['sector_mappings_df'])
 
         return tables
 
 
     @staticmethod
-    def top_trend_tickers(params, tables):
+    def top_trend_tickers(
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Prepare list of top trending securities.
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -299,15 +308,15 @@
         # Generate list of top trending securities
         top_trends, tables = TrendRank.top_trend_calc(
             tables, params)
 
         return top_trends, tables
 
 
-    def chart(self, chart_type, **kwargs):
+    def chart(self, chart_type: str, **kwargs) -> None:
         """
         Display the selcted chart of Trend Strength
 
         Parameters
         ----------
         chart_type : Str
             The typr of chart to display.
```

## trendvisualizer/trenddata.py

```diff
@@ -10,15 +10,18 @@
 class Fields():
     """
     Create trend strength fields across range of tickers
 
     """
 
     @classmethod
-    def generate_fields(cls, params, ticker_dict):
+    def generate_fields(
+        cls,
+        params: dict,
+        ticker_dict: dict) -> dict:
         """
         Create and add various trend indicators to each DataFrame in
         the dictionary of tickers
 
         Parameters
         ----------
         params : Dict
@@ -97,15 +100,19 @@
                 frame = cls._field_atr(
                     params=params, frame=frame, ticker=ticker)
 
         return ticker_dict
 
 
     @staticmethod
-    def _field_ma(params, frame, ticker):
+    def _field_ma(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor in params['ma_list']:
             try:
                 frame['MA_'+str(tenor)] = frame['Close'].rolling(
                     window=str(tenor)+'D').mean()
 
             except RuntimeWarning:
                 print("Error with "
@@ -116,15 +123,19 @@
                       + str(tenor)
                       + " consecutive days unchanged price")
 
         return frame
 
 
     @staticmethod
-    def _field_px_ma(params, frame, ticker):
+    def _field_px_ma(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor in params['price_cross_list']:
             try:
                 frame['PX_MA_'+str(tenor)+'_flag'] = np.where(
                     frame['Close'] > frame['MA_'+str(tenor)], 1, -1)
 
             except RuntimeWarning:
                 print("Error with "
@@ -135,15 +146,19 @@
                       + str(tenor)
                       + " consecutive days unchanged price")
 
         return frame
 
 
     @staticmethod
-    def _field_macd(params, frame, ticker):
+    def _field_macd(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         try:
             frame['MACD'], frame['MACD_SIGNAL'], \
                 frame['MACD_HIST'] = Indicators.MACD(
                     close=frame['Close'],
                     fast=params['macd_params'][0],
                     slow=params['macd_params'][1],
                     signal=params['macd_params'][2])
@@ -155,15 +170,19 @@
         except RuntimeWarning:
             print("Error with " + ticker + " MACD")
 
         return frame
 
 
     @staticmethod
-    def _field_adx(params, frame, ticker):
+    def _field_adx(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor in params['adx_list']:
             try:
                 frame['ADX_'+str(tenor)] = Indicators.ADX(
                     high=frame['High'],
                     low=frame['Low'],
                     close=frame['Close'],
                     time_period=tenor)
@@ -179,30 +198,38 @@
                       + str(tenor)
                       + " consecutive days unchanged price")
 
         return frame
 
 
     @staticmethod
-    def _field_ma_cross(params, frame, ticker):
+    def _field_ma_cross(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor_pair in params['ma_cross_list']:
             try:
                 frame['MA_'+str(tenor_pair[0])+'_'+str(
                     tenor_pair[1])+'_flag'] = np.where(
                         frame['MA_'+str(tenor_pair[0])] > frame[
                             'MA_'+str(tenor_pair[1])], 1, -1)
 
             except RuntimeWarning:
                 print("Error with " + ticker + " MA_"+str(tenor_pair))
 
         return frame
 
 
     @staticmethod
-    def _field_rsi(params, frame, ticker):
+    def _field_rsi(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor in params['rsi_list']:
             try:
                 frame['RSI_'+str(tenor)] = Indicators.RSI(
                     close=frame['Close'], time_period=tenor)
                 frame['RSI_'+str(tenor)+'_flag'] = np.where(
                     frame['RSI_'+str(tenor)] > 70, 1, np.where(
                         frame['RSI_'+str(tenor)] < 30, -1, 0))
@@ -215,15 +242,19 @@
                       + str(tenor)
                       + " consecutive days unchanged price")
 
         return frame
 
 
     @staticmethod
-    def _field_breakout(params, frame, ticker):
+    def _field_breakout(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor in params['breakout_list']:
             try:
                 frame['low_'+str(tenor)], frame['high_'+str(tenor)], \
                     frame['breakout_'+str(
                         tenor)+'_flag'] = Indicators.breakout(
                             high=frame['High'], low=frame['Low'],
                             time_period=tenor)
@@ -237,15 +268,19 @@
                       + str(tenor)
                       + " consecutive days unchanged price")
 
         return frame
 
 
     @staticmethod
-    def _field_atr(params, frame, ticker):
+    def _field_atr(
+        params:dict,
+        frame: pd.DataFrame,
+        ticker: str) -> pd.DataFrame:
+
         for tenor in params['atr_list']:
             try:
                 frame['ATR_'+str(tenor)] = Indicators.ATR(
                     high=frame['High'],
                     low=frame['Low'],
                     close=frame['Close'],
                     time_period=tenor)
@@ -260,15 +295,19 @@
                       + " consecutive days unchanged price")
 
         return frame
 
 
 
     @classmethod
-    def generate_trend_strength(cls, params, ticker_dict, sector_mappings_df):
+    def generate_trend_strength(
+        cls,
+        params: dict,
+        ticker_dict: dict,
+        sector_mappings_df: pd.DataFrame) -> pd.DataFrame:
         """
         Create a DataFrame showing the strength of trend for selected
         markets.
 
         Parameters
         ----------
 
@@ -356,15 +395,17 @@
         barometer = cls._barometer_sectors(
             params, barometer, sector_mappings_df)
 
         return barometer
 
 
     @staticmethod
-    def _prepframe(params, ticker_dict):
+    def _prepframe(
+        params: dict,
+        ticker_dict: dict) -> pd.DataFrame:
 
         # Create list of tickers from ticker_dict
         ticker_list = [ticker for ticker, df in ticker_dict.items()]
 
         # Convert ticker_name_dict to DataFrame
         ticker_name_df = pd.DataFrame.from_dict(
             params['ticker_name_dict'], orient='index', columns=['Long_name'])
@@ -383,15 +424,15 @@
                                       if col != frame.columns[-1]]
         frame = frame[cols]
 
         return frame
 
 
     @staticmethod
-    def _col_color(row):
+    def _col_color(row: pd.Series) -> pd.Series:
 
         # Create trend strength color column and absolute strength column
         row['Absolute Trend Strength'] = np.abs(row['Trend Strength'])
 
         if np.abs(row['Trend Strength']) < 5:
             row['Trend Color'] = 'red'
 
@@ -401,15 +442,18 @@
         else:
             row['Trend Color'] = 'green'
 
         return row
 
 
     @staticmethod
-    def _barometer_sectors(params, barometer, sector_mappings_df):
+    def _barometer_sectors(
+        params: dict,
+        barometer: pd.DataFrame,
+        sector_mappings_df: pd.DataFrame) -> pd.DataFrame:
         """
         Add sector mappings to the trend barometer table to use in summary
         graph
 
         Parameters
         ----------
         params : Dict
@@ -454,15 +498,17 @@
 class TrendRank():
     """
     Generate list of strongly trending securities
 
     """
 
     @staticmethod
-    def futures_split(tables, params):
+    def futures_split(
+        tables: dict,
+        params: dict) -> dict:
         """
         Split the futures from the rest of the norgate data (choosing
         backadjusted data or not)
 
         Parameters
         ----------
         tables : Dict
@@ -493,15 +539,18 @@
             tables['futures_barometer'] = tables['barometer'][
                 tables['barometer']['Ticker'].str.lower().str.startswith('c_')]
 
         return tables
 
 
     @classmethod
-    def top_trend_calc(cls, tables, params):
+    def top_trend_calc(
+        cls,
+        tables: dict,
+        params: dict) -> tuple[dict, dict]:
         """
         Prepare list of top trending securities.
 
         Parameters
         ----------
         barometer : DataFrame
             DataFrame showing trend strength for each ticker.
@@ -544,15 +593,18 @@
             if rank < params['top_trend_params']['final_size'] + 1:
                 top_trends['top_ticker_list'].append(ticker)
 
         return top_trends, tables
 
 
     @classmethod
-    def _filter_barometer(cls, tables, params):
+    def _filter_barometer(
+        cls,
+        tables: dict,
+        params: dict) -> pd.DataFrame:
         """
         Sort and filter the top trending securities
 
         Parameters
         ----------
         barometer : DataFrame
             DataFrame showing trend strength for each ticker.
@@ -606,8 +658,7 @@
                 filtered_barometer = pd.concat([filtered_barometer, frame])
 
         filtered_barometer = filtered_barometer.sort_values(
             by=['Absolute Trend Strength'],
             ascending=False).reset_index().drop(['index'], axis=1)
 
         return filtered_barometer
-
```

## Comparing `trendvisualizer-0.5.8.dist-info/LICENSE` & `trendvisualizer-0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

