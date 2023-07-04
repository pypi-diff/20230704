# Comparing `tmp/volvisualizer-1.1.3-py3-none-any.whl.zip` & `tmp/volvisualizer-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 27397 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-25 19:00 volvisualizer/__init__.py
--rw-rw-rw-  2.0 fat    26576 b- defN 22-Mar-16 10:04 volvisualizer/graph.py
--rw-rw-rw-  2.0 fat    11866 b- defN 23-Jun-14 14:40 volvisualizer/market_data.py
--rw-rw-rw-  2.0 fat    26180 b- defN 23-Jun-25 18:28 volvisualizer/market_data_prep.py
--rw-rw-rw-  2.0 fat     2857 b- defN 22-Mar-16 09:22 volvisualizer/utils.py
--rw-rw-rw-  2.0 fat    30001 b- defN 22-Mar-15 16:13 volvisualizer/vol_methods.py
--rw-rw-rw-  2.0 fat    13496 b- defN 22-Mar-16 09:22 volvisualizer/volatility.py
+Zip file size: 27912 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-04 09:00 volvisualizer/__init__.py
+-rw-rw-rw-  2.0 fat    27501 b- defN 23-Jun-29 15:34 volvisualizer/graph.py
+-rw-rw-rw-  2.0 fat    12096 b- defN 23-Jun-29 14:22 volvisualizer/market_data.py
+-rw-rw-rw-  2.0 fat    27175 b- defN 23-Jul-04 08:59 volvisualizer/market_data_prep.py
+-rw-rw-rw-  2.0 fat     2948 b- defN 23-Jun-29 14:24 volvisualizer/utils.py
+-rw-rw-rw-  2.0 fat    30755 b- defN 23-Jun-29 15:10 volvisualizer/vol_methods.py
+-rw-rw-rw-  2.0 fat    13614 b- defN 23-Jun-29 15:07 volvisualizer/volatility.py
 -rw-rw-rw-  2.0 fat     3914 b- defN 23-Jun-14 14:38 volvisualizer/volatility_params.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      727 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1093 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/RECORD
-13 files, 117928 bytes uncompressed, 25571 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-04 09:15 volvisualizer-1.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Jul-04 09:15 volvisualizer-1.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 09:15 volvisualizer-1.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-04 09:15 volvisualizer-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1093 b- defN 23-Jul-04 09:15 volvisualizer-1.1.6.dist-info/RECORD
+13 files, 121041 bytes uncompressed, 26086 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: volvisualizer/volatility.py
 Comment: 
 
 Filename: volvisualizer/volatility_params.py
 Comment: 
 
-Filename: volvisualizer-1.1.3.dist-info/LICENSE
+Filename: volvisualizer-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: volvisualizer-1.1.3.dist-info/METADATA
+Filename: volvisualizer-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: volvisualizer-1.1.3.dist-info/WHEEL
+Filename: volvisualizer-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: volvisualizer-1.1.3.dist-info/top_level.txt
+Filename: volvisualizer-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: volvisualizer-1.1.3.dist-info/RECORD
+Filename: volvisualizer-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## volvisualizer/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.3"
+__version__ = "1.1.6"
```

## volvisualizer/graph.py

```diff
@@ -1,31 +1,36 @@
 """
 Methods for graphing volatility data
 
 """
 import copy
 import os
 import warnings
+import matplotlib.figure as mplfig
 import matplotlib.pyplot as plt
 import numpy as np
 import plotly.graph_objects as go
 import scipy as sp
+from matplotlib import axes
 from mpl_toolkits.mplot3d import Axes3D # pylint: disable=unused-import
 from plotly.offline import plot
 from scipy.interpolate import griddata
 from volvisualizer.vol_methods import VolMethods
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name, consider-using-f-string
 
 class Graph():
     """
     Methods for graphing volatility data
 
     """
     @classmethod
