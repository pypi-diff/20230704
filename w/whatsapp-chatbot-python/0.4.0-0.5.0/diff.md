# Comparing `tmp/whatsapp-chatbot-python-0.4.0.tar.gz` & `tmp/whatsapp-chatbot-python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.4.0.tar", last modified: Wed Jun 21 17:38:48 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.5.0.tar", last modified: Tue Jul  4 19:54:37 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.4.0.tar` & `whatsapp-chatbot-python-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.245029 whatsapp-chatbot-python-0.4.0/
--rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.4.0/LICENSE
--rw-rw-rw-   0        0        0    10908 2023-06-21 17:38:48.244027 whatsapp-chatbot-python-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     9883 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 17:38:48.245029 whatsapp-chatbot-python-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.230992 whatsapp-chatbot-python-0.4.0/tests/
--rw-rw-rw-   0        0        0     1416 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.234001 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3783 2023-06-21 17:36:14.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.243024 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1881 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-06-15 14:08:46.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-06-21 17:38:48.240017 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0    10908 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-21 17:38:48.000000 whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.481515 whatsapp-chatbot-python-0.5.0/
+-rw-rw-rw-   0        0        0    18829 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    15378 2023-07-04 19:54:37.480823 whatsapp-chatbot-python-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14404 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:54:37.481515 whatsapp-chatbot-python-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.468943 whatsapp-chatbot-python-0.5.0/tests/
+-rw-rw-rw-   0        0        0     1416 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.0/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.471803 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      270 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-06-30 12:14:11.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     4091 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.479820 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     4513 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     2022 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-28 14:02:48.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/router.py
+-rw-rw-rw-   0        0        0     2643 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/state.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.475811 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    15378 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.4.0/LICENSE` & `whatsapp-chatbot-python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.4.0/PKG-INFO` & `whatsapp-chatbot-python-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
@@ -221,19 +220,129 @@
         }
     ])
 
 
 bot.run_forever()
 ```
 
+### How to manage user state
+
+As an example, a bot was created for user registration.
+
+To manage user states, we need to create states. Import the `BaseStates` class and inherit from it. To manage the state
+we need to use `notification.state_manager`. The manager has methods for getting, setting, updating and deleting state.
+You also have the option to save the user's data in his state.
+
+| Manager's method    | Description                                                                           |
+|---------------------|---------------------------------------------------------------------------------------|
+| `get_state`         | Returns a state class with state name and user data                                   |
+| `set_state`         | Sets the state for the user. If the state exists then the data will be deleted        |
+| `update_state`      | If a state exists, it changes it. If not, it creates a new state                      |
+| `delete_state`      | Deletes the user's state. Remember to get the data before deleting                    |
+| `get_state_data`    | If the state exists, it returns the data in the form of a dictionary (dict)           |
+| `set_state_data`    | If the state exists, it changes the data to the new data                              |
+| `update_state_data` | If the state exists, it updates the data. If no data exists, the data will be created |
+| `delete_state_data` | If the state exists, it deletes the data                                              |
+
+The first argument is the sender ID. It can be found by calling `notification.sender`.
+
+Link to example: [states.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/states.py).
+
+```python
+from whatsapp_chatbot_python import BaseStates, GreenAPIBot, Notification
+
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
+
+
+class States(BaseStates):
+    USERNAME = "username"
+    PASSWORD = "password"
+
+
+@bot.router.message(state=None)
+def message_handler(notification: Notification) -> None:
+    sender = notification.sender
+
+    notification.state_manager.set_state(sender, States.USERNAME.value)
+
+    notification.answer("Hello. Tell me your username.")
+
+
+@bot.router.message(command="cancel")
+def cancel_handler(notification: Notification) -> None:
+    sender = notification.sender
+
+    state = notification.state_manager.get_state(sender)
+    if not state:
+        return None
+    else:
+        notification.state_manager.delete_state(sender)
+
+        notification.answer("Bye")
+
+
+@bot.router.message(state=States.USERNAME.value)
+def username_handler(notification: Notification) -> None:
+    sender = notification.sender
+    username = notification.message_text
+
+    if not 5 <= len(username) <= 20:
+        notification.answer("Invalid username.")
+    else:
+        notification.state_manager.update_state(sender, States.PASSWORD.value)
+        notification.state_manager.set_state_data(
+            sender, {"username": username}
+        )
+
+        notification.answer("Tell me your password.")
+
+
+@bot.router.message(state=States.PASSWORD.value)
+def password_handler(notification: Notification) -> None:
+    sender = notification.sender
+    password = notification.message_text
+
+    if not 8 <= len(password) <= 20:
+        notification.answer("Invalid password.")
+    else:
+        data = notification.state_manager.get_state_data(sender)
+
+        username = data["username"]
+
+        notification.answer(
+            (
+                "Successful account creation.\n\n"
+                f"Your username: {username}.\n"
+                f"Your password: {password}."
+            )
+        )
+
+        notification.state_manager.delete_state(sender)
+
+
+bot.run_forever()
+```
+
 ### Example of a bot
 
-Link to example: [full_example.py](
-https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full_example.py
-).
+As an example, a bot was created to support the GREEN API. Command list:
+
+- start (the bot says hello and sends a list of commands)
+- 1 or Report a problem (the bot will send a link to GitHub to create the bug)
+- 2 or Show office address (the bot will send the office address as a map)
+- 3 or Show available rates (the bot will send a picture of the rates)
+- 4 or Call a support operator (the bot will send a text message)
+
+To send a text message, you have to use the `notification.answer` method.
+To send a location, you have to use the `sending.sendLocation` method from `notification.api`.
+To send a message with a file, you have to use the `notification.answer_with_file` method.
+
+Link to example: [full.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full.py).
 
 ```python
 from whatsapp_chatbot_python import GreenAPIBot, Notification
 
 bot = GreenAPIBot(
     "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
 )
