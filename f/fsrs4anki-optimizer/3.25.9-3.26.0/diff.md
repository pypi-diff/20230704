# Comparing `tmp/fsrs4anki_optimizer-3.25.9.tar.gz` & `tmp/fsrs4anki_optimizer-3.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.9.tar", last modified: Sat Jul  1 12:03:05 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.26.0.tar", last modified: Tue Jul  4 08:37:11 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.9.tar` & `fsrs4anki_optimizer-3.26.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:03:05.963891 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45447 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:37:11.672903 fsrs4anki_optimizer-3.26.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 08:37:11.668903 fsrs4anki_optimizer-3.26.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:37:11.668903 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:37:11.668903 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:37:11.672903 fsrs4anki_optimizer-3.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,33 +325,34 @@
     def anki_extract(filename: str):
         """Step 1"""
         # Extract the collection file or deck file to get the .anki21 database.
         with zipfile.ZipFile(f'{filename}', 'r') as zip_ref:
             zip_ref.extractall('./')
             print("Deck file extracted successfully!")
 
-    def create_time_series(self, timezone: str, revlog_start_date: str, next_day_starts_at: int):
+    def create_time_series(self, timezone: str, revlog_start_date: str, next_day_starts_at: int, filter_out_suspended_cards: bool = False):
         """Step 2"""
         if os.path.isfile("collection.anki21b"):
             os.remove("collection.anki21b")
             raise Exception(
                 "Please export the file with `support older Anki versions` if you use the latest version of Anki.")
         elif os.path.isfile("collection.anki21"):
             con = sqlite3.connect("collection.anki21")
         elif os.path.isfile("collection.anki2"):
             con = sqlite3.connect("collection.anki2")
         else:
             raise Exception("Collection not exist!")
         cur = con.cursor()
-        res = cur.execute("""
+        res = cur.execute(f"""
         SELECT *
         FROM revlog
         WHERE cid IN (
             SELECT id
             FROM cards
+            {"WHERE queue != -1" if filter_out_suspended_cards else ""}
         )
         """
         )
         revlog = res.fetchall()
         if len(revlog) == 0:
             raise Exception("No review log found!")
         df = pd.DataFrame(revlog)
@@ -402,15 +403,15 @@
         def cum_concat(x):
             return list(accumulate(x))
 
         t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
         r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
-        df = df[df['id'] >= time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000]
+        df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
         print("Trainset saved.")
 
         df['retention'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['y'].transform('mean')
         df['total_cnt'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['id'].transform('count')
         print("Retention calculated.")
```