-    def line_graph(cls, params, tables):
+    def line_graph(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Displays a linegraph of each option maturity plotted by strike
         and implied vol
 
         Parameters
         ----------
         voltype : Str
@@ -116,15 +121,18 @@
             # save the image as a png file
             fig = cls._image_save(params=params, fig=fig)
 
         return params, tables
 
 
     @classmethod
-    def scatter_3d(cls, params, tables):
+    def scatter_3d(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Displays a 3D scatter plot of each option implied vol against
         strike and maturity
 
         Parameters
         ----------
         voltype : Str
@@ -174,15 +182,18 @@
             # save the image as a png file
             fig = cls._image_save(params=params, fig=fig)
 
         return params, tables
 
 
     @classmethod
-    def surface_3d(cls, params, tables):
+    def surface_3d(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Displays a 3D surface plot of the implied vol surface against
         strike and maturity
 
         Parameters
         ----------
         surfacetype : Str
@@ -301,15 +312,15 @@
         # Set warnings back to default
         warnings.filterwarnings("default", category=UserWarning)
 
         return params, tables
 
 
     @classmethod
-    def _trisurf_graph(cls, params):
+    def _trisurf_graph(cls, params: dict) -> mplfig.Figure:
 
         # Create figure and axis objects and format
         fig, ax = cls._graph_format(params=params)
 
         # Display triangular surface plot, using colormap 'viridis'
         ax.plot_trisurf(params['x'],
                         params['y'],
@@ -317,15 +328,15 @@
                         cmap='viridis',
                         edgecolor='none')
 
         return fig
 
 
     @classmethod
-    def _mesh_graph(cls, params):
+    def _mesh_graph(cls, params: dict) -> mplfig.Figure:
 
         # Create arrays across x and y-axes of equally spaced points
         # from min to max values
         x1, y1 = np.meshgrid(
             np.linspace(min(params['x']),
                         max(params['x']),
                         int(params['spacegrain'])),
@@ -351,15 +362,18 @@
 
         plt.show()
 
         return fig
 
 
     @classmethod
-    def _spline_graph(cls, params, tables):
+    def _spline_graph(
+        cls,
+        params: dict,
+        tables: dict) -> mplfig.Figure:
 
         # Create arrays across x and y-axes of equally spaced points
         # from min to max values
         x1 = np.linspace(min(params['x']),
                          max(params['x']),
                          int(params['spacegrain']))
         y1 = np.linspace(min(params['y']),
@@ -396,15 +410,18 @@
             params['z'] = tables['data_3D'][str(
                 params['vols_dict'][str(params['voltype'])])] * 100
             ax.scatter3D(params['x'], params['y'], params['z'], c='r')
 
         return fig
 
     @classmethod
-    def _interactive_graph(cls, params, tables):
+    def _interactive_graph(
+        cls,
+        params: dict,
+        tables: dict) -> go.Figure:
 
         params = cls._set_contours(params=params, tables=tables)
 
         # Specify the 3 axis values
         params['x'] = tables['data_3D']['TTM'] * 365
         params['y'] = tables['data_3D']['Strike']
         params['z'] = tables['data_3D']['Graph Vol'] * 100
@@ -465,15 +482,17 @@
         else:
             plot(fig, auto_open=True)
 
         return fig
 
 
     @staticmethod
-    def _set_contours(params, tables):
+    def _set_contours(
+        params: dict,
+        tables: dict) -> dict:
 
         # Set the range of x, y and z contours and interval
         params['contour_x_start'] = 0
         params['contour_x_stop'] = 2 * 360
         params['contour_x_size'] = params['contour_x_stop'] / 18
         params['contour_y_start'] = tables['data_3D']['Strike'].min()
         params['contour_y_stop'] = tables['data_3D']['Strike'].max()
@@ -499,15 +518,17 @@
         params['contour_z_stop'] = 100
         params['contour_z_size'] = 5
 
         return params
 
 
     @staticmethod
-    def _int_scatter(params, tables):
+    def _int_scatter(
+        params: dict,
+        tables: dict) -> go.Figure:
 
         # Set z to raw data points
         params['z'] = (tables['data_3D'][str(
             params['vols_dict'][str(params['voltype'])])] * 100)
 
         # Create figure object with fitted surface and scatter
         # points
@@ -551,45 +572,45 @@
                 # Plot scatter of unsmoothed data
                 go.Scatter3d(
                     x=params['x'],
                     y=params['y'],
                     z=params['z'],
                     mode='markers',
                     # Set size, color and opacity of each data point
-                    marker=dict(
-                        size=2,
-                        color='red',
-                        opacity=0.9
-                        )
+                    marker={
+                        'size':2,
+                        'color':'red',
+                        'opacity':0.9
+                        }
                     )
                 ])
 
         # Plot just the scatter points
         else:
             fig = go.Figure(data=[
                 # Plot scatter of unsmoothed data
                 go.Scatter3d(
                     x=params['x'],
                     y=params['y'],
                     z=params['z'],
                     mode='markers',
                     # Set size, color and opacity of each data point
-                    marker=dict(
-                        size=2,
-                        color='red',
-                        opacity=0.9
-                        )
+                    marker={
+                        'size':2,
+                        'color':'red',
+                        'opacity':0.9
+                        }
                     )
                 ])
 
         return fig
 
 
     @staticmethod
-    def _int_surf(params):
+    def _int_surf(params: dict) -> go.Figure:
 
         # Create figure object with fitted surface
         fig = go.Figure(
             data=[go.Surface(
                 x=params['x2'],
                 y=params['y2'],
                 z=params['z2'],
@@ -624,78 +645,90 @@
                    # Set the surface opacity
                    opacity=params['opacity'])])
 
         return fig
 
 
     @staticmethod
-    def _int_layout(params, fig):
+    def _int_layout(
+        params: dict,
+        fig: go.Figure) -> go.Figure:
 
         # Set initial camera angle
-        params['camera'] = dict(
-            eye=dict(x=2, y=1, z=1)
-        )
+        params['camera'] = {
+            'eye': {
+                'x':2,
+                'y':1,
+                'z':1
+                }
+            }
 
         # Set Time To Expiration to increase left to right
         fig.update_scenes(xaxis_autorange="reversed")
         fig.update_layout(
-            scene = dict(
-                xaxis = dict(
-                    backgroundcolor="rgb(200, 200, 230)",
-                    gridcolor="white",
-                    showbackground=True,
-                    zerolinecolor="white"
-                    ),
-                yaxis = dict(
-                    backgroundcolor="rgb(230, 200,230)",
-                    gridcolor="white",
-                    showbackground=True,
-                    zerolinecolor="white"
-                    ),
-                zaxis = dict(
-                    backgroundcolor="rgb(230, 230,200)",
-                    gridcolor="white",
-                    showbackground=True,
-                    zerolinecolor="white"
-                    ),
-                aspectmode='cube',
+            scene={
+                'xaxis': {
+                    'backgroundcolor': "rgb(200, 200, 230)",
+                    'gridcolor': "white",
+                    'showbackground': True,
+                    'zerolinecolor': "white"
+                    },
+                'yaxis': {
+                    'backgroundcolor': "rgb(230, 200,230)",
+                    'gridcolor': "white",
+                    'showbackground': True,
+                    'zerolinecolor': "white"
+                    },
+                'zaxis': {
+                    'backgroundcolor': "rgb(230, 230,200)",
+                    'gridcolor': "white",
+                    'showbackground': True,
+                    'zerolinecolor': "white"
+                    },
+                'aspectmode': 'cube',
                 # Label axes
-                xaxis_title='Time to Expiration (Days)',
-                yaxis_title='Strike',
-                zaxis_title='Implied Volatility %',),
+                'xaxis_title': 'Time to Expiration (Days)',
+                'yaxis_title': 'Strike',
+                'zaxis_title': 'Implied Volatility %'
+                },
             # Specify title with ticker label, voltype
             # and date
             title={
                 'text':(
                     str(params['ticker_label'])
                     +' Implied Volatility '
                     +str(params['voltype'].title())
                     +' Price '
                     +str(params['start_date'])
                     ),
                 'y':0.9,
                 'x':0.5,
                 'xanchor':'center',
                 'yanchor':'top',
-                'font':dict(
-                    size=20,
-                    color="black"
-                    )
+                'font': {
+                    'size': 20,
+                    'color': "black"
+                    }
                 },
             autosize=False,
             width=800,
             height=800,
-            margin=dict(l=65, r=50, b=65, t=90),
+            margin={
+                'l':65,
+                'r':50,
+                'b':65,
+                't':90
+                },
             scene_camera=params['camera'])
 
         return fig
 
 
     @staticmethod
-    def _graph_format(params):
+    def _graph_format(params: dict) -> tuple[mplfig.Figure, axes.Axes]:
 
         # Update chart parameters
         plt.rcParams.update(params['mpl_3D_params'])
 
         # Create fig object
         fig = plt.figure(figsize=params['fig_size'])
 
@@ -748,15 +781,17 @@
         st.set_y(0.95)
         fig.subplots_adjust(top=1)
 
         return fig, ax
 
 
     @staticmethod
-    def _image_save(params, fig):
+    def _image_save(
+        params: dict,
+        fig: mplfig.Figure | go.Figure) -> mplfig.Figure | go.Figure:
 
         # Create image folder if it does not already exist
         if not os.path.exists(params['image_folder']):
             os.makedirs(params['image_folder'])
 
         # save the image as a png file
         plt.savefig('{}/{}{}.png'.format(
```

## volvisualizer/market_data.py

```diff
@@ -16,15 +16,18 @@
 
 class Data():
     """
     Market data import and transformation functions
 
     """
     @classmethod
-    def create_option_data(cls, params, tables):
+    def create_option_data(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Extract the URL for each of the listed option on Yahoo Finance
         for the given ticker. Extract option data from each URL.
 
         Filter / transform the data and calculate implied volatilities for
         specified put and call strikes.
 
@@ -97,15 +100,18 @@
         params, tables = DataPrep.combine(params=params, tables=tables)
         print("Data combined")
 
         return params, tables
 
 
     @classmethod
-    def extractoptions(cls, params, tables):
+    def extractoptions(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Extract the URL for each of the listed option on Yahoo Finance
         for the given ticker. Extract option data from each URL.
 
 
         Parameters
         ----------
@@ -139,15 +145,15 @@
 
         params, tables = cls._process_options(params=params, tables=tables)
 
         return params, tables
 
 
     @staticmethod
-    def _extracturls(params):
+    def _extracturls(params: dict) -> dict:
         """
         Extract the URL for each of the listed option on Yahoo Finance
         for the given ticker.
 
         Parameters
         ----------
         ticker : Str
@@ -203,15 +209,15 @@
                 'https://finance.yahoo.com/quote/'
                 +params['ticker']+'/options?date='+page)
 
         return params
 
 
     @staticmethod
-    def _extract_web_data(params):
+    def _extract_web_data(params: dict) -> dict:
 
         # Create an empty dictionary
         raw_web_data = {}
 
         # each url needs to have an option expiry date associated with
         # it in the url dict
         for input_date, url in params['url_dict'].items():
@@ -230,15 +236,15 @@
                 print("Problem with "+input_date+" data")
                 time.sleep(5)
 
         return raw_web_data
 
 
     @staticmethod
-    def _read_web_data(params):
+    def _read_web_data(params: dict) -> dict:
 
         # Create an empty dictionary
         params['option_dict'] = {}
         params['url_except_dict'] = {}
 
         for input_date, url in params['url_dict'].items():
             # if data exists
@@ -254,15 +260,17 @@
             except ValueError:
                 params['url_except_dict'][input_date] = url
 
         return params
 
 
     @staticmethod
-    def _process_options(params, tables):
+    def _process_options(
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
 
         # Create list to store exceptions
         params['opt_except_list'] = []
 
         # For each of these dates
         for input_date in params['date_list']:
 
@@ -318,15 +326,15 @@
                 except IndexError:
                     params['opt_except_list'].append(input_date)
 
         return params, tables
 
 
     @staticmethod
-    def trading_calendar(params):
+    def trading_calendar(params: dict) -> dict:
         """
         Generate list of trading holidays
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
```

## volvisualizer/market_data_prep.py

```diff
@@ -39,41 +39,45 @@
     }
     user_agent = random.choice(USER_AGENTS)
     request_headers["User-Agent"] = user_agent
 
     def __init__(self):
         self._session = requests
 
-    def open(self, url):
+    def open(self, url: str) -> requests.models.Response:
         """
         Extract data from Yahoo Finance URL
 
         Parameters
         ----------
         url : Str
             The URL to extract data from.
 
         Returns
         -------
         response : Response object
             Response object of requests module.
 
         """
-        response = self._session.get(url=url, headers=self.request_headers)
-        
+        response = self._session.get(
+            url=url, headers=self.request_headers, timeout=10)
+
         return response
 
 
 class DataPrep():
     """
     Market data transformation and combination functions
 
     """
     @classmethod
-    def transform(cls, params, tables):
+    def transform(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Perform some filtering / transforming of the option data
 
         Parameters
         ----------
         start_date : Str
             Date from when to include prices (some of the options
@@ -150,15 +154,15 @@
 
         params, tables = cls._filters(params=params, tables=tables)
 
         return params, tables
 
 
     @staticmethod
-    def _trade_columns(tables):
+    def _trade_columns(tables: dict) -> dict:
 
         # Create a column of the Trade Day
         tables['data']['Last Trade Day'] = (
             tables['data']['Last Trade Date'].dt.date)
 
         # Create a column of the Trade Time of Day
         tables['data']['Last Trade Time'] = (
@@ -192,15 +196,18 @@
         tables['data']['Mid'] = (
             tables['data']['Ask'] + tables['data']['Bid']) / 2
 
         return tables
 
 
     @classmethod
-    def _filters(cls, params, tables):
+    def _filters(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
 
         # If a minutes parameter is supplied, filter for most recent
         # minutes
         if params['lastmins'] is not None:
             tables['data'] = (tables['data'][tables['data']['Unixtime']  >= (
                 max(tables['data']['Unixtime']) - params['lastmins'] * 60)])
 
@@ -231,15 +238,17 @@
 
         params, tables = cls._monthlies(params=params, tables=tables)
 
         return params, tables
 
 
     @staticmethod
-    def _minopts(params, data):
+    def _minopts(
+        params: dict,
+        data: pd.DataFrame) -> pd.DataFrame:
         # Create a dictionary of the number of options for each
         # maturity
         mat_dict = dict(Counter(data['Days']))
         for ttm, count in mat_dict.items():
 
             # if there are less than minopts options for a given
             # maturity
@@ -249,15 +258,17 @@
                 data = (
                     data[data['Days'] != ttm])
 
         return data
 
 
     @staticmethod
-    def _monthlies(params, tables):
+    def _monthlies(
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
 
         # If the monthlies flag is set
         if params['monthlies'] is True:
 
             # Create an empty list
             date_list = []
 
@@ -308,15 +319,18 @@
                         tables['data'][tables['data']['Days']
                                        != days_to_expiry])
 
         return params, tables
 
 
     @classmethod
-    def combine(cls, params, tables):
+    def combine(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Calculate implied volatilities for specified put and call
         strikes and combine.
 
         Parameters
         ----------
         ticker_label : Str
@@ -411,15 +425,18 @@
             tables['imp_vol_data'] = cls._minopts(
                 params=params, data=tables['imp_vol_data'])
 
         return params, tables
 
 
     @classmethod
-    def _create_strike_range(cls, params, tables):
+    def _create_strike_range(
+        cls,
+        params: dict,
+        tables: dict) -> dict:
 
         # Extract the spot level from the html data
         if params['spot'] is None:
             tree = html.fromstring(params['html_doc'])
             priceparse = tree.xpath(
                 '//fin-streamer[@class="Fw(b) Fz(36px) Mb(-4px) D(ib)"]/text()')
             params['spot'] = float(
@@ -458,15 +475,17 @@
                     int((params['call_max'] - params['roundspot'])
                         / params['divisor']) + 1))
 
         return params
 
 
     @staticmethod
-    def _strike_filters(params, divisor):
+    def _strike_filters(
+        params: dict,
+        divisor: float) -> tuple[float, float, float]:
 
         # Calculate the point to switch from put to call options
         roundspot = (
             round(params['spot'] / divisor) * divisor)
 
         put_min = (
             round(params['spot'] * params['strike_limits'][0] / divisor)
@@ -476,15 +495,17 @@
             round(params['spot'] * params['strike_limits'][1] / divisor)
             * divisor)
 
         return roundspot, put_min, call_max
 
 
     @staticmethod
-    def _create_divisor(params, tables):
+    def _create_divisor(
+        params: dict,
+        tables: dict) -> dict:
 
         # Take the set of all the option strikes in the data
         strikes = set(tables['data']['Strike'])
 
         # Find the number of options with a remainder of zero for each of the
         # listed potential divisors
         avail_strikes = {}
@@ -500,15 +521,20 @@
              for divisor, strike_count in avail_strikes.items()
              if strike_count == max_strike_count])
 
         return params
 
 
     @classmethod
-    def _imp_vol_apply(cls, params, input_data, strike, option):
+    def _imp_vol_apply(
+        cls,
+        params: dict,
+        input_data: pd.DataFrame,
+        strike: float,
+        option: str) -> pd.DataFrame:
         """
         Apply _implied_vol_by_row method to each row of a DataFrame.
 
         Parameters
         ----------
         input_data : DataFrame
             DataFrame of Option prices.
@@ -544,15 +570,20 @@
         input_data = input_data.apply(
             lambda x: cls._imp_vol_by_row(x, params, strike, option), axis=1)
 
         return input_data
 
 
     @classmethod
-    def _imp_vol_by_row(cls, row, params, strike, option):
+    def _imp_vol_by_row(
+        cls,
+        row: pd.Series,
+        params: dict,
+        strike: float,
+        option: str) -> pd.Series:
         """
         Calculate implied vol for one row of a DataFrame.
 
         Parameters
         ----------
         row : Array
             Each row in the DataFrame.
@@ -626,15 +657,18 @@
         # Return warnings to default setting
         warnings.filterwarnings("default", category=RuntimeWarning)
 
         return row
 
 
     @classmethod
-    def interest_rate(cls, ttm, yield_curve=None):
+    def interest_rate(
+        cls,
+        ttm: int,
+        yield_curve: interpolate.interp1d | None = None) -> float:
         """
         Returns the interest rate for a given number of days to maturity
 
         Parameters
         ----------
         ttm : Int
             Number of days to maturity.
@@ -651,15 +685,15 @@
         if yield_curve is None:
             yield_curve = cls.generate_yield_curve()
 
         return np.round(float(yield_curve(ttm))/100, 5)
 
 
     @staticmethod
-    def generate_yield_curve(r=None):
+    def generate_yield_curve(r: float | None = None) -> interpolate.interp1d:
         """
         Returns a yield curve interpolation function
 
         Parameters
         ----------
         r : Float, optional
             If a single interest rate is supplied, the method will calculate a
@@ -724,15 +758,15 @@
         # Create a curve using cubic spline interpolation
         yield_curve = interpolate.interp1d(tenors, rates, kind='cubic')
 
         return yield_curve
 
 
     @classmethod
-    def dividend_yield(cls, ticker):
+    def dividend_yield(cls, ticker: str) -> float:
         """
         Returns the dividend yield for a given ticker
 
         Parameters
         ----------
         ticker : Str
             The underlying to calculate dividend yield for.
@@ -751,44 +785,47 @@
             except ValueError:
                 print("No dividend data for SPX")
                 div_yield = '0.0%'
         else:
             try:
                 div_yield = cls._stock_dividend_yield(ticker)
             except ValueError:
-                print("No dividend data for "+ticker)
+                print("No dividend data for "+ticker+" - Empty string")
+                div_yield = '0.0%'
+            except IndexError:
+                print("No dividend data for "+ticker+" - Invalid index")
                 div_yield = '0.0%'
 
-        try: 
+        try:
             result = np.round(float(div_yield.rstrip('%'))/100, 5)
         except ValueError:
             print("No valid dividend data for "+ticker)
             result = 0.0
 
         return result
 
 
     @staticmethod
-    def _stock_dividend_yield(ticker):
+    def _stock_dividend_yield(ticker: str) -> str:
 
         url = 'https://stockanalysis.com/stocks/'+ticker+'/dividend/'
 
-        r = requests.get(url)
+        r = requests.get(url, timeout=10)
 
         html_doc = r.text
 
         tree = html.fromstring(html_doc)
-        
+
         parse = tree.xpath("//*[contains(text(), 'Dividend Yield')]/div/text()")
 
         return [str(p) for p in parse][0].replace('\n','')
 
 
     @staticmethod
-    def _spx_div_yield():
+    def _spx_div_yield() -> str:
 
         url = 'https://www.multpl.com/s-p-500-dividend-yield'
 
         urlopener = UrlOpener()
         response = urlopener.open(url)
 
         html_doc = response.text
```

## volvisualizer/utils.py

```diff
@@ -12,15 +12,15 @@
 
 class Utils():
     """
     Utility functions for refreshing parameters
 
     """
     @classmethod
-    def init_params(cls, inputs):
+    def init_params(cls, inputs: dict) -> dict:
         """
         Initialise parameter dictionary
         Parameters
         ----------
         inputs : Dict
             Dictionary of parameters supplied to the function.
         Returns
@@ -47,15 +47,15 @@
 
         params = cls.set_start_date(params=params)
 
         return params
 
 
     @staticmethod
-    def set_start_date(params):
+    def set_start_date(params: dict) -> dict:
         """
         Set start date to previous working day if not provided
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -70,15 +70,17 @@
             start_date_as_dt = (dt.datetime.today() - BDay(1)).date()
             params['start_date'] = str(start_date_as_dt)
 
         return params
 
 
     @staticmethod
-    def set_interest_rate(params, r=None):
+    def set_interest_rate(
+        params: dict,
+        r: float | None = None) -> dict:
         """
         Returns the yield curve interpolation function
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
@@ -93,15 +95,15 @@
         """
         params['yield_curve'] = DataPrep.generate_yield_curve(r=r)
 
         return params
 
 
     @staticmethod
-    def set_dividend_yield(params):
+    def set_dividend_yield(params: dict) -> dict:
         """
         Returns the dividend yield
 
         Parameters
         ----------
         params : Dict
             Dictionary of key parameters.
```

## volvisualizer/vol_methods.py

```diff
@@ -6,24 +6,25 @@
 import copy
 from decimal import Decimal
 import datetime as dt
 from dateutil.relativedelta import relativedelta
 import numpy as np
 import pandas as pd
 import scipy as sp
+import scipy.interpolate as inter
 import scipy.stats as si
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name, consider-using-f-string
 
 class ImpliedVol():
     """
     Implied Volatility Extraction methods
 
     """
     @classmethod
-    def implied_vol_newton_raphson(cls, opt_params):
+    def implied_vol_newton_raphson(cls, opt_params: dict) -> float | str:
         """
         Finds implied volatility using Newton-Raphson method - needs
         knowledge of partial derivative of option pricing formula
         with respect to volatility (vega)
 
         Parameters
         ----------
@@ -91,15 +92,15 @@
         else:
             result = 'NA'
 
         return result
 
 
     @classmethod
-    def implied_vol_bisection(cls, opt_params):
+    def implied_vol_bisection(cls, opt_params: dict) -> float | str:
         """
         Finds implied volatility using bisection method.
 
         Parameters
         ----------
         S : Float
             Stock Price. The default is 100.
@@ -176,15 +177,15 @@
 
         result = opt_params['vi']
 
         return result
 
 
     @classmethod
-    def implied_vol_naive(cls, opt_params):
+    def implied_vol_naive(cls, opt_params: dict) -> float:
         """
         Finds implied volatility using simple naive iteration,
         increasing precision each time the difference changes sign.
 
         Parameters
         ----------
         S : Float
@@ -260,15 +261,15 @@
 
         result = opt_params['vi']
 
         return result
 
 
     @classmethod
-    def implied_vol_naive_verbose(cls, opt_params):
+    def implied_vol_naive_verbose(cls, opt_params: dict) -> float:
         """
         Finds implied volatility using simple naive iteration,
         increasing precision each time the difference changes sign.
 
         Parameters
         ----------
         S : Float
@@ -349,15 +350,17 @@
 
         result = opt_params['vi']
 
         return result
 
 
     @staticmethod
-    def black_scholes_merton(opt_params, sigma):
+    def black_scholes_merton(
+        opt_params: dict,
+        sigma: float) -> float:
         """
         Black-Scholes-Merton Option price
 
         Parameters
         ----------
         S : Float
             Stock Price. The default is 100.
@@ -418,15 +421,17 @@
         else:
             print("Please supply a value for option - 'put' or 'call'")
 
         return opt_price
 
 
     @staticmethod
-    def black_scholes_merton_vega(opt_params, sigma):
+    def black_scholes_merton_vega(
+        opt_params: dict,
+        sigma: float) -> float:
         """
         Black-Scholes-Merton Option Vega
 
         Parameters
         ----------
         S : Float
             Stock Price. The default is 100.
@@ -468,15 +473,18 @@
 
 class VolMethods():
     """
     Methods for extracting Implied Vol and producing skew reports
 
     """
     @classmethod
-    def smooth(cls, params, tables):
+    def smooth(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[dict, dict]:
         """
         Create a column of smoothed implied vols
 
         Parameters
         ----------
         order : Int
             Polynomial order used in numpy polyfit function. The
@@ -565,15 +573,17 @@
             tables['imp_vol_data_smoothed'].apply(
                 lambda x: cls._vol_map(x, tables), axis=1))
 
         return params, tables
 
 
     @staticmethod
-    def _vol_map(row, tables):
+    def _vol_map(
+        row: pd.Series,
+        tables: dict) -> pd.Series:
         """
         Map value calculated in smooth surface DataFrame to
         'Smoothed Vol' column.
 
         Parameters
         ----------
         row : Array
@@ -588,15 +598,18 @@
         row['Smoothed Vol'] = (
             tables['smooth_surf'].loc[row['Strike'], str(row['Days'])])
 
         return row
 
 
     @classmethod
-    def map_vols(cls, params, tables):
+    def map_vols(
+        cls,
+        params: dict,
+        tables: dict) -> tuple[inter._rbf.Rbf, inter._rbf.Rbf]:
         """
         Create vol surface mapping function
 
         Parameters
         ----------
         tables : Dict
             Dictionary containing the market data tables.
@@ -629,15 +642,19 @@
             smooth=5,
             epsilon=5)
 
         return vol_surface, vol_surface_smoothed
 
 
     @staticmethod
-    def get_vol(maturity, strike, params, surface_models):
+    def get_vol(
+        maturity: str,
+        strike: int,
+        params: dict,
+        surface_models: dict) -> float:
         """
         Return implied vol for a given maturity and strike
 
         Parameters
         ----------
         maturity : Str
             The date for the option maturity, expressed as 'YYYY-MM-DD'.
@@ -660,15 +677,18 @@
         else:
             imp_vol = surface_models['vol_surface'](strike_level, ttm)
 
         return np.round(imp_vol, 2)
 
 
     @classmethod
-    def create_vol_dict(cls, params, surface_models):
+    def create_vol_dict(
+        cls,
+        params: dict,
+        surface_models: dict) -> dict:
         """
         Create dictionary of implied vols by tenor and strike to use in skew
         report
 
         Parameters
         ----------
         params : Dict
@@ -692,15 +712,18 @@
                     maturity=maturity, strike=strike, params=params,
                     surface_models=surface_models)
 
         return vol_dict
 
 
     @classmethod
-    def print_skew_report(cls, vol_dict, params):
+    def print_skew_report(
+        cls,
+        vol_dict: dict,
+        params: dict) -> None:
         """
         Print a report showing implied vols for 80%, 90% and ATM strikes and
         selected tenor length
 
         Parameters
         ----------
         vol_dict : Dict
@@ -725,15 +748,15 @@
                 cls._upside_skew(vol_dict=vol_dict, params=params, dp2=dp2)
 
             else:
                 cls._downside_skew(vol_dict=vol_dict, params=params, dp2=dp2)
 
 
     @staticmethod
-    def _header(params):
+    def _header(params: dict) -> None:
 
         print('='*78)
         print(': {:^74} :'.format('Skew Summary'))
         print('-'*78)
 
         # Contract traded on left and period covered on right
         print(': Underlying Ticker : {:<19}{} : {} :'.format(
@@ -768,15 +791,18 @@
                 '90%',
                 'ATM',
                 '-10% Skew',
                 '-20% Skew'))
 
 
     @staticmethod
-    def _downside_skew(vol_dict, params, dp2):
+    def _downside_skew(
+        vol_dict: dict,
+        params: dict,
+        dp2: Decimal) -> None:
 
         # Monthly skew summary for selected number of months
         for month in range(1, params['skew_months'] + 1):
             if month < 10:
                 month_label = ' '+str(month)
             else:
                 month_label = str(month)
@@ -792,15 +818,18 @@
                          - vol_dict[(month, 100)]) / 20).quantize(dp2)))
 
         print('-'*78)
         print('='*78)
 
 
     @staticmethod
-    def _upside_skew(vol_dict, params, dp2):
+    def _upside_skew(
+        vol_dict: dict,
+        params: dict,
+        dp2: Decimal) -> None:
 
         # Monthly skew summary for selected number of months
         for month in range(1, params['skew_months'] + 1):
             if month < 10:
                 month_label = ' '+str(month)
             else:
                 month_label = str(month)
@@ -816,15 +845,18 @@
                          - vol_dict[(month, 100)]) / 20).quantize(dp2)))
 
         print('-'*78)
         print('='*78)
 
 
     @staticmethod
-    def _full_skew(vol_dict, params, dp2):
+    def _full_skew(
+        vol_dict: dict,
+        params: dict,
+        dp2: Decimal) -> None:
 
         print('='*115)
         print(': {:^111} :'.format('Skew Summary'))
         print('-'*115)
 
         # Contract traded on left and period covered on right
         print(': Underlying Ticker : {:<56}{} : {} :'.format(
```

## volvisualizer/volatility.py

```diff
@@ -335,15 +335,19 @@
             # Replace the default parameter with that provided
             self.params[key] = value
 
         self.params, self.tables = Graph.surface_3d(
             params=self.params, tables=self.tables)
 
 
-    def vol(self, maturity, strike, smoothing=None):
+    def vol(
+        self,
+        maturity: str,
+        strike: int,
+        smoothing: bool | None = None):
         """
         Return implied vol for a given maturity and strike
 
         Parameters
         ----------
         maturity : Str
             The date for the option maturity, expressed as 'YYYY-MM-DD'.
@@ -360,15 +364,18 @@
             self.params['smoothing'] = smoothing
 
         return VolMethods.get_vol(
             maturity=maturity, strike=strike, params=self.params,
             surface_models=self.surface_models)
 
 
-    def skewreport(self, months=None, direction=None):
+    def skewreport(
+        self,
+        months: int | None = None,
+        direction: str | None = None):
         """
         Print a report showing implied vols for 80%, 90% and ATM strikes and
         selected tenor length
 
         Parameters
         ----------
         months : Int
```

## Comparing `volvisualizer-1.1.3.dist-info/LICENSE` & `volvisualizer-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `volvisualizer-1.1.3.dist-info/METADATA` & `volvisualizer-1.1.6.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvisualizer
-Version: 1.1.3
+Version: 1.1.6
 Summary: Extract and visualize implied volatility from option data.
 Home-page: https://github.com/GBERESEARCH/volvisualizer
 Author: GBERESEARCH
 Author-email: gberesearch@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `volvisualizer-1.1.3.dist-info/RECORD` & `volvisualizer-1.1.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-volvisualizer/__init__.py,sha256=MNg8Ih17kliJwlnU9Nip6ZLjE9MDf-ibrAgQJVctAy4,23
-volvisualizer/graph.py,sha256=y6LePLlhdGJCkqg-WgpAHHH42PKkr2Bq5oQ_HRWCeZ0,26576
-volvisualizer/market_data.py,sha256=bmjzmB8HJMCPcQRnlvFvmDLzTYGlsDgXebQDqN_t8Kk,11866
-volvisualizer/market_data_prep.py,sha256=Thf4vYGC2RReN7b2m-GbyaXzY870-diySS1drI270QU,26180
-volvisualizer/utils.py,sha256=KkZn7dNsGDVuOkpQ04AVMAMUMF3l5XjbqyIoKWJK-mI,2857
-volvisualizer/vol_methods.py,sha256=GLJsL6LCEsl9JNXMfvrh1RZbZ778VmVJOfgC0aKbWvA,30001
-volvisualizer/volatility.py,sha256=euBLvjKd9ieBu0XkRFiLB5lAmf52MRJjkM2fLrwHVWE,13496
+volvisualizer/__init__.py,sha256=x9FL2OT2SXh3wQnwMN-1smbRacRTCOYcgAuQFQqi_0s,23
+volvisualizer/graph.py,sha256=VVfEluD0rxUFlj1rHfz7vHMBN-xRWWhLLuoago2wYKI,27501
+volvisualizer/market_data.py,sha256=hiAu3QEMQKUvOtaYZjyLwLrz44QnB7stG2MhQpRjgLg,12096
+volvisualizer/market_data_prep.py,sha256=LXq5XH3j0P73yXwUYRYrgxlaGC41ZOpYHM8aUpE36_s,27175
+volvisualizer/utils.py,sha256=beKuHS2pXOV9_sgqsVPrQUMVTDAjjmJc8DNbCmOU5sw,2948
+volvisualizer/vol_methods.py,sha256=2P1yTBHXAzumPcyoYuCLZxXJHOhMtO4_Z90RjduYRMA,30755
+volvisualizer/volatility.py,sha256=6mznSJJE1Ywzqbj13cWxnMcta0yUX1_MNplLDwzBFzg,13614
 volvisualizer/volatility_params.py,sha256=g2iiXI1Cbiz4ISDv8JGZyCNwOb81NxZtSAmUX6AEnuk,3914
-volvisualizer-1.1.3.dist-info/LICENSE,sha256=AE-WWqzPtajuHJajyfzO6uPCKh1DW3MqA1NXcnBImL0,1089
-volvisualizer-1.1.3.dist-info/METADATA,sha256=dxdnFpj4c7A4TCsvPwJ4yDZmo-GQENeH-UIBDINPVho,727
-volvisualizer-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-volvisualizer-1.1.3.dist-info/top_level.txt,sha256=Tfyh9PL2rX9P1DsThRUSnziSAZJU3o43o73eAOUHCMc,14
-volvisualizer-1.1.3.dist-info/RECORD,,
+volvisualizer-1.1.6.dist-info/LICENSE,sha256=AE-WWqzPtajuHJajyfzO6uPCKh1DW3MqA1NXcnBImL0,1089
+volvisualizer-1.1.6.dist-info/METADATA,sha256=sUomcqu4M6AR4EQoITnEp0_QbTjB9mMt1DbzE8UE8XY,727
+volvisualizer-1.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+volvisualizer-1.1.6.dist-info/top_level.txt,sha256=Tfyh9PL2rX9P1DsThRUSnziSAZJU3o43o73eAOUHCMc,14
+volvisualizer-1.1.6.dist-info/RECORD,,
```

