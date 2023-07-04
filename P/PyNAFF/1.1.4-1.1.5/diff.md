# Comparing `tmp/PyNAFF-1.1.4.tar.gz` & `tmp/PyNAFF-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyNAFF-1.1.4.tar", last modified: Wed Jul 18 07:54:39 2018, max compression
+gzip compressed data, was "PyNAFF-1.1.5.tar", last modified: Tue Jul  4 05:38:55 2023, max compression
```

## Comparing `PyNAFF-1.1.4.tar` & `PyNAFF-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 nkarast    (501) staff       (20)        0 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/
--rw-r--r--   0 nkarast    (501) staff       (20)     1703 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PKG-INFO
-drwxr-xr-x   0 nkarast    (501) staff       (20)        0 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF.egg-info/
--rw-r--r--   0 nkarast    (501) staff       (20)     1703 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF.egg-info/PKG-INFO
--rw-r--r--   0 nkarast    (501) staff       (20)      204 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF.egg-info/SOURCES.txt
--rw-r--r--   0 nkarast    (501) staff       (20)       13 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF.egg-info/requires.txt
--rw-r--r--   0 nkarast    (501) staff       (20)        7 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF.egg-info/top_level.txt
--rw-r--r--   0 nkarast    (501) staff       (20)        1 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF.egg-info/dependency_links.txt
--rw-r--r--   0 nkarast    (501) staff       (20)      958 2018-07-18 07:53:24.000000 PyNAFF-1.1.4/setup.py
-drwxr-xr-x   0 nkarast    (501) staff       (20)        0 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/PyNAFF/
--rw-r--r--   0 nkarast    (501) staff       (20)     9240 2018-07-18 07:52:10.000000 PyNAFF-1.1.4/PyNAFF/PyNAFF.py
--rw-r--r--   0 nkarast    (501) staff       (20)       44 2018-07-18 07:52:13.000000 PyNAFF-1.1.4/PyNAFF/__init__.py
--rw-r--r--   0 nkarast    (501) staff       (20)       38 2018-07-18 07:54:39.000000 PyNAFF-1.1.4/setup.cfg
--rw-r--r--   0 nkarast    (501) staff       (20)     1069 2018-07-18 07:49:37.000000 PyNAFF-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:55.398022 PyNAFF-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35077 2023-07-04 05:38:46.000000 PyNAFF-1.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-04 05:38:55.398022 PyNAFF-1.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:55.398022 PyNAFF-1.1.5/PyNAFF/
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-04 05:38:46.000000 PyNAFF-1.1.5/PyNAFF/PyNAFF.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 05:38:46.000000 PyNAFF-1.1.5/PyNAFF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:55.398022 PyNAFF-1.1.5/PyNAFF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-04 05:38:55.000000 PyNAFF-1.1.5/PyNAFF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-04 05:38:55.000000 PyNAFF-1.1.5/PyNAFF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:38:55.000000 PyNAFF-1.1.5/PyNAFF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 05:38:55.000000 PyNAFF-1.1.5/PyNAFF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 05:38:55.000000 PyNAFF-1.1.5/PyNAFF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-04 05:38:46.000000 PyNAFF-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 05:38:55.398022 PyNAFF-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-04 05:38:46.000000 PyNAFF-1.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyNAFF-1.1.4/PyNAFF/PyNAFF.py` & `PyNAFF-1.1.5/PyNAFF/PyNAFF.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
-try:
-	from builtins import range, int
-except ImportError:
-	from __builtin__ import range, int
 import numpy as np
+import math
+from warnings import warn, simplefilter
+simplefilter("ignore", np.ComplexWarning)  # suppress persisting cast to complex warnings from numpy
 """
 # NAFF - Numerical Analysis of Fundamental Frequencies
-# Version : 1.1.4
+# Version : 1.1.5
 # Authors : F. Asvesta, N. Karastathis, P.Zisopoulos
-# Contact : nkarast .at. cern .dot. ch
+# Contact : fasvesta@cern.ch
 #
 """
 
-__version   = '1.1.4'
-__PyVersion = [2.7, 3.6]
-__authors   = ['F. Asvesta','N. Karastathis', 'P. Zisopoulos']
-__contact   = ['nkarast .at. cern .dot. ch']
+__version = '1.1.5'
+__PyVersion = [2.7, 3.7]
+__authors = {'F. Asvesta': 'fasvesta@cern.ch',
+			  'N. Karastathis': 'nkarast@gmail.com',
+			  'P. Zisopoulos': 'pzisopou@cern.ch'
+			}
 
-
-def naff(data, turns=300, nterms=1, skipTurns=0, getFullSpectrum=False, window=1):
+def naff(data, turns=300, nterms=1, skipTurns=0, getFullSpectrum=False, window=1, tol=1e-4, warnings=True):
 	'''
 	The driving function for the NAFF algorithm.
 	Inputs :
 	*  data : NumPy array with TbT data
 	*  turns : number of points to consider from the input data
 	*  nterms : maximum number of harmonics to search for in the data sample
 	*  skipTurns : number of observations (data points) to skip from the start of the input iterable
 	*  getFullSpectrum : [True | False]
 					  If True, a normal FFT is used (both negative and positive frequencies)
 					  If False, an rFFT is used (only positive frequencies)
 	*  window : the order of window to be applied on the input data (default =1)
+	*  tol : Expert setting to increase the acceptance window for the harmonics, as long as `getFullSpectrum=True`.
+	         Higher values should let NAFF recover more frequencies, but the maximum number will always be `nterms`.
+	         Default value should be 1e-4.
+
 	Returns : Array with frequencies and amplitudes in the format:
 		  [order of harmonic, frequency, Amplitude, Re{Amplitude}, Im{Amplitude}]
 	'''
 	if turns >= len(data)+1:
 		raise ValueError('#naff : Input data must be at least of length turns+1.')
 	if turns < 6:
 		raise ValueError('#naff : Minimum number of turns is 6.')
