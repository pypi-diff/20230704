# Comparing `tmp/pymininec-0.4.0.tar.gz` & `tmp/pymininec-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymininec-0.4.0.tar", last modified: Sat May 13 11:10:19 2023, max compression
+gzip compressed data, was "pymininec-0.5.0.tar", last modified: Tue Jul  4 19:13:36 2023, max compression
```

## Comparing `pymininec-0.4.0.tar` & `pymininec-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 11:10:19.981212 pymininec-0.4.0/
--rw-r--r--   0 ralf      (1000) priv      (1011)    24708 2023-05-13 11:10:19.977212 pymininec-0.4.0/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)    20856 2023-05-13 11:05:34.000000 pymininec-0.4.0/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 11:10:19.933212 pymininec-0.4.0/mininec/
--rw-r--r--   0 ralf      (1000) priv      (1011)       16 2023-05-13 11:09:22.000000 pymininec-0.4.0/mininec/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-07-18 18:56:28.000000 pymininec-0.4.0/mininec/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)   140072 2023-05-13 10:41:36.000000 pymininec-0.4.0/mininec/mininec.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 11:10:19.965212 pymininec-0.4.0/pymininec.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)    24708 2023-05-13 11:10:19.000000 pymininec-0.4.0/pymininec.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      298 2023-05-13 11:10:19.000000 pymininec-0.4.0/pymininec.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-13 11:10:19.000000 pymininec-0.4.0/pymininec.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       52 2023-05-13 11:10:19.000000 pymininec-0.4.0/pymininec.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       23 2023-05-13 11:10:19.000000 pymininec-0.4.0/pymininec.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        8 2023-05-13 11:10:19.000000 pymininec-0.4.0/pymininec.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-13 11:10:19.981212 pymininec-0.4.0/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2838 2022-09-13 14:25:55.000000 pymininec-0.4.0/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 11:10:19.969212 pymininec-0.4.0/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)    28959 2023-05-13 10:42:27.000000 pymininec-0.4.0/test/test_mininec.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-04 19:13:36.007460 pymininec-0.5.0/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    29081 2023-07-04 19:13:36.007460 pymininec-0.5.0/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)    24621 2023-07-04 19:12:04.000000 pymininec-0.5.0/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-04 19:13:35.963460 pymininec-0.5.0/mininec/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       16 2023-07-04 19:12:46.000000 pymininec-0.5.0/mininec/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-07-18 18:56:28.000000 pymininec-0.5.0/mininec/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)   145033 2023-07-04 17:52:39.000000 pymininec-0.5.0/mininec/mininec.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-04 19:13:35.995460 pymininec-0.5.0/pymininec.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    29081 2023-07-04 19:13:35.000000 pymininec-0.5.0/pymininec.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      298 2023-07-04 19:13:35.000000 pymininec-0.5.0/pymininec.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-07-04 19:13:35.000000 pymininec-0.5.0/pymininec.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       52 2023-07-04 19:13:35.000000 pymininec-0.5.0/pymininec.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       23 2023-07-04 19:13:35.000000 pymininec-0.5.0/pymininec.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        8 2023-07-04 19:13:35.000000 pymininec-0.5.0/pymininec.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-07-04 19:13:36.007460 pymininec-0.5.0/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2838 2022-09-13 14:25:55.000000 pymininec-0.5.0/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-04 19:13:35.999460 pymininec-0.5.0/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    31064 2023-07-04 18:59:41.000000 pymininec-0.5.0/test/test_mininec.py
```

### Comparing `pymininec-0.4.0/PKG-INFO` & `pymininec-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymininec
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python version of the original MININEC Antenna Optimization code
 Home-page: https://github.com/schlatterbeck/pymininec
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: MININEC in Python
         =================
@@ -190,14 +190,76 @@
         This could (and should) be changed to use vector and matrix operations
         in `numpy`_. In the inner loop of the matrix fill operation there are
         several integrals computed using `gaussian quadrature`_ or a numeric
         solution to an `elliptic integral`_. These are now implemented using
         methods (or at least constants in the case of `gaussian quadrature`_)
         from |scipy.integrate|_ and |scipy.special.ellipk|_.
         
+        Multiple Inverted-V Example
+        +++++++++++++++++++++++++++
+        
+        An old `web-page from 1998 by Dr. Carol F. Milazzo, KP4MD`_ has examples
+        of antennas simulated with Mininec. The first of these examples is three
+        crossed inverted-V (one of which has loading inductors to boost the
+        effective length). The simulation results of pymininec are in the
+        ballpark of the Mininec-based *NEC4WIN* which was used by KP4MD. But it
+        looks like *NEC4WIN* might use what it prints as "Diam." as the radius
+        of the wire (see Fig. 1 in the website) as the radius (see Antenna Model
+        Files in the Appendix). At least if this format is inherited from NEC
+        the last column of the wire definition would hold the radius and this
+        interpretation of the format also is more consistent with the simulation
+        results of Pymininec. The following table shows the original data
+        compared to using half of the diameter in the original model in
+        Pymininec ("Pymininec r") and the diameter as the radius (Pymininec 2r).
+        When using the (supposed) diameter for the radius, the output data
+        matches better to the website data.
+        
+        +---------------+----------------+--------------+--------------+--------------+
+        | Frequency     |                | Original     | Pymininec r  | Pymininec 2r |
+        +---------------+----------------+--------------+--------------+--------------+
+        | 7MHz          | Gain Azimuth   | -2.42 dBi    | -2.52 dBi    | -2.49 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Gain Elevation |  7.21 dBi    |  7.21 dBi    |  7.21 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Impedance      | 38.74 +6.77j | 38.82 -3.66j | 39.28 +1.49j |
+        +---------------+----------------+--------------+--------------+--------------+
+        | 14MHz         | Gain Azimuth   |  4.33 dBi    |  4.60 dBi    |  4.37 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Gain Elevation |  7.23 dBi    |  7.73 dBi    |  7.38 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Impedance      | 46.16 -326j  | 31.86 -307j  | 43.00 -313j  |
+        +---------------+----------------+--------------+--------------+--------------+
+        
+        All of KP4MD's examples have been converted to Pymininec and are available as
+        ``inve802B.pym``, ``hloop40-14.pym``, ``hloop40-7.pym``,
+        ``vloop20.pym``, and ``lzh20.pym`` in the ``test`` directory. Only the
+        ``inve802B.pym`` (with the inverted-Vs) uses the diameter in the
+        original example as the radius in Pymininec, all others use half of the
+        value in the original example (which is supposed to be the diameter) as
+        the radius. But most examples match better to the values computed by
+        KP4MD when doubling the radius.
+        
+        Running the Tests
+        +++++++++++++++++
+        
+        You can run the tests with::
+        
+          python3 -m pytest test
+        
+        If coverage should be reported this becomes::
+        
+          python3 -m pytest --cov mininec test
+        
+        For a more detailed coverage report use::
+        
+          python3 -m pytest --cov-report term-missing --cov mininec test
+        
+        This will show a detailed report of the lines that are not covered by
+        tests.
+        
         Notes on Elliptic Integral Parameters
         -------------------------------------
         
         The Mininec code uses the implementation of an `elliptic integral`_ when
         computing the impedance matrix and in several other places. The integral
         uses a set of E-vector coefficients that are cited differently in
         different places. In the latest version of the open source Basic code
