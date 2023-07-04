# Comparing `tmp/gmail_draft_creator-1.0.1.tar.gz` & `tmp/gmail_draft_creator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_draft_creator-1.0.1.tar", max compression
+gzip compressed data, was "gmail_draft_creator-1.1.0.tar", max compression
```

## Comparing `gmail_draft_creator-1.0.1.tar` & `gmail_draft_creator-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-07-04 16:57:12.486189 gmail_draft_creator-1.0.1/LICENSE
--rw-r--r--   0        0        0     3457 2023-07-04 16:57:12.486189 gmail_draft_creator-1.0.1/gmail_draft_creator/__init__.py
--rw-r--r--   0        0        0      620 2023-07-04 16:57:33.906153 gmail_draft_creator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1745 2023-07-04 16:57:12.486189 gmail_draft_creator-1.0.1/readme.md
--rw-r--r--   0        0        0     2523 1970-01-01 00:00:00.000000 gmail_draft_creator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 17:40:55.128486 gmail_draft_creator-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3468 2023-07-04 17:40:55.128486 gmail_draft_creator-1.1.0/gmail_draft_creator/__init__.py
+-rw-r--r--   0        0        0     1016 2023-07-04 17:41:15.756877 gmail_draft_creator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1745 2023-07-04 17:40:55.128486 gmail_draft_creator-1.1.0/readme.md
+-rw-r--r--   0        0        0     2523 1970-01-01 00:00:00.000000 gmail_draft_creator-1.1.0/PKG-INFO
```

### Comparing `gmail_draft_creator-1.0.1/LICENSE` & `gmail_draft_creator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_draft_creator-1.0.1/gmail_draft_creator/__init__.py` & `gmail_draft_creator-1.1.0/gmail_draft_creator/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,95 @@
-from string import Template
-from google.oauth2.credentials import Credentials
-from google_auth_oauthlib.flow import InstalledAppFlow
-from google.auth.transport.requests import Request
-from googleapiclient.discovery import build
-from email.mime.text import MIMEText
-import os
 import base64
-import pickle
 import csv
 import logging
-import markdown
-from email.mime.multipart import MIMEMultipart
+import os
+import pickle
 import re
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from string import Template
+
+import markdown
+from google.auth.transport.requests import Request
+from google.oauth2.credentials import Credentials
+from google_auth_oauthlib.flow import InstalledAppFlow
+from googleapiclient.discovery import build
 
 SCOPES = [
-    'https://www.googleapis.com/auth/gmail.compose',
-    'https://www.googleapis.com/auth/gmail.readonly',
-    'https://www.googleapis.com/auth/calendar.readonly',
-    'https://www.googleapis.com/auth/calendar.events'
+    "https://www.googleapis.com/auth/gmail.compose",
+    "https://www.googleapis.com/auth/gmail.readonly",
+    "https://www.googleapis.com/auth/calendar.readonly",
+    "https://www.googleapis.com/auth/calendar.events",
 ]
 
 import click
 
+
 @click.command()
-@click.option('--csv', 'csv_file_path', type=click.Path(exists=True), help='Path to the CSV file.', required=True)
-@click.option('--template', 'template_file_path', type=click.Path(exists=True), help='Path to the template file.', required=True)
-@click.option('--subject', 'subject', type=str, help='Subject for the email drafts.', required=True)
-@click.option('--dry-run', is_flag=True, default=False, help='Run script without creating drafts.')
+@click.option("--csv", "csv_file_path", type=click.Path(exists=True), help="Path to the CSV file.", required=True)
+@click.option(
+    "--template", "template_file_path", type=click.Path(exists=True), help="Path to the template file.", required=True
+)
+@click.option("--subject", "subject", type=str, help="Subject for the email drafts.", required=True)
+@click.option("--dry-run", is_flag=True, default=False, help="Run script without creating drafts.")
 def send_drafts_from_csv_cli(csv_file_path, template_file_path, subject, dry_run):
     send_drafts_from_csv(csv_file_path, template_file_path, subject, dry_run)
 
+
 def send_drafts_from_csv(csv_file_path, template_file_path, subject, dry_run=False):
