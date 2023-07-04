# Comparing `tmp/xyz_exam-0.3.7-py3-none-any.whl.zip` & `tmp/xyz_exam-0.3.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 31485 bytes, number of entries: 32
+Zip file size: 31539 bytes, number of entries: 32
 -rw-r--r--  2.0 unx       43 b- defN 20-Jan-20 09:10 xyz_exam/__init__.py
 -rw-r--r--  2.0 unx     1631 b- defN 22-Dec-07 08:39 xyz_exam/admin.py
--rw-r--r--  2.0 unx    12193 b- defN 23-Apr-23 16:47 xyz_exam/apis.py
+-rw-r--r--  2.0 unx    12317 b- defN 23-Jun-24 09:44 xyz_exam/apis.py
 -rw-r--r--  2.0 unx      326 b- defN 20-Jan-20 09:08 xyz_exam/apps.py
 -rw-r--r--  2.0 unx     1381 b- defN 22-Oct-27 06:40 xyz_exam/choices.py
 -rw-r--r--  2.0 unx    13585 b- defN 23-Mar-14 03:26 xyz_exam/helper.py
 -rw-r--r--  2.0 unx    15559 b- defN 23-Apr-24 19:43 xyz_exam/models.py
 -rw-r--r--  2.0 unx     3688 b- defN 23-Jan-11 04:45 xyz_exam/receivers.py
 -rw-r--r--  2.0 unx     3469 b- defN 23-Apr-23 16:47 xyz_exam/serializers.py
--rw-r--r--  2.0 unx     3574 b- defN 22-Jun-23 18:16 xyz_exam/stats.py
+-rw-r--r--  2.0 unx     3578 b- defN 23-Jul-02 06:26 xyz_exam/stats.py
 -rw-r--r--  2.0 unx     3154 b- defN 23-Apr-09 13:18 xyz_exam/stores.py
 -rw-r--r--  2.0 unx     7732 b- defN 20-Jan-20 09:14 xyz_exam/migrations/0001_initial.py
 -rw-r--r--  2.0 unx     3123 b- defN 20-Jun-15 13:12 xyz_exam/migrations/0002_auto_20200615_2112.py
 -rw-r--r--  2.0 unx     2514 b- defN 20-Jun-25 21:11 xyz_exam/migrations/0003_auto_20200626_0511.py
 -rw-r--r--  2.0 unx     2405 b- defN 20-Aug-01 16:28 xyz_exam/migrations/0004_auto_20200802_0028.py
 -rw-r--r--  2.0 unx      518 b- defN 20-Sep-01 15:06 xyz_exam/migrations/0005_answer_pictures.py
 -rw-r--r--  2.0 unx      543 b- defN 20-Sep-14 19:21 xyz_exam/migrations/0006_answer_grade_detail.py
@@ -23,12 +23,12 @@
 -rw-r--r--  2.0 unx     1606 b- defN 22-Sep-08 16:15 xyz_exam/migrations/0011_content.py
 -rw-r--r--  2.0 unx      601 b- defN 22-Sep-17 06:10 xyz_exam/migrations/0012_auto_20220917_1410.py
 -rw-r--r--  2.0 unx      949 b- defN 22-Oct-27 06:41 xyz_exam/migrations/0013_auto_20221027_1441.py
 -rw-r--r--  2.0 unx      498 b- defN 22-Nov-27 11:39 xyz_exam/migrations/0014_paper_parent_id.py
 -rw-r--r--  2.0 unx      484 b- defN 22-Dec-07 08:37 xyz_exam/migrations/0015_paper_is_editable.py
 -rw-r--r--  2.0 unx      946 b- defN 23-Apr-11 14:11 xyz_exam/migrations/0016_auto_20230411_2211.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-20 09:14 xyz_exam/migrations/__init__.py
--rw-r--r--  2.0 unx      987 b- defN 23-Apr-24 19:45 xyz_exam-0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 19:45 xyz_exam-0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-24 19:45 xyz_exam-0.3.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2824 b- defN 23-Apr-24 19:45 xyz_exam-0.3.7.dist-info/RECORD
-32 files, 87350 bytes uncompressed, 26885 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx      987 b- defN 23-Jul-04 17:20 xyz_exam-0.3.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 17:20 xyz_exam-0.3.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-04 17:20 xyz_exam-0.3.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2824 b- defN 23-Jul-04 17:20 xyz_exam-0.3.8.dist-info/RECORD
+32 files, 87478 bytes uncompressed, 26939 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -78,20 +78,20 @@
 
 Filename: xyz_exam/migrations/0016_auto_20230411_2211.py
 Comment: 
 
 Filename: xyz_exam/migrations/__init__.py
 Comment: 
 
