# Comparing `tmp/nqtgbot-1.0.0a6.tar.gz` & `tmp/nqtgbot-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqtgbot-1.0.0a6.tar", max compression
+gzip compressed data, was "nqtgbot-1.0.0a7.tar", max compression
```

## Comparing `nqtgbot-1.0.0a6.tar` & `nqtgbot-1.0.0a7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      557 2023-03-26 09:02:50.446375 nqtgbot-1.0.0a6/LICENSE
--rw-r--r--   0        0        0      368 2023-05-20 13:15:49.684187 nqtgbot-1.0.0a6/README.md
--rw-r--r--   0        0        0        0 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a6/nqtgbot/__init__.py
--rw-r--r--   0        0        0     1174 2022-10-27 17:57:15.551527 nqtgbot-1.0.0a6/nqtgbot/message.py
--rw-r--r--   0        0        0     2253 2022-11-17 19:12:38.249444 nqtgbot-1.0.0a6/nqtgbot/provider.py
--rw-r--r--   0        0        0     1336 2023-01-22 20:06:46.830008 nqtgbot-1.0.0a6/nqtgbot/quotas.py
--rw-r--r--   0        0        0      264 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a6/nqtgbot/resources/config_schema.json
--rw-r--r--   0        0        0     1294 2023-05-30 12:02:06.035772 nqtgbot-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-07-04 12:38:04.332909 nqtgbot-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0      368 2023-07-04 12:38:04.332909 nqtgbot-1.0.0a7/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 12:38:04.336909 nqtgbot-1.0.0a7/nqtgbot/__init__.py
+-rw-r--r--   0        0        0     1174 2023-07-04 12:38:04.336909 nqtgbot-1.0.0a7/nqtgbot/message.py
+-rw-r--r--   0        0        0     2411 2023-07-04 12:38:04.336909 nqtgbot-1.0.0a7/nqtgbot/provider.py
+-rw-r--r--   0        0        0     1336 2023-07-04 12:38:04.336909 nqtgbot-1.0.0a7/nqtgbot/quotas.py
+-rw-r--r--   0        0        0      264 2023-07-04 12:38:04.336909 nqtgbot-1.0.0a7/nqtgbot/resources/config_schema.json
+-rw-r--r--   0        0        0     1549 2023-07-04 12:38:20.184906 nqtgbot-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a7/PKG-INFO
```

### Comparing `nqtgbot-1.0.0a6/LICENSE` & `nqtgbot-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a6/nqtgbot/message.py` & `nqtgbot-1.0.0a7/nqtgbot/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Inqana Ltd.
+Copyright (c) 2023 Inqana Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nqtgbot-1.0.0a6/nqtgbot/provider.py` & `nqtgbot-1.0.0a7/nqtgbot/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Inqana Ltd.
+Copyright (c) 2023 Inqana Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -22,16 +22,16 @@
 from importlib import resources
 from typing import TYPE_CHECKING, Dict, List, Type
 
 import pytz
 import telegram
 from nqsdk.abstract.channel import Channel
 from nqsdk.abstract.provider import Provider
-from nqsdk.exceptions import QuotaExceededException
-from telegram.error import RetryAfter
+from nqsdk.exceptions import QuotaExceededException, SentException
+from telegram.error import BadRequest, RetryAfter
 
 from .message import TelegramBotSentMeta
 from .quotas import PerSecondQuota, RetryAfterQuota
 
 if TYPE_CHECKING:  # pragma: no cover
     from nqsdk.abstract.message import Message
     from nqsdk.abstract.quotas import ProviderQuota
@@ -55,17 +55,21 @@
         return [PerSecondQuota()]
 
     def send(self, *, message: Message) -> TelegramBotSentMeta:
         bot = telegram.Bot(token=self.config["token"])
 
         try:
             bot_message = bot.send_message(
-                chat_id=message.get_recipient_id(), text=message.get_content()
+                chat_id=message.get_recipient_id(),
+                text=message.get_content(),
+                disable_web_page_preview=True,
             )
         except RetryAfter as e:
             raise QuotaExceededException(e, quota=RetryAfterQuota(delay=math.ceil(e.retry_after)))
+        except BadRequest as e:
+            raise SentException(e)
 
         return TelegramBotSentMeta(
             attempt_uid=message.attempt_uid,
             ext_id=bot_message.message_id,
             dt_sent=datetime.now(tz=pytz.timezone("UTC")),
         )
```

### Comparing `nqtgbot-1.0.0a6/nqtgbot/quotas.py` & `nqtgbot-1.0.0a7/nqtgbot/quotas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022 Inqana Ltd.
+Copyright (c) 2023 Inqana Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nqtgbot-1.0.0a6/PKG-INFO` & `nqtgbot-1.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nqtgbot
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: NQ Telegram Bot Provider
 Author: Inqana Ltd.
 Author-email: develop@inqana.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

