# Comparing `tmp/promemoria-1.1.0.tar.gz` & `tmp/promemoria-1.2.0.tar.gz`

## Comparing `promemoria-1.1.0.tar` & `promemoria-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 promemoria-1.1.0/.gitattributes
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 promemoria-1.1.0/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/__main__.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/files.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/help.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/reminders.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 promemoria-1.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 promemoria-1.1.0/LICENSE
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 promemoria-1.1.0/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 promemoria-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 promemoria-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 promemoria-1.2.0/.gitattributes
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 promemoria-1.2.0/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 promemoria-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/__main__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/files.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/git.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/help.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/reminders.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 promemoria-1.2.0/src/promemoria/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 promemoria-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 promemoria-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 promemoria-1.2.0/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 promemoria-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 promemoria-1.2.0/PKG-INFO
```

### Comparing `promemoria-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `promemoria-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `promemoria-1.1.0/.github/workflows/python-publish.yml` & `promemoria-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `promemoria-1.1.0/src/promemoria/__init__.py` & `promemoria-1.2.0/src/promemoria/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import pickle
 import sys
 
 from colorama import Fore, Style, init
 
 from .help import help
 from .files import getReminders, saveReminders
 from .reminders import reminder
-from .utilities import parser
+from .utilities import parser, msg
+from .git import gitContents
 
 # Colorama's initialization.
 init()
 
 
 # Defines promemoria's main function.
 # This makes possible calling promemoria as a script.
@@ -45,81 +45,96 @@
         newReminder = reminder(sys.argv)
 
         if newReminder.confirmation:
             reminders.append(newReminder)
 
             print("\n" + str(newReminder))
 
+    # GitHub integration.
+    elif "gh" in instructions:
+        status, gits = gitContents(sys.argv)
+
+        if status:
+            titles = [rem.title for rem in reminders]
+
+            # Try to avoid duplicates.
+            gits = [git for git in gits if git.title not in titles]
+
+            reminders += gits
+
+            string: str = "Imported {} {}(s)."
+            string = string.format(len(gits), "{}")
+            string = string.format("issue" if "pulls" not in ddOpts else "pull")
+            msg(string)
+
+            for git in gits:
+                print("\n" + str(git))
+
+        else:
+            msg("An error occurred during import.", error=True)
+
     # Delete all reminders.
     elif "clear" in instructions:
         reminders = []
 
         print("Your reminders have been deleted.")
 
     # Delete a reminder.
     elif "delete" in instructions:
         if index < 0:
-            print(Fore.RED + "Syntax error." + Style.RESET_ALL)
+            msg("Missing reminder index.", error=True)
             return -1
 
-        message = "You have deleted a reminder."
-
-        print(message)
-        print("-" * len(message))
-
+        msg("You have deleted a reminder.")
         print("\n" + str(reminders.pop(index)))
 
     # Toggle a reminder.
     elif "toggle" in instructions:
         if index < 0:
-            print(Fore.RED + "Syntax error." + Style.RESET_ALL)
+            msg("Missing reminder index.", error=True)
             return -1
 
-        message = "You toggled a reminder."
-
-        print(message)
-        print("-" * len(message))
-
+        msg("You toggled a reminder.")
         reminders[index].toggle()
         print("\n" + str(reminders[index]))
 
     # No reminders.
     elif not len(reminders):
-        hint = Style.BRIGHT + "promemoria new -t 'TITLE' ..." + Style.RESET_ALL
+        hintNew = Style.BRIGHT + "promemoria new -t 'TITLE' ..." + Style.RESET_ALL
+        hintGit = Style.BRIGHT + "promemoria gh -r 'USER/REPO' ..." + Style.RESET_ALL
 
-        print("You have no reminders.")
-        print("Try creating one using " + hint)
+        print("You have no reminders.\n")
+        print("Try creating one using " + hintNew)
+        print("or import some using " + hintGit)
 
     # Shows reminders by default.
     else:
         # Get printable reminders.
         if "all" not in ddOpts:
             printable = [rem for rem in reminders if not rem.dismissed]
 
         else:
             printable = reminders.copy()
 
         # Print reminders, if any.
         if len(printable):
-            message: str = "You have {} reminder(s).".format(len(printable))
-
-            print(message)
-            print("-" * len(message))
+            msg("You have {} reminder(s).".format(len(printable)))
 
             # Prints the list of reminders.
             for rem in printable:
                 pIndex = reminders.index(rem)
                 print("\n" + rem.__str__(pIndex + 1))
 
         else:
-            print("Nothing to show.")
+            msg("Nothing to show.")
 
         if "all" in ddOpts:
             # Prints the number of completed reminders.
             completed: int = [rem.dismissed for rem in reminders].count(True)
-            message: str = "{} completed.".format(completed)
 
-            print("\n" + "-" * len(message))
-            print(message)
+            print()  # Needed space.
+            message = "{}/{} completed."
+            message = message.format(completed, len(reminders))
+            msg(message, reversed=True)
 
     # Saves reminders.
     saveReminders(reminders)
```

