# Comparing `tmp/telstra_messaging-3.0.3.tar.gz` & `tmp/telstra_messaging-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telstra_messaging-3.0.3.tar", max compression
+gzip compressed data, was "telstra_messaging-3.1.0.tar", max compression
```

## Comparing `telstra_messaging-3.0.3.tar` & `telstra_messaging-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11378 2023-04-19 02:06:20.277949 telstra_messaging-3.0.3/LICENSE
--rw-r--r--   0        0        0    25497 2023-04-19 02:06:20.277949 telstra_messaging-3.0.3/README.md
--rw-r--r--   0        0        0      888 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/pyproject.toml
--rw-r--r--   0        0        0       32 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/__init__.py
--rw-r--r--   0        0        0       40 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/__init__.py
--rw-r--r--   0        0        0      762 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/exceptions.py
--rw-r--r--   0        0        0     4682 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/free_trial_numbers.py
--rw-r--r--   0        0        0     1063 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/health_check.py
--rw-r--r--   0        0        0    31574 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/message.py
--rw-r--r--   0        0        0     2847 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/oauth.py
--rw-r--r--   0        0        0     8901 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/reports.py
--rw-r--r--   0        0        0      903 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/types.py
--rw-r--r--   0        0        0       38 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/__init__.py
--rw-r--r--   0        0        0      743 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/callback_url.py
--rw-r--r--   0        0        0     6152 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/config.py
--rw-r--r--   0        0        0     1315 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/error_response.py
--rw-r--r--   0        0        0     2043 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/free_trial_number.py
--rw-r--r--   0        0        0      933 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/message_id.py
--rw-r--r--   0        0        0      409 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/querystring.py
--rw-r--r--   0        0        0     2961 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/reports_dates.py
--rw-r--r--   0        0        0      929 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/schedule_send.py
--rw-r--r--   0        0        0     1662 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/virtual_number.py
--rw-r--r--   0        0        0    16507 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/virtual_number.py
--rw-r--r--   0        0        0    25995 1970-01-01 00:00:00.000000 telstra_messaging-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11378 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/LICENSE
+-rw-r--r--   0        0        0    27526 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/README.md
+-rw-r--r--   0        0        0      888 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/__init__.py
+-rw-r--r--   0        0        0      762 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/exceptions.py
+-rw-r--r--   0        0        0     4678 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/free_trial_numbers.py
+-rw-r--r--   0        0        0     1056 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/health_check.py
+-rw-r--r--   0        0        0    31562 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/message.py
+-rw-r--r--   0        0        0     2814 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/oauth.py
+-rw-r--r--   0        0        0     8768 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/reports.py
+-rw-r--r--   0        0        0      903 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/types.py
+-rw-r--r--   0        0        0       38 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/callback_url.py
+-rw-r--r--   0        0        0     6152 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/config.py
+-rw-r--r--   0        0        0     1315 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/error_response.py
+-rw-r--r--   0        0        0     2043 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/free_trial_number.py
+-rw-r--r--   0        0        0      933 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/message_id.py
+-rw-r--r--   0        0        0      409 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/querystring.py
+-rw-r--r--   0        0        0     2961 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/reports_dates.py
+-rw-r--r--   0        0        0      929 2023-07-04 01:58:39.694228 telstra_messaging-3.1.0/telstra/messaging/utils/schedule_send.py
+-rw-r--r--   0        0        0     1662 2023-07-04 01:58:39.694228 telstra_messaging-3.1.0/telstra/messaging/utils/virtual_number.py
+-rw-r--r--   0        0        0    20267 2023-07-04 01:58:39.694228 telstra_messaging-3.1.0/telstra/messaging/virtual_number.py
+-rw-r--r--   0        0        0    28024 1970-01-01 00:00:00.000000 telstra_messaging-3.1.0/PKG-INFO
```

### Comparing `telstra_messaging-3.0.3/LICENSE` & `telstra_messaging-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/README.md` & `telstra_messaging-3.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+Metadata-Version: 2.1
+Name: telstra-messaging
+Version: 3.1.0
+Summary: SDK for the Telstra Messaging API V3 - Beta
+License: Apache-2.0
+Author: David Andersson
+Author-email: david-andersson@users.noreply.github.com 
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # Telstra Messaging
 
 The SDK for the Telstra Messaging API enables you to send and receive messages
 to Australian mobile numbers. For more information about this product, please
 see here:
-<https://dev.telstra.com/content/messaging-api-v3>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverview?version=3.x>.
 
 > :warning: **This SDK is experimental, everything is subject to change**
 
 ## Installing
 
 ```bash
 pip install telstra.messaging
@@ -84,29 +98,29 @@
 ## Free Trial
 
 Telstra offers a free trial for the messaging API to help you evaluate whether
 it meets your needs. There are some restrictions that apply compared to the
 full API, including a maximum number of messages that can be sent and requiring the
 registration of a limited number of destinations before a message can be sent
 to that destination. For more information, please see here:
-<https://dev.telstra.com/content/messaging-api#tag/Free-Trial>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FreeTrial>.
 
 ### Registering Free Trial Numbers
 
 > :information_source: **Only required for the free trial**
 
 Register numbers for the free trial. For more information, please see
 here:
-<https://dev.telstra.com/content/messaging-api-v3#tag/free-trial-numbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#RegisteraFreeTrialNumber>.
 
 The function `telstra.messaging.free_trial_numbers.create` can be used to register
 destinations. It takes the following arguments:
 
-- `phone_numbers`: A list of destinations, expected to be phone numbers of the
-  form `+614XXXXXXXX` or `04XXXXXXXX`.
+- `phone_numbers`: A list of destinations, expected to be phone numbers
+  of the form `04XXXXXXXX`.
 
 Raises `telstra.messaging.exceptions.FreeTrialNumbersError` if anything goes wrong.
 
 It returns the list of phone numbers that have been registered.
 
 For example:
 
@@ -120,15 +134,15 @@
 
 ### Fetch all Free Trial Numbers
 
 > :information_source: **Only required for the free trial**
 
 Fetch the Free Trial Number(s) currently assigned to your account. For more information,
 please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getTrialNumbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchyourFreeTrialNumbers>.
 
 The function `telstra.messaging.free_trial_numbers.get_all`
 can be used to retrieve registered destinations.
 It takes no arguments.
 
 Raises `telstra.messaging.exceptions.FreeTrialNumbersError` if anything goes wrong.
 
@@ -146,23 +160,23 @@
 ```
 
 ## Virtual Number
 
 Gives you a dedicated mobile number tied to an application which
 enables you to receive replies from your customers. For more information,
 please see here:
-<https://dev.telstra.com/content/messaging-api-v3#tag/virtual-numbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#VirtualNumbers>.
 
 ### Assign Virtual Number
 
 When a recipient receives your message, you can choose whether they'll see a privateNumber,
 Virtual Number or senderName (paid plans only) in the from field.
 If you want to use a Virtual Number, use this function to assign one.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/assignNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#AssignaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.create` can be used to create a
 numbers. It takes the following arguments:
 
 - `reply_callback_url` (optional): The URL that replies to the
   Virtual Number will be posted to.
 - `tags` (optional): Create your own tags and use them to fetch,
@@ -189,15 +203,15 @@
 print(assigned_numbers)
 ```
 
 ### Fetch a Virtual Number
 
 Fetch the tags, replyCallbackUrl and lastUse date for a Virtual Number.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getVirtualNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.get` can be used to get the current
 number. It takes the following arguments:
 
 - `virtual_number`: The Virtual Number assigned to your account.
 
 Raises `telstra.messaging.exceptions.VirtualNumbersError` if anything goes wrong.
@@ -221,15 +235,15 @@
 print(retrieved_number)
 ```
 
 ### Fetch all Virtual Numbers
 
 Fetch all Virtual Numbers currently assigned to your account.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getNumbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchallVirtualNumbers>.
 
 The function `telstra.messaging.virtual_number.get_all` can be used to
 get the all virtual numbers associated to your account.
 It takes the following arguments:
 
 - `limit`: Tell us how many results you want us to return, up to a maximum of 50.
 - `offset`: Use the offset to navigate between the response results.
@@ -254,15 +268,15 @@
 print(retrieved_virtual_numbers)
 ```
 
 ### Update a Virtual Number
 
 Update a virtual number attributes. For more information,
 please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/updateNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#UpdateaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.update` can be used to update a
 virtual number. It takes the following arguments:
 
 - `virtual_number`: The Virtual Number assigned to your account.
 - `reply_callback_url` (optional): The URL that replies to the
   Virtual Number will be posted to.
@@ -292,15 +306,15 @@
   )
 print(updated_virtual_number)
 ```
 
 ### Delete Virtual Number
 
 Delete the a virtual number. For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/deleteNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#DeleteaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.delete` can be used
 to delete the current number. It takes the following arguments:
 
 - `virtual_number`: The Virtual Number assigned to your account.
 
 Raises `telstra.messaging.exceptions.VirtualNumbersError` if anything goes wrong.
@@ -310,24 +324,59 @@
 ```python
 # Delete a virtual number
 from telstra.messaging import virtual_number
 
 virtual_number.delete(virtual_number="0400000001")
 ```
 
+### Fetch all Recipient Optouts list
+
+Fetch any mobile number(s) that have opted out of receiving messages
+from a Virtual Number assigned to your account.
+For more information, please see here:
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchallrecipientoptoutslist>.
+
+The function `telstra.messaging.virtual_number.get_optouts` can be used to
+get the list of mobile numbers that have opted out of receiving messages
+from a virtual number associated to your account.
+It takes the following arguments:
+
+- `virtual_number`: The Virtual Number assigned to your account.
+- `limit`: Tell us how many results you want us to return, up to a maximum of 50.
+- `offset`: Use the offset to navigate between the response results.
+  An offset of 0 will display the first page of results, and so on.
+
+Raises `telstra.messaging.exceptions.VirtualNumbersError` if anything goes wrong.
+
+It returns an object with the following
+properties:
+
+- `recipient_optouts`: A list of recipient optouts.
+- `paging`: Paging information.
+
+For example:
+
+```python
+# Get all virtual numbers
+from telstra.messaging import virtual_number
+
+retrieved_optout_numbers = virtual_number.get_optouts(virtual_number="0400000001")
+print(retrieved_optout_numbers)
+```
+
 ## Message
 
 Send and receive messages. For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#tag/messages>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Messages>.
 
 ### Send Message
 
 Send a message to a mobile number, or to multiple mobile numbers.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/sendMessages>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#SendanSMSorMMS>.
 
 The function `telstra.messaging.message.send` can be used to send a message.
 It takes the following arguments:
 
 - `to`: The destination address, expected to be a phone number of the form
   `+614XXXXXXXX` or `04XXXXXXXX`.
 - `from_`: This will be either "privateNumber", one of your Virtual Numbers
@@ -337,15 +386,16 @@
 - `multimedia` (Either one of messageContent or multimedia is required).
   MMS multimedia content.
 - `retry_timeout` (optional): How many minutes you asked the server to
   keep trying to send the message.
 - `schedule_send` (optional): The time (in Central Standard Time)
   the message is scheduled to send.
 - `delivery_notification` (optional): If set to true, you will receive
-  a notification to the statusCallbackUrl when your SMS is delivered (paid feature).
+  a notification to the statusCallbackUrl when your SMS or MMS
+  is delivered (paid feature).
 - `status_callback_url` (optional): The URL the API will call when the
   status of the message changes.
 - `tags` (optional): Any customisable tags assigned to the message.
 
 The dataclass `telstra.messaging.message.Multimedia`
 can be used to build an mms payload.
 It takes the following arguments:
@@ -367,15 +417,15 @@
 - `message_content`: The content of the message.
 - `multimedia`: The multimedia content of the message (MMS only).
 - `retry_timeout`: How many minutes you asked the server to keep
   trying to send the message.
 - `schedule_send`: The time (in Central Standard Time) a message
   is scheduled to send.
 - `delivery_notification`: If set to true, you will receive a notification to the
-  statusCallbackUrl when your SMS is delivered (paid feature).
+  statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url`: The URL the API will call when the status of
   the message changes.
 - `tags`: Any customisable tags assigned to the message.
 
 For example:
 
 ```python
@@ -402,29 +452,27 @@
 )
 ```
 
 ### Get a Message
 
 Use the messageId to fetch a message that's been sent from/to
 your account within the last 30 days.
-Note that in the current release, inbound MMS or messages sent in
-reply to an MMS will not be retrieved..
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getMessageById>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchamessage>.
 
 The function `telstra.messaging.message.get` can be used to retrieve
 the a message. It takes the following arguments:
 
 - `message_id`:Unique identifier for the message.
 
 Raises `telstra.messaging.exceptions.MessageError` if anything goes wrong.
 
 It returns an object with the following properties:
 
-- `messageId`: Use this UUID with our other endpoints to fetch,
+- `message_id`: Use this UUID with our other endpoints to fetch,
   update or delete the message.
 - `status`: The status will be either queued, sent, delivered or expired.
 - `create_timestamp`: The time you submitted the message to
   the queue for sending.
 - `sent_timestamp`: The time the message was sent from the server.
 - `received_timestamp`: The time the message was received by the
   recipient's device.
@@ -435,15 +483,15 @@
 - `multimedia`: The multimedia content of the message (MMS only).
 - `direction`: Direction of the message (outgoing or incoming).
 - `retry_timeout`: How many minutes you asked the server to keep
   trying to send the message.
 - `schedule_send`: The time (in Central Standard Time) the message is
   scheduled to send.
 - `delivery_notification`: If set to true, you will receive a notification
-  to the statusCallbackUrl when your SMS is delivered (paid feature).
+  to the statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url`: The URL the API will call when the status of
   the message changes.
 - `queue_priority`: The priority assigned to the message.
 - `tags`: Any customisable tags assigned to the message.
 
 For example:
 
