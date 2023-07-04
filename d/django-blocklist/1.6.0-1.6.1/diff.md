# Comparing `tmp/django_blocklist-1.6.0.tar.gz` & `tmp/django_blocklist-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_blocklist-1.6.0.tar", max compression
+gzip compressed data, was "django_blocklist-1.6.1.tar", max compression
```

## Comparing `django_blocklist-1.6.0.tar` & `django_blocklist-1.6.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1511 2022-07-11 13:00:57.903015 django_blocklist-1.6.0/LICENSE.md
--rw-r--r--   0        0        0     3306 2023-01-12 14:26:12.810526 django_blocklist-1.6.0/README.md
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.903572 django_blocklist-1.6.0/django_blocklist/__init__.py
--rw-r--r--   0        0        0     1236 2023-03-17 23:40:09.706587 django_blocklist-1.6.0/django_blocklist/admin.py
--rw-r--r--   0        0        0      378 2023-03-20 01:47:36.202242 django_blocklist-1.6.0/django_blocklist/apps.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904273 django_blocklist-1.6.0/django_blocklist/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904394 django_blocklist-1.6.0/django_blocklist/management/commands/__init__.py
--rw-r--r--   0        0        0     1544 2023-03-19 00:37:34.965195 django_blocklist-1.6.0/django_blocklist/management/commands/clean_blocklist.py
--rw-r--r--   0        0        0     1272 2022-07-11 13:00:57.904963 django_blocklist-1.6.0/django_blocklist/management/commands/fake_blocklist.py
--rw-r--r--   0        0        0     2807 2022-07-11 13:00:57.905202 django_blocklist-1.6.0/django_blocklist/management/commands/import_blocklist.py
--rw-r--r--   0        0        0      646 2022-07-11 13:00:57.905419 django_blocklist-1.6.0/django_blocklist/management/commands/remove_from_blocklist.py
--rw-r--r--   0        0        0     3412 2023-01-28 01:01:51.649948 django_blocklist-1.6.0/django_blocklist/management/commands/report_blocklist.py
--rw-r--r--   0        0        0     1074 2022-07-11 13:00:57.905793 django_blocklist-1.6.0/django_blocklist/management/commands/search_blocklist.py
--rw-r--r--   0        0        0     1710 2023-03-18 02:28:13.931382 django_blocklist-1.6.0/django_blocklist/management/commands/update_blocklist.py
--rw-r--r--   0        0        0     1076 2023-03-19 01:05:28.286932 django_blocklist-1.6.0/django_blocklist/middleware.py
--rw-r--r--   0        0        0     1401 2022-07-11 13:00:57.906960 django_blocklist-1.6.0/django_blocklist/migrations/0001_initial.py
--rw-r--r--   0        0        0      487 2023-03-18 02:29:58.084066 django_blocklist-1.6.0/django_blocklist/migrations/0002_alter_blockedip_tally.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.907461 django_blocklist-1.6.0/django_blocklist/migrations/__init__.py
--rw-r--r--   0        0        0     1821 2023-03-20 01:45:54.389456 django_blocklist-1.6.0/django_blocklist/models.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.908111 django_blocklist-1.6.0/django_blocklist/tests/__init__.py
--rw-r--r--   0        0        0     4673 2023-03-19 00:33:22.909579 django_blocklist-1.6.0/django_blocklist/tests/test_management.py
--rw-r--r--   0        0        0     1541 2022-07-11 13:00:57.908484 django_blocklist-1.6.0/django_blocklist/tests/test_middleware.py
--rw-r--r--   0        0        0      922 2022-07-11 13:00:57.908669 django_blocklist-1.6.0/django_blocklist/tests/test_settings.py
--rw-r--r--   0        0        0     1765 2022-07-11 13:00:57.908851 django_blocklist-1.6.0/django_blocklist/tests/test_utils.py
--rw-r--r--   0        0        0     2448 2023-03-20 01:48:36.172026 django_blocklist-1.6.0/django_blocklist/utils.py
--rw-r--r--   0        0        0      513 2023-03-20 01:53:56.057660 django_blocklist-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 django_blocklist-1.6.0/setup.py
--rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 django_blocklist-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1511 2022-07-11 13:00:57.903015 django_blocklist-1.6.1/LICENSE.md
+-rw-r--r--   0        0        0     3306 2023-01-12 14:26:12.810526 django_blocklist-1.6.1/README.md
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.903572 django_blocklist-1.6.1/django_blocklist/__init__.py
+-rw-r--r--   0        0        0     1236 2023-03-17 23:40:09.706587 django_blocklist-1.6.1/django_blocklist/admin.py
+-rw-r--r--   0        0        0      378 2023-03-20 01:47:36.202242 django_blocklist-1.6.1/django_blocklist/apps.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904273 django_blocklist-1.6.1/django_blocklist/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904394 django_blocklist-1.6.1/django_blocklist/management/commands/__init__.py
+-rw-r--r--   0        0        0     1544 2023-03-19 00:37:34.965195 django_blocklist-1.6.1/django_blocklist/management/commands/clean_blocklist.py
+-rw-r--r--   0        0        0     1272 2022-07-11 13:00:57.904963 django_blocklist-1.6.1/django_blocklist/management/commands/fake_blocklist.py
+-rw-r--r--   0        0        0     2827 2023-03-25 05:43:41.620808 django_blocklist-1.6.1/django_blocklist/management/commands/import_blocklist.py
+-rw-r--r--   0        0        0      646 2022-07-11 13:00:57.905419 django_blocklist-1.6.1/django_blocklist/management/commands/remove_from_blocklist.py
+-rw-r--r--   0        0        0     3666 2023-03-25 05:51:57.213391 django_blocklist-1.6.1/django_blocklist/management/commands/report_blocklist.py
+-rw-r--r--   0        0        0      947 2023-03-25 05:40:32.842232 django_blocklist-1.6.1/django_blocklist/management/commands/search_blocklist.py
+-rw-r--r--   0        0        0     1710 2023-03-18 02:28:13.931382 django_blocklist-1.6.1/django_blocklist/management/commands/update_blocklist.py
+-rw-r--r--   0        0        0     1076 2023-03-19 01:05:28.286932 django_blocklist-1.6.1/django_blocklist/middleware.py
+-rw-r--r--   0        0        0     1401 2022-07-11 13:00:57.906960 django_blocklist-1.6.1/django_blocklist/migrations/0001_initial.py
+-rw-r--r--   0        0        0      487 2023-03-18 02:29:58.084066 django_blocklist-1.6.1/django_blocklist/migrations/0002_alter_blockedip_tally.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.907461 django_blocklist-1.6.1/django_blocklist/migrations/__init__.py
+-rw-r--r--   0        0        0     1821 2023-03-20 01:45:54.389456 django_blocklist-1.6.1/django_blocklist/models.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.908111 django_blocklist-1.6.1/django_blocklist/tests/__init__.py
+-rw-r--r--   0        0        0     4771 2023-03-25 05:48:39.698802 django_blocklist-1.6.1/django_blocklist/tests/test_management.py
+-rw-r--r--   0        0        0     1541 2022-07-11 13:00:57.908484 django_blocklist-1.6.1/django_blocklist/tests/test_middleware.py
+-rw-r--r--   0        0        0      922 2022-07-11 13:00:57.908669 django_blocklist-1.6.1/django_blocklist/tests/test_settings.py
+-rw-r--r--   0        0        0     1765 2022-07-11 13:00:57.908851 django_blocklist-1.6.1/django_blocklist/tests/test_utils.py
+-rw-r--r--   0        0        0     2448 2023-03-20 01:48:36.172026 django_blocklist-1.6.1/django_blocklist/utils.py
+-rw-r--r--   0        0        0      513 2023-07-04 17:49:50.216816 django_blocklist-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 django_blocklist-1.6.1/PKG-INFO
```

### Comparing `django_blocklist-1.6.0/LICENSE.md` & `django_blocklist-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/README.md` & `django_blocklist-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/admin.py` & `django_blocklist-1.6.1/django_blocklist/admin.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/clean_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/clean_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/fake_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/fake_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/import_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/import_blocklist.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import logging
 import sys
 
 from django.conf import settings
 from django.core.management.base import BaseCommand
 from django.utils.dateparse import parse_datetime
 
