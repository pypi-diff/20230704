# Comparing `tmp/fastapi-sql-profiler-1.0.0.tar.gz` & `tmp/fastapi-sql-profiler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sql-profiler-1.0.0.tar", last modified: Wed Jun 28 12:41:52 2023, max compression
+gzip compressed data, was "fastapi-sql-profiler-1.0.1.tar", last modified: Tue Jul  4 05:31:02 2023, max compression
```

## Comparing `fastapi-sql-profiler-1.0.0.tar` & `fastapi-sql-profiler-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-06-28 12:41:52.412695 fastapi-sql-profiler-1.0.0/
--rw-r--r--   0 sarvadhi   (501) staff       (20)      611 2023-06-28 12:41:52.412236 fastapi-sql-profiler-1.0.0/PKG-INFO
--rw-r--r--   0 sarvadhi   (501) staff       (20)     1834 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/README.md
-drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-06-28 12:41:52.400375 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/
--rw-r--r--   0 sarvadhi   (501) staff       (20)       77 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/__init__.py
--rw-r--r--   0 sarvadhi   (501) staff       (20)     2846 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/add_request.py
--rw-r--r--   0 sarvadhi   (501) staff       (20)     1060 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/database.py
--rw-r--r--   0 sarvadhi   (501) staff       (20)    10175 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/middleware.py
--rw-r--r--   0 sarvadhi   (501) staff       (20)     1035 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/models.py
-drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-06-28 12:41:52.410240 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/
--rw-r--r--   0 sarvadhi   (501) staff       (20)     3449 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/base.html
--rw-r--r--   0 sarvadhi   (501) staff       (20)     4738 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/request.html
--rw-r--r--   0 sarvadhi   (501) staff       (20)     2440 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/request_show.html
--rw-r--r--   0 sarvadhi   (501) staff       (20)     2012 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/sql_query.html
--rw-r--r--   0 sarvadhi   (501) staff       (20)      987 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/sql_query_detail.html
-drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-06-28 12:41:52.405508 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/
--rw-r--r--   0 sarvadhi   (501) staff       (20)      611 2023-06-28 12:41:52.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/PKG-INFO
--rw-r--r--   0 sarvadhi   (501) staff       (20)      680 2023-06-28 12:41:52.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 sarvadhi   (501) staff       (20)        1 2023-06-28 12:41:52.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 sarvadhi   (501) staff       (20)       94 2023-06-28 12:41:52.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/requires.txt
--rw-r--r--   0 sarvadhi   (501) staff       (20)       21 2023-06-28 12:41:52.000000 fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/top_level.txt
--rw-r--r--   0 sarvadhi   (501) staff       (20)       90 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/pyproject.toml
--rw-r--r--   0 sarvadhi   (501) staff       (20)       38 2023-06-28 12:41:52.412833 fastapi-sql-profiler-1.0.0/setup.cfg
--rw-r--r--   0 sarvadhi   (501) staff       (20)      940 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/setup.py
-drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-06-28 12:41:52.410979 fastapi-sql-profiler-1.0.0/tests/
--rw-r--r--   0 sarvadhi   (501) staff       (20)     5009 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.0/tests/test_sql_profiler.py
+drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-07-04 05:31:02.845063 fastapi-sql-profiler-1.0.1/
+-rw-r--r--   0 sarvadhi   (501) staff       (20)      611 2023-07-04 05:31:02.844503 fastapi-sql-profiler-1.0.1/PKG-INFO
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     2213 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/README.md
+drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-07-04 05:31:02.832050 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/
+-rw-r--r--   0 sarvadhi   (501) staff       (20)       77 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/__init__.py
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     4170 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/add_request.py
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     1017 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/database.py
+-rw-r--r--   0 sarvadhi   (501) staff       (20)    10187 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/middleware.py
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     1035 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/models.py
+drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-07-04 05:31:02.841540 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     5356 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/base.html
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     4738 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/request.html
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     2875 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/request_show.html
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     2012 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/sql_query.html
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     1350 2023-07-04 05:29:35.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/sql_query_detail.html
+drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-07-04 05:31:02.835724 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/
+-rw-r--r--   0 sarvadhi   (501) staff       (20)      611 2023-07-04 05:31:02.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 sarvadhi   (501) staff       (20)      680 2023-07-04 05:31:02.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvadhi   (501) staff       (20)        1 2023-07-04 05:31:02.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvadhi   (501) staff       (20)       94 2023-07-04 05:31:02.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/requires.txt
+-rw-r--r--   0 sarvadhi   (501) staff       (20)       21 2023-07-04 05:31:02.000000 fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/top_level.txt
+-rw-r--r--   0 sarvadhi   (501) staff       (20)       90 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.1/pyproject.toml
+-rw-r--r--   0 sarvadhi   (501) staff       (20)       38 2023-07-04 05:31:02.845261 fastapi-sql-profiler-1.0.1/setup.cfg
+-rw-r--r--   0 sarvadhi   (501) staff       (20)      940 2023-07-04 05:29:48.000000 fastapi-sql-profiler-1.0.1/setup.py
+drwxr-xr-x   0 sarvadhi   (501) staff       (20)        0 2023-07-04 05:31:02.842768 fastapi-sql-profiler-1.0.1/tests/
+-rw-r--r--   0 sarvadhi   (501) staff       (20)     5009 2023-06-28 12:35:28.000000 fastapi-sql-profiler-1.0.1/tests/test_sql_profiler.py
```

### Comparing `fastapi-sql-profiler-1.0.0/PKG-INFO` & `fastapi-sql-profiler-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql-profiler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Middleware for profiling and logging database queries in a Python web application
 Home-page: https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git
 Author: Ganesh Sali
 Author-email: ganesh@sarvadhi.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-sql-profiler-1.0.0/README.md` & `fastapi-sql-profiler-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,40 +6,51 @@
 
     * Logs database queries made within the web application.
     * Captures query execution times, query texts, and stack traces.
     * Stores query information in a database table along with request details.
     * Provides insights into query performance for debugging and optimization.
 
 ## Installation
-
+```shell
 pip install fastapi-sql-profiler
-
+```
 ## Usage:
-Update the database connection URL in the .env file.
-```python
+1. Update the database connection URL in the .env file.
+```shell
 SQLALCHEMY_DATABASE_URL=<database_connection_url>
 ```
+2. Declare the middleware in your main FastAPI file.
 ```python
 from fastapi_sql_profiler.middleware import SQLProfilerMiddleware
 from fastapi_sql_profiler.add_request import router
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 
 app = FastAPI()
 base = declarative_base()
 engine = create_engine("your-database-connection-string")
 app.include_router(router)
 app.add_middleware(SQLProfilerMiddleware, engine=engine)
