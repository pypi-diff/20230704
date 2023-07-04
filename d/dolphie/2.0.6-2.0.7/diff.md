# Comparing `tmp/dolphie-2.0.6.tar.gz` & `tmp/dolphie-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-2.0.6.tar", max compression
+gzip compressed data, was "dolphie-2.0.7.tar", max compression
```

## Comparing `dolphie-2.0.6.tar` & `dolphie-2.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.6/LICENSE
--rw-r--r--   0        0        0     7199 2023-07-03 09:15:41.538676 dolphie-2.0.6/README.md
--rw-r--r--   0        0        0     1347 2023-07-03 06:44:11.377308 dolphie-2.0.6/dolphie/Database.py
--rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.6/dolphie/Functions.py
--rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.6/dolphie/KBHit.py
--rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.6/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.6/dolphie/Panels/innodb_io_panel.py
--rw-r--r--   0        0        0     5323 2023-07-03 01:29:41.157031 dolphie-2.0.6/dolphie/Panels/innodb_locks_panel.py
--rw-r--r--   0        0        0    10063 2023-07-03 01:37:34.898441 dolphie-2.0.6/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0    11948 2023-07-04 03:00:00.226598 dolphie-2.0.6/dolphie/Panels/replica_panel.py
--rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.6/dolphie/Queries.py
--rw-r--r--   0        0        0    51459 2023-07-03 10:22:51.305863 dolphie-2.0.6/dolphie/__init__.py
--rwxr-xr-x   0        0        0    15807 2023-07-04 03:02:02.732373 dolphie-2.0.6/dolphie/app.py
--rw-r--r--   0        0        0      521 2023-07-04 03:03:29.621625 dolphie-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 dolphie-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.7/LICENSE
+-rw-r--r--   0        0        0     7167 2023-07-04 03:13:04.900371 dolphie-2.0.7/README.md
+-rw-r--r--   0        0        0     1574 2023-07-04 07:09:03.000115 dolphie-2.0.7/dolphie/Database.py
+-rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.7/dolphie/Functions.py
+-rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.7/dolphie/KBHit.py
+-rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.7/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.7/dolphie/Panels/innodb_io_panel.py
+-rw-r--r--   0        0        0     5316 2023-07-04 07:06:37.671790 dolphie-2.0.7/dolphie/Panels/innodb_locks_panel.py
+-rw-r--r--   0        0        0    10056 2023-07-04 07:07:44.990022 dolphie-2.0.7/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0    11948 2023-07-04 03:00:00.226598 dolphie-2.0.7/dolphie/Panels/replica_panel.py
+-rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.7/dolphie/Queries.py
+-rw-r--r--   0        0        0    51168 2023-07-04 07:26:33.046048 dolphie-2.0.7/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    15809 2023-07-04 07:00:32.285625 dolphie-2.0.7/dolphie/app.py
+-rw-r--r--   0        0        0      521 2023-07-04 07:27:31.273098 dolphie-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7933 1970-01-01 00:00:00.000000 dolphie-2.0.7/PKG-INFO
```

### Comparing `dolphie-2.0.6/LICENSE` & `dolphie-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/README.md` & `dolphie-2.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   -h HOST, --host HOST  Hostname/IP address for MySQL
   -P PORT, --port PORT  Port for MySQL (Socket has precendence)
   -S SOCKET, --socket SOCKET
                         Socket file for MySQL
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         Absolute config file path to use. This should use [client] section. See below for options support [default: ~/.my.cnf]
   -f HOST_CACHE_FILE, --host-cache-file HOST_CACHE_FILE
-                        Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format: ip=hostname [default: /Users/cthompson/git/dolphie/host_cache]
+                        Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format: ip=hostname [default: None]
   -l LOGIN_PATH, --login-path LOGIN_PATH
                         Specify login path to use mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supercedes config file [default: client]
   -r REFRESH_INTERVAL, --refresh_interval REFRESH_INTERVAL
                         How much time to wait in seconds between each refresh [default: 1]
   -R REFRESH_INTERVAL_INNODB_STATUS, --refresh_interval_innodb_status REFRESH_INTERVAL_INNODB_STATUS
                         How much time to wait in seconds to execute SHOW ENGINE INNODB STATUS to refresh data its responsible for [default: 1]
   -H HEARTBEAT_TABLE, --heartbeat-table HEARTBEAT_TABLE