@@ -329,14 +391,26 @@
         NEC archive`_ by PA3KJ or from a `Mininec github project`_, I'm using
         the version from the `unofficial NEC archive`_ and have not verified if
         the two links I've given contain the same code.
         
         Release Notes
         -------------
         
+        v0.5.0: Bug fixes and new load types
+        
+        - New load types RLC load and Trap load: The first uses a series R-L-C
+          (with each being optional), the second serial R-L parallel to a C (for
+          a good emulation of traps in antennas)
+        - Bug-Fix in wire-end matching: If there are multiple wires connected
+          to a single point the previous implementation would not build the data
+          structures correctly
+        - Add more regression tests
+        - Get rid of unittest to avoid a mixture of the unittest and pytest
+          testing frameworks
+        
         v0.4.0: Split `plot-antenna`_ into own project
         
         - Own project `plot-antenna`_
         - Fix parsing of several medium options, mention ground in documentation
         
         v0.3.0: Laplace loads correctly implemented
         
@@ -405,14 +479,16 @@
             http://on5au.be/Books/allmodnotes.zip
         .. _`Antenna modelling notes episode 48`:
             http://on5au.be/content/amod/amod48.html
         .. _`gaussian quadrature`: https://en.wikipedia.org/wiki/Gaussian_quadrature
         .. _`elliptic integral`: https://en.wikipedia.org/wiki/Elliptic_integral
         .. _`scipy`: https://scipy.org/
         .. _`plot-antenna`: https://github.com/schlatterbeck/plot-antenna
+        .. _`web-page from 1998 by Dr. Carol F. Milazzo, KP4MD`:
+            https://www.qsl.net/kp4md/kp4mdnec.htm
         
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pymininec-0.4.0/README.rst` & `pymininec-0.5.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -182,14 +182,76 @@
 This could (and should) be changed to use vector and matrix operations
 in `numpy`_. In the inner loop of the matrix fill operation there are
 several integrals computed using `gaussian quadrature`_ or a numeric
 solution to an `elliptic integral`_. These are now implemented using
 methods (or at least constants in the case of `gaussian quadrature`_)
 from |scipy.integrate|_ and |scipy.special.ellipk|_.
 
+Multiple Inverted-V Example
++++++++++++++++++++++++++++
+
+An old `web-page from 1998 by Dr. Carol F. Milazzo, KP4MD`_ has examples
+of antennas simulated with Mininec. The first of these examples is three
+crossed inverted-V (one of which has loading inductors to boost the
+effective length). The simulation results of pymininec are in the
+ballpark of the Mininec-based *NEC4WIN* which was used by KP4MD. But it
+looks like *NEC4WIN* might use what it prints as "Diam." as the radius
+of the wire (see Fig. 1 in the website) as the radius (see Antenna Model
+Files in the Appendix). At least if this format is inherited from NEC
+the last column of the wire definition would hold the radius and this
+interpretation of the format also is more consistent with the simulation
+results of Pymininec. The following table shows the original data
+compared to using half of the diameter in the original model in
+Pymininec ("Pymininec r") and the diameter as the radius (Pymininec 2r).
+When using the (supposed) diameter for the radius, the output data
+matches better to the website data.
+
++---------------+----------------+--------------+--------------+--------------+
+| Frequency     |                | Original     | Pymininec r  | Pymininec 2r |
++---------------+----------------+--------------+--------------+--------------+
+| 7MHz          | Gain Azimuth   | -2.42 dBi    | -2.52 dBi    | -2.49 dBi    |
++               +----------------+--------------+--------------+--------------+
+|               | Gain Elevation |  7.21 dBi    |  7.21 dBi    |  7.21 dBi    |
++               +----------------+--------------+--------------+--------------+
+|               | Impedance      | 38.74 +6.77j | 38.82 -3.66j | 39.28 +1.49j |
++---------------+----------------+--------------+--------------+--------------+
+| 14MHz         | Gain Azimuth   |  4.33 dBi    |  4.60 dBi    |  4.37 dBi    |
++               +----------------+--------------+--------------+--------------+
+|               | Gain Elevation |  7.23 dBi    |  7.73 dBi    |  7.38 dBi    |
++               +----------------+--------------+--------------+--------------+
+|               | Impedance      | 46.16 -326j  | 31.86 -307j  | 43.00 -313j  |
++---------------+----------------+--------------+--------------+--------------+
+
+All of KP4MD's examples have been converted to Pymininec and are available as
+``inve802B.pym``, ``hloop40-14.pym``, ``hloop40-7.pym``,
+``vloop20.pym``, and ``lzh20.pym`` in the ``test`` directory. Only the
+``inve802B.pym`` (with the inverted-Vs) uses the diameter in the
+original example as the radius in Pymininec, all others use half of the
+value in the original example (which is supposed to be the diameter) as
+the radius. But most examples match better to the values computed by
+KP4MD when doubling the radius.
+
+Running the Tests
++++++++++++++++++
+
+You can run the tests with::
+
+  python3 -m pytest test
+
+If coverage should be reported this becomes::
+
+  python3 -m pytest --cov mininec test
+
+For a more detailed coverage report use::
+
+  python3 -m pytest --cov-report term-missing --cov mininec test
+
+This will show a detailed report of the lines that are not covered by
+tests.
+
 Notes on Elliptic Integral Parameters
 -------------------------------------
 
 The Mininec code uses the implementation of an `elliptic integral`_ when
 computing the impedance matrix and in several other places. The integral
 uses a set of E-vector coefficients that are cited differently in
 different places. In the latest version of the open source Basic code
@@ -321,14 +383,26 @@
 NEC archive`_ by PA3KJ or from a `Mininec github project`_, I'm using
 the version from the `unofficial NEC archive`_ and have not verified if
 the two links I've given contain the same code.
 
 Release Notes
 -------------
 
+v0.5.0: Bug fixes and new load types
+
+- New load types RLC load and Trap load: The first uses a series R-L-C
+  (with each being optional), the second serial R-L parallel to a C (for
+  a good emulation of traps in antennas)
+- Bug-Fix in wire-end matching: If there are multiple wires connected
+  to a single point the previous implementation would not build the data
+  structures correctly
+- Add more regression tests
+- Get rid of unittest to avoid a mixture of the unittest and pytest
+  testing frameworks
+
 v0.4.0: Split `plot-antenna`_ into own project
 
 - Own project `plot-antenna`_
 - Fix parsing of several medium options, mention ground in documentation
 
 v0.3.0: Laplace loads correctly implemented
 
@@ -397,7 +471,9 @@
     http://on5au.be/Books/allmodnotes.zip
 .. _`Antenna modelling notes episode 48`:
     http://on5au.be/content/amod/amod48.html
 .. _`gaussian quadrature`: https://en.wikipedia.org/wiki/Gaussian_quadrature
 .. _`elliptic integral`: https://en.wikipedia.org/wiki/Elliptic_integral
 .. _`scipy`: https://scipy.org/
 .. _`plot-antenna`: https://github.com/schlatterbeck/plot-antenna
+.. _`web-page from 1998 by Dr. Carol F. Milazzo, KP4MD`:
+    https://www.qsl.net/kp4md/kp4mdnec.htm
```

### Comparing `pymininec-0.4.0/mininec/mininec.py` & `pymininec-0.5.0/mininec/mininec.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,53 @@
     def __init__ (self, impedance):
         self._impedance = impedance
         super ().__init__ ()
     # end def __init__
 
 # end class Impedance_Load
 
+class Series_RLC_Load (_Load):
+    """ A load with R, L, C in series, an unspecified value is
+        considered to be a 0-Ohm resistor.
+        This was not in the original mininec code.
+        But it could be modelled with a Laplace load.
+        Frequency is in MHz (when calling impedance), otherwise we use
+        metric units Ohm, Henry, Farad.
+    >>> l = Series_RLC_Load (R = 0.1, L = 60e-6)
+    >>> z = l.impedance (7)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    0.1+2638.94j
+    >>> l = Series_RLC_Load (R = 1000, C = 60e-12)
+    >>> z = l.impedance (7)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    1000-378.94j
+    """
+    def __init__ (self, R = None, L = None, C = None):
+        super ().__init__ ()
+        self.r = R
+        self.l = L
+        self.c = C
+    # end def __init__
+
+    def impedance (self, f):
+        """ Impedance for given frequency
+        """
+        w = 2 * np.pi * f * 1e6
+        x = 0 + 0j
+        if self.r is not None:
+            x += self.r
+        if self.l is not None:
+            x += w * self.l * 1j
+        if self.c is not None:
+            x -= 1 / (w * self.c) * 1j
+        return x
+    # end def impedance
+
+# end class Series_RLC_Load
+
 class Laplace_Load (_Load):
     """ Laplace s-Parameter (s = j omega) load from mininec implementation
         We get two lists of parameters. They represent the numerator and
         denominator coefficients, respectively (sequence a is the denominator
         and sequence b is the numerator). This uses s*L for inductance,
         1/(s*C) for capacitance, and R for resistors. These are combined
         with the usual rules for parallel and serial connection.
@@ -360,14 +399,22 @@
     >>> z = l.impedance (7.15)
     >>> print ("%g%+gj" % (z.real, z.imag))
     -0+10.1472j
     >>> l = Laplace_Load (b = (0., 225.998e-9), a = (1,))
     >>> z = l.impedance (7.15)
     >>> print ("%g%+gj" % (z.real, z.imag))
     0+10.1529j
+    >>> l = Laplace_Load (b = (0.1, 60e-6), a = (1,))
+    >>> z = l.impedance (7)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    0.1+2638.94j
+    >>> l = Laplace_Load (b = (1, 1000 * 60e-12), a = (0, 60e-12))
+    >>> z = l.impedance (7)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    1000-378.94j
     """
     def __init__ (self, a, b):
         m = max (len (a), len (b))
         self.a = np.zeros (m)
         self.b = np.zeros (m)
         self.a [:len (a)] = a
         self.b [:len (b)] = b