-    with open(template_file_path, 'r') as template_file:
+    with open(template_file_path, "r") as template_file:
         template_string = markdown.markdown(template_file.read())
 
-    with open(csv_file_path, 'r') as file:
+    with open(csv_file_path, "r") as file:
         reader = csv.DictReader(file)
         for row in reader:
-            email = row.pop('email', None) or row.pop('Email', None)
+            email = row.pop("email", None) or row.pop("Email", None)
             template_params = {k.lower(): v for k, v in row.items()}
 
             if email is not None:
                 create_draft(email, subject, template_string, template_params, dry_run)
 
+
 def create_draft(email, subject, template_string, template_params, dry_run=False):
     creds = None
-    if os.path.exists('token.pickle'):
-        with open('token.pickle', 'rb') as token:
+    if os.path.exists("token.pickle"):
+        with open("token.pickle", "rb") as token:
             creds = pickle.load(token)
 
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
-            flow = InstalledAppFlow.from_client_secrets_file('credentials.json', SCOPES)
+            flow = InstalledAppFlow.from_client_secrets_file("credentials.json", SCOPES)
             creds = flow.run_local_server(port=0)
-        with open('token.pickle', 'wb') as token:
+        with open("token.pickle", "wb") as token:
             pickle.dump(creds, token)
 
-    service = build('gmail', 'v1', credentials=creds)
+    service = build("gmail", "v1", credentials=creds)
 
     message_template = Template(template_string)
     message_text = message_template.substitute(template_params)
 
     # remove <p> and </p> tags if they are on the first line
     # this causes weird formatting in gmail
-    first_line, remaining_text = message_text.split('\n', 1)
+    first_line, remaining_text = message_text.split("\n", 1)
     first_line = re.sub(r"^<p>(.*)</p>$", r"\1", first_line)
-    message_text = first_line + '\n' + remaining_text
+    message_text = first_line + "\n" + remaining_text
 
-    message = MIMEMultipart('alternative')
-    message['to'] = email
-    message['subject'] = subject
-    message.attach(MIMEText(message_text, 'html'))
+    message = MIMEMultipart("alternative")
+    message["to"] = email
+    message["subject"] = subject
+    message.attach(MIMEText(message_text, "html"))
 
     raw_message = base64.urlsafe_b64encode(message.as_bytes())
     raw_message = raw_message.decode()
-    body = {'message': {'raw': raw_message}}
+    body = {"message": {"raw": raw_message}}
 
     if not dry_run:
-        draft = service.users().drafts().create(userId='me', body=body).execute()
+        draft = service.users().drafts().create(userId="me", body=body).execute()
 
-    logging.info(f'draft created for email: {email}')
+    logging.info(f"draft created for email: {email}")
 
 
 def main():
     logging.basicConfig(level=logging.INFO)
     send_drafts_from_csv_cli()
```

### Comparing `gmail_draft_creator-1.0.1/pyproject.toml` & `gmail_draft_creator-1.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 [tool.poetry]
 name = "gmail_draft_creator"
-version = "1.0.1"
+version = "1.1.0"
 description = "Create draft messages in Gmail"
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 google-api-python-client = "^2.21.0"
 python-decouple = "^3.5"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.4.6"
 click = "^8.1.3"
 markdown = "^3.4.3"
 
-[tool.poetry.group.dev.dependencies]
-ipdb = "^0.13.13"
-
 [tool.poetry.scripts]
 gmail-draft-creator = "gmail_draft_creator:main"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
+target-version = ['py311']
+exclude = '''
+/(
+  .venv
+  | node_modules
+  | migrations
+)/
+'''
+
+# when changing this config, you need to restart your vscode isort server
+[tool.isort]
+profile = "black"
+multi_line_output = 3
+sections = "SETUP,FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,PRISMA,LOCALFOLDER"
+known_setup = "python.setup"
+known_prisma = "prisma"
```

### Comparing `gmail_draft_creator-1.0.1/readme.md` & `gmail_draft_creator-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `gmail_draft_creator-1.0.1/PKG-INFO` & `gmail_draft_creator-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail-draft-creator
-Version: 1.0.1
+Version: 1.1.0
 Summary: Create draft messages in Gmail
 License: MIT
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