@@ -261,15 +370,15 @@
     notification.answer(
         "https://github.com/green-api/issues/issues/new", link_preview=False
     )
 
 
 @bot.router.message(text_message=["2", "Show office address"])
 def show_office_address_handler(notification: Notification) -> None:
-    chat = notification.get_chat()
+    chat = notification.chat
 
     notification.api.sending.sendLocation(
         chatId=chat, latitude=55.7522200, longitude=37.6155600
     )
 
 
 @bot.router.message(text_message=["3", "Show available rates"])
```

### Comparing `whatsapp-chatbot-python-0.4.0/README.md` & `whatsapp-chatbot-python-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -198,19 +198,129 @@
         }
     ])
 
 
 bot.run_forever()
 ```
 
+### How to manage user state
+
+As an example, a bot was created for user registration.
+
+To manage user states, we need to create states. Import the `BaseStates` class and inherit from it. To manage the state
+we need to use `notification.state_manager`. The manager has methods for getting, setting, updating and deleting state.
+You also have the option to save the user's data in his state.
+
+| Manager's method    | Description                                                                           |
+|---------------------|---------------------------------------------------------------------------------------|
+| `get_state`         | Returns a state class with state name and user data                                   |
+| `set_state`         | Sets the state for the user. If the state exists then the data will be deleted        |
+| `update_state`      | If a state exists, it changes it. If not, it creates a new state                      |
+| `delete_state`      | Deletes the user's state. Remember to get the data before deleting                    |
+| `get_state_data`    | If the state exists, it returns the data in the form of a dictionary (dict)           |
+| `set_state_data`    | If the state exists, it changes the data to the new data                              |
+| `update_state_data` | If the state exists, it updates the data. If no data exists, the data will be created |
+| `delete_state_data` | If the state exists, it deletes the data                                              |
+
+The first argument is the sender ID. It can be found by calling `notification.sender`.
+
+Link to example: [states.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/states.py).
+
+```python
+from whatsapp_chatbot_python import BaseStates, GreenAPIBot, Notification
+
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
+
+
+class States(BaseStates):
+    USERNAME = "username"
+    PASSWORD = "password"
+
+
+@bot.router.message(state=None)
+def message_handler(notification: Notification) -> None:
+    sender = notification.sender
+
+    notification.state_manager.set_state(sender, States.USERNAME.value)
+
+    notification.answer("Hello. Tell me your username.")
+
+
+@bot.router.message(command="cancel")
+def cancel_handler(notification: Notification) -> None:
+    sender = notification.sender
+
+    state = notification.state_manager.get_state(sender)
+    if not state:
+        return None
+    else:
+        notification.state_manager.delete_state(sender)
+
+        notification.answer("Bye")
+
+
+@bot.router.message(state=States.USERNAME.value)
+def username_handler(notification: Notification) -> None:
+    sender = notification.sender
+    username = notification.message_text
+
+    if not 5 <= len(username) <= 20:
+        notification.answer("Invalid username.")
+    else:
+        notification.state_manager.update_state(sender, States.PASSWORD.value)
+        notification.state_manager.set_state_data(
+            sender, {"username": username}
+        )
+
+        notification.answer("Tell me your password.")
+
+
+@bot.router.message(state=States.PASSWORD.value)
+def password_handler(notification: Notification) -> None:
+    sender = notification.sender
+    password = notification.message_text
+
+    if not 8 <= len(password) <= 20:
+        notification.answer("Invalid password.")
+    else:
+        data = notification.state_manager.get_state_data(sender)
+
+        username = data["username"]
+
+        notification.answer(
+            (
+                "Successful account creation.\n\n"
+                f"Your username: {username}.\n"
+                f"Your password: {password}."
+            )
+        )
+
+        notification.state_manager.delete_state(sender)
+
+
+bot.run_forever()
+```
+
 ### Example of a bot
 
-Link to example: [full_example.py](
-https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full_example.py
-).
+As an example, a bot was created to support the GREEN API. Command list:
+
+- start (the bot says hello and sends a list of commands)
+- 1 or Report a problem (the bot will send a link to GitHub to create the bug)
+- 2 or Show office address (the bot will send the office address as a map)
+- 3 or Show available rates (the bot will send a picture of the rates)
+- 4 or Call a support operator (the bot will send a text message)
+
+To send a text message, you have to use the `notification.answer` method.
+To send a location, you have to use the `sending.sendLocation` method from `notification.api`.
+To send a message with a file, you have to use the `notification.answer_with_file` method.
+
+Link to example: [full.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full.py).
 
 ```python
 from whatsapp_chatbot_python import GreenAPIBot, Notification
 
 bot = GreenAPIBot(
     "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
 )