-from ...models import DEFAULT_COOLDOWN, BlockedIP
+from ...apps import Config
+from ...models import BlockedIP
 
 logger = logging.getLogger(__name__)
-DEFAULT_DAYS = settings.BLOCKLIST_CONFIG.get("cooldown") or DEFAULT_COOLDOWN
+DEFAULT_DAYS = settings.BLOCKLIST_CONFIG.get("cooldown") or Config.defaults["cooldown"]
 
 
 class Command(BaseCommand):
     def add_arguments(self, parser):
         parser.add_argument(
             "--dry-run", action="store_true", help="Preview the resulting update rather than performing it"
         )
```

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/remove_from_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/remove_from_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/report_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/report_blocklist.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,20 +45,19 @@
         how_long = datetime.timedelta(0)
         for entry in entries:
             active_period = entry.last_seen - entry.first_seen
             if active_period > how_long:
                 longest_lived, how_long = entry, active_period
         if longest_lived is not None:
             print(f"Longest lived:\n{longest_lived.verbose_str()}")
-        if counts := reason_counts():
-            print("\nIP counts by reason\n-------------------")
-            _width = len(str(counts[0][1])) + 1
-            for reason, count in counts:
+        if stats := reason_stats():
+            print("Tally and IP count by reason\n----------------------------")
+            for tally, ip_count, reason in stats:
                 if not selected_reasons or reason in selected_reasons:
-                    print(f"{count: {_width}} | {reason}")
+                    print(f"{tally:9} | {ip_count:9} | {reason}")
 
 
 def print_roster(title: str, queryset, activity_calc: bool = False) -> None:
     print(f"{title}:")
     activity = {}
     for perp in queryset:
         # For each IP, either print a line or calculate the rate, depending on activity_calc
@@ -71,11 +70,17 @@
     if activity_calc:
         most_active = sorted(activity.items(), key=itemgetter(1), reverse=True)[:5]
         for perp, per_hour in most_active:
             print(f"{perp.verbose_str()} -- {round(per_hour)} per hour")
     print()
 
 
-def reason_counts() -> Iterable[Tuple[str, int]]:
-    reason_data = Counter(BlockedIP.objects.exclude(reason="").values_list("reason"))
-    tuples = [(str(r[0][0]), r[1]) for r in reason_data.items()]
-    return sorted(tuples, key=itemgetter(1), reverse=True)
+def reason_stats() -> Iterable[Tuple[int, int, str]]:
+    """Gather ip-count and grand tally stats for each reason"""
+    stats = Counter(BlockedIP.objects.exclude(reason="").values_list("reason"))
+    tuples = []
+    for reason_datum in stats.items():
+        reason = str(reason_datum[0][0])
+        ip_count = reason_datum[1]
+        tally = BlockedIP.objects.filter(reason=reason).aggregate(tally=Sum("tally"))["tally"]
+        tuples.append((tally, ip_count, reason))
+    return sorted(tuples, key=itemgetter(0), reverse=True)
```

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/search_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/search_blocklist.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Look up provided IPs in the blocklist. Set --verbosity=2 to see full record for found IPs."""
 import logging
 import sys
 
-from django.conf import settings
 from django.core.management.base import BaseCommand
 
-from ...models import DEFAULT_COOLDOWN, BlockedIP
+from ...models import BlockedIP
+
 
 logger = logging.getLogger(__name__)
-DEFAULT_DAYS = settings.BLOCKLIST_CONFIG.get("cooldown") or DEFAULT_COOLDOWN
 
 
 class Command(BaseCommand):
     help = __doc__
 
     def add_arguments(self, parser):
         parser.add_argument("ips", nargs="+", type=str, help="IPs to look up (space separated)")
```

### Comparing `django_blocklist-1.6.0/django_blocklist/management/commands/update_blocklist.py` & `django_blocklist-1.6.1/django_blocklist/management/commands/update_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/middleware.py` & `django_blocklist-1.6.1/django_blocklist/middleware.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/migrations/0001_initial.py` & `django_blocklist-1.6.1/django_blocklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/models.py` & `django_blocklist-1.6.1/django_blocklist/models.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/tests/test_management.py` & `django_blocklist-1.6.1/django_blocklist/tests/test_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,12 +97,14 @@
         self.assertIn(f"{self.ip1} -- 0 blocks", result)
         self.assertIn("10 per hour", result)
 
     def test_reason_report(self):
         sys.stdout = (out := StringIO())
         reasons = ["A", "B"]
         for n, reason in enumerate(reasons):
-            BlockedIP.objects.create(ip=f"{n}.{n}.{n}.{n}", reason=reason)
-        call_command("report_blocklist", reason=reasons[0])
+            BlockedIP.objects.create(ip=f"{n}.{n}.{n}.{n}", reason=reason, tally=1)
+        call_command("report_blocklist", reason="A")
         result = out.getvalue()
+        # import pdb;pdb.set_trace()
         assert BlockedIP.objects.count() == 2
         self.assertIn("Entries in blocklist: 1", result)
+        self.assertIn("        1 |         1 | A", result)
```

### Comparing `django_blocklist-1.6.0/django_blocklist/tests/test_middleware.py` & `django_blocklist-1.6.1/django_blocklist/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/tests/test_settings.py` & `django_blocklist-1.6.1/django_blocklist/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/tests/test_utils.py` & `django_blocklist-1.6.1/django_blocklist/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/django_blocklist/utils.py` & `django_blocklist-1.6.1/django_blocklist/utils.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-1.6.0/pyproject.toml` & `django_blocklist-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-blocklist"
-version = "1.6.0"
+version = "1.6.1"
 description = "A Django app that implements IP-based blocklisting."
 authors = ["Paul Bissex <paul@bissex.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://gitlab.com/paul_bissex/django-blocklist"
 packages = [ {include = "django_blocklist"} ]
```

### Comparing `django_blocklist-1.6.0/PKG-INFO` & `django_blocklist-1.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-blocklist
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Django app that implements IP-based blocklisting.
 Home-page: https://gitlab.com/paul_bissex/django-blocklist
 License: BSD-3-Clause
 Author: Paul Bissex
 Author-email: paul@bissex.net
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: BSD License
```

