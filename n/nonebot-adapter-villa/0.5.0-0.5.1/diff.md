# Comparing `tmp/nonebot_adapter_villa-0.5.0.tar.gz` & `tmp/nonebot_adapter_villa-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.5.1.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.5.0.tar` & `nonebot_adapter_villa-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/LICENSE
--rw-r--r--   0        0        0     6796 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/README.md
--rw-r--r--   0        0        0      235 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10977 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9465 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    13057 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      649 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11641 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0    10115 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6796 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/README.md
+-rw-r--r--   0        0        0      235 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10977 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9511 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    13338 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      649 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11765 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0    10115 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-04 10:22:24.929162 nonebot_adapter_villa-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.1/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.5.0/LICENSE` & `nonebot_adapter_villa-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/README.md` & `nonebot_adapter_villa-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,19 @@
     rong_sdk_version: str
 
 
 class MessageContentInfo(BaseModel):
     content: Union[TextMessageContent, ImageMessageContent, PostMessageContent]
     mentioned_info: Optional[MentionedInfo] = Field(None, alias="mentionedInfo")
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
@@ -427,14 +430,15 @@
     "User",
     "Trace",
     "ImageSize",
     "Image",
     "PreviewLink",
     "Badge",
     "MessageContentInfo",
+    "MessageContentInfoGet",
     "Room",
     "RoomType",
     "RoomDefaultNotifyType",
     "SendMsgAuthRange",
     "GroupRoom",
     "ListRoomType",
     "CreateRoomType",
```

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from nonebot.typing import overrides
 from nonebot.message import handle_event
 from nonebot.internal.adapter.adapter import Adapter
 
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
-from .event import Event, SendMessageEvent
 from .message import Message, MessageSegment
+from .event import Event, SendMessageEvent, AddQuickEmoticonEvent
 from .api import (
     Link,
     Badge,
     Image,
     Robot,
     Command,
     ApiClient,
@@ -51,19 +51,20 @@
     """检查事件是否和机器人有关，如果有关则设置 to_me 为 True，并删除消息中的 at 信息。
 
     参数:
         bot: Bot对象
         event: 事件
 
     """
-    if (
-        event.content.mentioned_info
-        and bot.self_id in event.content.mentioned_info.user_id_list
-    ):
-        event.to_me = True
+    # 目前只能收到艾特机器人的消息，所以永远为 True
+    # if (
+    #     event.content.mentioned_info
+    #     and bot.self_id in event.content.mentioned_info.user_id_list
+    # ):
+    #     event.to_me = True
 
     def _is_at_me_seg(segment: MessageSegment) -> bool:
         return (
             segment.type == "mention_robot"
             and segment.data["mention_robot"].bot_id == bot.self_id
         )
 
@@ -193,24 +194,28 @@
 
         异常:
             RuntimeError: 事件不是消息事件时抛出
 
         返回:
             str: 消息ID
         """
-        if not isinstance(event, SendMessageEvent):
+        if not isinstance(event, (SendMessageEvent, AddQuickEmoticonEvent)):
             raise RuntimeError("Event cannot be replied to!")
         message = MessageSegment.text(message) if isinstance(message, str) else message
         message = message if isinstance(message, Message) else Message(message)
         if mention_sender:
             message.insert(
                 0,
                 MessageSegment.mention_user(
-                    user_id=event.from_user_id,
-                    user_name=event.content.user.name if event.content.user else None,
+                    user_id=event.from_user_id
+                    if isinstance(event, SendMessageEvent)
+                    else event.uid,
+                    user_name=event.content.user.name
+                    if isinstance(event, SendMessageEvent)
+                    else None,
                     villa_id=event.villa_id,
                 ),
             )
         if quote_message:
             message += MessageSegment.quote(event.msg_uid, event.send_at)
         content_info = await self.parse_message_content(message)
         if isinstance(content_info.content, TextMessageContent):
```

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from pydantic import root_validator
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 
 from nonebot.adapters import Event as BaseEvent
 
-from .api import Robot, MessageContentInfo
 from .message import Message, MessageSegment
+from .api import Robot, MessageContentInfoGet
 
 
 class EventType(IntEnum):
     """事件类型"""
 
     JoinVilla = 1
     SendMessage = 2
@@ -49,14 +49,19 @@
     """事件回调时间"""
 
     @property
     def bot_id(self) -> str:
         """机器人ID"""
         return self.robot.template.id
 
+    @property
+    def villa_id(self) -> int:
+        """事件所在大别野ID"""
+        return self.robot.villa_id
+
     @overrides(BaseEvent)
     def get_event_name(self) -> str:
         return self.type.name
 
     @overrides(BaseEvent)
     def get_event_description(self) -> str:
         return escape_tag(repr(self.dict()))
@@ -131,15 +136,15 @@
 
 class SendMessageEvent(MessageEvent):
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
@@ -148,15 +153,15 @@
     nickname: str
     """用户昵称"""
     msg_uid: str
     """消息ID"""
     bot_msg_id: Optional[str]
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
 
-    to_me: bool = False
+    to_me: bool = True
     """是否和Bot有关"""
     message: Message
     """事件消息"""
     raw_message: Message
     """事件原始消息"""
 
     @property
```

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.5.1/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.0/pyproject.toml` & `nonebot_adapter_villa-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.5.0"
+version = "0.5.1"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.5.0/PKG-INFO` & `nonebot_adapter_villa-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.5.0
+Version: 0.5.1
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.1 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