@@ -238,15 +348,15 @@
     notification.answer(
         "https://github.com/green-api/issues/issues/new", link_preview=False
     )
 
 
 @bot.router.message(text_message=["2", "Show office address"])
 def show_office_address_handler(notification: Notification) -> None:
-    chat = notification.get_chat()
+    chat = notification.chat
 
     notification.api.sending.sendLocation(
         chatId=chat, latitude=55.7522200, longitude=37.6155600
     )
 
 
 @bot.router.message(text_message=["3", "Show available rates"])
```

### Comparing `whatsapp-chatbot-python-0.4.0/setup.py` & `whatsapp-chatbot-python-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.4.0",
+    version="0.5.0",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -18,21 +18,20 @@
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["whatsapp-api-client-python==0.0.37"],
-    python_requires=">=3.7"
+    install_requires=["whatsapp-api-client-python==0.0.38"],
+    python_requires=">=3.8"
 )
```

### Comparing `whatsapp-chatbot-python-0.4.0/tests/test_manager.py` & `whatsapp-chatbot-python-0.5.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,87 @@
 from abc import ABC, abstractmethod
 from re import fullmatch
-from typing import Dict, List, Optional, Type, Union
+from typing import Dict, List, Optional, TYPE_CHECKING, Type, Union
+
+if TYPE_CHECKING:
+    from .manager.handler import Notification
 
 
 class AbstractFilter(ABC):
     @abstractmethod
     def __init__(self, *args, **kwargs):
         pass
 
     @abstractmethod
-    def check_event(self, event: dict) -> bool:
+    def check_event(self, notification: "Notification") -> bool:
         pass
 
 
 class ChatIDFilter(AbstractFilter):
     def __init__(self, chat: Union[str, List[str]]):
         self.chat = chat
         if isinstance(chat, str):
             self.chat = [chat]
 
-    def check_event(self, event: dict) -> bool:
-        chat = event["senderData"]["chatId"]
+    def check_event(self, notification: "Notification") -> bool:
+        chat = notification.chat
 
         if chat in self.chat:
             return True
         return False
 
 
 class SenderFilter(AbstractFilter):
     def __init__(self, sender: Union[str, List[str]]):
         self.sender = sender
         if isinstance(sender, str):
             self.sender = [sender]
 
