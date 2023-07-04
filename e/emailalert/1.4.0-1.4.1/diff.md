# Comparing `tmp/emailalert-1.4.0.tar.gz` & `tmp/emailalert-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.4.0.tar", last modified: Tue Jun 20 09:01:20 2023, max compression
+gzip compressed data, was "emailalert-1.4.1.tar", last modified: Tue Jul  4 04:53:17 2023, max compression
```

## Comparing `emailalert-1.4.0.tar` & `emailalert-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:01:20.929155 emailalert-1.4.0/
--rw-rw-rw-   0        0        0      178 2023-06-20 09:01:20.927309 emailalert-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 09:01:20.888142 emailalert-1.4.0/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 09:01:20.000000 emailalert-1.4.0/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 09:01:20.000000 emailalert-1.4.0/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 09:01:20.000000 emailalert-1.4.0/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 09:01:20.000000 emailalert-1.4.0/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 09:01:20.922153 emailalert-1.4.0/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.4.0/sck/__init__.py
--rw-rw-rw-   0        0        0     4134 2023-06-20 08:47:14.000000 emailalert-1.4.0/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 09:01:20.930158 emailalert-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 09:01:14.000000 emailalert-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:53:17.961551 emailalert-1.4.1/
+-rw-rw-rw-   0        0        0      178 2023-07-04 04:53:17.959388 emailalert-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 04:53:17.917005 emailalert-1.4.1/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 04:53:17.952032 emailalert-1.4.1/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.4.1/sck/__init__.py
+-rw-rw-rw-   0        0        0     4336 2023-07-04 04:51:57.000000 emailalert-1.4.1/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 04:53:17.963049 emailalert-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-07-04 04:52:51.000000 emailalert-1.4.1/setup.py
```

### Comparing `emailalert-1.4.0/README.md` & `emailalert-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.4.0/sck/emailalert.py` & `emailalert-1.4.1/sck/emailalert.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,60 +27,61 @@
     #msg = MIMEText(message)
     msg = MIMEMultipart()
     msg['Subject'] = subject
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ', '.join(recipients)
 
-    # Get all file paths in the folders
-    attachment_paths,attachment_filename = get_files_in_folders(folder_paths)
+    if folder_paths:
+        # Get all file paths in the folders
+        attachment_paths,attachment_filename = get_files_in_folders(folder_paths)
+        # Create the HTML table with CSS styles
+        table_html = '''
+        <style>
+            table {
+                border-collapse: collapse;
+                width: 70%;
+            }
+            th {
+                background-color: #f2f2f2;
+            }
+            th, td {
+                border: 1px solid black;
+                padding: 8px;
+                width: 300px;
+                text-align: left;
+            }        
+            table tr:hover {
+                background-color: #e6e6e6 !important;
+            }
+        </style>
+
+        <table>
+            <tr>
+                <th>データ仕様</th>
+                <th>エラー発生ファイル</th>
+            </tr>
+        '''
+        for index, (file_name, file_path) in enumerate(zip(attachment_filename, attachment_paths)):
+            spec = 'MCO'
+            if 'VHS' in file_path:
+                spec = 'LDD'
+            elif 'TT' in file_path:
+                spec = 'Tokyo'
+            row_color = "#d1ffd4" if index % 2 != 0 else "#ffffff"
+            table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';">'
+            table_html += f'<td style="width:30px;font-weight:bold">{spec}</td><td style="font-weight:bold">{file_name}</td></tr>'
+            
 
-    # Create the HTML table with CSS styles
-    table_html = '''
-    <style>
-        table {
-            border-collapse: collapse;
-            width: 70%;
-        }
-        th {
-            background-color: #f2f2f2;
-        }
-        th, td {
-            border: 1px solid black;
-            padding: 8px;
-            width: 300px;
-            text-align: left;
-        }        
-        table tr:hover {
-            background-color: #e6e6e6 !important;
-        }
-    </style>
-
-    <table>
-        <tr>
-            <th>データ仕様</th>
-            <th>エラー発生ファイル</th>
-        </tr>
-    '''
-    for index, (file_name, file_path) in enumerate(zip(attachment_filename, attachment_paths)):
-        spec = 'MCO'
-        if 'VHS' in file_path:
-            spec = 'LDD'
-        elif 'TT' in file_path:
-            spec = 'Tokyo'
-        row_color = "#d1ffd4" if index % 2 != 0 else "#ffffff"
-        table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';">'
-        table_html += f'<td style="width:30px;font-weight:bold">{spec}</td><td style="font-weight:bold">{file_name}</td></tr>'
-        
-
-    table_html += '</table>'
+        table_html += '</table>'
 
     # Create the email body as HTML
     message = message_header
-    message += f'<html><body>{table_html}</body></html>'
+    if folder_paths:
+        message += f'<html><body>{table_html}</body></html>'
     message += message_footer
 
     # Attach the email body
     msg.attach(MIMEText(message, 'html'))
 
 
     # Attach the files to the email
```