@@ -459,18 +507,16 @@
 message = message.get(message_id = sent_message.message_id)
 print(message)
 ```
 
 ### Get all Messages
 
 Fetch messages that have been sent from/to your account in the last 30 days.
-Note that in the current release, inbound MMS or messages sent
-in reply to an MMS will not be retrieved.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getMessages>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchallsent/receivedmessages>.
 
 The function `telstra.messaging.message.get_all` can be used to fetch
 all messages. It takes the
 following arguments:
 
 - `limit`: Tell us how many results you want us to return, up to a maximum of 50.
 - `offset`: Use the offset to navigate between the response results.
@@ -496,15 +542,15 @@
 ```
 
 ### Update a Message
 
 Update a message that's scheduled for sending, you can change any of
 the below parameters, as long as the message hasn't been sent yet.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/updateMessageById>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Updateamessage>.
 
 The function `telstra.messaging.message.update` can be used to update a message.
 It takes the following arguments:
 
 - `to`: The destination address, expected to be a phone number of the form
   `+614XXXXXXXX` or `04XXXXXXXX`.
 - `from_`: This will be either "privateNumber", one of your
@@ -513,15 +559,15 @@
   Either one of messageContent or multimedia is required.
 - `multimedia` MMS multimedia content.
 - `retry_timeout` (optional): How many minutes you asked the server to
   keep trying to send the message.
 - `schedule_send` (optional): The time (in Central Standard Time) the
   message is scheduled to send.
 - `delivery_notification` (optional): If set to true, you will receive a
-  notification to the statusCallbackUrl when your SMS is delivered (paid feature).
+  notification to the statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url` (optional): The URL the API will call when
   the status of the message changes.
 - `tags` (optional): Any customisable tags assigned to the message.
 
 Raises `telstra.messaging.exceptions.MessageError` if anything goes wrong.
 
 The dataclass `telstra.messaging.message.Multimedia` can be used to build
@@ -544,15 +590,15 @@
 - `message_content`: The content of the message.
 - `multimedia`: The multimedia content of the message (MMS only).
 - `retry_timeout`: How many minutes you asked the server to keep trying
   to send the message.
 - `schedule_send`: The time (in Central Standard Time) the message
   is scheduled to send.
 - `delivery_notification`: If set to true, you will receive a notification to the
-  statusCallbackUrl when your SMS is delivered (paid feature).
+  statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url`: The URL the API will call when the
   status of the message changes.
 - `tags`: Any customisable tags assigned to the message.
 
 For example:
 
 ```python
@@ -567,15 +613,15 @@
   )
 ```
 
 ### Update Message Tags
 
 Update message tags, you can update them even after your message has been delivered.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/updateMessageTags>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Updatemessagetags>.
 
 The function `telstra.messaging.message.update_tags` can be used to
 update message tags. It takes the following arguments:
 
 - `message_id`:Unique identifier for the message.
 - `tags` (optional): Any customisable tags assigned to the message.
 
@@ -592,15 +638,15 @@
 message.update_tags(message_id="8540d774-4863-4d2b-b788-4ecb19412e85", tags=["Python","V3"])
 ```
 
 ### Delete a Message
 
 Delete a scheduled message, but hasn't yet sent.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/deleteMessageById>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Deleteamessage>.
 
 The function `telstra.messaging.message.delete` can be used to delete a message.
 It takes the following arguments:
 
 - `message_id`: Unique identifier for the message.
 
 Raises `telstra.messaging.exceptions.MessageError` if anything goes wrong.
@@ -622,15 +668,15 @@
 <https://dev.telstra.com/content/messaging-api-v3#tag/reports>.
 
 ### Request a Report
 
 Request a CSV report of messages (both incoming and outgoing)
 that have been sent to/from your account within the last three months.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/messagesReport>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Submitarequestforamessagesreport>.
 
 The function `telstra.messaging.reports.create` can be used to create a report.
 It takes the following arguments:
 
 - `start_date`: Set the time period you want to generate a
   report for by typing the start date (inclusive) here. Note that we only
   retain data for three months, so please ensure your startDate is not more
@@ -668,15 +714,15 @@
     )
 ```
 
 ### Fetch a specific report
 
 Use the report_id to fetch a download link for a report generated.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getReport>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchaReport>.
 
 The function `telstra.messaging.reports.get` can be used to retrieve
 the a report download link. It takes the following arguments:
 
 - `report_id`:Unique identifier for the report.
 
 Raises `telstra.messaging.exceptions.ReportsError` if anything goes wrong.
@@ -689,25 +735,25 @@
 
 For example:
 
 ```python
 # Get a report download link
 from telstra.messaging import reports
 
-report_reponse = reports.get(report_id = '6940c774-4335-4d2b-b758-4ecb19412e85')
+report_response = reports.get(report_id = '6940c774-4335-4d2b-b758-4ecb19412e85')
 print(report_response)
 ```
 
 ### Fetch all reports
 
 Fetch details of all reports recently generated for your account.
 Use it to check the status of a report, plus fetch the report ID,
 status, report type and expiry date.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getReports>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchallreports>.
 
 The function `telstra.messaging.reports.get_all` can be used to fetch
 all reports. It doesn't take any arguments.
 
 Raises `telstra.messaging.exceptions.ReportsError` if anything goes wrong.
 
 It returns a list of objects with the following properties:
@@ -730,15 +776,15 @@
 
 ## Health Check
 
 ### Get operational status of the messaging service
 
 Check the operational status of the messaging service.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/healthCheck>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#HealthCheck>.
 
 The function `telstra.messaging.health_check.get` can be used to get the status.
 It takes no arguments.
 
 Raises `telstra.messaging.exceptions.HealthCheckError` if anything goes wrong.
 
 It returns nothing.
@@ -758,7 +804,8 @@
 ## Exceptions
 
 All exceptions that can be raised derive from `MessagingBaseException`:
 
 ```python
 from telstra.messaging.exceptions import MessagingBaseException
 ```
