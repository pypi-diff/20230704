# Comparing `tmp/datawhispers-0.2.8.2.tar.gz` & `tmp/datawhispers-0.2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.8.2.tar", last modified: Mon Jul  3 08:48:47 2023, max compression
+gzip compressed data, was "datawhispers-0.2.8.3.tar", last modified: Tue Jul  4 11:33:27 2023, max compression
```

## Comparing `datawhispers-0.2.8.2.tar` & `datawhispers-0.2.8.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-03 08:48:47.621478 datawhispers-0.2.8.2/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.2/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1816 2023-07-03 08:48:47.621340 datawhispers-0.2.8.2/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      694 2023-07-02 18:58:56.000000 datawhispers-0.2.8.2/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-03 08:48:47.620430 datawhispers-0.2.8.2/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.2/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-03 08:30:46.000000 datawhispers-0.2.8.2/datawhispers/advancedProg.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-03 08:34:03.000000 datawhispers-0.2.8.2/datawhispers/datavis.py
--rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.2/datawhispers/mathFuncs.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-03 08:48:47.621137 datawhispers-0.2.8.2/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1816 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      309 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-03 08:48:47.621531 datawhispers-0.2.8.2/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2273 2023-07-03 08:48:18.000000 datawhispers-0.2.8.2/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-04 11:33:27.169302 datawhispers-0.2.8.3/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.3/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     2315 2023-07-04 11:33:27.169188 datawhispers-0.2.8.3/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)     1193 2023-07-04 11:30:50.000000 datawhispers-0.2.8.3/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-04 11:33:27.168363 datawhispers-0.2.8.3/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.3/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)    11578 2023-07-03 09:25:40.000000 datawhispers-0.2.8.3/datawhispers/advancedProg.py
+-rw-r--r--   0 german     (501) staff       (20)     8603 2023-07-03 15:35:55.000000 datawhispers-0.2.8.3/datawhispers/datavis.py
+-rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.3/datawhispers/mathFuncs.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-04 11:33:27.168974 datawhispers-0.2.8.3/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     2315 2023-07-04 11:33:27.000000 datawhispers-0.2.8.3/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      309 2023-07-04 11:33:27.000000 datawhispers-0.2.8.3/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-04 11:33:27.000000 datawhispers-0.2.8.3/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-04 11:33:27.000000 datawhispers-0.2.8.3/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-04 11:33:27.000000 datawhispers-0.2.8.3/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-04 11:33:27.169346 datawhispers-0.2.8.3/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2273 2023-07-04 11:32:46.000000 datawhispers-0.2.8.3/setup.py
```

### Comparing `datawhispers-0.2.8.2/LICENSE` & `datawhispers-0.2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.2/PKG-INFO` & `datawhispers-0.2.8.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.2
+Version: 0.2.8.3
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
@@ -22,16 +22,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DataWhispers Module
 
 ![DataWhispers Logo](https://github.com/GermanPaul12/datawhispers/blob/main/assets/logo.png?raw=true)
 
-## Documentation: [![doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://germanpaul12.github.io/datawhispers/)
+## Documentation: [![doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://germanpaul12.github.io/datawhispers/) [![Documentation Status](https://readthedocs.org/projects/datawhispers/badge/?version=latest)](https://datawhispers.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/datawhispers) ![PyPI - Downloads](https://img.shields.io/pypi/dm/datawhispers) [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://datawhispers.streamlit.app/)
 
 ### The **DataWhispers** module is used for solving regression and statistical problems
 
 It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
 
 Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
 
+Feel free to check out the [Documentation](https://datawhispers.readthedocs.io/en/latest/index.html)
+
 To install just write ```pip install datawhispers``` in your command prompt of choice
```

### Comparing `datawhispers-0.2.8.2/datawhispers/advancedProg.py` & `datawhispers-0.2.8.3/datawhispers/advancedProg.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,42 +5,84 @@
 from sympy import sqrt, sin, cos, tan, exp, log, ln
 import matplotlib.pyplot as plt
 a, b, c, x = sym.symbols('a, b, c, x', real=True)
 
 def linReg(x_in,y):
     '''Time series linear regression. Returns coefs in polynomial descending order.
        Coefs computed analytically.
+       
+        Args:
+            x_in: Array with x-values
+            y: Array with y-values
+
+        Returns:
+            coefs in descending order
+
+        Raises:
+            None
     '''
     
     a = (np.inner(x_in,y) - (len(x_in) * np.mean(x_in) * np.mean(y))) / (np.inner(x_in,x_in) - (len(x_in) * ((np.mean(x_in))**2)))
     b = np.mean(y) - a * np.mean(x_in)
     return [a,b]
 
 def polReg(x_in,y, deg):
     '''Time series polynomial regression. Returns coefs in polynomial descending order.
        Coefs computed numerically.
+       
+       Args:
+            x_in: Array with x-values
+            y: Array with y-values
+            deg: the degree of the polynomial
+
+        Returns:
+            coefs in descending order
+
+        Raises:
+            None
     '''
     
     coefs = np.polyfit(x_in, y, deg)
     return coefs
 
 def freeReg(x_in, y_out, ansatz):
     '''Regression with user ansatz. The ansatz is expected to depend on three
        parameters, a, b, and c. The ansatz is expected to be a string with a 
        symbolic formulation. for instance: 'a*arctan(b*x_in+c)'.
+       
+       Args:
+            x_in: Array with x-values
+            y: Array with y-values
+            ansatz: "linReg", "polReg", "trigReg" or "expReg"
+
+        Returns:
+            coefs
+
+        Raises:
+            None
     '''    
     test_func = sym.lambdify((x, a, b, c), eval(ansatz))
     
     res = curve_fit(test_func, x_in, y_out)
 
     return res[0]    
 
 
 def trigReg(x_in, y):
     '''Time seriessine regression. Returns amplitude, frequency and phase
+    
+        Args:
+            x_in: Array with x-values
+            y: Array with y-values
+
+        Returns:
+            amplitude, frequency and phase
+
+        Raises:
+            None
     '''    
     timestep = x_in[1]-x_in[0]
     x_in = np.fft.fftfreq(len(x_in), timestep)
     Y = np.fft.fft(y)
 
     index = np.argmax(abs(Y))
     
@@ -81,14 +123,39 @@
         f_num = sym.lambdify(x, f)       
         values = f_num(x_in)
         
         
     return  values 
 
 def leastSquares(func,x):
+    '''Solve a nonlinear least-squares problem with bounds on the variables.
+    
+        Args:
+            func: Function which computes the vector of residuals, 
+            with the signature fun(x, *args, **kwargs), i.e., the minimization proceeds with respect to its first argument. 
+            The argument x passed to this function is an ndarray of shape (n,) (never a scalar, even for n=1). 
+            It must allocate and return a 1-D array_like of shape (m,) or a scalar. 
+            If the argument x is complex or the function fun returns complex residuals, 
+            it must be wrapped in a real function of real arguments, as shown at the end of the Examples section.
+            x: Array with x-values
+            
+
+        Returns:
+            x: ndarray, shape (n,)
+                Solution found.
+
+            cost: float
+                Value of the cost function at the solution.
+
+            func: ndarray, shape (m,)
+                Vector of residuals at the solution.
+
+        Raises:
+            None
+    '''
     return least_squares(func,x)
 
 
 def r2(y, y_pred):
         '''Coefficient of determination
         '''
         wert = 1-np.sum((y-y_pred)**2)/np.sum((y-np.mean(y))**2)
@@ -104,47 +171,78 @@
     print(f'# This is a polynomial of order {o}.')
     y = 0
     for i in range(o):
         y += coeffs[i]*x**i
     return y
 
 def make_plot(x,y,y_reg, xticks=[], yticks=[],xlabel="x", ylabel="y", colors=["lightblue", "black"], name="fig_reg.png"):
-    '''
-    Outputs a graph for (x and y) and (x and y_reg) and saves it as fig_reg.png
-    x: array with x-values
-    y: array with y-values
-    y_reg: array with regression y_values
+    '''Outputs a graph for (x and y) and (x and y_reg) and saves it as fig_reg.png
+    
+    Args:
+        x: array with x-values
+        y: array with y-values
+        y_reg: array with regression y_values
+        xticks (optional): list with values to use as x-ticks
+        yticks (optional): list with values to use as y-ticks
+        xlabel (optional): defualt "x"
+        ylabel (optional): defualt "y"
+        colors (optional): default ["lightblue", "black"] scatter=lightblue and line=black
+        name (optional): default "fig_reg.png"
+        
+    Returns:
+        Outputs the graph and saves it
+        
+    Raises:
+        None
     '''
     plt.plot(x,y_reg,color=colors[1]);
     plt.scatter(x,y, color=colors[0]);
     plt.xlabel(xlabel) 
     plt.ylabel(ylabel)
     if xticks: plt.xticks(xticks);
     if yticks: plt.yticks(yticks);
     plt.savefig(f"{name}");  
     plt.show()
 
 
 def show_mnist_from_array(arr):    
-    """
-    Returns the image of the mnist number and saves it as mnist_num.png
-    arr: array of shape (784,) or (28,28)
+    """Returns the image of the mnist number and saves it as mnist_num.png
+    
+    Args:
+        arr: of size (784,) or (28,28) with values from 0 to 255
+        
+    Returns:
+        Outputs the image
+        
+    Raises:
+        None
     """
     label = ''
     if arr.shape == (785,): label,arr = arr[0],arr[1:].reshape((28, 28))
     if arr.shape == (784,):   
         arr = arr.reshape((28, 28))
     # Plot
     plt.title(f"MNIST Number {label}")
     plt.imshow(arr, cmap='gray')
     plt.savefig("mnist_num.png", dpi=1200)
     plt.show()
     
 
 def show_mnist_from_file(filepath):    
+    """Returns the images of the mnist numbers in the file
+    
+    Args:
+        filepath: csv-filepath with lines consisting of values from 0 to 255 with length of 785 or 784
+        
+    Returns:
+        Outputs the images
+        
+    Raises:
+        None
+    """
     with open(filepath) as f: 
         try:
             label = ""
             for i in f:
                 if "," in i:   
                     arr = np.array([int(num) for num in i.split(",")])
                     if arr.shape == (785,): label,arr = arr[0],arr[1:].reshape((28, 28))
@@ -157,17 +255,25 @@
                 plt.imshow(arr, cmap="gray")
                 plt.show()   
         except Exception as e:
             print("Sorry try the func 'show_mnist_from_array' because your file does not seem to work with this method")         
 
 
 def add_mnist_num_arrays(num1,num2):
-    """
-    Returns the image of the result and saves it as mnist_result.png
-    arr: np.array of shape (784,) or (28,28)
+    """Returns the image of the result and saves it as mnist_result.png
+    
+    Args:
+        num1: np.array of length (784,) or (28,28)
+        num2: np.array of length (784,) or (28,28)
+        
+    Returns:
+        Outputs the image
+        
+    Raises:
+        None
     """        
     if num1.shape == (784,):
         num1 = num1.reshape((28,28))
     if num2.shape == (784,):
         num2 = num2.reshape((28,28))
     result = num1 + num2
     plt.savefig("mnist_result.png")
@@ -243,14 +349,29 @@
         '''Shows a plot of the data, the regression and saves the plot
         '''
         make_plot(x=self.x, y=self.y, y_reg=predict(self.ansatz, self.coef, self.x), name=file_name)
         print(f"r2: {self.r2}, coefs: {self.coef}")
     
     
 def plot_all_regs(x,y, xticks=None, yticks=None):
+    """
+    Returns the regression of all types and saves them as png
+    
+    Args:
+        x: array with x-values
+        y: array with y-values
+        xticks (optional): list with values to use as x-ticks
+        yticks (optional): list with values to use as y-ticks
+        
+    Returns:
+        Outputs the graphs and saves them
+        
+    Raises:
+        None
+    """ 
     model = Trend(x,y,"linReg")
     plt.title("Linear Regression");
     y_reg = model.pred(x)
     make_plot(x,y,y_reg, name="lin_reg_plot.png");
     print(f"Coefs: {model.coef}, r2: {model.r2}")
     
     for i in range(2,10):
```

### Comparing `datawhispers-0.2.8.2/datawhispers/datavis.py` & `datawhispers-0.2.8.3/datawhispers/datavis.py`

 * *Files 9% similar despite different names*

```diff
@@ -157,8 +157,42 @@
     print("                                   --------------------------------------------------")
     print("                                   |                     Analyse                    |")
     print("                                   --------------------------------------------------")
     Correlation_table(df,max) # Numerische Korrelationen
     #time.sleep(0.5)
     Correlation_analysis_all(df) # Grafiken zu numerischen Korrelationen
     T_Test(df,Zielvariable,Zielvariable_gut,Zielvariable_schlecht) # Numerisch - Kategorischen Korrelationen
-    chi_square_all(df,Zielvariable) # Kategorisch - Kategorisch Korrelationen
+    chi_square_all(df,Zielvariable) # Kategorisch - Kategorisch Korrelationen
+    
+def make_scatter_plot(x,y, width:int=8, height:int=6, xlabel:str="", ylabel:str="" ,title:str="", color="gray", filename:str="fig.png"):
+    """Outputs a scatter plot
+    
+    Args:
+        x: array with x-values
+        y: array with y-values
+        xticks (optional): list with values to use as x-ticks
+        yticks (optional): list with values to use as y-ticks
+        xlabel (optional): str with xlabel
+        ylabel (optional): str with ylabel
+        title (optional): str with title
+        color (optional): str or tuple consisting of rgb values for color
+        filename (optional): str with filename or path + filename
+        
+    Returns:
+        Outputs the graph and saves it
+        
+    Raises:
+        None
+    """
+    figure,axes=plt.subplots(figsize=(width,height), ncols=1)
+           
+    axes.set_xlabel(xlabel, );
+
+    axes.set_ylabel(ylabel);
+    axes.title.set_text(title)    
+
+    #plt.xticks(rotation="vertical")
+    axes.scatter(x=x, y=y, color=color,);
+
+    plt.savefig(filename)    
+    
+
```

### Comparing `datawhispers-0.2.8.2/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.8.3/datawhispers.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.2
+Version: 0.2.8.3
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
@@ -22,16 +22,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DataWhispers Module
 
 ![DataWhispers Logo](https://github.com/GermanPaul12/datawhispers/blob/main/assets/logo.png?raw=true)
 
-## Documentation: [![doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://germanpaul12.github.io/datawhispers/)
+## Documentation: [![doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://germanpaul12.github.io/datawhispers/) [![Documentation Status](https://readthedocs.org/projects/datawhispers/badge/?version=latest)](https://datawhispers.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/datawhispers) ![PyPI - Downloads](https://img.shields.io/pypi/dm/datawhispers) [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://datawhispers.streamlit.app/)
 
 ### The **DataWhispers** module is used for solving regression and statistical problems
 
 It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
 
 Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
 
+Feel free to check out the [Documentation](https://datawhispers.readthedocs.io/en/latest/index.html)
+
 To install just write ```pip install datawhispers``` in your command prompt of choice
```

### Comparing `datawhispers-0.2.8.2/setup.py` & `datawhispers-0.2.8.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.8.2',      # Start with a small number and increase it with every change you make
+  version = '0.2.8.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