-    def check_event(self, event: dict) -> bool:
-        sender = event["senderData"]["sender"]
+    def check_event(self, notification: "Notification") -> bool:
+        sender = notification.sender
 
         if sender in self.sender:
             return True
         return False
 
 
 class TypeMessageFilter(AbstractFilter):
     def __init__(self, type_message: Union[str, List[str]]):
         self.type_message = type_message
         if isinstance(type_message, str):
             self.type_message = [type_message]
 
-    def check_event(self, event: dict) -> bool:
-        type_message = event["messageData"]["typeMessage"]
+    def check_event(self, notification: "Notification") -> bool:
+        type_message = notification.event["messageData"]["typeMessage"]
 
         if type_message in self.type_message:
             return True
         return False
 
 
 class TextMessageFilter(AbstractFilter):
     def __init__(self, text_message: Union[str, List[str]]):
         self.text_message = text_message
         if isinstance(text_message, str):
             self.text_message = [text_message]
 
-    def check_event(self, event: dict) -> bool:
-        text_message = self.get_text_message(event)
+    def check_event(self, notification: "Notification") -> bool:
+        text_message = notification.message_text
 
         if text_message in self.text_message:
             return True
         return False
 
-    @staticmethod
-    def get_text_message(event: dict) -> Optional[str]:
-        message_data = event["messageData"]
-
-        type_message = message_data["typeMessage"]
-        if type_message == "textMessage":
-            return message_data["textMessageData"]["textMessage"]
-        elif type_message == "extendedTextMessage":
-            return message_data["extendedTextMessageData"]["text"]
-
 
 class RegExpFilter(AbstractFilter):
     def __init__(self, pattern: str):
         self.pattern = pattern
 
-    def check_event(self, event: dict) -> bool:
-        text_message = TextMessageFilter.get_text_message(event)
+    def check_event(self, notification: "Notification") -> bool:
+        text_message = notification.message_text
 
         if fullmatch(self.pattern, text_message):
             return True
         return False
 
 
 class CommandFilter(AbstractFilter):
@@ -96,36 +89,56 @@
         if isinstance(command, str):
             self.command = command
             self.prefixes = prefixes
         elif isinstance(command, tuple):
             if len(command) == 2:
                 self.command, self.prefixes = command
 
-    def check_event(self, event: dict) -> bool:
-        text_message = TextMessageFilter.get_text_message(event)
+    def check_event(self, notification: "Notification") -> bool:
+        text_message = notification.message_text
 
         for prefix in self.prefixes:
             if text_message.split()[0] != f"{prefix}{self.command}":
                 continue
             return True
         return False
 
 
+class StateFilter(AbstractFilter):
+    def __init__(self, state_name: Optional[str]):
+        self.state_name = state_name
+
+    def check_event(self, notification: "Notification") -> bool:
+        sender = notification.sender
+
+        state = notification.state_manager.get_state(sender)
+        if not state:
+            if self.state_name is None:
+                return True
+            return False
+
+        if state.name == self.state_name:
+            return True
+        return False
+
+
 filters: Dict[str, Type[AbstractFilter]] = {
     "from_chat": ChatIDFilter,
     "from_sender": SenderFilter,
     "type_message": TypeMessageFilter,
     "text_message": TextMessageFilter,
     "regexp": RegExpFilter,
-    "command": CommandFilter
+    "command": CommandFilter,
+    "state": StateFilter
 }
 
 __all__ = [
     "AbstractFilter",
     "ChatIDFilter",
     "SenderFilter",
     "TypeMessageFilter",
     "TextMessageFilter",
     "RegExpFilter",
     "CommandFilter",
+    "StateFilter",
     "filters"
 ]
