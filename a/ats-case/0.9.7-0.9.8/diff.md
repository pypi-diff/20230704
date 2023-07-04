# Comparing `tmp/ats_case-0.9.7.tar.gz` & `tmp/ats_case-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.9.7.tar", last modified: Wed Jun 21 09:21:19 2023, max compression
+gzip compressed data, was "ats_case-0.9.8.tar", last modified: Tue Jul  4 00:54:45 2023, max compression
```

## Comparing `ats_case-0.9.7.tar` & `ats_case-0.9.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.425235 ats_case-0.9.7/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.7/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-21 09:21:19.423241 ats_case-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.032062 ats_case-0.9.7/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.7/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.235763 ats_case-0.9.7/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.7/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18838 2023-06-21 00:54:29.000000 ats_case-0.9.7/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12511 2023-06-21 09:21:03.000000 ats_case-0.9.7/ats_case/case/context.py
--rw-rw-rw-   0        0        0     8333 2023-06-21 09:21:03.000000 ats_case-0.9.7/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.7/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.299591 ats_case-0.9.7/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.7/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.7/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.7/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.365423 ats_case-0.9.7/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.7/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.7/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.7/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.404291 ats_case-0.9.7/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.7/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.7/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-21 09:21:19.129047 ats_case-0.9.7/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-21 09:21:18.000000 ats_case-0.9.7/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-21 09:21:18.000000 ats_case-0.9.7/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 09:21:18.000000 ats_case-0.9.7/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-21 09:21:18.000000 ats_case-0.9.7/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 09:21:18.000000 ats_case-0.9.7/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 09:21:19.425235 ats_case-0.9.7/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-21 09:18:45.000000 ats_case-0.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.472667 ats_case-0.9.8/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-07-04 00:54:45.470339 ats_case-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.077017 ats_case-0.9.8/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.8/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.300824 ats_case-0.9.8/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.8/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    20212 2023-07-03 09:42:05.000000 ats_case-0.9.8/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11204 2023-07-01 07:55:39.000000 ats_case-0.9.8/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     8333 2023-06-21 09:21:03.000000 ats_case-0.9.8/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5968 2023-06-29 07:45:53.000000 ats_case-0.9.8/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.364868 ats_case-0.9.8/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.8/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.8/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.8/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.428697 ats_case-0.9.8/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.8/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.8/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.8/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.460576 ats_case-0.9.8/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.8/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.8/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.182486 ats_case-0.9.8/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 00:54:45.472667 ats_case-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-29 07:33:27.000000 ats_case-0.9.8/setup.py
```

### Comparing `ats_case-0.9.7/PKG-INFO` & `ats_case-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.9.7
+Version: 0.9.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.7/README.md` & `ats_case-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/ats_case/case/command.py` & `ats_case-0.9.8/ats_case/case/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,17 +262,17 @@
         if index == 0:
             self._parse = context.runtime.final_result
             self._flush(context)
             return self._parse
 
     def _flush(self, context: Context):
         context.runtime.sos.update({context.runtime.step: func.to_dict(obj='meter', op=self._operation
-                                                                         , element=self._element
-                                                                         , parameter=self._parameter,
-                                                                         result=self._parse)})
+                                                                       , element=self._element
+                                                                       , parameter=self._parameter,
+                                                                       result=self._parse)})
 
     def acv(self, context: Context):
         result = str(self._parse)
         if self._func is not None:
             if type(self._func_parameter) is dict:
                 self._func_parameter = _replace(context, self._func_parameter)
             try:
@@ -342,16 +342,16 @@
             '~ @EM-> protocol:{} operation:{} parameter:{}'.format(self._protocol, self._operation, self._parameter))
         self._result = em.handle(self._protocol.name, self._operation, self._parameter)
         logger.info('~ @EM<- protocol:{} operation:{} result:{}'.format(self._protocol, self._operation, self._result))
         self._flush(context)
 
     def _flush(self, context: Context):
         context.runtime.sos.update({context.runtime.step: func.to_dict(obj='em', op=self._operation
-                                                                         , parameter=self._parameter,
-                                                                         result=self._result)})
+                                                                       , parameter=self._parameter,
+                                                                       result=self._result)})
 
     def acv(self, context: Context):
         data = func.to_dict(result=self._result)
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             self._protocol.name, self._operation, self._parameter))
         result = udm.handle(module='em.{}'.format(self._protocol.name), function=self._operation
@@ -430,15 +430,15 @@
         logger.info('~ @BENCH<- manufacture:{} operation:{} result:{}'.format(context.bench.manufacture,
                                                                               self._operation, self._result))
         self._flush(context)
 
     def _build_in(self, context: Context):
         logger.info('~ @BUILTIN-> module:{} parameter:{}'.format('bench', self._parameter))
         for op, d in self._function.items():
-            v_data = build_in.handle(module='bench', function=op, data=func.to_dict(
+            v_data = build_in.handle(function=op, data=func.to_dict(
                 param=d, iabc=context.meter.iabc, voltage=context.meter.rated_voltage,
                 current=context.meter.rated_current, index=self._exec_times))
             self._parameter = _replace_bench1(self._parameter, v_data)
 
         logger.info('~ @BUILTIN<- module:{} parameter:{}'.format('bench', self._parameter))
 
     def acv(self, context: Context):
@@ -461,16 +461,16 @@
 
             context.runtime.sas[context.runtime.step] = result
 
         return result
 
     def _flush(self, context: Context):
         context.runtime.sos.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
-                                                                         , parameter=self._parameter,
-                                                                         result=self._result)})
+                                                                       , parameter=self._parameter,
+                                                                       result=self._result)})
 
     def rest(self, context: Context):
         if self._result == '1' and self._sleep > 0:
             send(context, todo={'app:show': {'msg': '系统休眠{}秒, 等待表台调整完毕...'.format(self._sleep)}})
             sleep(self._sleep)
 
     def _times(self, context: Context):