+
```

### Comparing `telstra_messaging-3.0.3/pyproject.toml` & `telstra_messaging-3.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telstra.messaging"
-version = "3.0.3"
+version = "3.1.0"
 readme = "README.md"
 description = "SDK for the Telstra Messaging API V3 - Beta"
 license = "Apache-2.0"
 authors = ["David Andersson <david-andersson@users.noreply.github.com >"]
 include = ["telstra"]
 exclude = ["tests"]
 packages = [
```

### Comparing `telstra_messaging-3.0.3/telstra/messaging/exceptions.py` & `telstra_messaging-3.1.0/telstra/messaging/exceptions.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/free_trial_numbers.py` & `telstra_messaging-3.1.0/telstra/messaging/free_trial_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         raise exceptions.FreeTrialNumbersError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     data = json.dumps({"freeTrialNumbers": phone_numbers}).encode()
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     trail_numbers_request = request.Request(
         _URL, data=data, headers=headers, method="POST"
@@ -96,15 +96,15 @@
     except exceptions.CredentialError as exc:
         raise exceptions.FreeTrialNumbersError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     free_trail_numbers_request = request.Request(_URL, headers=headers, method="GET")
     try:
```

### Comparing `telstra_messaging-3.0.3/telstra/messaging/health_check.py` & `telstra_messaging-3.1.0/telstra/messaging/health_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
     Returns nothing
 
     """
     try:
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
-        raise exceptions.FreeTrialNumbersError(
+        raise exceptions.HealthCheckError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     health_check_request = request.Request(_URL, headers=headers, method="GET")
     try:
```

### Comparing `telstra_messaging-3.0.3/telstra/messaging/message.py` & `telstra_messaging-3.1.0/telstra/messaging/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         data["statusCallbackUrl"] = status_callback_url
     if tags is not None:
         data["tags"] = tags
     data_str = json.dumps(data).encode()
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     message_request = request.Request(
         f"{_URL}",
@@ -460,15 +460,15 @@
     if status_callback_url is not None:
         data["statusCallbackUrl"] = status_callback_url
     if tags is not None:
         data["tags"] = tags
     data_str = json.dumps(data).encode()
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     message_request = request.Request(
         f"{_URL}/{parse.quote(message_id)}",
@@ -556,15 +556,15 @@
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     data: typing.Dict[str, typing.Any] = {"tags": tags}
     data_str = json.dumps(data).encode()
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     update_tags_request = request.Request(
         f"{_URL}/{parse.quote(message_id)}",
@@ -612,15 +612,15 @@
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
         raise exceptions.MessageError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     message_get_request = request.Request(
         f"{_URL}/{parse.quote(message_id)}",
@@ -725,15 +725,15 @@
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
         raise exceptions.MessageError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     messages_get_request = request.Request(
         f"{_URL}{querystring.build(limit=limit, offset=offset, filter_=filter_)}",
@@ -814,15 +814,15 @@
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
         raise exceptions.MessageError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     delete_request = request.Request(
         f"{_URL}/{parse.quote(message_id)}",
```

### Comparing `telstra_messaging-3.0.3/telstra/messaging/oauth.py` & `telstra_messaging-3.1.0/telstra/messaging/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,15 @@
 
     """
     data = parse.urlencode(
         {
             "grant_type": "client_credentials",
             "client_id": config.get().telstra_client_id,
             "client_secret": config.get().telstra_client_secret,
-            "scope": "free-trial-numbers:read free-trial-numbers:write "
-            "virtual-numbers:read virtual-numbers:write messages:read "
-            "messages:write messaging:read messaging:write",
+            "scope": "free-trial-numbers:read free-trial-numbers:write virtual-numbers:read virtual-numbers:write messages:read messaging:write reports:read reports:write",
         }
     ).encode("ascii")
     headers = {"Content-Type": "application/x-www-form-urlencoded", "Accept": "*/*"}
     oauth_request = request.Request(_URL, data=data, headers=headers, method="POST")
     try:
         with request.urlopen(oauth_request) as response:
             return TToken(**json.loads(response.read().decode()))
```

### Comparing `telstra_messaging-3.0.3/telstra/messaging/reports.py` & `telstra_messaging-3.1.0/telstra/messaging/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,21 +56,21 @@
     Returns:
         A list of reports.
 
     """
     try:
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
-        raise exceptions.FreeTrialNumbersError(
+        raise exceptions.ReportsError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     reports_request = request.Request(_URL, headers=headers, method="GET")
     try:
@@ -100,18 +100,16 @@
             list_of_error_dicts = error_response.get("errors", [])
             suggested_actions_string = (
                 error_response_util.get_suggeted_actions_list_str(
                     list_of_error_dicts=list_of_error_dicts, key="suggested_action"
                 )
             )
         except Exception:
-            raise exceptions.VirtualNumbersError(
-                f"Could not retrieve reports: {exc}"
-            ) from exc
-        raise exceptions.VirtualNumbersError(
+            raise exceptions.ReportsError(f"Could not retrieve reports: {exc}") from exc
+        raise exceptions.ReportsError(
             f"Could not retrieve reports. {suggested_actions_string}"
         ) from exc
 
 
 def get(report_id: str) -> TReport:
     """
     Retrieve the a report.
@@ -119,21 +117,21 @@
     Returns:
         A single report.
 
     """
     try:
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
-        raise exceptions.FreeTrialNumbersError(
+        raise exceptions.ReportsError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
     }
     report_request = request.Request(
         f"{_URL}/{report_id}", headers=headers, method="GET"
@@ -153,18 +151,16 @@
             list_of_error_dicts = error_response.get("errors", [])
             suggested_actions_string = (
                 error_response_util.get_suggeted_actions_list_str(
                     list_of_error_dicts=list_of_error_dicts, key="suggested_action"
                 )
             )
         except Exception:
-            raise exceptions.VirtualNumbersError(
-                f"Could not retrieve report: {exc}"
-            ) from exc
-        raise exceptions.VirtualNumbersError(
+            raise exceptions.ReportsError(f"Could not retrieve report: {exc}") from exc
+        raise exceptions.ReportsError(
             f"Could not retrieve report. {suggested_actions_string}"
         ) from exc
 
 
 def _validate_create_args(  # pylint: disable=too-many-arguments
     start_date: typing.Optional[str],
     end_date: typing.Optional[str],
@@ -219,15 +215,15 @@
         report_callback_url=report_callback_url,
         filter_=filter_,
     )
 
     try:
         token = oauth.get_token()
     except exceptions.CredentialError as exc:
-        raise exceptions.VirtualNumbersError(
+        raise exceptions.ReportsError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     data: typing.Dict[str, typing.Any] = {
         "startDate": start_date,
         "endDate": end_date,
     }
@@ -235,15 +231,15 @@
         data["reportCallbackUrl"] = report_callback_url
     if filter_ is not None:
         data["filter"] = filter_
     data_str = json.dumps(data).encode()
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Cache-Control": "no-cache",
     }
     numbers_request = request.Request(
@@ -264,13 +260,13 @@
             list_of_error_dicts = error_response.get("errors", [])
             suggested_actions_string = (
                 error_response_util.get_suggeted_actions_list_str(
                     list_of_error_dicts=list_of_error_dicts, key="suggested_action"
                 )
             )
         except Exception as inner_exc:
-            raise exceptions.VirtualNumbersError(
+            raise exceptions.ReportsError(
                 f"Could not create report: {inner_exc}"
             ) from inner_exc
-        raise exceptions.VirtualNumbersError(
+        raise exceptions.ReportsError(
             f"Could not create report. {suggested_actions_string}"
         ) from exc
```

### Comparing `telstra_messaging-3.0.3/telstra/messaging/types.py` & `telstra_messaging-3.1.0/telstra/messaging/types.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/callback_url.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/callback_url.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/config.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/config.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/error_response.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/error_response.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/free_trial_number.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/free_trial_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/message_id.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/message_id.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/reports_dates.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/reports_dates.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/schedule_send.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/schedule_send.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/utils/virtual_number.py` & `telstra_messaging-3.1.0/telstra/messaging/utils/virtual_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.3/telstra/messaging/virtual_number.py` & `telstra_messaging-3.1.0/telstra/messaging/virtual_number.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,14 +62,48 @@
 
     """
 
     virtual_numbers: list[TVirtualNumber]
     paging: TPaging
 
 
+@dataclasses.dataclass
+class TRecipientOptout:
+    """
+    A recipient optout mobile number.
+
+    Attrs:
+        message_id: A unique identifier for the message sent.
+        optout_number: Recipient optout number.
+        virtual_number: A virtual number assigned to your account.
+        create_timestamp:
+
+    """
+
+    message_id: str
+    virtual_number: str
+    optout_number: str
+    create_timestamp: str
+
+
+@dataclasses.dataclass
+class TRecipientOptouts:
+    """
+    List of recipient optout numbers.
+
+    Attrs:
+        recipient_optouts:
+        paging:
+
+    """
+
+    recipient_optouts: list[TRecipientOptout]
+    paging: TPaging
+
+
 def assign(
     reply_callback_url: typing.Optional[types.TStatusCallbackUrl] = None,
     tags: typing.Optional[typing.List[types.TTags]] = None,
 ) -> TVirtualNumber:
     """
     Assign a virtual number.
 
@@ -83,15 +117,15 @@
     """
     # Validate tags
     if (tags is not None and not isinstance(tags, list)) or (
         tags is not None
         and isinstance(tags, list)
         and (len(tags) < 1 or len(tags) > 10)
     ):
-        raise exceptions.MessageError(
+        raise exceptions.VirtualNumbersError(
             'the value of "tags" is not valid, expected a list of strings '
             "with alteast one tag or a maximum of 10, "
             f'received "{tags}"'
         )
     # Validate reply_callback_url
     callback_url_util.validate(
         name="reply_callback_url",
@@ -110,15 +144,15 @@
     if reply_callback_url is not None:
         data["replyCallbackUrl"] = reply_callback_url
     if tags is not None:
         data["tags"] = tags
     data_str = json.dumps(data).encode()
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Cache-Control": "no-cache",
     }
     numbers_request = request.Request(
@@ -159,33 +193,33 @@
 ) -> None:
     # Validate limit
     if (limit is not None and not isinstance(limit, types.TLimit)) or (
         limit is not None
         and isinstance(limit, types.TLimit)
         and (limit < 1 or limit > 50)
     ):
-        raise exceptions.MessageError(
+        raise exceptions.VirtualNumbersError(
             'the value of "limit" is not valid, expected a int value '
             f'between 1 and 50, received "{limit}"'
         )
 
     # Validate offset
     if (offset is not None and not isinstance(offset, types.TOffset)) or (
         offset is not None
         and isinstance(offset, types.TOffset)
         and (offset < 0 or offset > 999999)
     ):
-        raise exceptions.MessageError(
+        raise exceptions.VirtualNumbersError(
             'the value of "offset" is not valid, expected a int value '
             f'between 0 and 999999, received "{offset}"'
         )
 
     # Validate filter
     if filter_ is not None and not isinstance(filter_, types.TFilter):
-        raise exceptions.MessageError(
+        raise exceptions.VirtualNumbersError(
             'the value of "filter" is not valid, expected a string, '
             f'received "{filter_}"'
         )
 
 
 def get_all(
     limit: typing.Optional[types.TLimit] = None,
@@ -206,15 +240,15 @@
     except exceptions.CredentialError as exc:
         raise exceptions.VirtualNumbersError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Cache-Control": "no-cache",
     }
     virtual_numbers_request = request.Request(
@@ -292,15 +326,15 @@
     except exceptions.CredentialError as exc:
         raise exceptions.VirtualNumbersError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Cache-Control": "no-cache",
     }
     virtual_numbers_request = request.Request(
@@ -360,15 +394,15 @@
 
     # Validate tags
     if (tags is not None and not isinstance(tags, list)) or (
         tags is not None
         and isinstance(tags, list)
         and (len(tags) < 1 or len(tags) > 10)
     ):
-        raise exceptions.MessageError(
+        raise exceptions.VirtualNumbersError(
             'the value of "tags" is not valid, expected a list of '
             "strings with alteast one tag or a maximum of 10, "
             f'received "{tags}"'
         )
 
     # Validate reply_callback_url
     callback_url_util.validate(
@@ -388,15 +422,15 @@
     if reply_callback_url is not None:
         data["replyCallbackUrl"] = reply_callback_url
     if tags is not None:
         data["tags"] = tags
     data_str = json.dumps(data).encode()
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Cache-Control": "no-cache",
     }
     virtual_numbers_update_request = request.Request(
@@ -452,15 +486,15 @@
     except exceptions.CredentialError as exc:
         raise exceptions.VirtualNumbersError(
             f"Could not retrieve an OAuth token: {exc}"
         ) from exc
 
     headers = {
         "Authorization": token.authorization,
-        "Telstra-api-version": "3.1.0",
+        "Telstra-api-version": "3.x",
         "Content-Language": "en-au",
         "Accept-Charset": "utf-8",
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Cache-Control": "no-cache",
     }
     numbers_request = request.Request(
@@ -482,7 +516,89 @@
         except Exception:
             raise exceptions.VirtualNumbersError(
                 f"Could not delete virtual number: {exc}"
             ) from exc
         raise exceptions.VirtualNumbersError(
             f"Could not delete virtual number. {suggested_actions_string}"
         ) from exc
+
+
+def get_optouts(
+    virtual_number: str,
+    limit: typing.Optional[types.TLimit] = None,
+    offset: typing.Optional[types.TOffset] = None,
+) -> TRecipientOptouts:
+    """
+    Retrieve all virtual numbers assigned to you.
+
+    Raises VirtualNumbersError if anything goes wrong.
+
+    """
+
+    _validate_get_all_args(limit=limit, offset=offset, filter_=None)
+
+    try:
+        token = oauth.get_token()
+    except exceptions.CredentialError as exc:
+        raise exceptions.VirtualNumbersError(
+            f"Could not retrieve an OAuth token: {exc}"
+        ) from exc
+
+    headers = {
+        "Authorization": token.authorization,
+        "Telstra-api-version": "3.x",
+        "Content-Language": "en-au",
+        "Accept-Charset": "utf-8",
+        "Accept": "application/json",
+        "Content-Type": "application/json",
+        "Cache-Control": "no-cache",
+    }
+    optouts_request = request.Request(
+        f"{_URL}"
+        f"/{virtual_number}/optouts"
+        f"{querystring.build(limit=limit, offset=offset)}",
+        headers=headers,
+        method="GET",
+    )
+    try:
+        with request.urlopen(optouts_request) as response:
+            optouts: list[TRecipientOptout] = []
+            optouts_response_dict = json.loads(response.read().decode())
+            optouts_list = optouts_response_dict.get("recipientOptouts", [])
+
+            if optouts_list is not None and len(optouts_list) > 0:
+                optouts = [
+                    TRecipientOptout(
+                        message_id=d.get("messageId"),
+                        virtual_number=d.get("virtualNumber"),
+                        optout_number=d.get("optoutNumber"),
+                        create_timestamp=d.get("createTimestamp"),
+                    )
+                    for d in optouts_list
+                ]
+            paging = TPaging(
+                next_page=optouts_response_dict["paging"].get("nextPage", ""),
+                previous_page=optouts_response_dict["paging"].get("previousPage", ""),
+                last_page=optouts_response_dict["paging"].get("lastPage", ""),
+                total_count=optouts_response_dict["paging"].get("totalCount", 0),
+            )
+            return TRecipientOptouts(
+                recipient_optouts=([] if optouts is None else optouts),
+                paging=paging,
+            )
+    except error.HTTPError as exc:
+        suggested_actions_string = ""
+        try:
+            error_response = json.loads(exc.read().decode())
+            list_of_error_dicts = error_response.get("errors", [])
+            suggested_actions_string = (
+                error_response_util.get_suggeted_actions_list_str(
+                    list_of_error_dicts=list_of_error_dicts, key="suggested_action"
+                )
+            )
+        except Exception:
+            raise exceptions.VirtualNumbersError(
+                f"Could not retrieve the list of optout numbers: {exc}"
+            ) from exc
+        raise exceptions.VirtualNumbersError(
+            f"Could not retrieve the list of optout numbers. {suggested_actions_string}"
+        ) from exc
```

### Comparing `telstra_messaging-3.0.3/PKG-INFO` & `telstra_messaging-3.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-Metadata-Version: 2.1
-Name: telstra-messaging
-Version: 3.0.3
-Summary: SDK for the Telstra Messaging API V3 - Beta
-License: Apache-2.0
-Author: David Andersson
-Author-email: david-andersson@users.noreply.github.com 
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # Telstra Messaging
 
 The SDK for the Telstra Messaging API enables you to send and receive messages
 to Australian mobile numbers. For more information about this product, please
 see here:
-<https://dev.telstra.com/content/messaging-api-v3>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverview?version=3.x>.
 
 > :warning: **This SDK is experimental, everything is subject to change**
 
 ## Installing
 
 ```bash
 pip install telstra.messaging
@@ -98,29 +84,29 @@
 ## Free Trial
 
 Telstra offers a free trial for the messaging API to help you evaluate whether
 it meets your needs. There are some restrictions that apply compared to the
 full API, including a maximum number of messages that can be sent and requiring the
 registration of a limited number of destinations before a message can be sent
 to that destination. For more information, please see here:
-<https://dev.telstra.com/content/messaging-api#tag/Free-Trial>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FreeTrial>.
 
 ### Registering Free Trial Numbers
 
 > :information_source: **Only required for the free trial**
 
 Register numbers for the free trial. For more information, please see
 here:
-<https://dev.telstra.com/content/messaging-api-v3#tag/free-trial-numbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#RegisteraFreeTrialNumber>.
 
 The function `telstra.messaging.free_trial_numbers.create` can be used to register
 destinations. It takes the following arguments:
 
-- `phone_numbers`: A list of destinations, expected to be phone numbers of the
-  form `+614XXXXXXXX` or `04XXXXXXXX`.
+- `phone_numbers`: A list of destinations, expected to be phone numbers
+  of the form `04XXXXXXXX`.
 
 Raises `telstra.messaging.exceptions.FreeTrialNumbersError` if anything goes wrong.
 
 It returns the list of phone numbers that have been registered.
 
 For example:
 
@@ -134,15 +120,15 @@
 
 ### Fetch all Free Trial Numbers
 
 > :information_source: **Only required for the free trial**
 
 Fetch the Free Trial Number(s) currently assigned to your account. For more information,
 please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getTrialNumbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchyourFreeTrialNumbers>.
 
 The function `telstra.messaging.free_trial_numbers.get_all`
 can be used to retrieve registered destinations.
 It takes no arguments.
 
 Raises `telstra.messaging.exceptions.FreeTrialNumbersError` if anything goes wrong.
 
@@ -160,23 +146,23 @@
 ```
 
 ## Virtual Number
 
 Gives you a dedicated mobile number tied to an application which
 enables you to receive replies from your customers. For more information,
 please see here:
-<https://dev.telstra.com/content/messaging-api-v3#tag/virtual-numbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#VirtualNumbers>.
 
 ### Assign Virtual Number
 
 When a recipient receives your message, you can choose whether they'll see a privateNumber,
 Virtual Number or senderName (paid plans only) in the from field.
 If you want to use a Virtual Number, use this function to assign one.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/assignNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#AssignaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.create` can be used to create a
 numbers. It takes the following arguments:
 
 - `reply_callback_url` (optional): The URL that replies to the
   Virtual Number will be posted to.
 - `tags` (optional): Create your own tags and use them to fetch,
@@ -203,15 +189,15 @@
 print(assigned_numbers)
 ```
 
 ### Fetch a Virtual Number
 
 Fetch the tags, replyCallbackUrl and lastUse date for a Virtual Number.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getVirtualNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.get` can be used to get the current
 number. It takes the following arguments:
 
 - `virtual_number`: The Virtual Number assigned to your account.
 
 Raises `telstra.messaging.exceptions.VirtualNumbersError` if anything goes wrong.
@@ -235,15 +221,15 @@
 print(retrieved_number)
 ```
 
 ### Fetch all Virtual Numbers
 
 Fetch all Virtual Numbers currently assigned to your account.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getNumbers>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchallVirtualNumbers>.
 
 The function `telstra.messaging.virtual_number.get_all` can be used to
 get the all virtual numbers associated to your account.
 It takes the following arguments:
 
 - `limit`: Tell us how many results you want us to return, up to a maximum of 50.
 - `offset`: Use the offset to navigate between the response results.
@@ -268,15 +254,15 @@
 print(retrieved_virtual_numbers)
 ```
 
 ### Update a Virtual Number
 
 Update a virtual number attributes. For more information,
 please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/updateNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#UpdateaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.update` can be used to update a
 virtual number. It takes the following arguments:
 
 - `virtual_number`: The Virtual Number assigned to your account.
 - `reply_callback_url` (optional): The URL that replies to the
   Virtual Number will be posted to.
@@ -306,15 +292,15 @@
   )
 print(updated_virtual_number)
 ```
 
 ### Delete Virtual Number
 
 Delete the a virtual number. For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/deleteNumber>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#DeleteaVirtualNumber>.
 
 The function `telstra.messaging.virtual_number.delete` can be used
 to delete the current number. It takes the following arguments:
 
 - `virtual_number`: The Virtual Number assigned to your account.
 
 Raises `telstra.messaging.exceptions.VirtualNumbersError` if anything goes wrong.
@@ -324,24 +310,59 @@
 ```python
 # Delete a virtual number
 from telstra.messaging import virtual_number
 
 virtual_number.delete(virtual_number="0400000001")
 ```
 
+### Fetch all Recipient Optouts list
+
+Fetch any mobile number(s) that have opted out of receiving messages
+from a Virtual Number assigned to your account.
+For more information, please see here:
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchallrecipientoptoutslist>.
+
+The function `telstra.messaging.virtual_number.get_optouts` can be used to
+get the list of mobile numbers that have opted out of receiving messages
+from a virtual number associated to your account.
+It takes the following arguments:
+
+- `virtual_number`: The Virtual Number assigned to your account.
+- `limit`: Tell us how many results you want us to return, up to a maximum of 50.
+- `offset`: Use the offset to navigate between the response results.
+  An offset of 0 will display the first page of results, and so on.
+
+Raises `telstra.messaging.exceptions.VirtualNumbersError` if anything goes wrong.
+
+It returns an object with the following
+properties:
+
+- `recipient_optouts`: A list of recipient optouts.
+- `paging`: Paging information.
+
+For example:
+
+```python
+# Get all virtual numbers
+from telstra.messaging import virtual_number
+
+retrieved_optout_numbers = virtual_number.get_optouts(virtual_number="0400000001")
+print(retrieved_optout_numbers)
+```
+
 ## Message
 
 Send and receive messages. For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#tag/messages>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Messages>.
 
 ### Send Message
 
 Send a message to a mobile number, or to multiple mobile numbers.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/sendMessages>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#SendanSMSorMMS>.
 
 The function `telstra.messaging.message.send` can be used to send a message.
 It takes the following arguments:
 
 - `to`: The destination address, expected to be a phone number of the form
   `+614XXXXXXXX` or `04XXXXXXXX`.
 - `from_`: This will be either "privateNumber", one of your Virtual Numbers
@@ -351,15 +372,16 @@
 - `multimedia` (Either one of messageContent or multimedia is required).
   MMS multimedia content.
 - `retry_timeout` (optional): How many minutes you asked the server to
   keep trying to send the message.
 - `schedule_send` (optional): The time (in Central Standard Time)
   the message is scheduled to send.
 - `delivery_notification` (optional): If set to true, you will receive
-  a notification to the statusCallbackUrl when your SMS is delivered (paid feature).
+  a notification to the statusCallbackUrl when your SMS or MMS
+  is delivered (paid feature).
 - `status_callback_url` (optional): The URL the API will call when the
   status of the message changes.
 - `tags` (optional): Any customisable tags assigned to the message.
 
 The dataclass `telstra.messaging.message.Multimedia`
 can be used to build an mms payload.
 It takes the following arguments:
@@ -381,15 +403,15 @@
 - `message_content`: The content of the message.
 - `multimedia`: The multimedia content of the message (MMS only).
 - `retry_timeout`: How many minutes you asked the server to keep
   trying to send the message.
 - `schedule_send`: The time (in Central Standard Time) a message
   is scheduled to send.
 - `delivery_notification`: If set to true, you will receive a notification to the
-  statusCallbackUrl when your SMS is delivered (paid feature).
+  statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url`: The URL the API will call when the status of
   the message changes.
 - `tags`: Any customisable tags assigned to the message.
 
 For example:
 
 ```python
@@ -416,29 +438,27 @@
 )
 ```
 
 ### Get a Message
 
 Use the messageId to fetch a message that's been sent from/to
 your account within the last 30 days.
-Note that in the current release, inbound MMS or messages sent in
-reply to an MMS will not be retrieved..
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getMessageById>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchamessage>.
 
 The function `telstra.messaging.message.get` can be used to retrieve
 the a message. It takes the following arguments:
 
 - `message_id`:Unique identifier for the message.
 
 Raises `telstra.messaging.exceptions.MessageError` if anything goes wrong.
 
 It returns an object with the following properties:
 
-- `messageId`: Use this UUID with our other endpoints to fetch,
+- `message_id`: Use this UUID with our other endpoints to fetch,
   update or delete the message.
 - `status`: The status will be either queued, sent, delivered or expired.
 - `create_timestamp`: The time you submitted the message to
   the queue for sending.
 - `sent_timestamp`: The time the message was sent from the server.
 - `received_timestamp`: The time the message was received by the
   recipient's device.
@@ -449,15 +469,15 @@
 - `multimedia`: The multimedia content of the message (MMS only).
 - `direction`: Direction of the message (outgoing or incoming).
 - `retry_timeout`: How many minutes you asked the server to keep
   trying to send the message.
 - `schedule_send`: The time (in Central Standard Time) the message is
   scheduled to send.
 - `delivery_notification`: If set to true, you will receive a notification
-  to the statusCallbackUrl when your SMS is delivered (paid feature).
+  to the statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url`: The URL the API will call when the status of
   the message changes.
 - `queue_priority`: The priority assigned to the message.
 - `tags`: Any customisable tags assigned to the message.
 
 For example:
 
@@ -473,18 +493,16 @@
 message = message.get(message_id = sent_message.message_id)
 print(message)
 ```
 
 ### Get all Messages
 
 Fetch messages that have been sent from/to your account in the last 30 days.
-Note that in the current release, inbound MMS or messages sent
-in reply to an MMS will not be retrieved.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getMessages>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchallsent/receivedmessages>.
 
 The function `telstra.messaging.message.get_all` can be used to fetch
 all messages. It takes the
 following arguments:
 
 - `limit`: Tell us how many results you want us to return, up to a maximum of 50.
 - `offset`: Use the offset to navigate between the response results.
@@ -510,15 +528,15 @@
 ```
 
 ### Update a Message
 
 Update a message that's scheduled for sending, you can change any of
 the below parameters, as long as the message hasn't been sent yet.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/updateMessageById>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Updateamessage>.
 
 The function `telstra.messaging.message.update` can be used to update a message.
 It takes the following arguments:
 
 - `to`: The destination address, expected to be a phone number of the form
   `+614XXXXXXXX` or `04XXXXXXXX`.
 - `from_`: This will be either "privateNumber", one of your
@@ -527,15 +545,15 @@
   Either one of messageContent or multimedia is required.
 - `multimedia` MMS multimedia content.
 - `retry_timeout` (optional): How many minutes you asked the server to
   keep trying to send the message.
 - `schedule_send` (optional): The time (in Central Standard Time) the
   message is scheduled to send.
 - `delivery_notification` (optional): If set to true, you will receive a
-  notification to the statusCallbackUrl when your SMS is delivered (paid feature).
+  notification to the statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url` (optional): The URL the API will call when
   the status of the message changes.
 - `tags` (optional): Any customisable tags assigned to the message.
 
 Raises `telstra.messaging.exceptions.MessageError` if anything goes wrong.
 
 The dataclass `telstra.messaging.message.Multimedia` can be used to build
@@ -558,15 +576,15 @@
 - `message_content`: The content of the message.
 - `multimedia`: The multimedia content of the message (MMS only).
 - `retry_timeout`: How many minutes you asked the server to keep trying
   to send the message.
 - `schedule_send`: The time (in Central Standard Time) the message
   is scheduled to send.
 - `delivery_notification`: If set to true, you will receive a notification to the
-  statusCallbackUrl when your SMS is delivered (paid feature).
+  statusCallbackUrl when your SMS or MMS is delivered (paid feature).
 - `status_callback_url`: The URL the API will call when the
   status of the message changes.
 - `tags`: Any customisable tags assigned to the message.
 
 For example:
 
 ```python
@@ -581,15 +599,15 @@
   )
 ```
 
 ### Update Message Tags
 
 Update message tags, you can update them even after your message has been delivered.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/updateMessageTags>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Updatemessagetags>.
 
 The function `telstra.messaging.message.update_tags` can be used to
 update message tags. It takes the following arguments:
 
 - `message_id`:Unique identifier for the message.
 - `tags` (optional): Any customisable tags assigned to the message.
 
@@ -606,15 +624,15 @@
 message.update_tags(message_id="8540d774-4863-4d2b-b788-4ecb19412e85", tags=["Python","V3"])
 ```
 
 ### Delete a Message
 
 Delete a scheduled message, but hasn't yet sent.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/deleteMessageById>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Deleteamessage>.
 
 The function `telstra.messaging.message.delete` can be used to delete a message.
 It takes the following arguments:
 
 - `message_id`: Unique identifier for the message.
 
 Raises `telstra.messaging.exceptions.MessageError` if anything goes wrong.
@@ -636,15 +654,15 @@
 <https://dev.telstra.com/content/messaging-api-v3#tag/reports>.
 
 ### Request a Report
 
 Request a CSV report of messages (both incoming and outgoing)
 that have been sent to/from your account within the last three months.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/messagesReport>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Submitarequestforamessagesreport>.
 
 The function `telstra.messaging.reports.create` can be used to create a report.
 It takes the following arguments:
 
 - `start_date`: Set the time period you want to generate a
   report for by typing the start date (inclusive) here. Note that we only
   retain data for three months, so please ensure your startDate is not more
@@ -682,15 +700,15 @@
     )
 ```
 
 ### Fetch a specific report
 
 Use the report_id to fetch a download link for a report generated.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getReport>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#FetchaReport>.
 
 The function `telstra.messaging.reports.get` can be used to retrieve
 the a report download link. It takes the following arguments:
 
 - `report_id`:Unique identifier for the report.
 
 Raises `telstra.messaging.exceptions.ReportsError` if anything goes wrong.
@@ -703,25 +721,25 @@
 
 For example:
 
 ```python
 # Get a report download link
 from telstra.messaging import reports
 
-report_reponse = reports.get(report_id = '6940c774-4335-4d2b-b758-4ecb19412e85')
+report_response = reports.get(report_id = '6940c774-4335-4d2b-b758-4ecb19412e85')
 print(report_response)
 ```
 
 ### Fetch all reports
 
 Fetch details of all reports recently generated for your account.
 Use it to check the status of a report, plus fetch the report ID,
 status, report type and expiry date.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/getReports>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#Fetchallreports>.
 
 The function `telstra.messaging.reports.get_all` can be used to fetch
 all reports. It doesn't take any arguments.
 
 Raises `telstra.messaging.exceptions.ReportsError` if anything goes wrong.
 
 It returns a list of objects with the following properties:
@@ -744,15 +762,15 @@
 
 ## Health Check
 
 ### Get operational status of the messaging service
 
 Check the operational status of the messaging service.
 For more information, please see here:
-<https://dev.telstra.com/content/messaging-api-v3#operation/healthCheck>.
+<https://dev.telstra.com/docs/messaging-api/apiReference/apiReferenceOverviewEndpoints?version=3.x#HealthCheck>.
 
 The function `telstra.messaging.health_check.get` can be used to get the status.
 It takes no arguments.
 
 Raises `telstra.messaging.exceptions.HealthCheckError` if anything goes wrong.
 
 It returns nothing.
@@ -772,8 +790,7 @@
 ## Exceptions
 
 All exceptions that can be raised derive from `MessagingBaseException`:
 
 ```python
 from telstra.messaging.exceptions import MessagingBaseException
 ```
-
```