@@ -90,16 +90,16 @@
   --ssl-mode SSL_MODE   Desired security state of the connection to the host. Supports: REQUIRED/VERIFY_CA/VERIFY_IDENTITY [default: OFF]
   --ssl-ca SSL_CA       Path to the file that contains a PEM-formatted CA certificate
   --ssl-cert SSL_CERT   Path to the file that contains a PEM-formatted client certificate
   --ssl-key SSL_KEY     Path to the file that contains a PEM-formatted private key for the client certificate
   --hide-dashboard      Start without showing dashboard. This is good to use if you want to reclaim terminal space and not execute the additional queries for it
   --show-trxs-only      Start with only showing queries that are running a transaction
   --additional-columns  Start with additional columns in processlist panel
-  --use-processlist     Start with using Processlist instead of Performance Schema for listing queries.
-  --debug               Print tracebacks on errors. Useful for debugging.
+  --use-processlist     Start with using Processlist instead of Performance Schema for listing queries
+  --debug               Print tracebacks on errors for more verbose debugging
   -V, --version         Display version and exit
 
 Config file with [client] section supports these options:
     host
     user
     password
     port
```

### Comparing `dolphie-2.0.6/dolphie/Functions.py` & `dolphie-2.0.7/dolphie/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/dolphie/KBHit.py` & `dolphie-2.0.7/dolphie/KBHit.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/dolphie/Panels/dashboard_panel.py` & `dolphie-2.0.7/dolphie/Panels/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/dolphie/Panels/innodb_io_panel.py` & `dolphie-2.0.7/dolphie/Panels/innodb_io_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/dolphie/Panels/innodb_locks_panel.py` & `dolphie-2.0.7/dolphie/Panels/innodb_locks_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich.style import Style
 from rich.table import Table
 
 
 def create_panel(dolphie: Dolphie):
     innodb_lock_threads = {}
 
