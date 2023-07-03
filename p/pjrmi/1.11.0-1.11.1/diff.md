# Comparing `tmp/pjrmi-1.11.0.tar.gz` & `tmp/pjrmi-1.11.1.tar.gz`

## Comparing `pjrmi-1.11.0.tar` & `pjrmi-1.11.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0   295812 2020-02-02 00:00:00.000000 pjrmi-1.11.0/pjrmi/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pjrmi-1.11.0/pjrmi/_config.py
--rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 pjrmi-1.11.0/pjrmi/_util.py
--rw-r--r--   0        0        0   726928 2020-02-02 00:00:00.000000 pjrmi-1.11.0/pjrmi/lib/pjrmi.jar
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pjrmi-1.11.0/.gitignore
--rw-r--r--   0        0        0    26186 2020-02-02 00:00:00.000000 pjrmi-1.11.0/README.md
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pjrmi-1.11.0/pyproject.toml
--rw-r--r--   0        0        0    27413 2020-02-02 00:00:00.000000 pjrmi-1.11.0/PKG-INFO
+-rw-r--r--   0        0        0   295812 2020-02-02 00:00:00.000000 pjrmi-1.11.1/pjrmi/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pjrmi-1.11.1/pjrmi/_config.py
+-rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 pjrmi-1.11.1/pjrmi/_util.py
+-rw-r--r--   0        0        0   726928 2020-02-02 00:00:00.000000 pjrmi-1.11.1/pjrmi/lib/pjrmi.jar
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pjrmi-1.11.1/.gitignore
+-rw-r--r--   0        0        0    26186 2020-02-02 00:00:00.000000 pjrmi-1.11.1/README.md
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pjrmi-1.11.1/pyproject.toml
+-rw-r--r--   0        0        0    27434 2020-02-02 00:00:00.000000 pjrmi-1.11.1/PKG-INFO
```

### Comparing `pjrmi-1.11.0/pjrmi/__init__.py` & `pjrmi-1.11.1/pjrmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pjrmi-1.11.0/pjrmi/_util.py` & `pjrmi-1.11.1/pjrmi/_util.py`

 * *Files identical despite different names*

### Comparing `pjrmi-1.11.0/pjrmi/lib/pjrmi.jar` & `pjrmi-1.11.1/pjrmi/lib/pjrmi.jar`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,192 +1,192 @@
 Zip file size: 726928 bytes, number of entries: 243
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-03 18:24 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/io/
--rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-03 18:24 com/deshaw/io/BlockingPipe.class
--rw-rw-r--  2.0 unx      792 b- defN 23-Jul-03 18:24 com/deshaw/io/BlockingPipe$Output.class
--rw-rw-r--  2.0 unx      752 b- defN 23-Jul-03 18:24 com/deshaw/io/BlockingPipe$Input.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/
--rw-rw-r--  2.0 unx     5916 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/AsType.class
--rw-rw-r--  2.0 unx      124 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/JavaProxyBase.class
--rw-rw-r--  2.0 unx    11977 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/JniPJRmi.class
--rw-rw-r--  2.0 unx      757 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/JniPJRmi$ArrayHandle.class
--rw-rw-r--  2.0 unx     2344 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PipedProvider.class
--rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PipedProvider$BidirectionalPipe.class
--rw-rw-r--  2.0 unx     3095 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PipedProvider$PipedPJRmi.class
--rw-rw-r--  2.0 unx     1922 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PipedTransport.class
--rw-rw-r--  2.0 unx     6019 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonMinionProvider.class
--rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonMinionProvider$1.class
--rw-rw-r--  2.0 unx     5605 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonMinionTransport.class
--rw-rw-r--  2.0 unx     1498 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonSlice.class
--rw-rw-r--  2.0 unx     5353 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SSLSocketProvider.class
--rw-rw-r--  2.0 unx     1002 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonKwargsFunction.class
--rw-rw-r--  2.0 unx      442 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonFunction.class
--rw-rw-r--  2.0 unx     5307 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject.class
--rw-rw-r--  2.0 unx     2044 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$8.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$7.class
--rw-rw-r--  2.0 unx     1992 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$6.class
--rw-rw-r--  2.0 unx     1915 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$5.class
--rw-rw-r--  2.0 unx     2169 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$4.class
--rw-rw-r--  2.0 unx     2092 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$3.class
--rw-rw-r--  2.0 unx     2142 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$2.class
--rw-rw-r--  2.0 unx     1884 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonObject$1.class
--rw-rw-r--  2.0 unx      493 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonCallbackException.class
--rw-rw-r--  2.0 unx     2144 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonMinion.class
--rw-rw-r--  2.0 unx     1171 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PythonMinion$ByValue.class
--rw-rw-r--  2.0 unx     3228 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SSLSocketTransport.class
--rw-rw-r--  2.0 unx    25886 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi.class
--rw-rw-r--  2.0 unx     2986 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$3.class
--rw-rw-r--  2.0 unx     1274 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$2.class
--rw-rw-r--  2.0 unx      621 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$1.class
--rw-rw-r--  2.0 unx    67472 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection.class
--rw-rw-r--  2.0 unx     5136 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$3.class
--rw-rw-r--  2.0 unx     1730 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$2.class
--rw-rw-r--  2.0 unx     1626 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$1.class
--rw-rw-r--  2.0 unx     8176 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl.class
--rw-rw-r--  2.0 unx     7829 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler.class
--rw-rw-r--  2.0 unx     6602 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler.class
--rw-rw-r--  2.0 unx     2750 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate.class
--rw-rw-r--  2.0 unx     2646 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate.class
--rw-rw-r--  2.0 unx     2411 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer.class
--rw-rw-r--  2.0 unx     2310 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer.class
--rw-rw-r--  2.0 unx     2427 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction.class
--rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction.class
--rw-rw-r--  2.0 unx     2330 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator.class
--rw-rw-r--  2.0 unx     2014 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable.class
--rw-rw-r--  2.0 unx     5853 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallback.class
--rw-rw-r--  2.0 unx     1393 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult.class
--rw-rw-r--  2.0 unx     2125 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle.class
--rw-rw-r--  2.0 unx     3730 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$MethodCaller.class
--rw-rw-r--  2.0 unx     8410 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Connection$Worker.class
--rw-rw-r--  2.0 unx      234 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$ThreadId.class
--rw-rw-r--  2.0 unx     1146 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream.class
--rw-rw-r--  2.0 unx      788 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.class
--rw-rw-r--  2.0 unx      995 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$ClassInjector.class
--rw-rw-r--  2.0 unx     3608 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$HandleMapping.class
--rw-rw-r--  2.0 unx      697 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.class
--rw-rw-r--  2.0 unx     3891 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$TypeMapping.class
--rw-rw-r--  2.0 unx     4206 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MethodDescription.class
--rw-rw-r--  2.0 unx     2631 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.class
--rw-rw-r--  2.0 unx     3177 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MethodCallFuture.class
--rw-rw-r--  2.0 unx     2237 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$SyncMode.class
--rw-rw-r--  2.0 unx     1766 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MethodFlags.class
--rw-rw-r--  2.0 unx     1964 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$FieldDescription.class
--rw-rw-r--  2.0 unx      585 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$ReadObjectResult.class
--rw-rw-r--  2.0 unx     1242 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MethodSignature.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MethodComparator.class
--rw-rw-r--  2.0 unx     5930 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$WrappedArrayLike.class
--rw-rw-r--  2.0 unx     1480 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator.class
--rw-rw-r--  2.0 unx      420 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$ArrayLike.class
--rw-rw-r--  2.0 unx      343 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PythonItemAssignable.class
--rw-rw-r--  2.0 unx      487 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PythonSubscriptable.class
--rw-rw-r--  2.0 unx    17628 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$TypeDescription.class
--rw-rw-r--  2.0 unx     1585 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$TypeFlags.class
--rw-rw-r--  2.0 unx     2640 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PythonValueFormat.class
--rw-rw-r--  2.0 unx     4710 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$MessageType.class
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$Flags.class
--rw-rw-r--  2.0 unx      496 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$GenericReturnType.class
--rw-rw-r--  2.0 unx     7296 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PJRmiLockManager.class
--rw-rw-r--  2.0 unx     1248 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2.class
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1.class
--rw-rw-r--  2.0 unx     3589 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock.class
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/MethodUtil.class
--rw-rw-r--  2.0 unx     1521 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/MethodUtil$ConstructorWrapper.class
--rw-rw-r--  2.0 unx     1273 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/MethodUtil$MethodWrapper.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/MethodUtil$CallableWrapper.class
--rw-rw-r--  2.0 unx     1629 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SocketProvider.class
--rw-rw-r--  2.0 unx     1626 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SocketTransport.class
--rw-rw-r--  2.0 unx     5792 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SourceInjector.class
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SourceInjector$2.class
--rw-rw-r--  2.0 unx     1709 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SourceInjector$1.class
--rw-rw-r--  2.0 unx     1781 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SourceInjector$JavaByteObject.class
--rw-rw-r--  2.0 unx     1616 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/SourceInjector$JavaStringObject.class
--rw-rw-r--  2.0 unx     3965 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/UnixFifoProvider.class
--rw-rw-r--  2.0 unx     2802 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/UnixFifoProvider$1.class
--rw-rw-r--  2.0 unx     1817 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/UnixFifoProvider$Fifo.class
--rw-rw-r--  2.0 unx      645 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/Transport.class
--rw-rw-r--  2.0 unx      486 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/Transport$Provider.class
--rw-rw-r--  2.0 unx     2873 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/Transport$Provider$Arguments.class
--rw-rw-r--  2.0 unx     1848 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/UnixFifoTransport.class
--rw-rw-r--  2.0 unx     1213 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/UnixSignals.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/
--rw-rw-r--  2.0 unx     3947 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers.class
--rw-rw-r--  2.0 unx     1068 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThrowIterator.class
--rw-rw-r--  2.0 unx     1187 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator.class
--rw-rw-r--  2.0 unx      650 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator$CustomNoSuchElementException.class
--rw-rw-r--  2.0 unx     1653 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$MorePrecedenceMethods.class
--rw-rw-r--  2.0 unx     6513 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$PrecedenceMethods.class
--rw-rw-r--  2.0 unx      455 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$C.class
--rw-rw-r--  2.0 unx      455 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$B.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$A.class
--rw-rw-r--  2.0 unx      639 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$1Result.class
--rw-rw-r--  2.0 unx      288 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$ObjectInterface.class
--rw-rw-r--  2.0 unx      770 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsDerived.class
--rw-rw-r--  2.0 unx      588 b- defN 23-Jul-03 18:24 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsBase.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/python/
--rw-rw-r--  2.0 unx     2696 b- defN 23-Jul-03 18:24 com/deshaw/python/BinString.class
--rw-rw-r--  2.0 unx     5140 b- defN 23-Jul-03 18:24 com/deshaw/python/Dict.class
--rw-rw-r--  2.0 unx      581 b- defN 23-Jul-03 18:24 com/deshaw/python/Dict$MissingKeyException.class
--rw-rw-r--  2.0 unx     4410 b- defN 23-Jul-03 18:24 com/deshaw/python/Operations.class
--rw-rw-r--  2.0 unx    15197 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonPickle.class
--rw-rw-r--  2.0 unx     1046 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonPickle$1.class
--rw-rw-r--  2.0 unx    18293 b- defN 23-Jul-03 18:24 com/deshaw/python/NumpyArray.class
--rw-rw-r--  2.0 unx      994 b- defN 23-Jul-03 18:24 com/deshaw/python/NumpyArray$1.class
--rw-rw-r--  2.0 unx      337 b- defN 23-Jul-03 18:24 com/deshaw/python/NumpyArray$ElementVisitor.class
--rw-rw-r--  2.0 unx     5031 b- defN 23-Jul-03 18:24 com/deshaw/python/DType.class
--rw-rw-r--  2.0 unx     2009 b- defN 23-Jul-03 18:24 com/deshaw/python/DType$Type.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Jul-03 18:24 com/deshaw/python/MalformedPickleException.class
--rw-rw-r--  2.0 unx    15644 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle.class
--rw-rw-r--  2.0 unx     3276 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$2.class
--rw-rw-r--  2.0 unx      528 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$1.class
--rw-rw-r--  2.0 unx     1130 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$UnpickleableDType.class
--rw-rw-r--  2.0 unx     2260 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$NumpyFromstringArray.class
--rw-rw-r--  2.0 unx     3503 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$UnpickleableNumpyArray.class
--rw-rw-r--  2.0 unx     2079 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$BytesPlaceholder.class
--rw-rw-r--  2.0 unx     2755 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$Encoder.class
--rw-rw-r--  2.0 unx     1679 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$DTypeFactory.class
--rw-rw-r--  2.0 unx      983 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$NDArrayType.class
--rw-rw-r--  2.0 unx     2760 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayScalar.class
--rw-rw-r--  2.0 unx     1709 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$NumpyFromstring.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayReconstruct.class
--rw-rw-r--  2.0 unx      392 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$Global.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$Instance.class
--rw-rw-r--  2.0 unx     1208 b- defN 23-Jul-03 18:24 com/deshaw/python/PythonUnpickle$ShrinkableList.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/util/
--rw-rw-r--  2.0 unx     4673 b- defN 23-Jul-03 18:24 com/deshaw/util/ByteList.class
--rw-rw-r--  2.0 unx     3081 b- defN 23-Jul-03 18:24 com/deshaw/util/StringUtil.class
--rw-rw-r--  2.0 unx     3465 b- defN 23-Jul-03 18:24 com/deshaw/util/StringUtil$HashableSubSequence.class
--rw-rw-r--  2.0 unx     3312 b- defN 23-Jul-03 18:24 com/deshaw/util/SwappingPool.class
--rw-rw-r--  2.0 unx     1443 b- defN 23-Jul-03 18:24 com/deshaw/util/SwappingPool$1.class
--rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-03 18:24 com/deshaw/util/SwappingPool$Stack.class
--rw-rw-r--  2.0 unx      982 b- defN 23-Jul-03 18:24 com/deshaw/util/ThreadLocalStringBuilder.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Jul-03 18:24 com/deshaw/util/Pool.class
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-03 18:24 com/deshaw/util/Instrumentor.class
--rw-rw-r--  2.0 unx      728 b- defN 23-Jul-03 18:24 com/deshaw/util/Instrumentor$2.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Jul-03 18:24 com/deshaw/util/Instrumentor$1.class
--rw-rw-r--  2.0 unx      335 b- defN 23-Jul-03 18:24 com/deshaw/util/Instrumentor$Factory.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/
--rw-rw-r--  2.0 unx    22242 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager.class
--rw-rw-r--  2.0 unx     1110 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$2.class
--rw-rw-r--  2.0 unx     5322 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$NamedReentrantLock.class
--rw-rw-r--  2.0 unx     1456 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$1.class
--rw-rw-r--  2.0 unx     3244 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$LockManagerLock.class
--rw-rw-r--  2.0 unx     4194 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$LockManagerLock$Locker.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$ColouredList.class
--rw-rw-r--  2.0 unx     4778 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$ThreadLockState.class
--rw-rw-r--  2.0 unx     2039 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$ThreadLockState$Details.class
--rw-rw-r--  2.0 unx     1407 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$SafeReadWriteLock.class
--rw-rw-r--  2.0 unx     3227 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$SafeLock.class
--rw-rw-r--  2.0 unx     1443 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$SafeLock$AcquireFailedException.class
--rw-rw-r--  2.0 unx      566 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/LockManager$DeadlockException.class
--rw-rw-r--  2.0 unx     6390 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/VirtualThreadLock.class
--rw-rw-r--  2.0 unx      895 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/VirtualThreadLock$1.class
--rw-rw-r--  2.0 unx     1273 b- defN 23-Jul-03 18:24 com/deshaw/util/concurrent/VirtualThreadLock$VirtualThread.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-03 18:33 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/io/
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-03 18:33 com/deshaw/io/BlockingPipe.class
+-rw-rw-r--  2.0 unx      792 b- defN 23-Jul-03 18:33 com/deshaw/io/BlockingPipe$Output.class
+-rw-rw-r--  2.0 unx      752 b- defN 23-Jul-03 18:33 com/deshaw/io/BlockingPipe$Input.class
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/
+-rw-rw-r--  2.0 unx     5916 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/AsType.class
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/JavaProxyBase.class
+-rw-rw-r--  2.0 unx    11977 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/JniPJRmi.class
+-rw-rw-r--  2.0 unx      757 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/JniPJRmi$ArrayHandle.class
+-rw-rw-r--  2.0 unx     2344 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PipedProvider.class
+-rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PipedProvider$BidirectionalPipe.class
+-rw-rw-r--  2.0 unx     3095 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PipedProvider$PipedPJRmi.class
+-rw-rw-r--  2.0 unx     1922 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PipedTransport.class
+-rw-rw-r--  2.0 unx     6019 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonMinionProvider.class
+-rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonMinionProvider$1.class
+-rw-rw-r--  2.0 unx     5605 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonMinionTransport.class
+-rw-rw-r--  2.0 unx     1498 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonSlice.class
+-rw-rw-r--  2.0 unx     5353 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SSLSocketProvider.class
+-rw-rw-r--  2.0 unx     1002 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonKwargsFunction.class
+-rw-rw-r--  2.0 unx      442 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonFunction.class
+-rw-rw-r--  2.0 unx     5307 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject.class
+-rw-rw-r--  2.0 unx     2044 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$8.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$7.class
+-rw-rw-r--  2.0 unx     1992 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$6.class
+-rw-rw-r--  2.0 unx     1915 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$5.class
+-rw-rw-r--  2.0 unx     2169 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$4.class
+-rw-rw-r--  2.0 unx     2092 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$3.class
+-rw-rw-r--  2.0 unx     2142 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$2.class
+-rw-rw-r--  2.0 unx     1884 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonObject$1.class
+-rw-rw-r--  2.0 unx      493 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonCallbackException.class
+-rw-rw-r--  2.0 unx     2144 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonMinion.class
+-rw-rw-r--  2.0 unx     1171 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PythonMinion$ByValue.class
+-rw-rw-r--  2.0 unx     3228 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SSLSocketTransport.class
+-rw-rw-r--  2.0 unx    25886 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi.class
+-rw-rw-r--  2.0 unx     2986 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$3.class
+-rw-rw-r--  2.0 unx     1274 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$2.class
+-rw-rw-r--  2.0 unx      621 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$1.class
+-rw-rw-r--  2.0 unx    67472 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection.class
+-rw-rw-r--  2.0 unx     5136 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$3.class
+-rw-rw-r--  2.0 unx     1730 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$2.class
+-rw-rw-r--  2.0 unx     1626 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$1.class
+-rw-rw-r--  2.0 unx     8176 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl.class
+-rw-rw-r--  2.0 unx     7829 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler.class
+-rw-rw-r--  2.0 unx     6602 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler.class
+-rw-rw-r--  2.0 unx     2750 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate.class
+-rw-rw-r--  2.0 unx     2646 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate.class
+-rw-rw-r--  2.0 unx     2411 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer.class
+-rw-rw-r--  2.0 unx     2310 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer.class
+-rw-rw-r--  2.0 unx     2427 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction.class
+-rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction.class
+-rw-rw-r--  2.0 unx     2330 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator.class
+-rw-rw-r--  2.0 unx     2014 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable.class
+-rw-rw-r--  2.0 unx     5853 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallback.class
+-rw-rw-r--  2.0 unx     1393 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult.class
+-rw-rw-r--  2.0 unx     2125 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle.class
+-rw-rw-r--  2.0 unx     3730 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$MethodCaller.class
+-rw-rw-r--  2.0 unx     8410 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Connection$Worker.class
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$ThreadId.class
+-rw-rw-r--  2.0 unx     1146 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream.class
+-rw-rw-r--  2.0 unx      788 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.class
+-rw-rw-r--  2.0 unx      995 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$ClassInjector.class
+-rw-rw-r--  2.0 unx     3608 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$HandleMapping.class
+-rw-rw-r--  2.0 unx      697 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.class
+-rw-rw-r--  2.0 unx     3891 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$TypeMapping.class
+-rw-rw-r--  2.0 unx     4206 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MethodDescription.class
+-rw-rw-r--  2.0 unx     2631 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.class
+-rw-rw-r--  2.0 unx     3177 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MethodCallFuture.class
+-rw-rw-r--  2.0 unx     2237 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$SyncMode.class
+-rw-rw-r--  2.0 unx     1766 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MethodFlags.class
+-rw-rw-r--  2.0 unx     1964 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$FieldDescription.class
+-rw-rw-r--  2.0 unx      585 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$ReadObjectResult.class
+-rw-rw-r--  2.0 unx     1242 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MethodSignature.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MethodComparator.class
+-rw-rw-r--  2.0 unx     5930 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$WrappedArrayLike.class
+-rw-rw-r--  2.0 unx     1480 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator.class
+-rw-rw-r--  2.0 unx      420 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$ArrayLike.class
+-rw-rw-r--  2.0 unx      343 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PythonItemAssignable.class
+-rw-rw-r--  2.0 unx      487 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PythonSubscriptable.class
+-rw-rw-r--  2.0 unx    17628 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$TypeDescription.class
+-rw-rw-r--  2.0 unx     1585 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$TypeFlags.class
+-rw-rw-r--  2.0 unx     2640 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PythonValueFormat.class
+-rw-rw-r--  2.0 unx     4710 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$MessageType.class
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$Flags.class
+-rw-rw-r--  2.0 unx      496 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$GenericReturnType.class
+-rw-rw-r--  2.0 unx     7296 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PJRmiLockManager.class
+-rw-rw-r--  2.0 unx     1248 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2.class
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1.class
+-rw-rw-r--  2.0 unx     3589 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock.class
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/MethodUtil.class
+-rw-rw-r--  2.0 unx     1521 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/MethodUtil$ConstructorWrapper.class
+-rw-rw-r--  2.0 unx     1273 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/MethodUtil$MethodWrapper.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/MethodUtil$CallableWrapper.class
+-rw-rw-r--  2.0 unx     1629 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SocketProvider.class
+-rw-rw-r--  2.0 unx     1626 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SocketTransport.class
+-rw-rw-r--  2.0 unx     5792 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SourceInjector.class
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SourceInjector$2.class
+-rw-rw-r--  2.0 unx     1709 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SourceInjector$1.class
+-rw-rw-r--  2.0 unx     1781 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SourceInjector$JavaByteObject.class
+-rw-rw-r--  2.0 unx     1616 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/SourceInjector$JavaStringObject.class
+-rw-rw-r--  2.0 unx     3965 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/UnixFifoProvider.class
+-rw-rw-r--  2.0 unx     2802 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/UnixFifoProvider$1.class
+-rw-rw-r--  2.0 unx     1817 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/UnixFifoProvider$Fifo.class
+-rw-rw-r--  2.0 unx      645 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/Transport.class
+-rw-rw-r--  2.0 unx      486 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/Transport$Provider.class
+-rw-rw-r--  2.0 unx     2873 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/Transport$Provider$Arguments.class
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/UnixFifoTransport.class
+-rw-rw-r--  2.0 unx     1213 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/UnixSignals.class
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/
+-rw-rw-r--  2.0 unx     3947 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers.class
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThrowIterator.class
+-rw-rw-r--  2.0 unx     1187 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator.class
+-rw-rw-r--  2.0 unx      650 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator$CustomNoSuchElementException.class
+-rw-rw-r--  2.0 unx     1653 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$MorePrecedenceMethods.class
+-rw-rw-r--  2.0 unx     6513 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$PrecedenceMethods.class
+-rw-rw-r--  2.0 unx      455 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$C.class
+-rw-rw-r--  2.0 unx      455 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$B.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$A.class
+-rw-rw-r--  2.0 unx      639 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$1Result.class
+-rw-rw-r--  2.0 unx      288 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$ObjectInterface.class
+-rw-rw-r--  2.0 unx      770 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsDerived.class
+-rw-rw-r--  2.0 unx      588 b- defN 23-Jul-03 18:33 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsBase.class
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/python/
+-rw-rw-r--  2.0 unx     2696 b- defN 23-Jul-03 18:33 com/deshaw/python/BinString.class
+-rw-rw-r--  2.0 unx     5140 b- defN 23-Jul-03 18:33 com/deshaw/python/Dict.class
+-rw-rw-r--  2.0 unx      581 b- defN 23-Jul-03 18:33 com/deshaw/python/Dict$MissingKeyException.class
+-rw-rw-r--  2.0 unx     4410 b- defN 23-Jul-03 18:33 com/deshaw/python/Operations.class
+-rw-rw-r--  2.0 unx    15197 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonPickle.class
+-rw-rw-r--  2.0 unx     1046 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonPickle$1.class
+-rw-rw-r--  2.0 unx    18293 b- defN 23-Jul-03 18:33 com/deshaw/python/NumpyArray.class
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jul-03 18:33 com/deshaw/python/NumpyArray$1.class
+-rw-rw-r--  2.0 unx      337 b- defN 23-Jul-03 18:33 com/deshaw/python/NumpyArray$ElementVisitor.class
+-rw-rw-r--  2.0 unx     5031 b- defN 23-Jul-03 18:33 com/deshaw/python/DType.class
+-rw-rw-r--  2.0 unx     2009 b- defN 23-Jul-03 18:33 com/deshaw/python/DType$Type.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Jul-03 18:33 com/deshaw/python/MalformedPickleException.class
+-rw-rw-r--  2.0 unx    15644 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle.class
+-rw-rw-r--  2.0 unx     3276 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$2.class
+-rw-rw-r--  2.0 unx      528 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$1.class
+-rw-rw-r--  2.0 unx     1130 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$UnpickleableDType.class
+-rw-rw-r--  2.0 unx     2260 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$NumpyFromstringArray.class
+-rw-rw-r--  2.0 unx     3503 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$UnpickleableNumpyArray.class
+-rw-rw-r--  2.0 unx     2079 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$BytesPlaceholder.class
+-rw-rw-r--  2.0 unx     2755 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$Encoder.class
+-rw-rw-r--  2.0 unx     1679 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$DTypeFactory.class
+-rw-rw-r--  2.0 unx      983 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$NDArrayType.class
+-rw-rw-r--  2.0 unx     2760 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayScalar.class
+-rw-rw-r--  2.0 unx     1709 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$NumpyFromstring.class
+-rw-rw-r--  2.0 unx     1032 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayReconstruct.class
+-rw-rw-r--  2.0 unx      392 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$Global.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$Instance.class
+-rw-rw-r--  2.0 unx     1208 b- defN 23-Jul-03 18:33 com/deshaw/python/PythonUnpickle$ShrinkableList.class
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/util/
+-rw-rw-r--  2.0 unx     4673 b- defN 23-Jul-03 18:33 com/deshaw/util/ByteList.class
+-rw-rw-r--  2.0 unx     3081 b- defN 23-Jul-03 18:33 com/deshaw/util/StringUtil.class
+-rw-rw-r--  2.0 unx     3465 b- defN 23-Jul-03 18:33 com/deshaw/util/StringUtil$HashableSubSequence.class
+-rw-rw-r--  2.0 unx     3312 b- defN 23-Jul-03 18:33 com/deshaw/util/SwappingPool.class
+-rw-rw-r--  2.0 unx     1443 b- defN 23-Jul-03 18:33 com/deshaw/util/SwappingPool$1.class
+-rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-03 18:33 com/deshaw/util/SwappingPool$Stack.class
+-rw-rw-r--  2.0 unx      982 b- defN 23-Jul-03 18:33 com/deshaw/util/ThreadLocalStringBuilder.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jul-03 18:33 com/deshaw/util/Pool.class
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-03 18:33 com/deshaw/util/Instrumentor.class
+-rw-rw-r--  2.0 unx      728 b- defN 23-Jul-03 18:33 com/deshaw/util/Instrumentor$2.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Jul-03 18:33 com/deshaw/util/Instrumentor$1.class
+-rw-rw-r--  2.0 unx      335 b- defN 23-Jul-03 18:33 com/deshaw/util/Instrumentor$Factory.class
+drwxrwxr-x  2.0 unx        0 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/
+-rw-rw-r--  2.0 unx    22242 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager.class
+-rw-rw-r--  2.0 unx     1110 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$2.class
+-rw-rw-r--  2.0 unx     5322 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$NamedReentrantLock.class
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$1.class
+-rw-rw-r--  2.0 unx     3244 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$LockManagerLock.class
+-rw-rw-r--  2.0 unx     4194 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$LockManagerLock$Locker.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$ColouredList.class
+-rw-rw-r--  2.0 unx     4778 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$ThreadLockState.class
+-rw-rw-r--  2.0 unx     2039 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$ThreadLockState$Details.class
+-rw-rw-r--  2.0 unx     1407 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$SafeReadWriteLock.class
+-rw-rw-r--  2.0 unx     3227 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$SafeLock.class
+-rw-rw-r--  2.0 unx     1443 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$SafeLock$AcquireFailedException.class
+-rw-rw-r--  2.0 unx      566 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/LockManager$DeadlockException.class
+-rw-rw-r--  2.0 unx     6390 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/VirtualThreadLock.class
+-rw-rw-r--  2.0 unx      895 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/VirtualThreadLock$1.class
+-rw-rw-r--  2.0 unx     1273 b- defN 23-Jul-03 18:33 com/deshaw/util/concurrent/VirtualThreadLock$VirtualThread.class
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 META-INF/maven/
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 META-INF/maven/org.xerial.snappy/
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 META-INF/maven/org.xerial.snappy/snappy-java/
 -rw-r--r--  2.0 unx    11560 b- defN 13-Mar-22 15:33 META-INF/maven/org.xerial.snappy/snappy-java/LICENSE
 -rw-r--r--  2.0 unx      139 b- defN 13-Nov-08 00:11 META-INF/maven/org.xerial.snappy/snappy-java/pom.properties
 -rw-r--r--  2.0 unx    11865 b- defN 13-Nov-08 00:10 META-INF/maven/org.xerial.snappy/snappy-java/pom.xml
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 org/
```

### Comparing `pjrmi-1.11.0/README.md` & `pjrmi-1.11.1/README.md`

 * *Files identical despite different names*

### Comparing `pjrmi-1.11.0/pyproject.toml` & `pjrmi-1.11.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 artifacts = [ "pjrmi/lib/*.jar",
 ]
 
 [project]
 name = "pjrmi"
 dependencies = [
-    "snappy",
+    "snappy", "numpy"
 ]
 
 # Using https://peps.python.org/pep-0639/ which is still in draft
 license = {text = "BSD-3-Clause"}
 
 description = "PJRmi, RMI between Python and Java"
 authors = [{name = "D. E. Shaw & Co LP"}]
```

### Comparing `pjrmi-1.11.0/PKG-INFO` & `pjrmi-1.11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pjrmi
-Version: 1.11.0
+Version: 1.11.1
 Summary: PJRmi, RMI between Python and Java
 Project-URL: Source code, https://github.com/deshaw/pjrmi
 Author: D. E. Shaw & Co LP
 Maintainer-email: "D. E. Shaw & Co LP" <pjrmi@deshaw.com>
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
+Requires-Dist: numpy
 Requires-Dist: snappy
 Description-Content-Type: text/markdown
 
 PJRmi
 =====
 
 ## Overview
```