@@ -545,19 +545,59 @@
 
 
 class ATS(object):
     def __init__(self):
         self._name = 'ats'
         self._operation = None
         self._parameter = None
+        self._glo = None
+        self._ctx = None
+        self._secs = 0
+        self._result = None
 
     def operation(self, command: str):
         self._operation = command
         return self
 
     def parameter(self, param=None):
         self._parameter = param
         return self
 
+    def glo(self, g=None):
+        self._glo = g
+        return self
+
+    def ctx(self, c=None):
+        self._ctx = c
+        return self
+
+    def secs(self, s=0):
+        self._secs = s
+        return self
+
+    def build_in(self, context: Context):
+        if isinstance(self._operation, str):
+            logger.info('~ @ATS:BUILD-IN-> operation:{} parameter:{}'.format(self._operation, self._parameter))
+            self._result = build_in.handle(function=self._operation
+                                           , data=self._parameter, debug_url=context.build_in_url)
+
+    def flush(self, context: Context):
+        if isinstance(self._glo, dict) and len(self._glo) > 0:
+            logger.info('~ @ATS:GLOBAL-> global:{} result:{}'.format(self._glo, self._result))
+            for result, name in self._glo.items():
+                eval('context.runtime.glo[{}] = {}'.format(name, self._result[result]))
+
+    def set(self, context: Context):
+        if isinstance(self._ctx, dict) and len(self._ctx) > 0:
+            logger.info('~ @ATS:SET-> context:{} result:{}'.format(self._ctx, self._result))
+            for result, name in self._ctx.items():
+                eval('{} = {}'.format(name, self._result[result]))
+
+    def sleep(self):
+        if isinstance(self._secs, int) and self._secs > 0:
+            sleep(self._secs)
+
     def exec(self, context: Context):
-        logger.info('~ @ATS-> operation:{} parameter:{}'.format(self._operation, self._parameter))
-        return eval('{}(context, {})'.format(self._operation, self._parameter))
+        self.build_in(context)
+        self.flush(context)
+        self.set(context)
+        self.sleep()
```

### Comparing `ats_case-0.9.7/ats_case/case/context.py` & `ats_case-0.9.8/ats_case/case/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self._meter = self.Meter(tl.get('meter'))
         self._bench = self.Bench(tl.get('bench'))
         # 运行时
         self._runtime = self.Runtime(self)
         self._session = self.Session(self)
         # Debug模式 - 测试开发人员本机调试数据比对服务使用
         self._acd_url = tl.get('acd_url')
+        self._build_in_url = tl.get('build_in_url')
 
     @property
     def mode(self):
         return self._mode
 
     @property
     def renew(self):
@@ -63,14 +64,18 @@
     def session(self):
         return self._session
 
     @property
     def acd_url(self):
         return self._acd_url
 
+    @property
+    def build_in_url(self):
+        return self._build_in_url
+
     class Tester(object):
         def __init__(self, data: dict):
             self._ip = data.get('ip')
             self._port = data.get('port')
             self._username = data.get('username')
             self._hostname = data.get('hostname')
 
@@ -122,16 +127,14 @@
 
     class Case(object):
         def __init__(self, data: dict):
             self._id = data.get('id', -1)
             self._name = data.get('name', 'test')
             self._code = data.get('code')
             self._version = data.get('version')
-            #         self._scope = data.get('scope')
-            #         self._purpose = data.get('purpose')
             self._script = ScriptClazz(data.get('script', 1))
             self._control = data.get('control', {})
             self._steps = data.get('steps', {})
 
             if self._code is not None:
                 self._name = '{}_{}'.format(self._name, self._code)
             if self._version is not None:
@@ -139,34 +142,14 @@
             if isinstance(self._control, str):
                 self._control = self._control.replace('null', 'None')
                 self._control = eval(self._control)
             if isinstance(self._steps, str):
                 self._steps = self._steps.replace('null', 'None')
                 self._steps = eval(self._steps)
 
-        #         self._script = 'script.{}'.format(data.get('script'))
-        #         self._bench_step_orders = data.get('bench_step_orders', [])
-        #         # 用户发起的参数
-        #         self._req_params = self.ReqParams(data.get('req_params'))
-        #
-        #         lps = data.get('loops')
-        #         if lps is not None and lps != '':
-        #             self._loops = []
-        #             lps = eval(data.get('loops'))
-        #             if type(lps) is list:
-        #                 for lp in lps:
-        #                     self._loops.append(self.Loop(lp))
-        #
-        #             if self._script is None:
-        #                 raise Exception('Path of script file is null.')
-        #             pfs = self._script.split('.')
-        #             pfs[-1] = '{}.py'.format(pfs[-1])
-        #             if not util.exist(*pfs):
-        #                 raise Exception('Script file[{}] is not exist.'.format(self._script))
-
         @property
         def id(self):
             return self._id
 
         @property
         def name(self):
             return self._name
@@ -179,46 +162,21 @@
         def control(self):
             return self._control
 
         @property
         def steps(self):
             return self._steps
 
-        # @property
-        # def code(self):
-        #     return self._code
-        #
-        # @property
-        # def version(self):
-        #     return self._version
-
-    #
-    #     @property
-    #     def scope(self):
-    #         return self._scope
-    #
-    #     @property
-    #     def purpose(self):
-    #         return self._purpose
-    #
-    #     @property
-    #     def loops(self):
-    #         return self._loops
-    #
-    #     @property
-    #     def script(self):
-    #         return self._script
-    #
-    #     @property
-    #     def bench_step_orders(self):
-    #         return self._bench_step_orders
-    #
-    #     @property
-    #     def req_params(self):
-    #         return self._req_params
+        @property
+        def code(self):
+            return self._code
+
+        @property
+        def version(self):
+            return self._version
 
     class Meter(object):
         def __init__(self, data: dict):
             self._index = data.get('index', 0)
             self._pos = data.get('pos')
             self._addr = data.get('addr')
             self._no = data.get('no')
@@ -326,17 +284,23 @@
             self._loop_end_step = 0
             self._loop_count = 0
             self._loop_index = 0
             # 步骤操作返回结果集
             self._sos = {}
             # 步骤对比返回结果集 - 用例结束时统计执行结果
             self._sas = {}
+            # 全局变量 - 用户自定义
+            self._glo = {}
             # 多帧时使用
             self._final_result = None
 
+            g = self._parent.case.control.get('global')
+            if isinstance(g, dict) and len(g) > 0:
+                self._glo = g
+
         def test_report(self):
             sc = fc = 0
             fs = []
             error = None
             for s, result in self.sas.items():
                 if str(result).find('代码发生异常') >= 0:
                     error = result
@@ -411,14 +375,18 @@
             return self._sos
 
         @property
         def sas(self):
             return self._sas
 
         @property
+        def glo(self):
+            return self._glo
+
+        @property
         def final_result(self):
             return self._final_result
 
         @final_result.setter
         def final_result(self, value):
             self._final_result = value
```

### Comparing `ats_case-0.9.7/ats_case/case/executor.py` & `ats_case-0.9.8/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/ats_case/case/translator.py` & `ats_case-0.9.8/ats_case/case/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,18 +181,27 @@
         return code
 
 
 class ATS(Operation):
     def translate(self, op: dict):
         opt = op.get('operation')
         param = op.get('parameter')
+        glo = op.get('cache')
+        ctx = op.get('set')
+        secs = op.get('sleep')
 
         code = "command.ats().operation('{}')".format(opt)
 
         if param is not None:
             code += ".parameter({})".format(param)
+        if glo is not None:
+            code += ".glo({})".format(glo)
+        if ctx is not None:
+            code += ".ctx({})".format(ctx)
+        if secs is not None:
+            code += ".secs({})".format(secs)
 
         code += ".exec(context)"
 
         return code
```

### Comparing `ats_case-0.9.7/ats_case/common/error.py` & `ats_case-0.9.8/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/ats_case/manage/core.py` & `ats_case-0.9.8/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/ats_case/manage/start.py` & `ats_case-0.9.8/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/ats_case/template/testcase_v1.tmp` & `ats_case-0.9.8/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/ats_case.egg-info/PKG-INFO` & `ats_case-0.9.8/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.9.7
+Version: 0.9.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.7/ats_case.egg-info/SOURCES.txt` & `ats_case-0.9.8/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.7/setup.py` & `ats_case-0.9.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.9.7",
+    version="0.9.8",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