### Comparing `promemoria-1.1.0/src/promemoria/files.py` & `promemoria-1.2.0/src/promemoria/files.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Handles promemoria files.
 
+import pickle
 from os import makedirs
 from os.path import expanduser
 
 from .reminders import reminder
-import pickle
 
 
 def getReminders() -> list[reminder]:
     """
     Returns reminders from ~/.promemoria/reminders.pickle
     """
 
@@ -30,14 +30,17 @@
                 raise FileNotFoundError
 
     except FileNotFoundError:
         reminders: list[reminder] = []
 
         saveReminders(reminders)
 
+    except:
+        reminders = []
+
     # Runs a check on reminders.
     for rem in reminders:
         rem.check()
 
     return reminders
```

### Comparing `promemoria-1.1.0/src/promemoria/help.py` & `promemoria-1.2.0/src/promemoria/help.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def help() -> str:
     """
     Returns the help string.
     """
     spaces = " " * 4
-    introduction: str = "Available commands."
+    introduction: str = "Base commands."
     introduction += "\n" + "-" * len(introduction)
 
     # Empty command.
     cmd: str = Style.BRIGHT + "promemoria " + Style.RESET_ALL
     cmd += Style.DIM + "Shows the list of active reminders." + Style.RESET_ALL
 
     cmd += "\n" + spaces + Style.BRIGHT + "--all " + Style.RESET_ALL
@@ -51,10 +51,33 @@
     cmdToggle += "\n" + spaces + Fore.RED + Style.BRIGHT + "-i " + Style.RESET_ALL
     cmdToggle += Style.DIM + "index, integer." + Style.RESET_ALL
 
     # clear.
     cmdClear: str = Style.BRIGHT + "promemoria clear " + Style.RESET_ALL
     cmdClear += Style.DIM + "Deletes every reminder" + Style.RESET_ALL
 
+    # GitHub integration.
+    introductionGit: str = "GitHub integration."
+    introductionGit += "\n" + "-" * len(introductionGit)
+
+    # git.
+    cmdGit: str = Style.BRIGHT + "promemoria gh " + Style.RESET_ALL
+    cmdGit += (
+        Style.DIM + "Imports issues and pull requests from GitHub" + Style.RESET_ALL
+    )
+
+    cmdGit += "\n" + spaces + Fore.RED + Style.BRIGHT + "-r " + Style.RESET_ALL
+    cmdGit += Style.DIM + "public repo, string [user/repo]." + Style.RESET_ALL
+
+    cmdGit += "\n" + spaces + Style.BRIGHT + "-u " + Style.RESET_ALL
+    cmdGit += Style.DIM + "user, string." + Style.RESET_ALL
+
+    cmdGit += "\n" + spaces + Style.BRIGHT + "--pulls " + Style.RESET_ALL
+    cmdGit += Style.DIM + "Imports pull requests instead of issues." + Style.RESET_ALL
+
     # Full help.
     entries: list[str] = [introduction, cmd, cmdNew, cmdDelete, cmdToggle, cmdClear]
+
+    # GitHub integration.
+    entries += [introductionGit, cmdGit]
+
     return "\n\n".join(entries)
```

### Comparing `promemoria-1.1.0/src/promemoria/reminders.py` & `promemoria-1.2.0/src/promemoria/reminders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,105 @@
 from __future__ import annotations
 
 from datetime import datetime
+
 from colorama import Fore, Style
 
-from .utilities import parser, valiDate
+from .utilities import parser, valiDate, msg
 
 
 class reminder:
-    def __init__(self: reminder, prompt: list[str], old: reminder = None):
-        _, sdOpts, _ = parser(prompt)
+    def __init__(self: reminder, prompt: "list, dict", git: bool = False):
+        if git:
+            # Create a reminder from a git issue or pull request.
+            # prompt: dict[str, str]
+
+            self.title = prompt["title"]
+            self.description = prompt["description"]
+
+            self.priority = 2  # Default priority.
+            self.date = ""
+            self.time = ""
 
-        try:
-            # Checks title.
-            assert "t" in sdOpts
+            # Flags.
+            self.expired: bool = False
+            self.dismissed: bool = False
 
-            # Title.
-            self.title: str = sdOpts["t"]
+        else:
+            try:
+                # Create a reminder 'from scratch'.
+                # prompt: list[str]
 
-            # Checks priority.
-            if "p" in sdOpts:
-                assert isinstance(sdOpts["p"], int)
-                assert 1 <= sdOpts["p"] <= 3
+                _, sdOpts, _ = parser(prompt)
 
-                # Priority.
-                self.priority: int = sdOpts["p"]
+                # Checks title.
+                assert "t" in sdOpts
 
-            else:
-                self.priority = 0
+                # Title.
+                self.title: str = sdOpts["t"]
 
-            # Checks description.
-            if "de" in sdOpts:
-                assert isinstance(sdOpts["de"], str)
+                # Checks priority.
+                if "p" in sdOpts:
+                    assert isinstance(sdOpts["p"], int)
+                    assert 1 <= sdOpts["p"] <= 3
 
-                # Description.
-                self.description: str = sdOpts["de"]
+                    # Priority.
+                    self.priority: int = sdOpts["p"]
 
-            else:
-                self.description = ""
+                else:
+                    self.priority = 0
 
-            # Checks date.
-            if "da" in sdOpts:
-                assert isinstance(sdOpts["da"], str)
-                assert valiDate(sdOpts["da"])
+                # Checks description.
+                if "de" in sdOpts:
+                    assert isinstance(sdOpts["de"], str)
 
-                # Date.
-                self.date: str = sdOpts["da"]
+                    # Description.
+                    self.description: str = sdOpts["de"]
 
-            else:
-                self.date = ""
+                else:
+                    self.description = ""
 
-            # Checks time.
-            if "ti" in sdOpts:
-                assert isinstance(sdOpts["ti"], str)
-                assert valiDate(sdOpts["ti"], "%H:%M")
+                # Checks date.
+                if "da" in sdOpts:
+                    assert isinstance(sdOpts["da"], str)
+                    assert valiDate(sdOpts["da"])
 
-                if not self.date:
-                    self.date = datetime.now().strftime("%Y-%m-%d")
+                    # Date.
+                    self.date: str = sdOpts["da"]
 
-                # Time.
-                self.time: str = sdOpts["ti"]
+                else:
+                    self.date = ""
 
-            else:
-                self.time = ""
+                # Checks time.
+                if "ti" in sdOpts:
+                    assert isinstance(sdOpts["ti"], str)
+                    assert valiDate(sdOpts["ti"], "%H:%M")
 
-            # Flags.
-            self.expired = False
-            self.dismissed: bool = False
-            self.confirmation: bool = True
+                    if not self.date:
+                        self.date = datetime.now().strftime("%Y-%m-%d")
+
+                    # Time.
+                    self.time: str = sdOpts["ti"]
+
+                else:
+                    self.time = ""
 
-            # Post-creation check.
-            self.check()
+                # Flags.
+                self.expired: bool = False
+                self.dismissed: bool = False
+                self.confirmation: bool = True
 
-            message = "Reminder created succesfully!"
+                # Post-creation check.
+                self.check()
 
-        except AssertionError:
-            message = "Reminder creation failed!"
-            self.confirmation: bool = False
+                msg("Reminder created succesfully.")
 
-        print(message)
-        print("-" * len(message))
+            except AssertionError:
+                msg("Reminder creation failed.", error=True)
+                self.confirmation: bool = False
 
     def __str__(self: reminder, index: int = -1) -> str:
         # Mark.
         mark = "\u25cf " if self.dismissed else "\u25ef "
 
         if index != -1:
             mark += "[{}] ".format(index)
```

### Comparing `promemoria-1.1.0/src/promemoria/utilities.py` & `promemoria-1.2.0/src/promemoria/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,35 @@
 from datetime import datetime
 