-Filename: xyz_exam-0.3.7.dist-info/METADATA
+Filename: xyz_exam-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: xyz_exam-0.3.7.dist-info/WHEEL
+Filename: xyz_exam-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_exam-0.3.7.dist-info/top_level.txt
+Filename: xyz_exam-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_exam-0.3.7.dist-info/RECORD
+Filename: xyz_exam-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_exam/apis.py

```diff
@@ -272,14 +272,17 @@
         return super(ExamViewSet, self).create(request)
 
     def perform_create(self, serializer):
         super(ExamViewSet, self).perform_create(serializer)
         if self.action == 'auto_gen':
             data = self.request.data
             questions = data.get('questions')
+            for i, q in enumerate(questions):
+                n = q['number'] = i+1
+                q['id'] = 'g1q%d' % (n)
             exam = serializer.instance
             from django.contrib.contenttypes.models import ContentType
             paper, created = models.Paper.objects.update_or_create(
                 owner_id=exam.pk,
                 owner_type=ContentType.objects.get_for_model(exam),
                 defaults=dict(
                     user=self.request.user,
```

## xyz_exam/stats.py

```diff
@@ -19,23 +19,23 @@
 def stats_paper(qset=None, measures=None, period=None, time_field=None):
     qset = qset if qset is not None else models.Paper.objects.all()
     qset = statutils.using_stats_db(qset)
     dstat = statutils.DateStat(qset, 'create_time')
     from . import stores
     funcs = {
         'all': lambda: qset.count(),
-        'tags': lambda : statutils.count_by(qset, 'tags'),
-        'outline': lambda : stores.group_paper_questions(qset)
+        'tags': lambda: statutils.count_by(qset, 'tags'),
+        'outline': lambda: stores.group_paper_questions(qset)
     }
     return dict([(m, funcs[m]()) for m in measures])
 
-def stats_answer(qset=None, measures=None, period=None, time_field=None):
+def stats_answer(qset=None, measures=None, period=None, time_field='create_time'):
     qset = qset if qset is not None else models.Answer.objects.all()
     qset = statutils.using_stats_db(qset)
-    dstat = statutils.DateStat(qset, 'create_time')
+    dstat = statutils.DateStat(qset, time_field)
     funcs = {
         'today': lambda: dstat.stat("今天", count_field="user_id", distinct=True, only_first=True),
         'yesterday': lambda: dstat.stat("昨天", count_field="user_id", distinct=True, only_first=True),
         'all': lambda: qset.values("user_id").distinct().count(),
         'count': lambda: dstat.get_period_query_set(period).count(),
         'daily': lambda: dstat.stat(period, count_field='user_id', distinct=True),
         'class': lambda: statutils.count_by(
```

## Comparing `xyz_exam-0.3.7.dist-info/METADATA` & `xyz_exam-0.3.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-exam
-Version: 0.3.7
+Version: 0.3.8
 Summary: exam app
 Home-page: https://github.com/szuprefix/py-xyz-exam
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_exam-0.3.7.dist-info/RECORD` & `xyz_exam-0.3.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 xyz_exam/__init__.py,sha256=R09BZ9ss3CC_upX6gf82fFdHuqU_3vh0SavPOcBtQr0,43
 xyz_exam/admin.py,sha256=hP889pXJfcfqy9_5gPq6AYsXE5CyZ8SVYbbR8BjhfQ8,1631
