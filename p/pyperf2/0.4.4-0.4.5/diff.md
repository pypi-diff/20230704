# Comparing `tmp/pyperf2-0.4.4-py3-none-any.whl.zip` & `tmp/pyperf2-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11535 bytes, number of entries: 6
--rw-r--r--  2.0 unx    26742 b- defN 23-Jul-03 11:08 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-03 11:09 pyperf2-0.4.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3340 b- defN 23-Jul-03 11:09 pyperf2-0.4.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 11:09 pyperf2-0.4.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-03 11:09 pyperf2-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-03 11:09 pyperf2-0.4.4.dist-info/RECORD
-6 files, 42002 bytes uncompressed, 10701 bytes compressed:  74.5%
+Zip file size: 11552 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26905 b- defN 23-Jul-04 10:45 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3340 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/RECORD
+6 files, 42165 bytes uncompressed, 10718 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.4.4.dist-info/LICENSE
+Filename: pyperf2-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.4.4.dist-info/METADATA
+Filename: pyperf2-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.4.4.dist-info/WHEEL
+Filename: pyperf2-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.4.4.dist-info/top_level.txt
+Filename: pyperf2-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.4.4.dist-info/RECORD
+Filename: pyperf2-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -11,14 +11,15 @@
 from decimal import Decimal
 from pprint import pprint, pformat
 import logging
 import datetime
 from pyroute2 import netns
 import atexit
 
+
 def output_reader(proc, outq, parent):
     for line in iter(proc.stdout.readline, b""):
         outq.put(line.decode("utf-8"))
 
         # print("{0} {1}".format(parent.name,line.decode('utf-8')))
 
         parent.line_ready_callback()
@@ -68,15 +69,14 @@
             )
         else:
             self.expected_interval_packets = None
         self._log = logging.getLogger("")
         self._current_event_number = 0
         atexit.register(self.stop)
 
-
     def __del__(self):
         try:
             self._raw_log_filehandler.close()
         except:
             pass
 
     def set_raw_log_path(self, path):
@@ -122,16 +122,15 @@
                     "info": result.groupdict(),
                     "events": [],
                     "timestamp": timestamp,
                 }
                 self.currently_has_loss[stream_id] = False
 
         result = self._result_regex.match(line)  # check if it's a report line
-        
-        
+
         if result:
             report_data = result.groupdict()
             stream_id = report_data["stream_id"]
 
             interval_begin = Decimal(report_data["interval_begin"])
             interval_end = Decimal(report_data["interval_end"])
             if "packets_lost" in report_data:
@@ -155,16 +154,14 @@
                 self._log.debug("got summary result")
                 return True  # suppress any message for summary
 
             if is_sender:
                 report_message = copy.copy(report_data)
                 report_message["stream_name"] = self.name
 
-
-
             if is_receiver:
                 report_message = copy.copy(report_data)
                 report_message["stream_name"] = self.name
 
                 if packets_received < self.expected_interval_packets:
                     probably_packets_lost = (
                         self.expected_interval_packets - packets_received
@@ -456,17 +453,21 @@
             if self.use_linux_namespace not in list(netns.listnetns()):
                 raise NameSpaceNotFoundError(
                     f"Namespace {self.use_linux_namespace} cannot be found."
                 )
             _cli.extend("ip netns exec {0}".format(self.use_linux_namespace).split(" "))
         _cli.append(self.iperf_binary_path)
         _cli.append("-e")
-        if self.test_duration:
+        if int(self.test_duration) and self.type == "client":
             _cli.append("-t")
             _cli.append(self.test_duration)
+        elif int(self.test_duration) > 0:
+            _cli.append("-t")
+            _cli.append(self.test_duration)
+
         if self.type == "server":
             _cli.append("-s")
             if self.bind_ip:
                 _cli.append("-B")
                 _cli.append(self.bind_ip)
             ####Ü
             if self.protocol == "tcp":
@@ -577,15 +578,15 @@
                 _cli.append("-S")
                 _cli.append(self.dscp)
             else:
                 raise ValueError(f'"{self.dscp}" is not a valid DSCP Value')
 
             _cli.append("-S")
             _cli.append(self.dscp)
-
+        # print(" ".join(_cli))
         return _cli
 
     def start(self, create_thread_function=threading.Thread):
         self._results = {}
         if self._cleanup_timer_thread:
             self._cleanup_timer_thread.join()
             del self._cleanup_timer_thread
@@ -603,15 +604,16 @@
                 target=output_reader, args=(self._proc, self._outq, self)
             )
 
         self._output_reader_thread.start()
         self._running = True
         self.status = "running"
         time.sleep(0.2)
-        if int(self.test_duration)>0:
+
+        if int(self.test_duration) > 0:
             self._cleanup_timer_thread = threading.Timer(
                 int(self.test_duration) + 10, self.stop
             )
             self._cleanup_timer_thread.start()
         if self._proc.poll() is not None:
             self.stop()
             return False
```

## Comparing `pyperf2-0.4.4.dist-info/LICENSE` & `pyperf2-0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.4.4.dist-info/METADATA` & `pyperf2-0.4.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.4.4
+Version: 0.4.5
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