```

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,66 @@
 
 from whatsapp_api_client_python.response import Response
 
 from ..filters import filters as event_filters
 
 if TYPE_CHECKING:
     from .observer import Observer
+    from .state import AbstractStateManager
     from ..bot import GreenAPI
 
 
 class Notification:
     event: dict
 
     api: "GreenAPI"
+    state_manager: "AbstractStateManager"
 
-    def __init__(self, event: dict, api: "GreenAPI"):
+    def __init__(
+            self,
+            event: dict,
+            api: "GreenAPI",
+            state_manager: "AbstractStateManager"
+    ):
         self.event = event
 
         self.api = api
+        self.state_manager = state_manager
+
+    @property
+    def chat(self) -> Optional[str]:
+        return self.get_chat()
+
+    @property
+    def sender(self) -> Optional[str]:
+        return self.get_sender()
+
+    @property
+    def message_text(self) -> Optional[str]:
+        return self.get_message_text()
 
     def get_chat(self) -> Optional[str]:
         type_webhook = self.event["typeWebhook"]
         if type_webhook != "outgoingMessageStatus":
             return self.event["senderData"]["chatId"]
 
+    def get_sender(self) -> Optional[str]:
+        type_webhook = self.event["typeWebhook"]
+        if type_webhook != "outgoingMessageStatus":
+            return self.event["senderData"]["sender"]
+
+    def get_message_text(self) -> Optional[str]:
+        message_data = self.event["messageData"]
+
+        type_message = message_data["typeMessage"]
+        if type_message == "textMessage":
+            return message_data["textMessageData"]["textMessage"]
+        elif type_message == "extendedTextMessage":
+            return message_data["extendedTextMessageData"]["text"]
+
     def answer(
             self,
             message: str,
             quoted_message_id: Optional[str] = None,
             archive_chat: Optional[bool] = None,
             link_preview: Optional[bool] = None
     ) -> Optional[Response]:
@@ -70,41 +104,45 @@
 
 
 class AbstractHandler(ABC):
     handler: HandlerType
     filters: Dict[str, Any]
 
     @abstractmethod
-    def check_event(self, event: dict) -> bool:
+    def check_event(self, notification: Notification) -> bool:
         pass
 
     @abstractmethod
     def execute_handler(self, observer: "Observer") -> bool:
         pass
 
 
 class Handler(AbstractHandler):
     def __init__(self, handler: HandlerType, **filters: Any):
         self.handler = handler
         self.filters = filters
 
-    def check_event(self, event: dict) -> bool:
+    def check_event(self, notification: Notification) -> bool:
         for filter_name in self.filters.keys():
             filter_ = event_filters.get(filter_name)
             if filter_:
                 filter_data = self.filters[filter_name]
-                response = filter_(filter_data).check_event(event)
+                response = filter_(filter_data).check_event(notification)
                 if not response:
                     return False
 
         return True
 
     def execute_handler(self, observer: "Observer") -> bool:
-        response = self.check_event(observer.event)
+        notification = Notification(
+            observer.event, observer.router.api, observer.state_manager
+        )
+
+        response = self.check_event(notification)
         if response:
-            self.handler(Notification(observer.event, observer.router.api))
+            self.handler(notification)
 
             return True
         return False
 
 
 __all__ = ["Notification", "HandlerType", "AbstractHandler", "Handler"]
```

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List, TYPE_CHECKING
 
 from .handler import HandlerType, AbstractHandler, Handler
+from .state import AbstractStateManager, StateManager
 
 if TYPE_CHECKING:
     from .router import Router
 
 
 class AbstractObserver(ABC):
     event: dict
     handlers: List[AbstractHandler]
+    state_manager: AbstractStateManager
 
     def update_event(self, event: dict) -> None:
         self.event = event
 
         self.propagate_event()
 
     @abstractmethod
@@ -27,14 +29,15 @@
 
 class Observer(AbstractObserver):
     def __init__(self, router: "Router"):
         self.router = router
 
         self.event = {}
         self.handlers = []
+        self.state_manager = StateManager()
 
     def add_handler(self, handler: HandlerType, **filters: Any) -> None:
         self.handlers.append(Handler(handler, **filters))
 
     def propagate_event(self) -> None:
         for handler in self.handlers:
             response = handler.execute_handler(self)
```

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
@@ -221,19 +220,129 @@
         }
     ])
 
 
 bot.run_forever()
 ```
 