-xyz_exam/apis.py,sha256=PpuebkLIfnoiYkwIvjRRx-IUlKCPmwJZk_ETDdXz9aI,12193
+xyz_exam/apis.py,sha256=y_EXUaivmx3RFbLjlZKpEO8EvX6C7D8XfBlxHK1fR9o,12317
 xyz_exam/apps.py,sha256=vQwce8vZ81IpBtAVpe8wvqqZXfV0Ht5AJeMY7rRsP6g,326
 xyz_exam/choices.py,sha256=2lKMyQAWnl_yoow98cpQHwqpk-RXxnxij4xcvxeVUko,1381
 xyz_exam/helper.py,sha256=lKVyMH8fOF4JL1wbdr0Hbhm8nFiJWpY2vh3vc_sdvkQ,13585
 xyz_exam/models.py,sha256=Fujzmj3A5Uk71CHevgz1MuQYPkYHbpBtiW3wO-Rl5Rg,15559
 xyz_exam/receivers.py,sha256=oOthYcU_vabvgLLAWrjq3BubC7DQbA-ek6_hQhsqhg4,3688
 xyz_exam/serializers.py,sha256=1hNoFpJJwoKBkpxOhrXH7cfw6G-QZO5Dj5C173EUBHU,3469
-xyz_exam/stats.py,sha256=u6XcKw7wkLOm_JtCLoF6241sAZghHQNh5sQfjmjBkSs,3574
+xyz_exam/stats.py,sha256=sKTHkGFvO0CLMN7vgm85Kb7jHefPHPgaojITkIlHgPY,3578
 xyz_exam/stores.py,sha256=2T5aMjrMQ4w-qxgkrkx2ZmNcbZq_8lojUZf8dWjGh90,3154
 xyz_exam/migrations/0001_initial.py,sha256=Poa0-alDt7Ylgm6YeJ2cUwNPvHJz55qsuuPTT0IPBR0,7732
 xyz_exam/migrations/0002_auto_20200615_2112.py,sha256=JofSLAwEIoJ1pjZu6MLRiPyWn1nAhxQUuTketVO81Yc,3123
 xyz_exam/migrations/0003_auto_20200626_0511.py,sha256=sAkmKE3fYO9gi9aDOPbZALKZ8T0ZRCvSHiiJjMbRzmM,2514
 xyz_exam/migrations/0004_auto_20200802_0028.py,sha256=oJxvhMj_uh5qYoqTe68wNNrtFLTaIYUbjIfLX14u7pc,2405
 xyz_exam/migrations/0005_answer_pictures.py,sha256=TMr2dBWmxvq0rHsqH20rkO-0uz9k0vMgHgiZqJf8TII,518
 xyz_exam/migrations/0006_answer_grade_detail.py,sha256=LhvXN8qNpjIQT_QKCftSLdm02-lcg75sWA4_CxudVYs,543
@@ -22,11 +22,11 @@
 xyz_exam/migrations/0011_content.py,sha256=FqT4q-o8xJywQ2382G6js1Av7ZEgROr7NmLGSxBp6NU,1606
 xyz_exam/migrations/0012_auto_20220917_1410.py,sha256=RHYolr37Gk2lqZifxypAcylcADeTNZBRRvDGJWAoDmE,601
 xyz_exam/migrations/0013_auto_20221027_1441.py,sha256=_iFsdTKrADPb_EGTTw-3gMD8FMakD8nTbBJOsXRLhY4,949
 xyz_exam/migrations/0014_paper_parent_id.py,sha256=WpMmFmzN2c_4UiSJl2x2QiNv7MZccIbA8kq6M8WWZd8,498
 xyz_exam/migrations/0015_paper_is_editable.py,sha256=8Fbh6vDwxJnKcXar8s6LfGfvAsPdp0vAjxb0XrtjNU0,484
 xyz_exam/migrations/0016_auto_20230411_2211.py,sha256=VuS7lHAoDJ37OpZsBBNKkN-cETJEZ0TJfXxWkKt1-Mk,946
 xyz_exam/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xyz_exam-0.3.7.dist-info/METADATA,sha256=gR38eAd0LOiOyaRAE7KLj_AI6-cDcOskqhn4wAjN6xw,987
-xyz_exam-0.3.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_exam-0.3.7.dist-info/top_level.txt,sha256=AdR0uTxGwndkM__gIaBc3_DMomtP0FQ-PKg_WJP2KTE,9
-xyz_exam-0.3.7.dist-info/RECORD,,
+xyz_exam-0.3.8.dist-info/METADATA,sha256=3m_2krI4XIggbLj9tBySFvhoCtfAbAUWL5_Fu0MsJSo,987
+xyz_exam-0.3.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_exam-0.3.8.dist-info/top_level.txt,sha256=AdR0uTxGwndkM__gIaBc3_DMomtP0FQ-PKg_WJP2KTE,9
+xyz_exam-0.3.8.dist-info/RECORD,,
```

