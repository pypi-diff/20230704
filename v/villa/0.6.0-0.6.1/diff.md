# Comparing `tmp/villa-0.6.0.tar.gz` & `tmp/villa-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.6.0.tar", max compression
+gzip compressed data, was "villa-0.6.1.tar", max compression
```

## Comparing `villa-0.6.0.tar` & `villa-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-07-02 12:00:40.831813 villa-0.6.0/LICENSE
--rw-r--r--   0        0        0     3428 2023-07-02 12:00:40.831813 villa-0.6.0/README.md
--rw-r--r--   0        0        0     1034 2023-07-02 12:00:40.831813 villa-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      285 2023-07-02 12:00:40.831813 villa-0.6.0/villa/__init__.py
--rw-r--r--   0        0        0    36474 2023-07-02 12:00:40.831813 villa-0.6.0/villa/bot.py
--rw-r--r--   0        0        0    10792 2023-07-02 12:00:40.831813 villa-0.6.0/villa/event.py
--rw-r--r--   0        0        0      728 2023-07-02 12:00:40.835813 villa-0.6.0/villa/exception.py
--rw-r--r--   0        0        0     3177 2023-07-02 12:00:40.835813 villa-0.6.0/villa/handle.py
--rw-r--r--   0        0        0     1524 2023-07-02 12:00:40.835813 villa-0.6.0/villa/log.py
--rw-r--r--   0        0        0    20754 2023-07-02 12:00:40.835813 villa-0.6.0/villa/message.py
--rw-r--r--   0        0        0     9310 2023-07-02 12:00:40.835813 villa-0.6.0/villa/models.py
--rw-r--r--   0        0        0      935 2023-07-02 12:00:40.835813 villa-0.6.0/villa/store.py
--rw-r--r--   0        0        0      240 2023-07-02 12:00:40.835813 villa-0.6.0/villa/typing.py
--rw-r--r--   0        0        0      995 2023-07-02 12:00:40.835813 villa-0.6.0/villa/utils.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 villa-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 10:47:34.997868 villa-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3428 2023-07-04 10:47:34.997868 villa-0.6.1/README.md
+-rw-r--r--   0        0        0     1034 2023-07-04 10:47:34.997868 villa-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-07-04 10:47:34.997868 villa-0.6.1/villa/__init__.py
+-rw-r--r--   0        0        0    36853 2023-07-04 10:47:34.997868 villa-0.6.1/villa/bot.py
+-rw-r--r--   0        0        0    11947 2023-07-04 10:47:34.997868 villa-0.6.1/villa/event.py
+-rw-r--r--   0        0        0      728 2023-07-04 10:47:34.997868 villa-0.6.1/villa/exception.py
+-rw-r--r--   0        0        0     3177 2023-07-04 10:47:34.997868 villa-0.6.1/villa/handle.py
+-rw-r--r--   0        0        0     1524 2023-07-04 10:47:35.001868 villa-0.6.1/villa/log.py
+-rw-r--r--   0        0        0    21270 2023-07-04 10:47:35.001868 villa-0.6.1/villa/message.py
+-rw-r--r--   0        0        0     9335 2023-07-04 10:47:35.001868 villa-0.6.1/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-04 10:47:35.001868 villa-0.6.1/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-04 10:47:35.001868 villa-0.6.1/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-07-04 10:47:35.001868 villa-0.6.1/villa/utils.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 villa-0.6.1/PKG-INFO
```

### Comparing `villa-0.6.0/LICENSE` & `villa-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/README.md` & `villa-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/pyproject.toml` & `villa-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.6.0"
+version = "0.6.1"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.6.0/villa/bot.py` & `villa-0.6.1/villa/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from urllib.parse import urlparse
 from collections import defaultdict
 from typing import Any, Set, Dict, List, Type, Union, Literal, Optional, DefaultDict
 
 import httpx
 import uvicorn
 from pydantic import parse_obj_as
+from httpx._types import TimeoutTypes
 from fastapi.responses import JSONResponse
 from fastapi import FastAPI, BackgroundTasks
 
 from .models import *
 from .message import Message
 from .utils import escape_tag
 from .handle import EventHandler
@@ -49,29 +50,31 @@
 
     def __init__(
         self,
         bot_id: str,
         bot_secret: str,
         callback_url: Optional[str] = None,
         wait_util_complete: bool = False,
+        api_timeout: TimeoutTypes = 10,
     ):
         """初始化一个 Bot 实例
 
         参数:
             bot_id: 机器人 ID
             bot_secret: 机器人密钥
             callback_url: 事件回调地址
         """
         self.bot_id = bot_id
         self.bot_secret = bot_secret
         if callback_url is not None:
             self.callback_endpoint = urlparse(callback_url).path
         self.wait_util_complete = wait_util_complete
         self._client = httpx.AsyncClient(
-            base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/"
+            base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/",
+            timeout=api_timeout,
         )
         store_bot(self)
 
     @property
     def nickname(self) -> str:
         """Bot 昵称"""
         if self._bot_info is None:
@@ -960,28 +963,34 @@
                                 bot_id=seg.bot_id, bot_name=seg.bot_name
                             ),
                         )
                     )
                     mentioned.user_id_list.append(seg.bot_id)
                 elif isinstance(seg, MentionUserSegment):
                     # 需要调用API获取被@的用户的昵称
-                    user = await self.get_member(villa_id=seg.villa_id, uid=seg.user_id)
-                    seg_text = f"@{user.basic.nickname} "
+                    if not seg.user_name and seg.villa_id:
+                        user = await self.get_member(
+                            villa_id=seg.villa_id, uid=seg.user_id
+                        )
+                        seg_text = f"@{user.basic.nickname} "
+                        seg.user_name = user.basic.nickname
+                    else:
+                        seg_text = f"@{seg.user_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=MentionedUser(
-                                user_id=str(user.basic.uid),
-                                user_name=user.basic.nickname,
+                                user_id=str(seg.user_id),
+                                user_name=seg.user_name,  # type: ignore
                             ),
                         )
                     )
-                    mentioned.user_id_list.append(str(user.basic.uid))
+                    mentioned.user_id_list.append(str(seg.user_id))
                 elif isinstance(seg, RoomLinkSegment):
                     # 需要调用API获取房间的名称
                     room = await self.get_room(
                         villa_id=seg.villa_id, room_id=seg.room_id
                     )
                     seg_text = f"#{room.room_name} "
                     length = cal_len(seg_text)
```

### Comparing `villa-0.6.0/villa/event.py` & `villa-0.6.1/villa/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict, Union, Literal, Optional
 
 from pydantic import BaseModel, root_validator
 
 from .store import get_bot
 from .utils import escape_tag
 from .message import Message, MessageSegment
-from .models import Robot, MessageContentInfo
+from .models import Robot, MessageContentInfoGet
 
 
 class EventType(IntEnum):
     """事件类型"""
 
     JoinVilla = 1
     SendMessage = 2
@@ -84,15 +84,15 @@
 
 class SendMessageEvent(Event):
     """用户@机器人发送消息事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage"""
 
     type: Literal[EventType.SendMessage] = EventType.SendMessage
-    content: MessageContentInfo
+    content: MessageContentInfoGet
     """消息内容"""
     from_user_id: int
     """发送者ID"""
     send_at: int
     """发送时间的时间戳"""
     room_id: int
     """房间ID"""