@@ -129,23 +132,22 @@
 			else:
 				break
 		return X2, Y2, A2, B2
 	# - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - -
 	def fretes(FR, FREFON):
 		'''
 		If more than one term found, check how different they are
-		'''
-		TOL   = 1.0e-4 # this is defined in mftnaf in lashkar
+                '''
 		IFLAG = 1
 		NUMFR = 0
 		ECART = np.abs(FREFON)
 		for i in range(len(vars['TFS'])):
 			TEST = np.abs(vars['TFS'][i] - FR)
 			if TEST < ECART:
-				if np.float(TEST)/np.float(ECART) < TOL:
+				if float(TEST)/float(ECART) < tol: # tolerance value was 1e-4 in Laskar's original work.
 					IFLAG = -1
 					NUMFR = i
 					break
 				else:
 					IFLAG = 0
 					continue
 		return IFLAG, NUMFR
@@ -204,15 +206,15 @@
 		vars['ZALP'][NF-1, NF-1] = 1.0+0.0j
 		DIV  = 1.0
 		ZDIV = 0.0+0.0j
 		for i in range(0, NF):
 			ZDIV = ZDIV + np.conj(vars['ZALP'][NF-1, i])*ZTEE[i]
 		DIV = np.sqrt(np.abs(ZDIV))
 		vars['ZALP'][NF-1,:] = vars['ZALP'][NF-1,:]/DIV
-		ZMUL = np.complex(A,B)/DIV
+		ZMUL = complex(A,B)/DIV
 		ZI = 0.0+1.0j
 
 		for i in range(0, NF):
 			ZOM = 1.0j*vars['TFS'][i]
 			ZA  = vars['ZALP'][NF-1,i]*ZMUL
 			vars['ZAMP'][i] = vars['ZAMP'][i]+ZA
 			ZT_zero = np.array([ZA])
@@ -225,32 +227,31 @@
 	# - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - - * - -
 	FREFON = 1.0/turns
 	NEPS   = 100000000
 	EPS    = FREFON/NEPS
 
 	T    = np.linspace(0, turns, num=turns+1, endpoint=True)*2.0*np.pi - np.pi*turns
 	vars['TWIN'] = 1.0+np.cos(T/turns)
-	vars['TWIN'] = ((2.0**window*np.math.factorial(window)**2)/float(np.math.factorial(2*window)))*(1.0+np.cos(T/turns))**window
+	vars['TWIN'] = ((2.0**window*math.factorial(window)**2)/float(math.factorial(2*window)))*(1.0+np.cos(T/turns))**window
 	vars['ZTABS'] = data[skipTurns:skipTurns+turns+1]
 
-	TOL = 1.0e-4
 	STAREP = FREFON/3.0
 	for term in range(nterms):
 		data_for_fft = np.multiply(vars['ZTABS'], vars['TWIN'])[:-1] # .astype('complex128')
 		if getFullSpectrum:
 			y = np.fft.fft(data_for_fft)
 		else:
-			y = np.fft.rfft(data_for_fft.astype('float64'))
+			y = np.fft.rfft(data_for_fft)
 
 		RTAB = np.sqrt(np.real(y)**2 + np.imag(y)**2)/turns  # normalized
 		INDX = np.argmax(RTAB)
 		VMAX = np.max(RTAB)
 
-		if INDX == 0 :
-			print('## PyNAFF::naff: Remove the DC component from the data (i.e. the mean).')
+		if INDX == 0 and warnings:
+			warn('## PyNAFF::naff: Remove the DC component from the data (i.e. the mean).')
 		if INDX <= turns/2.0:
 			IFR = INDX - 1
 		else:
 			IFR = INDX-1-turns
 
 		FR = (IFR+1)*FREFON
 		FR, RMD, A, B = frefin(turns, FR, STAREP, EPS)
@@ -272,10 +273,13 @@
 
 
 ### - - - ### - - - ### - - - ### - - - ### - - - ### - - - ### - - - ### - - - ### - - - ### - - - ###
 
 # Example
 if __name__ == '__main__':
 	x = np.linspace(1, 500, num=500, endpoint=True)
-	data = np.sin(2.0*np.pi*0.34*x)+np.sin(2.0*np.pi*0.36*x)
-	a = naff(data, 300, 20, 0, False)
-	print(a)
+	f0, a0 = [0.31, 0.32, 0.33, 0.34, 0.34 + 0.016, 0.34 - 0.016], [1, 0.5, 0.25, 0.12, 0.06, 0.03]
+	data = np.array(sum([a * np.sin(2.0 * np.pi * (q * x)) for q, a in zip(f0, a0)]))
+	a = naff(data, 300, 20, 0, True)
+	print(f"Frequencies:\n{a[:,1]}")
+	print(f"Amplitudes:\n{a[:, 2]}")
+
```