@@ -389,14 +436,50 @@
             d += self.a [j] * m
             m *= (1j * w)
         return u / d
     # end def impedance
 
 # end class Laplace_Load
 
+class Trap_Load (Laplace_Load):
+    """ A trap consisting of L+R in series parallel to a C.
+           +---L----R---+
+        ---+            +---
+           +-----C------+
+        This is a convenience method as it can already be specified with
+        the Laplace_Load type.
+        Note that you should not specify R=0, otherwise you'll get a
+        division by zero at the resonance frequency.
+    >>> c = 10e-12
+    >>> l = 10e-6
+    >>> r = 1
+    >>> t = Trap_Load (r, l, c)
+    >>> z = t.impedance (15.91548635144039)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    1e+06+2.87559e-08j
+    >>> t = Trap_Load (r, l, c)
+    >>> z = t.impedance (15.915)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    996218+60882.7j
+    >>> t = Trap_Load (r, l, c)
+    >>> z = t.impedance (15.916)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    995915-64286.3j
+    >>> t = Trap_Load (1e-10, l, c)
+    >>> z = t.impedance (15.915494309189534)
+    >>> print ("%g%+gj" % (z.real, z.imag))
+    1e+16-1000j
+    """
+
+    def __init__ (self, R, L, C):
+        super ().__init__ (a = (1, R*C, L*C), b = (R, L))
+    # end def __init__
+
+# end class Trap_Load
+
 class Medium:
     """ This encapsulates the media (e.g. ground screen etc.)
         With permittivity and conductivity zero we asume ideal ground.
         Note that it seems only the first medium can have a
         ground screen of radials.
         The boundary is the type of boundary between different media (if
         there is more than one). It is either 'linear' (X-coordinate it
@@ -577,36 +660,50 @@
         self.is_ground = ((self.p1 [-1] == 0), (self.p2 [-1] == 0))
         if self.is_ground [0] and self.is_ground [1]:
             raise ValueError ("Both ends of a wire may not be grounded")
         if self.p1 [-1] < 0 or self.p2 [-1] < 0:
             raise ValueError ("height cannot not be negative with ground")
     # end def compute_ground
 
-    def compute_connections (self, end_dicts):
+    def compute_connections (self, end_dict):
         """ Compute links to connected wires
             Also compute sets of indeces of pulses.
-            Note that we're using dictionaries for matching endpoints,
+            Note that we're using a dictionary for matching endpoints,
             this reduces two nested loops over the wires which is O(N**2)
             to a single loop O(N).
+
+            We do not use a second loop but instead put each wire end
+            into a dictionary linking to the wire. That way the
+            algorithm is O(N) not O(N^2). The dictionaries for the wire
+            ends is end_dict, we store a tuple of end index and wire in
+            this dictionary.
+
+            In the future we may want to introduce fuzzy matching of
+            endpoints (similar to how NEC does it). This means that we
+            would probably first try to match via dictionary and only if
+            that doesn't return a match we might use a binary search via
+            one of the coordinates (and then determine the euclidian
+            distance).
         """
 
-        # These are two loops of two elements each. This rolls the
-        # end-matching computation of 4 explicitly-programmed cases in
-        # the Basic program lines 1325-1356 into a few statements.
-        # The idea is to use two dictionaries of end-point coordinates.
+        # This rolls the end-matching computation of 4
+        # explicitly-programmed cases in the Basic program lines
+        # 1325-1356 into a few statements.
+        # The idea is to use a dictionary of end-point coordinates.
         for n1, current_end in enumerate (self.endpoints):
+            if self.is_ground [n1]:
+                continue
             ep_tuple = tuple (current_end)
-            for n2, other_end_dict in enumerate (end_dicts):
-                if not self.is_ground [n1] and ep_tuple in other_end_dict:
-                    other = other_end_dict [ep_tuple]
-                    s = -1 if (n2 == n1) else 1
-                    other.conn [n2].add (self,  self, n1, s, s)
-                    self.conn  [n1].add (other, self, n1, 1, s)
-            if ep_tuple not in end_dicts [n1]:
-                end_dicts [n1][ep_tuple] = self
+            if ep_tuple in end_dict:
+                n2, other = end_dict [ep_tuple]
+                s = -1 if (n2 == n1) else 1
+                other.conn [n2].add (self,  self, n1, s, s)
+                self.conn  [n1].add (other, self, n1, 1, s)
+            else:
+                end_dict [ep_tuple] = (n1, self)
     # end def compute_connections
 
     def connections (self):
         return self.conn [0].wires.union (self.conn [1].wires)
     # end def connections
 
     def idx (self, end_idx):
@@ -798,17 +895,20 @@
         w: 0 idx: 9 s:1
         conn r:
         <BLANKLINE>
         """
         self.f          = f
         self.media      = media
         self.loads      = []
+        self.loadidx    = set ()
         self.check_ground ()
         self.sources    = []
         self.geo        = geo
+        # Dictionary of ends to compute matches
+        self.end_dict   = {}
         self.print_opts = print_opts or set (('far-field',))
         if not self.media or len (self.media) == 1:
             self.boundary = 'linear'
         self.check_geo ()
         self.compute_connectivity ()
         self.output_date = False
     # end __init__
@@ -904,35 +1004,28 @@
             Then the segments are computed.
             In the original code this starts on line 1198 with the
             comment "compute connectivity data (pulses N1 to N)"
             The variable seg replaces the X, Y, Z arrays in the original
             code, it has consequently dimension 3.
             Looks like index n1 is the index of the next start segment.
             And n is the index of the next end segment.
-
-            Note that we do not use a second loop but instead put each
-            wire end into a dictionary linking to the wire. That way the
-            algorithm is O(N) not O(N^2). The dictionaries for the wire
-            ends is end_dicts, this is a list of two dictionaries, one
-            for each end.
         """
         n = 0
         self.c_per = c_per = {}
         self.w_per = w_per = {}
         self.seg   = seg   = {}
-        end_dicts  = [{}, {}]
         for i, w in enumerate (self.geo):
             # This part starts at 1298 comment "connections"
             # We do not use the E, L, M array with the X, Y, Z
             # coordinates of the start of the wires and the second half
             # with the end of the wires, we use the Wire objects
             # instead.
 
             # Try to match existing wire endpoints
-            w.compute_connections (end_dicts)
+            w.compute_connections (self.end_dict)
 
             # i1 and i2 are the indeces of the previous/next wire.
             # This is 0 when there is no prev/next wire. It is -n
             # (where n is the wire.n) if the end is grounded. The index
             # is negative if the polarity changes, i.e. when we have a
             # connection from end1 to end1 of the other wire or end2 to
             # end2 of the other wire.
@@ -2045,15 +2138,18 @@
             absolute index, otherwise it's the index of a pulse on the
             wire given by wire_idx. Indeces are 0-based.
         """
         if pulse is None:
             for wire in self.geo:
                 for p in wire.segment_iter ():
                     load.add_pulse (p)
-            self.loads.append (load)
+            # Avoid adding same load several times
+            if load.n not in self.loadidx:
+                self.loads.append (load)
+                self.loadidx.add (load.n)
         else:
             if pulse < 0:
                 raise ValueError ("Pulse index must be >= 0")
             if wire_idx is not None:
                 if wire_idx >= len (self.geo):
                     raise ValueError ('Invalid wire index %d' % (wire_idx))
                 w = self.geo [wire_idx]
@@ -2062,15 +2158,18 @@
                     raise ValueError \
                         ('Invalid pulse %d for wire %d' % (pulse, wire_idx))
             elif pulse >= len (self.c_per):
                 raise ValueError ('Invalid pulse %d' % pulse)
             else:
                 p = pulse
             load.add_pulse (p)