-```
+``` 
 
 ## Endpoints
 Please paste the following endpoints in the browser to see the results.
+1. `/all_request`: Displays all captured requests with pagination support.
+
+    ![](https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler/blob/main/doc/images/request.png)
+
+2. `/request_detail/{id}`: Displays details of a specific request identified by its ID.
+
+    ![](https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler/blob/main/doc/images/request_detail.png)
+
+3. `/request_query/{id}`: Displays the queries associated with a specific request identified its ID.
+
+    ![](https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler/blob/main/doc/images/query.png)
+
+4. `/request_query_details/{id}`: Displays details of a specific query identified by its ID.
+
+    ![](https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler/blob/main/doc/images/query_detail.png)
 
-    * `/all_request`: Displays all captured requests with pagination support.
-    * `/request_detail/{id}`: Displays details of a specific request identified by its ID.
-    * `/request_query/{id}`: Displays the queries associated with a specific request identified its ID.
-    * `/request_query_details/{id}`: Displays details of a specific query identified by its ID.
 
-![](https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler/blob/main/doc/images/request.png)
 ## Contributing
 
 Contributions are welcome! If you find a bug or have suggestions for improvements, please open an issue or submit a pull request.
```

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/database.py` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
 load_dotenv()
 SQLALCHEMY_DATABASE_URL = os.getenv("SQLALCHEMY_DATABASE_URL")
 
 engine = create_engine(
-    SQLALCHEMY_DATABASE_URL, connect_args={"check_same_thread": False},
+    SQLALCHEMY_DATABASE_URL,
 )
 SessionLocal = sessionmaker(
     autocommit=False, autoflush=False, bind=engine)
 session = SessionLocal()
 
 
 Base = declarative_base()
```

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/middleware.py` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         elif "application/json" in content_type:
             raw_body = await request.body()
             body = raw_body.decode()
         else:
             raw_body = ''
             body = ''
         request_path = request.url.path
-        if request_path == '/all_request' or request_path.startswith(('/request_detail', '/request_query','/favicon')):
+        if request_path == '/all_request' or request_path.startswith(('/request_detail', '/request_query','/favicon','/clear_db')):
             response = await call_next(request)
         else:
             requset_data = self.add_request(request, raw_body, body)
             request_id = requset_data.id
             session_handler = SessionHandler(self.engine)
             session_handler.start()
             response = await call_next(request)
