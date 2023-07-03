# Comparing `tmp/easy_post_twitter-1.0.7.tar.gz` & `tmp/easy_post_twitter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_post_twitter-1.0.7.tar", max compression
+gzip compressed data, was "easy_post_twitter-1.0.8.tar", max compression
```

## Comparing `easy_post_twitter-1.0.7.tar` & `easy_post_twitter-1.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.7/easy_post_twitter/__init__.py
--rw-r--r--   0        0        0    11800 2023-05-21 21:35:18.594562 easy_post_twitter-1.0.7/easy_post_twitter/twitter.py
--rw-r--r--   0        0        0      415 2023-05-23 12:20:17.184434 easy_post_twitter-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.8/easy_post_twitter/__init__.py
+-rw-r--r--   0        0        0    11839 2023-07-03 22:52:45.422586 easy_post_twitter-1.0.8/easy_post_twitter/twitter.py
+-rw-r--r--   0        0        0      415 2023-07-03 22:55:22.575447 easy_post_twitter-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.8/PKG-INFO
```

### Comparing `easy_post_twitter-1.0.7/easy_post_twitter/twitter.py` & `easy_post_twitter-1.0.8/easy_post_twitter/twitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,23 +228,24 @@
     def tweetIt(self, text, img, isThread, id):
         ''' This method do not use twitter's api search to determine if
         a tweet is the day's opening one or a response to an early one. 
         Tweets with or without images.
         '''
         # with image
         if img != '':
+          client = self.__get_client()
           if isThread:
               api = self.__get_api()
               media = api.media_upload(img)
-              response = api.update_status(status=text, media_ids=[media.media_id], in_reply_to_status_id=id)
+              response = client.create_tweet(text=text, media_ids=[media.media_id], in_reply_to_tweet_id=id)
               return response
           else:
               api = self.__get_api()
               media = api.media_upload(img)
-              response = api.update_status(status=text, media_ids=[media.media_id])
+              response = client.create_tweet(text=text, media_ids=[media.media_id])
               return response
 
         # no image
         else:          
           client = self.__get_client()
           if isThread:
               try:
@@ -258,12 +259,13 @@
                   response = client.create_tweet(text=text)
                   log.info(f'Tweet created successfully. ID: {response.data["id"]}')
                   return response
               except Exception as e:
                   log.error(f'Error creating tweet. Error: {e}')
 
 
+
 if __name__ == '__main__':
     img = '/home/drakon/Documents/DEV/projetos/easy_post_twitter/imgs/market1.png'
     tw = Twitter(with_images=True)
     status = 'B3 interbank deposit futures: today and a month ago #FuturodoCDI #mercadofinanceiro'
     tw.tweet_to_publish_with_image(text=status, imgs=img, sequential=False)
```

### Comparing `easy_post_twitter-1.0.7/PKG-INFO` & `easy_post_twitter-1.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: easy-post-twitter
-Version: 1.0.7
+Version: 1.0.8
 Summary: The easy way to send posts to twitter.
 Author: Thiago Oliveira
 Author-email: thiceconelo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
-Requires-Dist: tweepy (>=4.10.0,<5.0.0)
+Requires-Dist: tweepy (>=4.14.0,<5.0.0)
```