-            self.loads.append (load)
+            # Avoid adding same load several times
+            if load.n not in self.loadidx:
+                self.loads.append (load)
+                self.loadidx.add (load.n)
     # end def register_load
 
     def register_source (self, source, pulse, wire_idx = None):
         """ Register a source, either with absolute pulse index or with
             a pulse index relative to a wire. Indeces are 0-based.
         """
         if pulse < 0:
@@ -2488,19 +2587,19 @@
             p2 = 0.0
             r.append ('*' * 20 + 'NEAR ELECTRIC FIELDS' + '*' * 20)
             r.append \
                 ( ' ' * 9 + 'FIELD POINT: X = %s  Y = %s  Z = %s'
                 % (format_float (coord))
                 )
             r.append \
-                ( '  VECTOR%sREAL%sIMAGINARY%sMAGNITUDE%sPHASE' 
+                ( '  VECTOR%sREAL%sIMAGINARY%sMAGNITUDE%sPHASE'
                 % tuple (' ' * k for k in (6, 10, 5, 5))
                 )
             r.append \
-                ( ' COMPONENT%sV/M%sV/M%sV/M%sDEG' 
+                ( ' COMPONENT%sV/M%sV/M%sV/M%sDEG'
                 % tuple (' ' * k for k in (5, 11, 11, 11))
                 )
             ax = 'XYZ'
             for n, value in enumerate (v):
                 a   = np.angle (value)
                 b   = np.abs (value)
                 b2  = b ** 2
@@ -2530,19 +2629,19 @@
             p2 = 0.0
             r.append ('*' * 20 + 'NEAR MAGNETIC FIELDS' + '*' * 20)
             r.append \
                 ( ' ' * 9 + 'FIELD POINT: X = %s  Y = %s  Z = %s'
                 % (format_float (coord))
                 )
             r.append \
-                ( '  VECTOR%sREAL%sIMAGINARY%sMAGNITUDE%sPHASE' 
+                ( '  VECTOR%sREAL%sIMAGINARY%sMAGNITUDE%sPHASE'
                 % tuple (' ' * k for k in (6, 10, 5, 5))
                 )
             r.append \
-                ( ' COMPONENT%sAMPS/M%sAMPS/M%sAMPS/M%sDEG' 
+                ( ' COMPONENT%sAMPS/M%sAMPS/M%sAMPS/M%sDEG'
                 % tuple (' ' * k for k in (5, 8, 8, 8))
                 )
             ax = 'XYZ'
             for n, value in enumerate (v):
                 a   = np.angle (value)
                 b   = np.abs (value)
                 b2  = b ** 2
@@ -2654,15 +2753,22 @@
                 seg = tuple (self.seg [idx])
                 r.append (self.seg_as_mininec (wire, seg, k))
         return '\n'.join (r)
     # end def wires_as_mininec
 
 # end class Mininec
 
-def main (argv = sys.argv [1:], f_err = sys.stderr):
+def parse_floatlist (s, l = 3, fill = None):
+    """ Parse comma-separated list of floats with length l.
+        Missing values are filled with the value of fill.
+    """
+    return [float (x) if x else fill for x in s.split (',')]
+# end def parse_floatlist
+
+def main (argv = sys.argv [1:], f_err = sys.stderr, return_mininec = False):
     """ The main routine called from the command-line
     >>> args = ['-f', '7.15', '-w', '5,0,0,0,0,0,10.0838,0.0127']
     >>> args.extend (['--frequency-increment=.01', '--frequency-steps=2'])
     >>> args.extend (['--medium=0,0,0', '--excitation-segment=1'])
     >>> args.extend (['--theta=0,45,3', '--phi=0,180,3'])
     >>> main (args)
                        ****************************************
@@ -2693,14 +2799,15 @@
     <BLANKLINE>
     NO. OF SOURCES :  1
     PULSE NO., VOLTAGE MAGNITUDE, PHASE (DEGREES):  1 , 1 , 0
     NUMBER OF LOADS 0
     <BLANKLINE>
     FREQUENCY (MHZ): 7.15
         WAVE LENGTH =  41.93007  METERS
+    <BLANKLINE>
     ********************    SOURCE DATA     ********************
     PULSE  1      VOLTAGE = ( 1 , 0 J)
                   CURRENT = ( 2.857798E-02 ,  1.660853E-03 J)
                   IMPEDANCE = ( 34.87418 , -2.026766 J)
                   POWER =  1.428899E-02  WATTS
     <BLANKLINE>
     ********************    CURRENT DATA    ********************
@@ -2713,16 +2820,16 @@
      3             2.346944E-02  8.170773E-05  2.346959E-02  .199472  
      4             1.744657E-02 -2.362219E-04  1.744817E-02 -.775722  
      5             9.607629E-03 -2.685486E-04  9.611381E-03 -1.601092 
     E              0             0             0             0
     <BLANKLINE>
     ********************     FAR FIELD      ********************
     <BLANKLINE>
-    ZENITH ANGLE : INITIAL,INCREMENT,NUMBER:  0 , 45 , 3
-    AZIMUTH ANGLE: INITIAL,INCREMENT,NUMBER:  0 , 180 , 3
+    ZENITH ANGLE : INITIAL,INCREMENT,NUMBER: 0 , 45 , 3
+    AZIMUTH ANGLE: INITIAL,INCREMENT,NUMBER: 0 , 180 , 3
     <BLANKLINE>
     ********************    PATTERN DATA    ********************
     ZENITH        AZIMUTH       VERTICAL      HORIZONTAL    TOTAL
      ANGLE         ANGLE        PATTERN (DB)  PATTERN (DB)  PATTERN (DB)
      0             0            -999          -999          -999     
      45            0             1.163918     -999           1.163918
      90            0             5.119285     -999           5.119285
@@ -3138,14 +3245,26 @@
     >>> args = ['-f', '7.15']
     >>> args.extend (['--excitation-segment=1'])
     >>> args.extend (['--theta=0,45,nonint', '--phi=0,180,3'])
     >>> r = main (args, sys.stdout)
     Invalid theta angle, need float, float, int
     >>> r
     23
+
+    >>> args = ['--rlc-load=a,b,c']
+    >>> r = main (args, sys.stdout)
+    Error in series RLC load: could not convert string to float: 'a'
+    >>> r
+    23
+
+    >>> args = ['--trap-load=a,b,c']
+    >>> r = main (args, sys.stdout)
+    Error in trap load: could not convert string to float: 'a'
+    >>> r
+    23
     """
     boundaries = ('linear', 'circular')
     from argparse import ArgumentParser
     cmd = ArgumentParser ()
     cmd.add_argument \
         ( '--attach-load'
         , help    = 'Attach load with given index to pulse, needs '
@@ -3165,15 +3284,14 @@
     cmd.add_argument \
         (  '--excitation-segment'
         , help    = "Segment number for excitation, can be specified "
                     "more than once, default is the single segment 5"
         , type    = int
         , action  = 'append'
         , default = []
-        , 
         )
     cmd.add_argument \
         ( '--excitation-voltage'
         , help    = "Voltage for excitation, can be specified more than "
                     "once and can be a complex number, "
                     "default is a single source of 1V"
         , type    = complex
@@ -3221,15 +3339,31 @@
                     ' are numbered last.'
         , action  = 'append'
         , default = []
         )
     cmd.add_argument \
         ( '-l', '--load'
         , type    = complex
-        , help    = 'Complex load'
+        , help    = 'Complex load, specify complex impedance, e.g.  50+3j,'
+                    ' complex loads are numbered first'
+        , action  = 'append'
+        , default = []
+        )
+    cmd.add_argument \
+        ( '--rlc-load'
+        , help    = 'RLC (series) load, specify R,L,C in Ohm, Henry, Farad,'
+                    ' RLC loads are numbered second'
+        , action  = 'append'
+        , default = []
+        )
+    cmd.add_argument \
+        ( '--trap-load'
+        , help    = 'Trap load, R+L in series parallel to C, '
+                    'specify R,L,C in Ohm, Henry, Farad,'
+                    ' Trap loads are numbered third'
         , action  = 'append'
         , default = []
         )
     cmd.add_argument \
         ( '--medium'
         , help    = "Media (ground), free space if not given, "
                     "specify permittivity (dielectric constant), "
@@ -3369,14 +3503,26 @@
     m = Mininec (args.frequency, wires, media = media)
     for i, v in zip (args.excitation_segment, args.excitation_voltage):
         s = Excitation (cvolt = v)
         m.register_source (s, i - 1)
     loads = []
     for l in args.load:
         loads.append (Impedance_Load (l))
+    for l in args.rlc_load:
+        try:
+            loads.append (Series_RLC_Load (*parse_floatlist (l)))
+        except ValueError as err:
+            print ("Error in series RLC load: %s" % err, file = f_err)
+            return 23
+    for l in args.trap_load:
+        try:
+            loads.append (Trap_Load (*parse_floatlist (l, fill=0)))
+        except ValueError as err:
+            print ("Error in trap load: %s" % err, file = f_err)
+            return 23
     laplace = []
     for a in args.laplace_load_a:
         try:
             af = [float (x) for x in a.split (',')]
         except ValueError as err:
             print ("Error in Laplace load A: %s" % err, file = f_err)
             return 23
@@ -3468,14 +3614,16 @@
             print ("Error near-field start: %s" % err, file = f_err)
             return 23
         try:
             nf_inc = [float (x) for x in nf [3:6]]
         except ValueError as err:
             print ("Error near-field inc: %s" % err, file = f_err)
             return 23
+    if return_mininec:
+        return m
     options = set ()
     far_field = False
     for opt in args.option:
         if opt not in allowed_options:
             print ("Invalid print option: %s" % opt)
             return 23
         options.add (opt)
```

### Comparing `pymininec-0.4.0/pymininec.egg-info/PKG-INFO` & `pymininec-0.5.0/pymininec.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymininec
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python version of the original MININEC Antenna Optimization code
 Home-page: https://github.com/schlatterbeck/pymininec
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: MININEC in Python
         =================
@@ -190,14 +190,76 @@
         This could (and should) be changed to use vector and matrix operations
         in `numpy`_. In the inner loop of the matrix fill operation there are
         several integrals computed using `gaussian quadrature`_ or a numeric
         solution to an `elliptic integral`_. These are now implemented using
         methods (or at least constants in the case of `gaussian quadrature`_)
         from |scipy.integrate|_ and |scipy.special.ellipk|_.
         
+        Multiple Inverted-V Example
+        +++++++++++++++++++++++++++
+        
+        An old `web-page from 1998 by Dr. Carol F. Milazzo, KP4MD`_ has examples
+        of antennas simulated with Mininec. The first of these examples is three
+        crossed inverted-V (one of which has loading inductors to boost the
+        effective length). The simulation results of pymininec are in the
+        ballpark of the Mininec-based *NEC4WIN* which was used by KP4MD. But it
+        looks like *NEC4WIN* might use what it prints as "Diam." as the radius
+        of the wire (see Fig. 1 in the website) as the radius (see Antenna Model
+        Files in the Appendix). At least if this format is inherited from NEC
+        the last column of the wire definition would hold the radius and this
+        interpretation of the format also is more consistent with the simulation
+        results of Pymininec. The following table shows the original data
+        compared to using half of the diameter in the original model in
+        Pymininec ("Pymininec r") and the diameter as the radius (Pymininec 2r).
+        When using the (supposed) diameter for the radius, the output data
+        matches better to the website data.
+        
+        +---------------+----------------+--------------+--------------+--------------+
+        | Frequency     |                | Original     | Pymininec r  | Pymininec 2r |
+        +---------------+----------------+--------------+--------------+--------------+
+        | 7MHz          | Gain Azimuth   | -2.42 dBi    | -2.52 dBi    | -2.49 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Gain Elevation |  7.21 dBi    |  7.21 dBi    |  7.21 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Impedance      | 38.74 +6.77j | 38.82 -3.66j | 39.28 +1.49j |
+        +---------------+----------------+--------------+--------------+--------------+
+        | 14MHz         | Gain Azimuth   |  4.33 dBi    |  4.60 dBi    |  4.37 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Gain Elevation |  7.23 dBi    |  7.73 dBi    |  7.38 dBi    |
+        +               +----------------+--------------+--------------+--------------+
+        |               | Impedance      | 46.16 -326j  | 31.86 -307j  | 43.00 -313j  |
+        +---------------+----------------+--------------+--------------+--------------+
+        
+        All of KP4MD's examples have been converted to Pymininec and are available as
+        ``inve802B.pym``, ``hloop40-14.pym``, ``hloop40-7.pym``,
+        ``vloop20.pym``, and ``lzh20.pym`` in the ``test`` directory. Only the
+        ``inve802B.pym`` (with the inverted-Vs) uses the diameter in the
+        original example as the radius in Pymininec, all others use half of the
+        value in the original example (which is supposed to be the diameter) as
+        the radius. But most examples match better to the values computed by
+        KP4MD when doubling the radius.
+        
+        Running the Tests
+        +++++++++++++++++
+        
+        You can run the tests with::
+        
+          python3 -m pytest test
+        
+        If coverage should be reported this becomes::
+        
+          python3 -m pytest --cov mininec test
+        
+        For a more detailed coverage report use::
+        
+          python3 -m pytest --cov-report term-missing --cov mininec test
+        
+        This will show a detailed report of the lines that are not covered by
+        tests.
+        
         Notes on Elliptic Integral Parameters
         -------------------------------------
         
         The Mininec code uses the implementation of an `elliptic integral`_ when
         computing the impedance matrix and in several other places. The integral
         uses a set of E-vector coefficients that are cited differently in
         different places. In the latest version of the open source Basic code
@@ -329,14 +391,26 @@
         NEC archive`_ by PA3KJ or from a `Mininec github project`_, I'm using
         the version from the `unofficial NEC archive`_ and have not verified if
         the two links I've given contain the same code.
         
         Release Notes
         -------------
         
+        v0.5.0: Bug fixes and new load types
+        
+        - New load types RLC load and Trap load: The first uses a series R-L-C
+          (with each being optional), the second serial R-L parallel to a C (for
+          a good emulation of traps in antennas)
+        - Bug-Fix in wire-end matching: If there are multiple wires connected
+          to a single point the previous implementation would not build the data
+          structures correctly
+        - Add more regression tests
+        - Get rid of unittest to avoid a mixture of the unittest and pytest
+          testing frameworks
+        
         v0.4.0: Split `plot-antenna`_ into own project
         
         - Own project `plot-antenna`_
         - Fix parsing of several medium options, mention ground in documentation
         
         v0.3.0: Laplace loads correctly implemented
         
@@ -405,14 +479,16 @@
             http://on5au.be/Books/allmodnotes.zip
         .. _`Antenna modelling notes episode 48`:
             http://on5au.be/content/amod/amod48.html
         .. _`gaussian quadrature`: https://en.wikipedia.org/wiki/Gaussian_quadrature
         .. _`elliptic integral`: https://en.wikipedia.org/wiki/Elliptic_integral
         .. _`scipy`: https://scipy.org/
         .. _`plot-antenna`: https://github.com/schlatterbeck/plot-antenna
+        .. _`web-page from 1998 by Dr. Carol F. Milazzo, KP4MD`:
+            https://www.qsl.net/kp4md/kp4mdnec.htm
         
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pymininec-0.4.0/setup.py` & `pymininec-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymininec-0.4.0/test/test_mininec.py` & `pymininec-0.5.0/test/test_mininec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Ralf Schlatterbeck. All rights reserved
+# Copyright (C) 2022-23 Ralf Schlatterbeck. All rights reserved
 # Reichergasse 131, A-3411 Weidling
 # ****************************************************************************
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -18,30 +18,31 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ****************************************************************************
 
 import os
-import unittest
 import pytest
 import doctest
 import numpy as np
 import mininec
 from mininec.mininec import *
+from mininec.mininec import main
 from zmatrix import *
 from ohio import Near_Far_Comparison
 
 class _Test_Base_With_File:
 
-    def simple_setup (self, filename, mininec):
+    def simple_setup (self, filename, mininec = None):
         with open (os.path.join ('test', filename), 'r') as f:
             self.expected_output = f.read ()
         self.expected_output = self.expected_output.rstrip ('\n')
-        mininec.compute ()
+        if mininec:
+            mininec.compute ()
     # end def simple_setup
 
     def dipole_7mhz (self, wire_dia, filename):
         w = []
         w.append (Wire (10, 0, 0, 0, 21.414285, 0, 0, wire_dia))
         s = Excitation (1, 0)
         m = Mininec (7, w)
@@ -213,82 +214,86 @@
             m.compute_far_field (zenith, azimuth)
         return m
     # end def t_antenna
 
     def compare_far_field_data (self, m, may_fail_last_digit = False):
         """ dB values below -200 contain large rounding errors.
             This makes tests fail on different architectures, notably on
-            Intel vs. AMD CPUs. Seems the trigonometric functions are
-            slightly different on these architectures. We compare values
-            above -200dB exactly and assert that the value is below -200
-            for the others.
+            Intel vs. AMD CPUs. But also on different python versions
+            (self-compiled python10 vs debian bullseye python9).
+            Seems the trigonometric functions are slightly different on
+            these architectures. We compare values above -200dB exactly,
+            and assert that the value is below -200 for the others.
+            In addition if may_fail_last_digit is True the last digit of
+            a dB value may differ.
         """
         ex  = self.expected_output.split ('\n')
         ac  = m.as_mininec ().split ('\n')
         idx = self.expected_output.find ('PATTERN DATA')
         l   = len (self.expected_output [:idx].split ('\n'))
         off = l + 2
-        self.assertEqual (ex [:off], ac [:off])
+        assert ex [:off] == ac [:off]
         for e, a in zip (ex [off:], ac [off:]):
             el = e.strip ().split ()
             al = a.strip ().split ()
-            self.assertEqual (el [:2], al [:2])
+            assert el [:2] == al [:2]
             for ef, af in zip (el, al):
                 eff = float (ef)
                 aff = float (af)
                 if eff > -200:
                     if may_fail_last_digit:
-                        self.assertEqual (ef [:-1], af [:-1])
+                        m = min (len (ef), len (af))
+                        assert ef [:m-1] == af [:m-1]
                     else:
-                        self.assertEqual (ef, af)
+                        assert ef == af
                 else:
-                    self.assertLess (aff, -200)
+                    assert aff < -200
     # end def compare_far_field_data
 
     def compare_currents (self, exs, acs):
         """ This is used when the CURRENT line in the feed pulse is
             slightly off on different architectures. In addition the
             individual CURRENT DATA lines are also compared
             approximately
         """
         ex  = exs.split ('\n')
         ac  = acs.split ('\n')
         idx = exs.find ('CURRENT')
         l   = len (exs [:idx].split ('\n'))
         off = l - 1
-        self.assertEqual (ex [:off], ac [:off])
+        assert ex [:off] == ac [:off]
         exc = ex [off].strip ()
         acc = ac [off].strip ()
         assert acc.startswith ('CURRENT = ( ')
         assert acc.endswith (' J)')
         exc = [float (x) for x in exc [12:-3].split (',')]
         acc = [float (x) for x in acc [12:-3].split (',')]
-        self.assertAlmostEqual (exc [0], acc [0], 12)
-        self.assertAlmostEqual (exc [1], acc [1], 12)
+        assert round (abs (exc [0] - acc [0]), 12) == 0
+        assert round (abs (exc [1] - acc [1]), 12) == 0
         off += 1
         state = 0
         for l_ex, l_ac in zip (ex [off:], ac [off:]):
             if state == 0 or state == 2:
-                self.assertEqual (l_ex, l_ac)
+                assert l_ex == l_ac
             if '(DEGREES)' in l_ex:
                 state = 1
                 continue
             if state == 1:
                 sp_ex = l_ex.strip ().split ()
                 sp_ac = l_ac.strip ().split ()
                 if len (sp_ex) != 5 or sp_ex [0] in 'JE':
                     state = 2
-                    self.assertEqual (l_ex, l_ac)
+                    assert l_ex == l_ac
                     continue
                 num_ex = [float (x) for x in sp_ex]
                 num_ac = [float (x) for x in sp_ac]
-                self.assertEqual (num_ex [0], num_ac [0])
+                assert num_ex [0] == num_ac [0]
                 for a, b in zip (num_ex [1:-1], num_ac [1:-1]):
-                    self.assertAlmostEqual (a, b, 12)
-                self.assertAlmostEqual (num_ex [-1], num_ac [-1], 10)
+                    assert round (abs (a - b), 12) == 0
+                assert round (abs (num_ex [-1] - num_ac [-1]), 10) == 0
     # end def compare_currents
 
     def compare_near_field_data (self, m, opts = None):
         """ Near field data below absolute values of 1e-15 may be
             different on different architectures
         """
         if opts is None:
@@ -299,177 +304,216 @@
         l   = len (self.expected_output [:idx].split ('\n'))
         off = l - 2
         self.compare_currents ('\n'.join (ex [:off]), '\n'.join (ac [:off]))
         for e, a in zip (ex [off:], ac [off:]):
             el = e.strip ().split ()
             al = a.strip ().split ()
             if not el:
-                self.assertEqual (e, a)
+                assert e == a
                 continue
             if el [0] in 'XYZ':
                 fe = [float (x) for x in el [1:]]
                 fa = [float (x) for x in al [1:]]
                 found = False
                 for n, (ffe, ffa) in enumerate (zip (fe, fa)):
                     # Don't compare angle if below threshold
                     if found and n == 3:
                         continue
                     if ffe != 0 and abs (ffe) < 1e-15:
-                        self.assertLess (abs (ffa), 1e-15)
+                        assert abs (ffa) < 1e-15
                         found = True
                     else:
-                        self.assertEqual (ffe, ffa)
+                        assert ffe == ffa
             else:
-                self.assertEqual (e, a)
+                assert e == a
     # end def compare_near_field_data
 
+    def setup_generic_file (self, basename, azi = None, ele = None):
+        path = os.path.join ('test', basename)
+        pym  = path + '.pym'
+        args = []
+        with open (pym, 'r') as f:
+            for line in f:
+                if line.startswith ('#'):
+                    continue
+                args.append (line)
+        args = ' '.join (args)
+        args = args.split ()
+        m    = main (args, return_mininec = True)
+        self.simple_setup (basename + '.pout')
+        elevation = ele or Angle (0, 10, 10)
+        azimuth   = azi or Angle (0, 10, 37)
+        m.compute ()
+        m.compute_far_field (elevation, azimuth)
+        return m
+    # end def setup_generic_file
+
 # end class _Test_Base_With_File
 
-class Test_Case_Known_Structure (_Test_Base_With_File, unittest.TestCase):
+class Test_Case_Known_Structure (_Test_Base_With_File):
 
     def test_excitation (self):
         """ Test error cases
         """
-        self.assertRaises (ValueError, Excitation, 1+1j, 1)
+        with pytest.raises (ValueError):
+            Excitation (1+1j, 1)
         w = []
         w.append (Wire (10, 0, 0, 0, 21.414285, 0, 0, 0.01))
         m = Mininec (7, w)
         x = Excitation (cvolt = 5)
         # Pulse index must be > 0
-        self.assertRaises (ValueError, m.register_source, x, -1)
+        with pytest.raises (ValueError):
+            m.register_source (x, -1)
         # Invalid pulse
-        self.assertRaises (ValueError, m.register_source, x, 55)
+        with pytest.raises (ValueError):
+            m.register_source (x, 55)
         # Invalid pulse for wire
-        self.assertRaises (ValueError, m.register_source, x, 11, 0)
+        with pytest.raises (ValueError):
+            m.register_source (x, 11, 0)
         # Invalid *first* pulse:
         # We create two 1-seg wires, the first will have no pulse
         w = []
         w.append (Wire (1, 0, 0, 0, 1, 0, 0, 0.01))
         w.append (Wire (1, 1, 0, 0, 2, 0, 0, 0.01))
         m = Mininec (7, w)
-        self.assertRaises (ValueError, m.register_source, x, 0, 0)
+        with pytest.raises (ValueError):
+            m.register_source (x, 0, 0)
     # end def test_excitation
 
     def test_load (self):
         """ Test error case
         """
-        self.assertRaises (ValueError, Laplace_Load, [], [])
+        with pytest.raises (ValueError):
+            Laplace_Load ([], [])
     # end def test_load
 
     def test_medium (self):
         """ Test error cases
         """
-        self.assertRaises (ValueError, Medium, 0, 0, nradials = 1)
-        self.assertRaises (ValueError, Medium, 0, 0, height = 1)
-        self.assertRaises (ValueError, Medium, 1, 1, nradials = 1)
-        self.assertRaises (ValueError, Medium, 1, 0)
-        self.assertRaises \
-            (ValueError, Medium, 1, 1, nradials = 1, coord = 5, dist = 7)
+        with pytest.raises (ValueError):
+            Medium (0, 0, nradials = 1)
+        with pytest.raises (ValueError):
+            Medium (0, 0, height = 1)
+        with pytest.raises (ValueError):
+            Medium (1, 1, nradials = 1)
+        with pytest.raises (ValueError):
+            Medium (1, 0)
+        with pytest.raises (ValueError):
+            Medium (1, 1, nradials = 1, coord = 5, dist = 7)
         w = []
         w.append (Wire (10, 0, 0, 0, 21.414285, 0, 0, 0.01))
-        self.assertRaises (ValueError, Mininec, 7, w, media = [])
+        with pytest.raises (ValueError):
+            Mininec (7, w, media = [])
         ideal = ideal_ground
         media = [ideal, ideal]
-        self.assertRaises (ValueError, Mininec, 7, w, media = media)
+        with pytest.raises (ValueError):
+            Mininec (7, w, media = media)
         rad = Medium (1, 1, nradials = 1, radius = 1, dist = 1)
         media = [rad, rad]
-        self.assertRaises (ValueError, Mininec, 7, w, media = media)
+        with pytest.raises (ValueError):
+            Mininec (7, w, media = media)
         # Radials may not be the only medium
-        self.assertRaises (ValueError, Mininec, 7, w, media = [rad])
+        with pytest.raises (ValueError):
+            Mininec (7, w, media = [rad])
     # end def test_medium
 
     def test_wire (self):
         """ Test error cases
         """
-        self.assertRaises (ValueError, Wire, 7, 1, 1, 1, 2, 2, 2, 0)
-        self.assertRaises (ValueError, Wire, 7, 1, 1, 1, 1, 1, 1, 1)
+        with pytest.raises (ValueError):
+            Wire (7, 1, 1, 1, 2, 2, 2, 0)
+        with pytest.raises (ValueError):
+            Wire (7, 1, 1, 1, 1, 1, 1, 1)
         wire = Wire (7, 0, 0, 0, 1, 1, 0, 0.01)
         ideal = ideal_ground
-        self.assertRaises (ValueError, wire.compute_ground, 0, ideal)
+        with pytest.raises (ValueError):
+            wire.compute_ground (0, ideal)
         wire = Wire (7, 0, 0, -1, 1, 1, -1, 0.01)
-        self.assertRaises (ValueError, wire.compute_ground, 0, ideal)
+        with pytest.raises (ValueError):
+            wire.compute_ground (0, ideal)
     # end def test_excitation
 
     def test_source_index (self):
         w = []
         w.append (Wire (10, 0, 0, 0, 21.414285, 0, 0, 0.01))
         # Wrong index: Exceeds valid segments
         s = Excitation (1, 0)
         m = Mininec (7, w)
-        self.assertRaises (ValueError, m.register_source, s, 10)
+        with pytest.raises (ValueError):
+            m.register_source (s, 10)
     # end def test_source_index
 
     def test_matrix_fill_vdipole_ideal_ground (self):
-        """ This uses assertAlmostEqual number of decimal places to
-            compare significant digits (approximately)
+        """ This uses rounding to a number of decimal places to compare
+            significant digits (approximately)
         """
         mat   = matrix_ideal_ground_vdipole_from_mininec
         ideal = ideal_ground
         m = self.vertical_dipole \
             (wire_dia = 0.01, filename = None, media = [ideal])
         for i in range (len (m.w_per)):
             for j in range (len (m.w_per)):
                 f = int (np.log (abs (mat [i][j].real)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].real, m.Z [i][j].real, 3-f)
+                assert round (abs (mat [i][j].real - m.Z [i][j].real), 3-f) == 0
                 f = int (np.log (abs (mat [i][j].imag)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].imag, m.Z [i][j].imag, 3-f)
+                assert round (abs (mat [i][j].imag - m.Z [i][j].imag), 3-f) == 0
     # end def test_matrix_fill_vdipole_ideal_ground
 
     def test_matrix_fill_quarter_ideal_ground (self):
-        """ This uses assertAlmostEqual number of decimal places to
-            compare significant digits (approximately)
+        """ This uses rounding to a number of decimal places to compare
+            significant digits (approximately)
         """
         mat   = np.array (matrix_ideal_ground_quarter_from_mininec_r) \
               + 1j * np.array (matrix_ideal_ground_quarter_from_mininec_i)
         ideal = [ideal_ground]
         m = self.vertical_quarterwave (filename = None, media = ideal)
         for i in range (len (m.w_per)):
             for j in range (len (m.w_per)):
                 f = int (np.log (abs (mat [i][j].real)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].real, m.Z [i][j].real, 3-f)
+                assert round (abs (mat [i][j].real - m.Z [i][j].real), 3-f) == 0
                 f = int (np.log (abs (mat [i][j].imag)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].imag, m.Z [i][j].imag, 3-f)
+                assert round (abs (mat [i][j].imag - m.Z [i][j].imag), 3-f) == 0
     # end def test_matrix_fill_quarter_ideal_ground
 
     def test_matrix_fill_quarter_ideal_ground_load (self):
-        """ This uses assertAlmostEqual number of decimal places to
-            compare significant digits (approximately)
+        """ This uses rounding to a number of decimal places to compare
+            significant digits (approximately)
         """
         mat   = np.array (matrix_ideal_ground_quarter_l_from_mininec_r) \
               + 1j * np.array (matrix_ideal_ground_quarter_l_from_mininec_i)
         ideal = [ideal_ground]
         l = Laplace_Load (b = (1., 0), a = (0., -2.193644e-9))
         m = self.vertical_quarterwave \
             (filename = None, media = ideal, load = l, dia = 0.002)
         for i in range (len (m.w_per)):
             for j in range (1, len (m.w_per)):
                 f = int (np.log (abs (mat [i][j].real)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].real, m.Z [i][j].real, 3-f)
+                assert round (abs (mat [i][j].real - m.Z [i][j].real), 3-f) == 0
                 f = int (np.log (abs (mat [i][j].imag)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].imag, m.Z [i][j].imag, 3-f)
+                assert round (abs (mat [i][j].imag - m.Z [i][j].imag), 3-f) == 0
     # end def test_matrix_fill_quarter_ideal_ground_load
 
     def test_matrix_fill_inverted_l (self):
-        """ This uses assertAlmostEqual number of decimal places to
-            compare significant digits (approximately)
+        """ This uses rounding to a number of decimal places to compare
+            significant digits (approximately)
         """
         mat   = np.array (matrix_inverted_l_r) \
               + 1j * np.array (matrix_inverted_l_i)
         m = self.inverted_l (filename = None)
         for i in range (len (m.w_per)):
             for j in range (len (m.w_per)):
                 f = int (np.log (abs (mat [i][j].real)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].real, m.Z [i][j].real, 3-f)
+                assert round (abs (mat [i][j].real - m.Z [i][j].real), 3-f) == 0
                 f = int (np.log (abs (mat [i][j].imag)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].imag, m.Z [i][j].imag, 3-f)
+                assert round (abs (mat [i][j].imag - m.Z [i][j].imag), 3-f) == 0
     # end def test_matrix_fill_inverted_l
 
     def test_matrix_fill_quarter_radials (self):
-        """ This uses assertAlmostEqual number of decimal places to
-            compare significant digits (approximately)
+        """ This uses rounding to a number of decimal places to compare
+            significant digits (approximately)
             Note that the matrix is identical to the ideal ground case.
             This is because mininec computes the currents in the wires
             using ideal ground (which in turn make problems with wires
             too near to ground with a parallel component).
         """
         mat   = np.array (matrix_ideal_ground_quarter_from_mininec_r) \
               + 1j * np.array (matrix_ideal_ground_quarter_from_mininec_i)
@@ -477,79 +521,79 @@
         m2 = Medium (5, 0.001, -5)
         media = [m1, m2]
         m = self.vertical_quarterwave \
             (filename = 'vertical-rad.pout', media = media)
         for i in range (len (m.w_per)):
             for j in range (len (m.w_per)):
                 f = int (np.log (abs (mat [i][j].real)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].real, m.Z [i][j].real, 3-f)
+                assert round (abs (mat [i][j].real - m.Z [i][j].real), 3-f) == 0
                 f = int (np.log (abs (mat [i][j].imag)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].imag, m.Z [i][j].imag, 3-f)
+                assert round (abs (mat [i][j].imag - m.Z [i][j].imag), 3-f) == 0
     # end def test_matrix_fill_quarter_radials
 
     def test_matrix_fill_ohio_example (self):
-        """ This uses assertAlmostEqual number of decimal places to
-            compare significant digits (approximately)
+        """ This uses rounding to a number of decimal places to compare
+            significant digits (approximately)
             Note that the matrix is identical to the ideal ground case.
             This is because mininec computes the currents in the wires
             using ideal ground (which in turn make problems with wires
             too near to ground with a parallel component).
         """
         mat = np.array (matrix_ohio_r) + 1j * np.array (matrix_ohio_i)
         nfc = Near_Far_Comparison ()
         m   = nfc.m
         for i in range (len (m.w_per)):
             for j in range (len (m.w_per)):
                 f = int (np.log (abs (mat [i][j].real)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].real, m.Z [i][j].real, 3-f)
+                assert round (abs (mat [i][j].real - m.Z [i][j].real), 3-f) == 0
                 f = int (np.log (abs (mat [i][j].imag)) / np.log (10))
-                self.assertAlmostEqual (mat [i][j].imag, m.Z [i][j].imag, 3-f)
+                assert round (abs (mat [i][j].imag - m.Z [i][j].imag), 3-f) == 0
     # end def test_matrix_fill_ohio_example
 
     def test_dipole_wiredia_01 (self):
         m = self.dipole_7mhz (wire_dia = 0.01, filename = 'dipole-01.pout')
         out = m.as_mininec ()
-        self.assertEqual (self.expected_output, out)
+        assert self.expected_output == out
     # end def test_dipole_wiredia_01
 
     def test_dipole_wiredia_001 (self):
         m = self.dipole_7mhz (wire_dia = 0.001, filename = 'dipole-001.pout')
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_dipole_wiredia_001
 
     def test_vdipole_wiredia_01 (self):
         m = self.vertical_dipole (wire_dia = 0.01, filename = 'vdipole-01.pout')
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vdipole_wiredia_01
 
     def test_vdipole_wiredia_01_ground (self):
         ideal = [ideal_ground]
         m = self.vertical_dipole \
             (wire_dia = 0.01, filename = 'vdipole-01g0.pout', media = ideal)
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vdipole_wiredia_01_ground
 
     def test_vdipole_wiredia_01_ground_loaded (self):
         ideal = [ideal_ground]
         load  = Impedance_Load (2e-6)
         m = self.vertical_dipole \
             ( wire_dia = 0.01
             , filename = 'vdipole-01g0l.pout'
             , media    = ideal
             , load     = load
             )
         # Attach to *all* segments
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vdipole_wiredia_01_ground_loaded
 
     def test_vdipole_wiredia_001_ground (self):
         ideal = [ideal_ground]
         m = self.vertical_dipole \
             (wire_dia = 0.001, filename = 'vdipole-001g0.pout', media = ideal)
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vdipole_wiredia_001_ground
 
     def test_vdipole_wiredia_01_avg_ground (self):
         """ This test computes different results on Intel vs. AMD
             processors. The gain at 90° theta falls below the -300 dBi
             cutoff point on AMD while it is about -297 dBi on Intel.
             This is probably due to differences in sin/cos and/or
@@ -573,34 +617,34 @@
         m = self.folded_dipole ('folded-18.pout')
         self.compare_far_field_data (m, may_fail_last_digit = True)
     # end def test_folded_dipole
 
     def test_vertical_ideal_ground (self):
         ideal = [ideal_ground]
         m = self.vertical_quarterwave ('vertical-ig.pout', ideal)
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vertical_ideal_ground
 
     def test_vertical_ideal_ground_upside_down (self):
         ideal = [ideal_ground]
         m = self.vertical_quarterwave ('vertical-ig-ud.pout', ideal, inv = True)
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vertical_ideal_ground_upside_down
 
     def test_vertical_radials (self):
         m1 = Medium (20, .0303, 0, coord = 5, nradials = 16, radius = 0.001)
         m2 = Medium (5, 0.001, -5)
         media = [m1, m2]
         m = self.vertical_quarterwave ('vertical-rad.pout', media = media)
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_vertical_radials
 
     def test_inverted_l (self):
         m = self.inverted_l ('inv-l.pout')
-        self.assertEqual (self.expected_output, m.as_mininec ())
+        assert self.expected_output == m.as_mininec ()
     # end def test_inverted_l
 
     def test_t_ant (self):
         m = self.t_antenna ('t-ant.pout')
         self.compare_far_field_data (m)
     # end def test_t_ant
 
@@ -611,15 +655,15 @@
 
     def test_dipole_wiredia_01_near (self):
         m = self.dipole_7mhz (wire_dia = 0.01, filename = 'dipole-01-near.pout')
         opts = set (('near-field',))
         #with open ('z.out', 'w') as f:
         #    print (m.as_mininec (opts).rstrip (), file = f)
         actual_output = m.as_mininec (opts).rstrip ()
-        self.assertEqual (self.expected_output, actual_output)
+        assert self.expected_output == actual_output
     # end def test_dipole_wiredia_01_near
 
     def test_vertical_ideal_ground_near (self):
         ideal = [ideal_ground]
         l = Laplace_Load (b = (0., 225.998e-9), a = (1., 0.))
         m = self.vertical_quarterwave \
             ('vertical-ig-near.pout', ideal, dia = 0.002, load = l)
@@ -629,44 +673,78 @@
     def test_vertical_ideal_ground_far_abs (self):
         ideal = [ideal_ground]
         opt = dict (pwr = 100, dist = 1000)
         m = self.vertical_quarterwave \
             ('vertical-ig-ffabs.pout', ideal, opt = opt)
         opts = set (('far-field-absolute',))
         actual_output = m.as_mininec (opts).rstrip ()
-        self.assertEqual (self.expected_output, actual_output)
+        assert self.expected_output == actual_output
     # end def test_vertical_ideal_ground_far_abs
 
     def test_near_far (self):
         r = []
         nfc = Near_Far_Comparison ()
         r.append (nfc.output_currents ())
         r.append (nfc.output_near ())
         r.append (nfc.output_far  ())
         actual_output = '\n'.join (r).rstrip ()
         with open (os.path.join ('test', 'ohio.pout'), 'r') as f:
             self.expected_output = f.read ().rstrip ()
-        self.assertEqual (self.expected_output, actual_output)
+        assert self.expected_output == actual_output
     # end def test_near_far
 
+    def test_hloop40_14 (self):
+        m = self.setup_generic_file ('hloop40-14')
+        self.compare_far_field_data (m)
+    # end def test_hloop40_14
+
+    def test_hloop40_7 (self):
+        m = self.setup_generic_file ('hloop40-7')
+        self.compare_far_field_data (m)
+    # end def test_hloop40_7
+
+    def test_vloop20 (self):
+        m = self.setup_generic_file ('vloop20')
+        self.compare_far_field_data (m, may_fail_last_digit = True)
+    # end def test_vloop20
+
+    def test_lzh20 (self):
+        m = self.setup_generic_file ('lzh20')
+        self.compare_far_field_data (m)
+    # end def test_lzh20
+
+    def test_inve802B (self):
+        self.maxDiff = None
+        ele = Angle (0, 11, 9)
+        m   = self.setup_generic_file ('inve802B', ele = ele)
+        opt = set (['far-field'])
+        out =  m.frq_independent_as_mininec ()  + '\n'
+        out += m.frq_dependent_as_mininec (opt) + '\n'
+        m.f = 14
+        m.compute ()
+        m.compute_far_field (ele, Angle (0, 10, 37))
+        out += m.frq_dependent_as_mininec (opt)
+        assert self.expected_output == out
+    # end def test_inve802B
+
 # end class Test_Case_Known_Structure
 
-class Test_Doctest (unittest.TestCase):
+class Test_Doctest:
 
     flags = doctest.NORMALIZE_WHITESPACE
 
     def test_mininec (self):
-        num_tests = 307
+        num_tests = 340
         f, t  = doctest.testmod \
             (mininec.mininec, verbose = False, optionflags = self.flags)
         fn = os.path.basename (mininec.mininec.__file__)
         format_ok  = '%(fn)s passes all of %(t)s doc-tests'
         format_nok = '%(fn)s fails %(f)s of %(t)s doc-tests'
         if f:
             msg = format_nok % locals ()
         else:
             msg = format_ok % locals ()
         exp = 'mininec.py passes all of %d doc-tests' % num_tests
-        self.assertEqual (exp, msg)
+        assert exp == msg
     # end def test_mininec
 
 # end class Test_Doctest
```