-    dolphie.db.cursor.execute(dolphie.innodb_locks_sql)
+    dolphie.db.execute(dolphie.innodb_locks_sql)
     threads = dolphie.db.cursor.fetchall()
 
     for counter, thread in enumerate(threads):
         w_query = re.sub(r"\s+", " ", thread["waiting_query"].decode(detect_encoding(thread["waiting_query"])))
         b_query = re.sub(r"\s+", " ", thread["blocking_query"].decode(detect_encoding(thread["blocking_query"])))
 
         innodb_lock_threads[counter] = {
```

### Comparing `dolphie-2.0.6/dolphie/Panels/processlist_panel.py` & `dolphie-2.0.7/dolphie/Panels/processlist_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         processlist_query = processlist_query.replace("$placeholder", "")
 
     # Limit the SELECT query to only retrieve how many lines the terminal has
     processlist_query = processlist_query + " LIMIT %s" % (dolphie.console.size.height)
 
     processlist_threads = {}
     # Run the processlist query
-    dolphie.db.cursor.execute(processlist_query)
+    dolphie.db.execute(processlist_query)
     threads = dolphie.db.cursor.fetchall()
 
     for thread in threads:
         # Don't include Dolphie's thread
         if dolphie.connection_id == thread["id"]:
             continue
```

### Comparing `dolphie-2.0.6/dolphie/Panels/replica_panel.py` & `dolphie-2.0.7/dolphie/Panels/replica_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/dolphie/Queries.py` & `dolphie-2.0.7/dolphie/Queries.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.6/dolphie/__init__.py` & `dolphie-2.0.7/dolphie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.innodb_locks_sql: bool = False
         self.host_is_rds: bool = False
         self.server_uuid: str = None
         self.full_version: str = None
         self.host_distro: str = None
 
         self.app_version = __version__
-        self.base_title = f"[b steel_blue1]dolphie :dolphin: {self.app_version}[/b steel_blue1]"
+        self.base_title = f"[b steel_blue1]dolphie :dolphin: v{self.app_version}[/b steel_blue1]"
         self.title = f"{self.base_title}[grey62] press ? for help"
 
     def check_for_update(self):
         # Query PyPI API to get the latest version
         url = f"https://pypi.org/pypi/{__package_name__}/json"
         response = requests.get(url)
 
@@ -110,15 +110,17 @@
             # Compare the current version with the latest version
             if parse_version(latest_version) > parse_version(__version__):
                 self.console.print(
                     (
                         "[bright_green]New version available!\n\n[grey93]Current version:"
                         f" [steel_blue1]{__version__}\n[grey93]Latest version:"
                         f" [steel_blue1]{latest_version}\n\n[grey93]Please update to the latest version at your"
-                        " convenience\n\n[steel_blue1]Press any key to continue"
+                        " convenience\n[grey66]You can find more details at:"
+                        " [underline]https://github.com/charles-001/dolphie[/underline]\n\n[steel_blue1]Press any key"
+                        " to continue"
                     ),
                     highlight=False,
                 )
 
                 key = self.kb.key_press_blocking()
                 if key:
                     pass
@@ -174,32 +176,30 @@
 
         query = "SELECT @@version_comment"
         version_comment = self.db.fetchone(query, "@@version_comment").lower()
 
         query = "SELECT @@basedir"
         basedir = self.db.fetchone(query, "@@basedir")
 
-        self.db.cursor.execute("SHOW GLOBAL VARIABLES LIKE 'aurora_version'")
+        self.db.execute("SHOW GLOBAL VARIABLES LIKE 'aurora_version'")
         data = self.db.cursor.fetchone()
         aurora_version = None
         if data:
             aurora_version = data["Value"].decode()
 
         query = "SELECT @@version"
         version = self.db.fetchone(query, "@@version").lower()
         version_split = version.split(".")
 
         self.full_version = "%s.%s.%s" % (
             version_split[0],
             version_split[1],
             version_split[2].split("-")[0],
         )
-
-        major_minor_version = "%s.%s" % (version_split[0], version_split[1])
-        major_version = version_split[0]
+        major_version = int(version_split[0])
 
         # Get proper host version and fork
         if "percona xtradb cluster" in version_comment:
             self.host_distro = "Percona XtraDB Cluster"
         elif "percona server" in version_comment:
             self.host_distro = "Percona Server"
         elif "mariadb cluster" in version_comment:
@@ -212,37 +212,31 @@
         elif "rdsdb" in basedir:
             self.host_distro = "Amazon RDS"
             self.host_is_rds = True
         else:
             self.host_distro = "MySQL"
 
         # Determine if InnoDB locks panel is available for a version and which query to use
-        # Major version 10 is for MariaDB
         self.innodb_locks_sql = None
-        innodb_locks_queries = {
-            "5.6": Queries["locks_query-5"],
-            "5.7": Queries["locks_query-5"],
-            "8": Queries["locks_query-8"] if self.use_performance_schema else None,
-            "10": Queries["locks_query-5"],
-        }
-        if major_minor_version in innodb_locks_queries or major_version in innodb_locks_queries:
-            self.innodb_locks_sql = innodb_locks_queries.get(major_minor_version) or innodb_locks_queries.get(
-                major_version
-            )
+        server_uuid_query = "SELECT @@server_uuid"
+        if "MariaDB" in self.host_distro and major_version >= 10:
+            server_uuid_query = "SELECT @@server_id AS @@server_uuid"
+            self.innodb_locks_sql = Queries["locks_query-5"]
+        elif major_version == 5:
+            self.innodb_locks_sql = Queries["locks_query-5"]
+        elif major_version == 8 and self.use_performance_schema:
+            self.innodb_locks_sql = Queries["locks_query-8"]
 
-        query = "SELECT @@server_uuid"
-        if "MariaDB" in self.host_distro:
-            query = "SELECT @@server_id AS @@server_uuid"
-        self.server_uuid = self.db.fetchone(query, "@@server_uuid")
+        self.server_uuid = self.db.fetchone(server_uuid_query, "@@server_uuid")
 
     def fetch_data(self, command):
         command_data = {}
 
         if command == "status" or command == "variables":
-            self.db.cursor.execute(Queries[command])
+            self.db.execute(Queries[command])
             data = self.db.cursor.fetchall()
 
             for row in data:
                 variable = row["Variable_name"].decode()
                 value = row["Value"]
 
                 try:
@@ -252,21 +246,21 @@
                         converted_value = int(converted_value)
                 except (UnicodeDecodeError, AttributeError):
                     converted_value = value
 
                 command_data[variable] = converted_value
 
         elif command == "innodb_status":
-            self.db.cursor.execute(Queries[command])
+            self.db.execute(Queries[command])
             data = self.db.cursor.fetchone()
 
             command_data["status"] = data["Status"].decode(detect_encoding(data["Status"]))
 
         else:
-            self.db.cursor.execute(Queries[command])
+            self.db.execute(Queries[command])
             data = self.db.cursor.fetchall()
 
             for row in data:
                 for column, value in row.items():
                     try:
                         converted_value = value.decode()
 
@@ -433,16 +427,16 @@
                     if self.processlist_threads[thread_id]["query"] and self.processlist_threads[thread_id]["db"]:
                         explain_failure = None
                         explain_data = None
 
                         self.console.print("")
 
                         try:
-                            self.db.cursor.execute("USE %s" % self.processlist_threads[thread_id]["db"])
-                            self.db.cursor.execute("EXPLAIN %s" % self.processlist_threads[thread_id]["query"])
+                            self.db.execute("USE %s" % self.processlist_threads[thread_id]["db"])
+                            self.db.execute("EXPLAIN %s" % self.processlist_threads[thread_id]["query"])
 
                             explain_data = self.db.cursor.fetchall()
                         except pymysql.Error as e:
                             explain_failure = "[bright_red]EXPLAIN ERROR:[/bright_red] [red]%s" % e.args[1]
 
                         if explain_data:
                             explain_table = Table(box=box.ROUNDED, style="grey70")
@@ -506,17 +500,17 @@
         elif key == "k":
             thread_id = self.console.input("[steel_blue1]Thread ID to kill[/steel_blue1]: ")
 
             if thread_id:
                 if thread_id in self.processlist_threads:
                     try:
                         if self.host_is_rds:
-                            self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                            self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                         else:
-                            self.db.cursor.execute("KILL %s" % thread_id)
+                            self.db.execute("KILL %s" % thread_id)
                     except pymysql.OperationalError:
                         self.update_footer("[bright_red]Thread ID '[grey93]%s[bright_red]' does not exist!" % thread_id)
                 else:
                     self.update_footer("[bright_red]Thread ID '[grey93]%s[bright_red]' does not exist!" % thread_id)
 
         elif key == "K":
             include_sleep = self.console.input("[steel_blue1]Include queries in sleep state? (y/n)[/steel_blue1]: ")
@@ -537,50 +531,50 @@
 
                     for thread_id, thread in self.processlist_threads.items():
                         try:
                             if thread["user"] == user:
                                 if include_sleep == "y":
                                     if thread["command"] in commands_with_sleep:
                                         if self.host_is_rds:
-                                            self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                                            self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                                         else:
-                                            self.db.cursor.execute("KILL %s" % thread_id)
+                                            self.db.execute("KILL %s" % thread_id)
 
                                         threads_killed += 1
                                 else:
                                     if thread["command"] in commands_without_sleep:
                                         if self.host_is_rds:
-                                            self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                                            self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                                         else:
-                                            self.db.cursor.execute("KILL %s" % thread_id)
+                                            self.db.execute("KILL %s" % thread_id)
 
                                         threads_killed += 1
                         except pymysql.OperationalError:
                             continue
 
                 elif kill_type == "h":
                     host = self.console.input("[steel_blue1]Host/IP[/steel_blue1]: ")
 
                     for thread_id, thread in self.processlist_threads.items():
                         try:
                             if thread["host"] == host:
                                 if include_sleep == "y":
                                     if thread["command"] in commands_with_sleep:
                                         if self.host_is_rds:
-                                            self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                                            self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                                         else:
-                                            self.db.cursor.execute("KILL %s" % thread_id)
+                                            self.db.execute("KILL %s" % thread_id)
 
                                         threads_killed += 1
                                 else:
                                     if thread["command"] in commands_without_sleep:
                                         if self.host_is_rds:
-                                            self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                                            self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                                         else:
-                                            self.db.cursor.execute("KILL %s" % thread_id)
+                                            self.db.execute("KILL %s" % thread_id)
 
                                         threads_killed += 1
                         except pymysql.OperationalError:
                             continue
 
                 elif kill_type == "t":
                     time = self.console.input("[steel_blue1]Time range (ex. 10-20)[/steel_blue1]: ")
@@ -597,25 +591,25 @@
                         else:
                             for thread_id, thread in self.processlist_threads.items():
                                 try:
                                     if thread["time"] >= lower_limit and thread["time"] <= upper_limit:
                                         if include_sleep == "y":
                                             if thread["command"] in commands_with_sleep:
                                                 if self.host_is_rds:
-                                                    self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                                                    self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                                                 else:
-                                                    self.db.cursor.execute("KILL %s" % thread_id)
+                                                    self.db.execute("KILL %s" % thread_id)
 
                                                 threads_killed += 1
                                         else:
                                             if thread["command"] in commands_without_sleep:
                                                 if self.host_is_rds:
-                                                    self.db.cursor.execute("CALL mysql.rds_kill(%s)" % thread_id)
+                                                    self.db.execute("CALL mysql.rds_kill(%s)" % thread_id)
                                                 else:
-                                                    self.db.cursor.execute("KILL %s" % thread_id)
+                                                    self.db.execute("KILL %s" % thread_id)
 
                                                 threads_killed += 1
                                 except pymysql.OperationalError:
                                     continue
                     else:
                         self.update_footer("[bright_red]Invalid time range!")
                 else:
@@ -629,15 +623,15 @@
         elif key == "l":
             if self.innodb_locks_sql:
                 if self.layout["innodb_locks"].visible:
                     self.layout["innodb_locks"].visible = False
                 else:
                     self.layout["innodb_locks"].visible = True
             else:
-                self.update_footer("[red]Lock panel isn't supported for this host's version!")
+                self.update_footer("[red]InnoDB Locks panel isn't supported for this host's version!")
 
         elif key == "L":
             os.system("clear")
             self.console.print(Align.right(self.title))
 
             deadlock = ""
             output = re.search(
@@ -733,15 +727,15 @@
 
             db_counter = 1
             row_counter = 1
             table_counter = 1
             tables = {}
             all_tables = []
 
-            db_count = self.db.cursor.execute(Queries["databases"])
+            db_count = self.db.execute(Queries["databases"])
             databases = self.db.cursor.fetchall()
 
             # Determine how many tables to provide data
             if db_count <= 20:
                 max_num_tables = 1
             else:
                 max_num_tables = 3
@@ -1073,21 +1067,21 @@
 
         return valid_key
 
     def create_user_stats_table(self):
         table = Table(header_style="bold white", box=box.ROUNDED, style="grey70")
         columns = {}
 
-        if self.db.cursor.execute("SELECT @@userstat") == 1:
+        if self.db.execute("SELECT @@userstat") == 1:
             userstat_enabled = self.db.cursor.fetchone()["@@userstat"] == 1
 
             if userstat_enabled:
-                self.db.cursor.execute(Queries["userstat_user_statisitics"])
+                self.db.execute(Queries["userstat_user_statisitics"])
             elif self.performance_schema_enabled:
-                self.db.cursor.execute(Queries["ps_user_statisitics"])
+                self.db.execute(Queries["ps_user_statisitics"])
             else:
                 return False
 
             users = self.db.cursor.fetchall()
             user_stats = {}
 
             for user in users:
```

### Comparing `dolphie-2.0.6/dolphie/app.py` & `dolphie-2.0.7/dolphie/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
             for option in basic_options:
                 if option in login_path_data:
                     setattr(dolphie, option, login_path_data[option])
         except Exception as e:
             # Don't error out for default login path
             if parameter_options["login_path"] != "client":
-                raise Exception(f"Problem reading login path file Reason: {e}")
+                raise Exception(f"Problem reading login path file - Reason: {e}")
 
     # Use environment variables for basic options if specified
     for option in basic_options:
         environment_var = "DOLPHIE_%s" % option.upper()
         if environment_var in os.environ and os.environ[environment_var]:
             setattr(dolphie, option, os.environ[environment_var])
 
@@ -439,12 +439,12 @@
                     loop_counter += 1
 
                 dolphie.first_loop = False
     except Exception as e:
         if dolphie.debug:
             dolphie.console.print_exception()
         else:
-            dolphie.console.print(f"[b][red]ERROR[/red]![/b] {str(e)}", highlight=False)
+            dolphie.console.print(f"[b][red]ERROR![/red][/b] {str(e)}", highlight=False)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dolphie-2.0.6/pyproject.toml` & `dolphie-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolphie"
-version = "2.0.6"
+version = "2.0.7"
 description = "An intuitive feature-rich top tool for monitoring MySQL in real time"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.4.2"
```

### Comparing `dolphie-2.0.6/PKG-INFO` & `dolphie-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 2.0.6
+Version: 2.0.7
 Summary: An intuitive feature-rich top tool for monitoring MySQL in real time
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -94,15 +94,15 @@
   -h HOST, --host HOST  Hostname/IP address for MySQL
   -P PORT, --port PORT  Port for MySQL (Socket has precendence)
   -S SOCKET, --socket SOCKET
                         Socket file for MySQL
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         Absolute config file path to use. This should use [client] section. See below for options support [default: ~/.my.cnf]
   -f HOST_CACHE_FILE, --host-cache-file HOST_CACHE_FILE
-                        Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format: ip=hostname [default: /Users/cthompson/git/dolphie/host_cache]
+                        Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format: ip=hostname [default: None]
   -l LOGIN_PATH, --login-path LOGIN_PATH
                         Specify login path to use mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supercedes config file [default: client]
   -r REFRESH_INTERVAL, --refresh_interval REFRESH_INTERVAL
                         How much time to wait in seconds between each refresh [default: 1]
   -R REFRESH_INTERVAL_INNODB_STATUS, --refresh_interval_innodb_status REFRESH_INTERVAL_INNODB_STATUS
                         How much time to wait in seconds to execute SHOW ENGINE INNODB STATUS to refresh data its responsible for [default: 1]
   -H HEARTBEAT_TABLE, --heartbeat-table HEARTBEAT_TABLE
@@ -110,16 +110,16 @@
   --ssl-mode SSL_MODE   Desired security state of the connection to the host. Supports: REQUIRED/VERIFY_CA/VERIFY_IDENTITY [default: OFF]
   --ssl-ca SSL_CA       Path to the file that contains a PEM-formatted CA certificate
   --ssl-cert SSL_CERT   Path to the file that contains a PEM-formatted client certificate
   --ssl-key SSL_KEY     Path to the file that contains a PEM-formatted private key for the client certificate
   --hide-dashboard      Start without showing dashboard. This is good to use if you want to reclaim terminal space and not execute the additional queries for it
   --show-trxs-only      Start with only showing queries that are running a transaction
   --additional-columns  Start with additional columns in processlist panel
-  --use-processlist     Start with using Processlist instead of Performance Schema for listing queries.
-  --debug               Print tracebacks on errors. Useful for debugging.
+  --use-processlist     Start with using Processlist instead of Performance Schema for listing queries
+  --debug               Print tracebacks on errors for more verbose debugging
   -V, --version         Display version and exit
 
 Config file with [client] section supports these options:
     host
     user
     password
     port
```