+from colorama import Fore
+
+
+def msg(string: str, error: bool = False, reversed: bool = False) -> None:
+    """
+    Pretty messages.
+    """
+
+    if error:
+        output = Fore.RED + string + Fore.RESET
+
+    else:
+        output = string
+
+    if not reversed:
+        print(output + "\n" + "-" * len(string))
+
+    else:
+        print("-" * len(string) + "\n" + output)
+
 
 def valiDate(date: str, string: str = "%Y-%m-%d") -> bool:
+    """
+    Validate a date.
+    """
+
     try:
         if date != datetime.strptime(date, string).strftime(string):
             raise ValueError
 
         return True
 
     except ValueError:
```

### Comparing `promemoria-1.1.0/LICENSE` & `promemoria-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promemoria-1.1.0/pyproject.toml` & `promemoria-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "promemoria"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["colorama", "setuptools"]
+dependencies = ["colorama", "setuptools", "requests"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
```

### Comparing `promemoria-1.1.0/PKG-INFO` & `promemoria-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: promemoria
-Version: 1.1.0
-Project-URL: Homepage, https://github.com/diantonioandrea/promemoria
-Project-URL: Bug Tracker, https://github.com/diantonioandrea/promemoria/issues
-Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: colorama
-Requires-Dist: setuptools
-Description-Content-Type: text/markdown
-
 ![GitHub](https://img.shields.io/github/license/diantonioandrea/promemoria)
 
 ![PyPI](https://img.shields.io/pypi/v/promemoria?label=promemoria%20on%20pypi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/promemoria)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/promemoria)
 
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/diantonioandrea/promemoria)
@@ -29,14 +14,19 @@
 
 # [promemoria]
 
 Intuitive Python based tool to create reminders in the shell.
 
 **promemoria** is a Python based tool to help you stay organized and on top of your tasks! Quickly *create reminders in the shell* with the ability to *set a title, description, priority and date* to make sure you never forget anything.
 
+## Main features
+
+- Create and manage reminders directly from the shell.
+- Import the latest *Issues* and *Pull Requests* as reminders from a public GitHub repository. ![New feature](https://img.shields.io/badge/new-green)
+
 ## Installation
 
 **promemoria** can be installed from [PyPI](https://pypi.org) by:
 
 ```
 python3 -m pip install --upgrade promemoria
 ```
@@ -54,15 +44,15 @@
 
 ```
 [promemoria]
 
 Available commands.
 -------------------
 
-promemoria Shows the list of active reminders
+promemoria Shows the list of active reminders.
     --all Shows every reminder.
 
 promemoria new Creates a new reminder
     -t title, string.
     -de description, string. 
     -da date, string, ISO 8601 compliant.
     -ti time, string.
@@ -71,14 +61,22 @@
 promemoria delete Deletes the specified reminder
     -i index, integer.
 
 promemoria toggle Toggles the specified reminder
     -i index, integer.
 
 promemoria clear Deletes every reminder
+
+GitHub integration.
+-------------------
+
+promemoria gh Imports issues and pull requests from GitHub
+    -r public repo, string [user/repo].
+    -u user, string.
+    --pulls Imports pull requests instead of issues.
 ```
 
 ## Examples
 
 ### Quickly check your reminders
 
 ```
@@ -112,23 +110,43 @@
 -----------------------------
 
 ◯ Christmas !!!
   It's Christmas!
   2023-12-25
 ```
 
+### Import from a GitHub repository
+
+```
+promemoria gh -r "python/cpython" -u "sobolevn"
+```
+
+which results[^4] in:
+
+[^4]: An example from the official [Python](https://github.com/python/cpython) repository.
+
+```
+[promemoria]
+
+Imported 1 issue(s).
+____________________
+
+◯ New warning: "'_Py_IsInterpreterFinalizing' undefined; assuming extern returning in" !!
+  https://api.github.com/repos/python/cpython/issues/106406
+```
+
 ### Toggling a reminder
 
 ```
 promemoria toggle -i 1
 ````
 
-which results[^2][^4] in:
+which results[^2][^5] in:
 
-[^4]: The mark changes and the title gets dimmed.
+[^5]: The mark changes and the title gets dimmed.
 
 ```
 [promemoria]
 
 You toggled a reminder.
 -----------------------
```