@@ -214,15 +214,18 @@
         """
         if (bot := get_bot(self.bot_id)) is None:
             raise ValueError(f"Bot {self.bot_id} not found. Cannot send message.")
         if isinstance(message, (str, MessageSegment)):
             message = Message(message)
         if mention_sender:
             message.insert(
-                0, MessageSegment.mention_user(self.villa_id, self.from_user_id)
+                0,
+                MessageSegment.mention_user(
+                    self.from_user_id, self.content.user.name, self.villa_id
+                ),
             )
         if quote_message:
             message.append(MessageSegment.quote(self.msg_uid, self.send_at))
         return await bot.send(self.villa_id, self.room_id, message)
 
 
 class CreateRobotEvent(Event):
@@ -279,14 +282,45 @@
     """是否是取消表情"""
 
     def get_event_description(self) -> str:
         return escape_tag(
             f"Emoticon(name={self.emoticon}, id={self.emoticon_id}) was {'removed from' if self.is_cancel else 'added to'} Message(id={self.msg_uid}) by User(id={self.uid}) in Room(id=Villa(id={self.room_id}) of Villa(id={self.villa_id})"
         )
 
+    async def send(
+        self,
+        message: Union[str, MessageSegment, Message],
+        mention_sender: bool = False,
+        quote_message: bool = False,
+    ) -> str:
+        """对事件进行快速发送消息
+
+        参数:
+            message: 消息内容
+            mention_sender: 是否@发送者. 默认为 False.
+            quote_message: 是否引用事件消息. 默认为 False.
+
+        异常:
+            ValueError: 找不到 Bot 实例
+
+        返回:
+            str: 消息 ID
+        """
+        if (bot := get_bot(self.bot_id)) is None:
+            raise ValueError(f"Bot {self.bot_id} not found. Cannot send message.")
+        if isinstance(message, (str, MessageSegment)):
+            message = Message(message)
+        if mention_sender:
+            message.insert(
+                0, MessageSegment.mention_user(self.uid, None, self.villa_id)
+            )
+        if quote_message:
+            message.append(MessageSegment.quote(self.msg_uid, self.send_at))
+        return await bot.send(self.villa_id, self.room_id, message)
+
 
 class AuditCallbackEvent(Event):
     """审核结果回调事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback"""
 
     type: Literal[EventType.AuditCallback] = EventType.AuditCallback
```

### Comparing `villa-0.6.0/villa/exception.py` & `villa-0.6.1/villa/exception.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/villa/handle.py` & `villa-0.6.1/villa/handle.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/villa/log.py` & `villa-0.6.1/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/villa/message.py` & `villa-0.6.1/villa/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from abc import ABC
 from typing_extensions import Self
 from typing import List, Tuple, Union, Literal, Iterable, Iterator, Optional, overload
 
-from pydantic import Field, BaseModel
 from pydantic.utils import get_args  # type: ignore
+from pydantic import Field, BaseModel, root_validator
 
 MessageType = Literal[
     "text",
     "mention_user",
     "mention_all",
     "mention_robot",
     "room_link",
@@ -30,16 +30,18 @@
         return Text(content=text)
 
     @staticmethod
     def mention_robot(bot_id: str, bot_name: str) -> "MentionRobot":
         return MentionRobot(bot_id=bot_id, bot_name=bot_name)
 
     @staticmethod
-    def mention_user(villa_id: int, user_id: int) -> "MentionUser":
-        return MentionUser(villa_id=villa_id, user_id=user_id)
+    def mention_user(
+        user_id: int, user_name: Optional[str] = None, villa_id: Optional[int] = None
+    ) -> "MentionUser":
+        return MentionUser(user_id=user_id, user_name=user_name, villa_id=villa_id)
 
     @staticmethod
     def mention_all(show_text: str = "全体成员") -> "MentionAll":
         return MentionAll(show_text=show_text)
 
     @staticmethod
     def room_link(villa_id: int, room_id: int) -> "RoomLink":
@@ -135,16 +137,23 @@
     bot_name: str
 
 
 class MentionUser(MessageSegment):
     """@用户消息段"""
 
     type: Literal["mention_user"] = Field(default="mention_user", repr=False)
-    villa_id: int
     user_id: int
+    user_name: Optional[str] = None
+    villa_id: Optional[int] = None
+
+    @root_validator
+    def _(cls, values):
+        if values.get("user_name") is None and values.get("villa_id") is None:
+            raise ValueError("user_name和villa_id必须至少有一个不为None")
+        return values
 
 
 class MentionAll(MessageSegment):
     """@全体成员消息段"""
 
     type: Literal["mention_all"] = Field(default="mention_all", repr=False)
     show_text: str = "全体成员"
@@ -260,25 +269,32 @@
             ```python
             message = Message().text("hello world")
             ```
         """
         self.__root__.append(Text(content=content))
         return self
 
-    def mention_user(self, villa_id: int, user_id: int) -> Self:
+    def mention_user(
+        self,
+        user_id: int,
+        user_name: Optional[str] = None,
+        villa_id: Optional[int] = None,
+    ) -> Self:
         """提及(@at)消息
 
         参数:
             villa_id: 要提及的用户所在的大别野ID
             user_id: 要提及的用户ID
 
         返回:
             Self: 消息对象
         """
-        self.__root__.append(MentionUser(villa_id=villa_id, user_id=user_id))
+        self.__root__.append(
+            MentionUser(user_id=user_id, user_name=user_name, villa_id=villa_id)
+        )
         return self
 
     def mention_all(self) -> Self:
         """提及(@at)全体成员消息
 
         返回:
             Self: 消息对象
```

### Comparing `villa-0.6.0/villa/models.py` & `villa-0.6.1/villa/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,18 +224,21 @@
     client: str
     env: str
     rong_sdk_version: str
 
 
 class MessageContentInfo(BaseModel):
     content: Union[TextMessageContent, ImageMessageContent, PostMessageContent]
-    mentioned_info: Optional[MentionedInfo] = Field(None, alias="mentionedInfo")
+    mentioned_info: Optional[MentionedInfo] = Field(default=None, alias="mentionedInfo")
     quote: Optional[QuoteInfo] = None
-    user: Optional[User] = None
-    trace: Optional[Trace] = None
+
+
+class MessageContentInfoGet(MessageContentInfo):
+    user: User
+    trace: Trace
 
 
 # 房间部分
 # see https://webstatic.mihoyo.com/vila/bot/doc/room_api/
 class Room(BaseModel):
     room_id: int
     room_name: str
```

### Comparing `villa-0.6.0/villa/store.py` & `villa-0.6.1/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/villa/utils.py` & `villa-0.6.1/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.0/PKG-INFO` & `villa-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.6.0
+Version: 0.6.1
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