```

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/models.py` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/request.html` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/request.html`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/request_show.html` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/request_show.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,180 @@
 00000000: 7b25 2065 7874 656e 6473 2027 6261 7365  {% extends 'base
 00000010: 2e68 746d 6c27 2025 7d0a 0a7b 2520 626c  .html' %}..{% bl
-00000020: 6f63 6b20 636f 6e74 656e 7420 257d 0a0a  ock content %}..
-00000030: 3c64 6976 2063 6c61 7373 3d22 726f 7720  <div class="row 
-00000040: 726f 772d 636f 6c73 2d31 2072 6f77 2d63  row-cols-1 row-c
-00000050: 6f6c 732d 6d64 2d35 2067 2d34 206d 742d  ols-md-5 g-4 mt-
-00000060: 3220 7078 2d34 223e 0a20 2020 207b 2520  2 px-4">.    {% 
-00000070: 666f 7220 7265 7175 6573 745f 696e 666f  for request_info
-00000080: 2069 6e20 7265 7175 6573 745f 696e 666f   in request_info
-00000090: 2025 7d0a 2020 2020 3c64 6976 2063 6c61   %}.    <div cla
-000000a0: 7373 3d22 636f 6c22 3e0a 2020 2020 2020  ss="col">.      
-000000b0: 2020 3c61 2073 7479 6c65 3d22 7465 7874    <a style="text
-000000c0: 2d64 6563 6f72 6174 696f 6e3a 206e 6f6e  -decoration: non
-000000d0: 653b 2220 6872 6566 3d22 7b7b 2075 726c  e;" href="{{ url
-000000e0: 5f66 6f72 2827 7265 7175 6573 745f 7368  _for('request_sh
-000000f0: 6f77 272c 2069 643d 7265 7175 6573 745f  ow', id=request_
-00000100: 696e 666f 2e69 6429 207d 7d22 3e0a 2020  info.id) }}">.  
-00000110: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00000120: 6c61 7373 3d22 6361 7264 2062 6f72 6465  lass="card borde
-00000130: 722d 3220 626f 7264 6572 2d73 6563 6f6e  r-2 border-secon
-00000140: 6461 7279 2073 6861 646f 7722 3e0a 2020  dary shadow">.  
-00000150: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000160: 6976 2063 6c61 7373 3d22 6361 7264 2d62  iv class="card-b
-00000170: 6f64 7922 3e0a 2020 2020 2020 2020 2020  ody">.          
-00000180: 2020 2020 2020 2020 2020 3c68 3520 636c            <h5 cl
-00000190: 6173 733d 2263 6172 642d 7469 746c 6520  ass="card-title 
-000001a0: 6d62 2d32 223e 0a20 2020 2020 2020 2020  mb-2">.         
-000001b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000001c0: 7370 616e 2063 6c61 7373 3d22 6261 6467  span class="badg
-000001d0: 6520 7b25 2069 6620 7265 7175 6573 745f  e {% if request_
-000001e0: 696e 666f 2e6d 6574 686f 6420 3d3d 2027  info.method == '
-000001f0: 4745 5427 2025 7d62 672d 7375 6363 6573  GET' %}bg-succes
-00000200: 737b 2520 656c 6966 2072 6571 7565 7374  s{% elif request
-00000210: 5f69 6e66 6f2e 6d65 7468 6f64 203d 3d20  _info.method == 
-00000220: 2750 4f53 5427 2025 7d62 672d 7761 726e  'POST' %}bg-warn
-00000230: 696e 677b 2520 656c 6966 2072 6571 7565  ing{% elif reque
-00000240: 7374 5f69 6e66 6f2e 6d65 7468 6f64 203d  st_info.method =
-00000250: 3d20 2744 454c 4554 4527 2025 7d62 672d  = 'DELETE' %}bg-
-00000260: 6461 6e67 6572 7b25 2065 6c69 6620 7265  danger{% elif re
-00000270: 7175 6573 745f 696e 666f 2e6d 6574 686f  quest_info.metho
-00000280: 6420 3d3d 2027 5055 5427 2025 7d62 672d  d == 'PUT' %}bg-
-00000290: 696e 666f 7b25 2065 6c73 6520 257d 6267  info{% else %}bg
-000002a0: 2d73 6563 6f6e 6461 7279 7b25 2065 6e64  -secondary{% end
-000002b0: 6966 2025 7d22 3e0a 2020 2020 2020 2020  if %}">.        
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 2020 2020 7b7b 2072 6571 7565 7374 5f69      {{ request_i
-000002e0: 6e66 6f2e 6d65 7468 6f64 207d 7d0a 2020  nfo.method }}.  
-000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000300: 2020 2020 2020 3c2f 7370 616e 3e0a 2020        </span>.  
-00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000320: 2020 3c2f 6835 3e0a 2020 2020 2020 2020    </h5>.        
-00000330: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000340: 2063 6c61 7373 3d22 6361 7264 2d74 6578   class="card-tex
-00000350: 7422 2073 7479 6c65 3d22 6d61 782d 7769  t" style="max-wi
-00000360: 6474 683a 2032 3030 7078 3b20 6f76 6572  dth: 200px; over
-00000370: 666c 6f77 3a20 6869 6464 656e 3b20 7465  flow: hidden; te
-00000380: 7874 2d6f 7665 7266 6c6f 773a 2065 6c6c  xt-overflow: ell
-00000390: 6970 7369 733b 2077 6869 7465 2d73 7061  ipsis; white-spa
-000003a0: 6365 3a20 6e6f 7772 6170 3b22 3e0a 2020  ce: nowrap;">.  
-000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003c0: 2020 2020 2020 3c73 7472 6f6e 673e 5061        <strong>Pa
-000003d0: 7468 3a3c 2f73 7472 6f6e 673e 207b 7b20  th:</strong> {{ 
-000003e0: 7265 7175 6573 745f 696e 666f 2e70 6174  request_info.pat
-000003f0: 6820 7d7d 0a20 2020 2020 2020 2020 2020  h }}.           
-00000400: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000430: 6361 7264 2d74 6578 7422 2073 7479 6c65  card-text" style
-00000440: 3d22 6d61 782d 7769 6474 683a 2032 3030  ="max-width: 200
-00000450: 7078 3b20 6f76 6572 666c 6f77 3a20 6869  px; overflow: hi
-00000460: 6464 656e 3b20 7465 7874 2d6f 7665 7266  dden; text-overf
-00000470: 6c6f 773a 2065 6c6c 6970 7369 733b 2077  low: ellipsis; w
-00000480: 6869 7465 2d73 7061 6365 3a20 6e6f 7772  hite-space: nowr
-00000490: 6170 3b22 3e0a 2020 2020 2020 2020 2020  ap;">.          
-000004a0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-000004b0: 7472 6f6e 673e 5469 6d65 2054 616b 656e  trong>Time Taken
-000004c0: 3a3c 2f73 7472 6f6e 673e 207b 7b20 7265  :</strong> {{ re
-000004d0: 7175 6573 745f 696e 666f 2e74 696d 655f  quest_info.time_
-000004e0: 7461 6b65 6e20 7d7d 206d 730a 2020 2020  taken }} ms.    
-000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000500: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000510: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000520: 636c 6173 733d 2263 6172 642d 7465 7874  class="card-text
-00000530: 2220 7374 796c 653d 226d 6178 2d77 6964  " style="max-wid
-00000540: 7468 3a20 3230 3070 783b 206f 7665 7266  th: 200px; overf
-00000550: 6c6f 773a 2068 6964 6465 6e3b 2074 6578  low: hidden; tex
-00000560: 742d 6f76 6572 666c 6f77 3a20 656c 6c69  t-overflow: elli
-00000570: 7073 6973 3b20 7768 6974 652d 7370 6163  psis; white-spac
-00000580: 653a 206e 6f77 7261 703b 223e 0a20 2020  e: nowrap;">.   
-00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005a0: 2020 2020 203c 7374 726f 6e67 3e54 6f74       <strong>Tot
-000005b0: 616c 2051 7565 7269 6573 3a3c 2f73 7472  al Queries:</str
-000005c0: 6f6e 673e 207b 7b20 7265 7175 6573 745f  ong> {{ request_
-000005d0: 696e 666f 2e74 6f74 616c 5f71 7565 7269  info.total_queri
-000005e0: 6573 207d 7d20 7175 6572 6965 730a 2020  es }} queries.  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00000610: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000620: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000630: 763e 0a20 2020 2020 2020 203c 2f61 3e0a  v>.        </a>.
-00000640: 2020 2020 3c2f 6469 763e 0a20 2020 207b      </div>.    {
-00000650: 2520 656e 6466 6f72 2025 7d0a 3c2f 6469  % endfor %}.</di
-00000660: 763e 0a0a 3c6e 6176 3e0a 2020 2020 3c75  v>..<nav>.    <u
-00000670: 6c20 636c 6173 733d 2270 6167 696e 6174  l class="paginat
-00000680: 696f 6e20 6a75 7374 6966 792d 636f 6e74  ion justify-cont
-00000690: 656e 742d 6365 6e74 6572 206d 742d 3422  ent-center mt-4"
-000006a0: 3e0a 2020 2020 2020 2020 7b25 2069 6620  >.        {% if 
-000006b0: 7061 6765 203e 2031 2025 7d0a 2020 2020  page > 1 %}.    
-000006c0: 2020 2020 3c6c 6920 636c 6173 733d 2270      <li class="p
-000006d0: 6167 652d 6974 656d 223e 0a20 2020 2020  age-item">.     
-000006e0: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
-000006f0: 2270 6167 652d 6c69 6e6b 2220 6872 6566  "page-link" href
-00000700: 3d22 3f70 6167 653d 7b7b 2070 6167 6520  ="?page={{ page 
-00000710: 2d20 3120 7d7d 266c 696d 6974 3d7b 7b20  - 1 }}&limit={{ 
-00000720: 6c69 6d69 7420 7d7d 223e 5072 6576 696f  limit }}">Previo
-00000730: 7573 3c2f 613e 0a20 2020 2020 2020 203c  us</a>.        <
-00000740: 2f6c 693e 0a20 2020 2020 2020 207b 2520  /li>.        {% 
-00000750: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
-00000760: 3c6c 6920 636c 6173 733d 2270 6167 652d  <li class="page-
-00000770: 6974 656d 2064 6973 6162 6c65 6422 3e0a  item disabled">.
-00000780: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
-00000790: 6c61 7373 3d22 7061 6765 2d6c 696e 6b22  lass="page-link"
-000007a0: 2068 7265 663d 2223 2220 7461 6269 6e64   href="#" tabind
-000007b0: 6578 3d22 2d31 2220 6172 6961 2d64 6973  ex="-1" aria-dis
-000007c0: 6162 6c65 643d 2274 7275 6522 3e50 7265  abled="true">Pre
-000007d0: 7669 6f75 733c 2f61 3e0a 2020 2020 2020  vious</a>.      
-000007e0: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
-000007f0: 7b25 2065 6e64 6966 2025 7d0a 0a20 2020  {% endif %}..   
-00000800: 2020 2020 207b 2520 6966 2070 6167 6520       {% if page 
-00000810: 3c20 746f 7461 6c5f 7061 6765 7320 257d  < total_pages %}
-00000820: 203c 6c69 2063 6c61 7373 3d22 7061 6765   <li class="page
-00000830: 2d69 7465 6d22 3e0a 2020 2020 2020 2020  -item">.        
-00000840: 2020 2020 3c61 2063 6c61 7373 3d22 7061      <a class="pa
-00000850: 6765 2d6c 696e 6b22 2068 7265 663d 223f  ge-link" href="?
-00000860: 7061 6765 3d7b 7b20 7061 6765 202b 2031  page={{ page + 1
-00000870: 207d 7d26 6c69 6d69 743d 7b7b 206c 696d   }}&limit={{ lim
-00000880: 6974 207d 7d22 3e4e 6578 743c 2f61 3e0a  it }}">Next</a>.
-00000890: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
-000008a0: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
-000008b0: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-000008c0: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
-000008d0: 7061 6765 2d69 7465 6d20 6469 7361 626c  page-item disabl
-000008e0: 6564 223e 0a20 2020 2020 2020 2020 2020  ed">.           
-000008f0: 2020 2020 203c 6120 636c 6173 733d 2270       <a class="p
-00000900: 6167 652d 6c69 6e6b 2220 6872 6566 3d22  age-link" href="
-00000910: 2322 2074 6162 696e 6465 783d 222d 3122  #" tabindex="-1"
-00000920: 2061 7269 612d 6469 7361 626c 6564 3d22   aria-disabled="
-00000930: 7472 7565 223e 4e65 7874 3c2f 613e 0a20  true">Next</a>. 
-00000940: 2020 2020 2020 2020 2020 203c 2f6c 693e             </li>
-00000950: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00000960: 656e 6469 6620 257d 0a20 2020 203c 2f75  endif %}.    </u
-00000970: 6c3e 0a3c 2f6e 6176 3e0a 7b25 2065 6e64  l>.</nav>.{% end
-00000980: 626c 6f63 6b20 257d                      block %}
+00000020: 6f63 6b20 7374 796c 6520 257d 0a3c 7374  ock style %}.<st
+00000030: 796c 653e 0a20 2020 202e 7061 6769 6e61  yle>.    .pagina
+00000040: 7469 6f6e 207b 0a20 2020 2020 2020 2064  tion {.        d
+00000050: 6973 706c 6179 3a20 666c 6578 3b0a 2020  isplay: flex;.  
+00000060: 2020 2020 2020 6a75 7374 6966 792d 636f        justify-co
+00000070: 6e74 656e 743a 2066 6c65 782d 656e 643b  ntent: flex-end;
+00000080: 0a20 2020 207d 0a20 2020 202e 7072 2d33  .    }.    .pr-3
+00000090: 207b 0a20 2020 2020 2020 2070 6164 6469   {.        paddi
+000000a0: 6e67 2d72 6967 6874 3a20 3172 656d 3b20  ng-right: 1rem; 
+000000b0: 0a20 2020 207d 0a3c 2f73 7479 6c65 3e0a  .    }.</style>.
+000000c0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a7b  {% endblock %}.{
+000000d0: 2520 626c 6f63 6b20 636f 6e74 656e 7420  % block content 
+000000e0: 257d 0a0a 3c64 6976 2063 6c61 7373 3d22  %}..<div class="
+000000f0: 726f 7720 726f 772d 636f 6c73 2d31 2072  row row-cols-1 r
+00000100: 6f77 2d63 6f6c 732d 6d64 2d35 2067 2d34  ow-cols-md-5 g-4
+00000110: 206d 742d 3220 7078 2d34 223e 0a20 2020   mt-2 px-4">.   
+00000120: 207b 2520 666f 7220 7265 7175 6573 745f   {% for request_
+00000130: 696e 666f 2069 6e20 7265 7175 6573 745f  info in request_
+00000140: 696e 666f 2025 7d0a 2020 2020 3c64 6976  info %}.    <div
+00000150: 2063 6c61 7373 3d22 636f 6c22 3e0a 2020   class="col">.  
+00000160: 2020 2020 2020 3c61 2073 7479 6c65 3d22        <a style="
+00000170: 7465 7874 2d64 6563 6f72 6174 696f 6e3a  text-decoration:
+00000180: 206e 6f6e 653b 2220 6872 6566 3d22 7b7b   none;" href="{{
+00000190: 2075 726c 5f66 6f72 2827 7265 7175 6573   url_for('reques
+000001a0: 745f 7368 6f77 272c 2069 643d 7265 7175  t_show', id=requ
+000001b0: 6573 745f 696e 666f 2e69 6429 207d 7d22  est_info.id) }}"
+000001c0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+000001d0: 6976 2063 6c61 7373 3d22 6361 7264 2062  iv class="card b
+000001e0: 6f72 6465 722d 3220 626f 7264 6572 2d73  order-2 border-s
+000001f0: 6563 6f6e 6461 7279 2073 6861 646f 7722  econdary shadow"
+00000200: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000210: 2020 3c64 6976 2063 6c61 7373 3d22 6361    <div class="ca
+00000220: 7264 2d62 6f64 7922 3e0a 2020 2020 2020  rd-body">.      
+00000230: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+00000240: 3520 636c 6173 733d 2263 6172 642d 7469  5 class="card-ti
+00000250: 746c 6520 6d62 2d32 223e 0a20 2020 2020  tle mb-2">.     
+00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000270: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+00000280: 6261 6467 6520 7b25 2069 6620 7265 7175  badge {% if requ
+00000290: 6573 745f 696e 666f 2e6d 6574 686f 6420  est_info.method 
+000002a0: 3d3d 2027 4745 5427 2025 7d62 672d 7375  == 'GET' %}bg-su
+000002b0: 6363 6573 737b 2520 656c 6966 2072 6571  ccess{% elif req
+000002c0: 7565 7374 5f69 6e66 6f2e 6d65 7468 6f64  uest_info.method
+000002d0: 203d 3d20 2750 4f53 5427 2025 7d62 672d   == 'POST' %}bg-
+000002e0: 7761 726e 696e 677b 2520 656c 6966 2072  warning{% elif r
+000002f0: 6571 7565 7374 5f69 6e66 6f2e 6d65 7468  equest_info.meth
+00000300: 6f64 203d 3d20 2744 454c 4554 4527 2025  od == 'DELETE' %
+00000310: 7d62 672d 6461 6e67 6572 7b25 2065 6c69  }bg-danger{% eli
+00000320: 6620 7265 7175 6573 745f 696e 666f 2e6d  f request_info.m
+00000330: 6574 686f 6420 3d3d 2027 5055 5427 2025  ethod == 'PUT' %
+00000340: 7d62 672d 696e 666f 7b25 2065 6c73 6520  }bg-info{% else 
+00000350: 257d 6267 2d73 6563 6f6e 6461 7279 7b25  %}bg-secondary{%
+00000360: 2065 6e64 6966 2025 7d22 3e0a 2020 2020   endif %}">.    
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 2020 2020 2020 7b7b 2072 6571 7565          {{ reque
+00000390: 7374 5f69 6e66 6f2e 6d65 7468 6f64 207d  st_info.method }
+000003a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000003b0: 2020 2020 2020 2020 2020 3c2f 7370 616e            </span
+000003c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000003d0: 2020 2020 2020 3c2f 6835 3e0a 2020 2020        </h5>.    
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 3c64 6976 2063 6c61 7373 3d22 6361 7264  <div class="card
+00000400: 2d74 6578 7422 2073 7479 6c65 3d22 6d61  -text" style="ma
+00000410: 782d 7769 6474 683a 2032 3530 7078 3b20  x-width: 250px; 
+00000420: 6f76 6572 666c 6f77 3a20 6869 6464 656e  overflow: hidden
+00000430: 3b20 7465 7874 2d6f 7665 7266 6c6f 773a  ; text-overflow:
+00000440: 2065 6c6c 6970 7369 733b 2077 6869 7465   ellipsis; white
+00000450: 2d73 7061 6365 3a20 6e6f 7772 6170 3b22  -space: nowrap;"
+00000460: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000470: 2020 2020 2020 2020 2020 7b7b 2072 6571            {{ req
+00000480: 7565 7374 5f69 6e66 6f2e 7374 6172 745f  uest_info.start_
+00000490: 7469 6d65 207d 7d0a 2020 2020 2020 2020  time }}.        
+000004a0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+000004b0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+000004c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000004d0: 733d 2263 6172 642d 7465 7874 2220 7374  s="card-text" st
+000004e0: 796c 653d 226d 6178 2d77 6964 7468 3a20  yle="max-width: 
+000004f0: 3230 3070 783b 206f 7665 7266 6c6f 773a  200px; overflow:
+00000500: 2068 6964 6465 6e3b 2074 6578 742d 6f76   hidden; text-ov
+00000510: 6572 666c 6f77 3a20 656c 6c69 7073 6973  erflow: ellipsis
+00000520: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+00000530: 6f77 7261 703b 223e 0a20 2020 2020 2020  owrap;">.       
+00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000550: 203c 7374 726f 6e67 3e50 6174 683a 3c2f   <strong>Path:</
+00000560: 7374 726f 6e67 3e20 7b7b 2072 6571 7565  strong> {{ reque
+00000570: 7374 5f69 6e66 6f2e 7061 7468 207d 7d0a  st_info.path }}.
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+000005a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000005b0: 6469 7620 636c 6173 733d 2263 6172 642d  div class="card-
+000005c0: 7465 7874 2220 7374 796c 653d 226d 6178  text" style="max
+000005d0: 2d77 6964 7468 3a20 3230 3070 783b 206f  -width: 200px; o
+000005e0: 7665 7266 6c6f 773a 2068 6964 6465 6e3b  verflow: hidden;
+000005f0: 2074 6578 742d 6f76 6572 666c 6f77 3a20   text-overflow: 
+00000600: 656c 6c69 7073 6973 3b20 7768 6974 652d  ellipsis; white-
+00000610: 7370 6163 653a 206e 6f77 7261 703b 223e  space: nowrap;">
+00000620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000630: 2020 2020 2020 2020 203c 7374 726f 6e67           <strong
+00000640: 3e54 696d 6520 5461 6b65 6e3a 3c2f 7374  >Time Taken:</st
+00000650: 726f 6e67 3e20 7b7b 2072 6571 7565 7374  rong> {{ request
+00000660: 5f69 6e66 6f2e 7469 6d65 5f74 616b 656e  _info.time_taken
+00000670: 207d 7d20 6d73 0a20 2020 2020 2020 2020   }} ms.         
+00000680: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000690: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000006a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000006b0: 3d22 6361 7264 2d74 6578 7422 2073 7479  ="card-text" sty
+000006c0: 6c65 3d22 6d61 782d 7769 6474 683a 2032  le="max-width: 2
+000006d0: 3030 7078 3b20 6f76 6572 666c 6f77 3a20  00px; overflow: 
+000006e0: 6869 6464 656e 3b20 7465 7874 2d6f 7665  hidden; text-ove
+000006f0: 7266 6c6f 773a 2065 6c6c 6970 7369 733b  rflow: ellipsis;
+00000700: 2077 6869 7465 2d73 7061 6365 3a20 6e6f   white-space: no
+00000710: 7772 6170 3b22 3e0a 2020 2020 2020 2020  wrap;">.        
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000730: 3c73 7472 6f6e 673e 546f 7461 6c20 5175  <strong>Total Qu
+00000740: 6572 6965 733a 3c2f 7374 726f 6e67 3e20  eries:</strong> 
+00000750: 7b7b 2072 6571 7565 7374 5f69 6e66 6f2e  {{ request_info.
+00000760: 746f 7461 6c5f 7175 6572 6965 7320 7d7d  total_queries }}
+00000770: 2071 7565 7269 6573 0a20 2020 2020 2020   queries.       
+00000780: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00000790: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000007a0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+000007b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000007c0: 2020 2020 2020 3c2f 613e 0a20 2020 203c        </a>.    <
+000007d0: 2f64 6976 3e0a 2020 2020 7b25 2065 6e64  /div>.    {% end
+000007e0: 666f 7220 257d 0a3c 2f64 6976 3e0a 0a7b  for %}.</div>..{
+000007f0: 2520 6966 2074 6f74 616c 5f70 6167 6573  % if total_pages
+00000800: 203e 3d20 3220 257d 0a3c 6e61 763e 0a20   >= 2 %}.<nav>. 
+00000810: 2020 203c 756c 2063 6c61 7373 3d22 7061     <ul class="pa
+00000820: 6769 6e61 7469 6f6e 206a 7573 7469 6679  gination justify
+00000830: 2d63 6f6e 7465 6e74 2d65 6e64 206d 742d  -content-end mt-
+00000840: 3420 7072 2d33 223e 0a20 2020 2020 2020  4 pr-3">.       
+00000850: 207b 2520 6966 2070 6167 6520 3e20 3120   {% if page > 1 
+00000860: 257d 0a20 2020 2020 2020 203c 6c69 2063  %}.        <li c
+00000870: 6c61 7373 3d22 7061 6765 2d69 7465 6d22  lass="page-item"
+00000880: 3e0a 2020 2020 2020 2020 2020 2020 3c61  >.            <a
+00000890: 2063 6c61 7373 3d22 7061 6765 2d6c 696e   class="page-lin
+000008a0: 6b22 2068 7265 663d 223f 7061 6765 3d7b  k" href="?page={
+000008b0: 7b20 7061 6765 202d 2031 207d 7d26 6c69  { page - 1 }}&li
+000008c0: 6d69 743d 7b7b 206c 696d 6974 207d 7d22  mit={{ limit }}"
+000008d0: 3e50 7265 7669 6f75 733c 2f61 3e0a 2020  >Previous</a>.  
+000008e0: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+000008f0: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+00000900: 2020 2020 2020 203c 6c69 2063 6c61 7373         <li class
+00000910: 3d22 7061 6765 2d69 7465 6d20 6469 7361  ="page-item disa
+00000920: 626c 6564 223e 0a20 2020 2020 2020 2020  bled">.         
+00000930: 2020 203c 6120 636c 6173 733d 2270 6167     <a class="pag
+00000940: 652d 6c69 6e6b 2220 6872 6566 3d22 2322  e-link" href="#"
+00000950: 2074 6162 696e 6465 783d 222d 3122 2061   tabindex="-1" a
+00000960: 7269 612d 6469 7361 626c 6564 3d22 7472  ria-disabled="tr
+00000970: 7565 223e 5072 6576 696f 7573 3c2f 613e  ue">Previous</a>
+00000980: 0a20 2020 2020 2020 203c 2f6c 693e 0a20  .        </li>. 
+00000990: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000009a0: 257d 0a0a 2020 2020 2020 2020 7b25 2069  %}..        {% i
+000009b0: 6620 7061 6765 203c 2074 6f74 616c 5f70  f page < total_p
+000009c0: 6167 6573 2025 7d20 3c6c 6920 636c 6173  ages %} <li clas
+000009d0: 733d 2270 6167 652d 6974 656d 223e 0a20  s="page-item">. 
+000009e0: 2020 2020 2020 2020 2020 203c 6120 636c             <a cl
+000009f0: 6173 733d 2270 6167 652d 6c69 6e6b 2220  ass="page-link" 
+00000a00: 6872 6566 3d22 3f70 6167 653d 7b7b 2070  href="?page={{ p
+00000a10: 6167 6520 2b20 3120 7d7d 266c 696d 6974  age + 1 }}&limit
+00000a20: 3d7b 7b20 6c69 6d69 7420 7d7d 223e 4e65  ={{ limit }}">Ne
+00000a30: 7874 3c2f 613e 0a20 2020 2020 2020 2020  xt</a>.         
+00000a40: 2020 203c 2f6c 693e 0a20 2020 2020 2020     </li>.       
+00000a50: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+00000a60: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+00000a70: 636c 6173 733d 2270 6167 652d 6974 656d  class="page-item
+00000a80: 2064 6973 6162 6c65 6422 3e0a 2020 2020   disabled">.    
+00000a90: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
+00000aa0: 6c61 7373 3d22 7061 6765 2d6c 696e 6b22  lass="page-link"
+00000ab0: 2068 7265 663d 2223 2220 7461 6269 6e64   href="#" tabind
+00000ac0: 6578 3d22 2d31 2220 6172 6961 2d64 6973  ex="-1" aria-dis
+00000ad0: 6162 6c65 643d 2274 7275 6522 3e4e 6578  abled="true">Nex
+00000ae0: 743c 2f61 3e0a 2020 2020 2020 2020 2020  t</a>.          
+00000af0: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
+00000b00: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00000b10: 2020 2020 3c2f 756c 3e0a 3c2f 6e61 763e      </ul>.</nav>
+00000b20: 0a7b 2520 656e 6469 6620 257d 0a7b 2520  .{% endif %}.{% 
+00000b30: 656e 6462 6c6f 636b 2025 7d              endblock %}
```

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/sql_query.html` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/sql_query.html`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler/templates/sql_query_detail.html` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler/templates/sql_query_detail.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,85 @@
 00000000: 7b25 2065 7874 656e 6473 2027 6261 7365  {% extends 'base
 00000010: 2e68 746d 6c27 2025 7d0a 0a7b 2520 626c  .html' %}..{% bl
-00000020: 6f63 6b20 636f 6e74 656e 7420 257d 0a3c  ock content %}.<
-00000030: 6469 7620 6964 3d22 642d 666c 6578 2066  div id="d-flex f
-00000040: 6c65 782d 636f 6c75 6d6e 2220 636c 6173  lex-column" clas
-00000050: 733d 226d 742d 3422 2073 7479 6c65 3d22  s="mt-4" style="
-00000060: 7061 6464 696e 672d 6c65 6674 3a20 3232  padding-left: 22
-00000070: 3570 783b 223e 0a20 2020 203c 7072 6520  5px;">.    <pre 
-00000080: 6964 3d22 7175 6572 7922 2073 7479 6c65  id="query" style
-00000090: 3d22 666f 6e74 2d73 697a 653a 206d 6564  ="font-size: med
-000000a0: 6975 6d3b 223e 3c63 6f64 653e 7b7b 2071  ium;"><code>{{ q
-000000b0: 7565 7279 5f64 6574 6169 6c2e 7175 6572  uery_detail.quer
-000000c0: 7920 7d7d 3c62 723e 3c2f 636f 6465 3e3c  y }}<br></code><
-000000d0: 2f70 7265 3e0a 2020 2020 3c64 6976 2069  /pre>.    <div i
-000000e0: 643d 2271 7565 7279 2d69 6e66 6f2d 6469  d="query-info-di
-000000f0: 7622 3e0a 2020 2020 2020 2020 3c64 6976  v">.        <div
-00000100: 2069 643d 2274 696d 652d 7461 6b65 6e2d   id="time-taken-
-00000110: 6469 7622 3e0a 2020 2020 2020 2020 2020  div">.          
-00000120: 2020 3c73 7061 6e20 636c 6173 733d 226e    <span class="n
-00000130: 756d 6572 6963 223e 7b7b 7175 6572 795f  umeric">{{query_
-00000140: 6465 7461 696c 2e74 696d 655f 7461 6b65  detail.time_take
-00000150: 6e7d 7d3c 7370 616e 2063 6c61 7373 3d22  n}}<span class="
-00000160: 756e 6974 223e 206d 7320 6f6e 2071 7565  unit"> ms on que
-00000170: 7279 3c2f 7370 616e 3e3c 2f73 7061 6e3e  ry</span></span>
-00000180: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00000190: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
-000001a0: 3e0a 0a0a 3c64 6976 2063 6c61 7373 3d22  >...<div class="
-000001b0: 642d 666c 6578 2066 6c65 782d 636f 6c75  d-flex flex-colu
-000001c0: 6d6e 2061 6c69 676e 2d69 7465 6d73 2d63  mn align-items-c
-000001d0: 656e 7465 7220 6a75 7374 6966 792d 636f  enter justify-co
-000001e0: 6e74 656e 742d 6365 6e74 6572 2067 6170  ntent-center gap
-000001f0: 2d33 206d 742d 3322 3e0a 2020 2020 3c64  -3 mt-3">.    <d
-00000200: 6976 2063 6c61 7373 3d22 6361 7264 206d  iv class="card m
-00000210: 742d 3222 2073 7479 6c65 3d22 7769 6474  t-2" style="widt
-00000220: 683a 2037 3025 3b20 626f 7264 6572 3a20  h: 70%; border: 
-00000230: 3170 7820 736f 6c69 6420 2363 6363 3b20  1px solid #ccc; 
-00000240: 626f 7264 6572 2d72 6164 6975 733a 2031  border-radius: 1
-00000250: 3070 783b 2062 6f78 2d73 6861 646f 773a  0px; box-shadow:
-00000260: 2030 2032 7078 2034 7078 2072 6762 6128   0 2px 4px rgba(
-00000270: 302c 2030 2c20 302c 2030 2e31 293b 223e  0, 0, 0, 0.1);">
-00000280: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
-00000290: 6173 733d 2263 6172 642d 6865 6164 6572  ass="card-header
-000002a0: 2220 7374 796c 653d 2262 6163 6b67 726f  " style="backgro
-000002b0: 756e 642d 636f 6c6f 723a 2023 6638 6639  und-color: #f8f9
-000002c0: 6661 3b20 626f 7264 6572 2d62 6f74 746f  fa; border-botto
-000002d0: 6d3a 2031 7078 2073 6f6c 6964 2023 6363  m: 1px solid #cc
-000002e0: 633b 2062 6f72 6465 722d 7261 6469 7573  c; border-radius
-000002f0: 3a20 3130 7078 2031 3070 7820 3020 303b  : 10px 10px 0 0;
-00000300: 223e 0a20 2020 2020 2020 2020 2020 2054  ">.            T
-00000310: 7261 6365 6261 636b 0a20 2020 2020 2020  raceback.       
-00000320: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000330: 3c64 6976 2063 6c61 7373 3d22 6361 7264  <div class="card
-00000340: 2d62 6f64 7922 3e0a 2020 2020 2020 2020  -body">.        
-00000350: 2020 2020 3c70 7265 2073 7479 6c65 3d22      <pre style="
-00000360: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
-00000370: 2d77 7261 703b 206f 7665 7266 6c6f 772d  -wrap; overflow-
-00000380: 783a 2061 7574 6f3b 223e 7b7b 7175 6572  x: auto;">{{quer
-00000390: 795f 6465 7461 696c 2e74 7261 6365 6261  y_detail.traceba
-000003a0: 636b 7d7d 3c2f 7072 653e 0a20 2020 2020  ck}}</pre>.     
-000003b0: 2020 203c 2f64 6976 3e0a 2020 2020 3c2f     </div>.    </
-000003c0: 6469 763e 0a0a 3c2f 6469 763e 0a7b 2520  div>..</div>.{% 
-000003d0: 656e 6462 6c6f 636b 2025 7d              endblock %}
+00000020: 6f63 6b20 7374 796c 6520 257d 0a3c 7374  ock style %}.<st
+00000030: 796c 653e 0a20 2020 202e 6361 7264 2d62  yle>.    .card-b
+00000040: 6f64 797b 0a20 2020 2020 2020 2066 6f6e  ody{.        fon
+00000050: 742d 7369 7a65 3a20 736d 616c 6c3b 0a20  t-size: small;. 
+00000060: 2020 207d 0a20 2020 202e 6669 6c65 2d70     }.    .file-p
+00000070: 6174 682d 6973 2d74 6869 7264 2d70 6172  ath-is-third-par
+00000080: 7479 207b 0a20 2020 2020 2020 2020 2020  ty {.           
+00000090: 2066 6f6e 742d 7765 6967 6874 3a20 626f   font-weight: bo
+000000a0: 6c64 3b0a 2020 2020 2020 2020 7d0a 3c2f  ld;.        }.</
+000000b0: 7374 796c 653e 0a20 2020 200a 7b25 2065  style>.    .{% e
+000000c0: 6e64 626c 6f63 6b20 257d 0a0a 0a7b 2520  ndblock %}...{% 
+000000d0: 626c 6f63 6b20 636f 6e74 656e 7420 257d  block content %}
+000000e0: 0a3c 6469 7620 6964 3d22 642d 666c 6578  .<div id="d-flex
+000000f0: 2066 6c65 782d 636f 6c75 6d6e 2220 636c   flex-column" cl
+00000100: 6173 733d 226d 742d 3422 2073 7479 6c65  ass="mt-4" style
+00000110: 3d22 7061 6464 696e 672d 6c65 6674 3a20  ="padding-left: 
+00000120: 3232 3570 783b 223e 0a20 2020 203c 7072  225px;">.    <pr
+00000130: 6520 6964 3d22 7175 6572 7922 2073 7479  e id="query" sty
+00000140: 6c65 3d22 666f 6e74 2d73 697a 653a 206d  le="font-size: m
+00000150: 6564 6975 6d3b 223e 3c63 6f64 653e 7b7b  edium;"><code>{{
+00000160: 2071 7565 7279 5f64 6574 6169 6c2e 7175   query_detail.qu
+00000170: 6572 7920 7d7d 3c62 723e 3c2f 636f 6465  ery }}<br></code
+00000180: 3e3c 2f70 7265 3e0a 2020 2020 3c64 6976  ></pre>.    <div
+00000190: 2069 643d 2271 7565 7279 2d69 6e66 6f2d   id="query-info-
+000001a0: 6469 7622 3e0a 2020 2020 2020 2020 3c64  div">.        <d
+000001b0: 6976 2069 643d 2274 696d 652d 7461 6b65  iv id="time-take
+000001c0: 6e2d 6469 7622 3e0a 2020 2020 2020 2020  n-div">.        
+000001d0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+000001e0: 226e 756d 6572 6963 223e 7b7b 7175 6572  "numeric">{{quer
+000001f0: 795f 6465 7461 696c 2e74 696d 655f 7461  y_detail.time_ta
+00000200: 6b65 6e7d 7d3c 7370 616e 2063 6c61 7373  ken}}<span class
+00000210: 3d22 756e 6974 223e 206d 733c 2f73 7061  ="unit"> ms</spa
+00000220: 6e3e 3c2f 7370 616e 3e0a 2020 2020 2020  n></span>.      
+00000230: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
+00000240: 6976 3e0a 3c2f 6469 763e 0a0a 0a3c 6469  iv>.</div>...<di
+00000250: 7620 636c 6173 733d 2264 2d66 6c65 7820  v class="d-flex 
+00000260: 666c 6578 2d63 6f6c 756d 6e20 616c 6967  flex-column alig
+00000270: 6e2d 6974 656d 732d 6365 6e74 6572 206a  n-items-center j
+00000280: 7573 7469 6679 2d63 6f6e 7465 6e74 2d63  ustify-content-c
+00000290: 656e 7465 7220 6761 702d 3320 6d74 2d33  enter gap-3 mt-3
+000002a0: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
+000002b0: 733d 2263 6172 6420 6d74 2d32 2220 7374  s="card mt-2" st
+000002c0: 796c 653d 2277 6964 7468 3a20 3730 253b  yle="width: 70%;
+000002d0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000002e0: 6964 2023 6363 633b 2062 6f72 6465 722d  id #ccc; border-
+000002f0: 7261 6469 7573 3a20 3130 7078 3b20 626f  radius: 10px; bo
+00000300: 782d 7368 6164 6f77 3a20 3020 3270 7820  x-shadow: 0 2px 
+00000310: 3470 7820 7267 6261 2830 2c20 302c 2030  4px rgba(0, 0, 0
+00000320: 2c20 302e 3129 3b22 3e0a 2020 2020 2020  , 0.1);">.      
+00000330: 2020 3c64 6976 2063 6c61 7373 3d22 6361    <div class="ca
+00000340: 7264 2d68 6561 6465 7222 2073 7479 6c65  rd-header" style
+00000350: 3d22 6261 636b 6772 6f75 6e64 2d63 6f6c  ="background-col
+00000360: 6f72 3a20 2366 3866 3966 613b 2062 6f72  or: #f8f9fa; bor
+00000370: 6465 722d 626f 7474 6f6d 3a20 3170 7820  der-bottom: 1px 
+00000380: 736f 6c69 6420 2363 6363 3b20 626f 7264  solid #ccc; bord
+00000390: 6572 2d72 6164 6975 733a 2031 3070 7820  er-radius: 10px 
+000003a0: 3130 7078 2030 2030 3b22 3e0a 2020 2020  10px 0 0;">.    
+000003b0: 2020 2020 2020 2020 5472 6163 6562 6163          Tracebac
+000003c0: 6b0a 2020 2020 2020 2020 3c2f 6469 763e  k.        </div>
+000003d0: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
+000003e0: 6173 733d 2263 6172 642d 626f 6479 223e  ass="card-body">
+000003f0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00000400: 666f 7220 6c6e 2069 6e20 7472 6163 6562  for ln in traceb
+00000410: 6163 6b20 257d 0a20 2020 2020 2020 2020  ack %}.         
+00000420: 2020 2020 2020 207b 2520 6966 206c 6e20         {% if ln 
+00000430: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000440: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000450: 733d 2266 696c 652d 7061 7468 2d7b 2520  s="file-path-{% 
+00000460: 6966 2076 6972 7475 616c 656e 765f 7061  if virtualenv_pa
+00000470: 7468 2069 6e20 6c6e 2025 7d6e 6f74 2d7b  th in ln %}not-{
+00000480: 2520 656c 7365 2025 7d69 732d 7b25 2065  % else %}is-{% e
+00000490: 6e64 6966 2025 7d74 6869 7264 2d70 6172  ndif %}third-par
+000004a0: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+000004b0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+000004c0: 6c6e 207d 7d0a 2020 2020 2020 2020 2020  ln }}.          
+000004d0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000004e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004f0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+00000500: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
+00000510: 6f72 2025 7d0a 2020 2020 2020 2020 3c2f  or %}.        </
+00000520: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
+00000530: 0a3c 2f64 6976 3e0a 7b25 2065 6e64 626c  .</div>.{% endbl
+00000540: 6f63 6b20 257d                           ock %}
```

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/PKG-INFO` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql-profiler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Middleware for profiling and logging database queries in a Python web application
 Home-page: https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git
 Author: Ganesh Sali
 Author-email: ganesh@sarvadhi.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-sql-profiler-1.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt` & `fastapi-sql-profiler-1.0.1/fastapi_sql_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-1.0.0/setup.py` & `fastapi-sql-profiler-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fastapi-sql-profiler',
-    version='1.0.0',
+    version='1.0.1',
     description='Middleware for profiling and logging database queries in a Python web application',
     package_data={'fastapi_sql_profiler': ['templates/*']},
     author='Ganesh Sali',
     author_email='ganesh@sarvadhi.com',
     url="https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git",
     install_requires=[
         "fastapi >= 0.97.0",
```

### Comparing `fastapi-sql-profiler-1.0.0/tests/test_sql_profiler.py` & `fastapi-sql-profiler-1.0.1/tests/test_sql_profiler.py`

 * *Files identical despite different names*