+### How to manage user state
+
+As an example, a bot was created for user registration.
+
+To manage user states, we need to create states. Import the `BaseStates` class and inherit from it. To manage the state
+we need to use `notification.state_manager`. The manager has methods for getting, setting, updating and deleting state.
+You also have the option to save the user's data in his state.
+
+| Manager's method    | Description                                                                           |
+|---------------------|---------------------------------------------------------------------------------------|
+| `get_state`         | Returns a state class with state name and user data                                   |
+| `set_state`         | Sets the state for the user. If the state exists then the data will be deleted        |
+| `update_state`      | If a state exists, it changes it. If not, it creates a new state                      |
+| `delete_state`      | Deletes the user's state. Remember to get the data before deleting                    |
+| `get_state_data`    | If the state exists, it returns the data in the form of a dictionary (dict)           |
+| `set_state_data`    | If the state exists, it changes the data to the new data                              |
+| `update_state_data` | If the state exists, it updates the data. If no data exists, the data will be created |
+| `delete_state_data` | If the state exists, it deletes the data                                              |
+
+The first argument is the sender ID. It can be found by calling `notification.sender`.
+
+Link to example: [states.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/states.py).
+
+```python
+from whatsapp_chatbot_python import BaseStates, GreenAPIBot, Notification
+
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
+
+
+class States(BaseStates):
+    USERNAME = "username"
+    PASSWORD = "password"
+
+
+@bot.router.message(state=None)
+def message_handler(notification: Notification) -> None:
+    sender = notification.sender
+
+    notification.state_manager.set_state(sender, States.USERNAME.value)
+
+    notification.answer("Hello. Tell me your username.")
+
+
+@bot.router.message(command="cancel")
+def cancel_handler(notification: Notification) -> None:
+    sender = notification.sender
+
+    state = notification.state_manager.get_state(sender)
+    if not state:
+        return None
+    else:
+        notification.state_manager.delete_state(sender)
+
+        notification.answer("Bye")
+
+
+@bot.router.message(state=States.USERNAME.value)
+def username_handler(notification: Notification) -> None:
+    sender = notification.sender
+    username = notification.message_text
+
+    if not 5 <= len(username) <= 20:
+        notification.answer("Invalid username.")
+    else:
+        notification.state_manager.update_state(sender, States.PASSWORD.value)
+        notification.state_manager.set_state_data(
+            sender, {"username": username}
+        )
+
+        notification.answer("Tell me your password.")
+
+
+@bot.router.message(state=States.PASSWORD.value)
+def password_handler(notification: Notification) -> None:
+    sender = notification.sender
+    password = notification.message_text
+
+    if not 8 <= len(password) <= 20:
+        notification.answer("Invalid password.")
+    else:
+        data = notification.state_manager.get_state_data(sender)
+
+        username = data["username"]
+
+        notification.answer(
+            (
+                "Successful account creation.\n\n"
+                f"Your username: {username}.\n"
+                f"Your password: {password}."
+            )
+        )
+
+        notification.state_manager.delete_state(sender)
+
+
+bot.run_forever()
+```
+
 ### Example of a bot
 
-Link to example: [full_example.py](
-https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full_example.py
-).
+As an example, a bot was created to support the GREEN API. Command list:
+
+- start (the bot says hello and sends a list of commands)
+- 1 or Report a problem (the bot will send a link to GitHub to create the bug)
+- 2 or Show office address (the bot will send the office address as a map)
+- 3 or Show available rates (the bot will send a picture of the rates)
+- 4 or Call a support operator (the bot will send a text message)
+
+To send a text message, you have to use the `notification.answer` method.
+To send a location, you have to use the `sending.sendLocation` method from `notification.api`.
+To send a message with a file, you have to use the `notification.answer_with_file` method.
+
+Link to example: [full.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full.py).
 
 ```python
 from whatsapp_chatbot_python import GreenAPIBot, Notification
 
 bot = GreenAPIBot(
     "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
 )
@@ -261,15 +370,15 @@
     notification.answer(
         "https://github.com/green-api/issues/issues/new", link_preview=False
     )
 
 
 @bot.router.message(text_message=["2", "Show office address"])
 def show_office_address_handler(notification: Notification) -> None:
-    chat = notification.get_chat()
+    chat = notification.chat
 
     notification.api.sending.sendLocation(
         chatId=chat, latitude=55.7522200, longitude=37.6155600
     )
 
 
 @bot.router.message(text_message=["3", "Show available rates"])
```

### Comparing `whatsapp-chatbot-python-0.4.0/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 whatsapp_chatbot_python.egg-info/SOURCES.txt
 whatsapp_chatbot_python.egg-info/dependency_links.txt
 whatsapp_chatbot_python.egg-info/requires.txt
 whatsapp_chatbot_python.egg-info/top_level.txt
 whatsapp_chatbot_python/manager/__init__.py
 whatsapp_chatbot_python/manager/handler.py
 whatsapp_chatbot_python/manager/observer.py
-whatsapp_chatbot_python/manager/router.py
+whatsapp_chatbot_python/manager/router.py
+whatsapp_chatbot_python/manager/state.py
```

