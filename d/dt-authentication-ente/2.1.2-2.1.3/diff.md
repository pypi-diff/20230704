# Comparing `tmp/dt-authentication-ente-2.1.2.tar.gz` & `tmp/dt-authentication-ente-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-authentication-ente-2.1.2.tar", last modified: Wed Jun  7 13:37:21 2023, max compression
+gzip compressed data, was "dt-authentication-ente-2.1.3.tar", last modified: Tue Jul  4 04:22:53 2023, max compression
```

## Comparing `dt-authentication-ente-2.1.2.tar` & `dt-authentication-ente-2.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.2/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.2/README.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2374 2023-05-23 13:18:48.000000 dt-authentication-ente-2.1.2/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.204474 dt-authentication-ente-2.1.2/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/src/dt_authentication/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-06-07 13:37:19.000000 dt-authentication-ente-2.1.2/src/dt_authentication/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3659 2023-05-30 05:44:24.000000 dt-authentication-ente-2.1.2/src/dt_authentication/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      741 2023-06-07 13:33:39.000000 dt-authentication-ente-2.1.2/src/dt_authentication/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.2/src/dt_authentication/scope.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13453 2023-06-07 13:35:36.000000 dt-authentication-ente-2.1.2/src/dt_authentication/token.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-22 20:52:39.000000 dt-authentication-ente-2.1.2/src/dt_authentication/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-04 04:22:53.491299 dt-authentication-ente-2.1.3/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.3/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-07-04 04:22:53.491299 dt-authentication-ente-2.1.3/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.3/README.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-07-04 04:22:53.491299 dt-authentication-ente-2.1.3/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2374 2023-05-23 13:18:48.000000 dt-authentication-ente-2.1.3/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-04 04:22:53.487299 dt-authentication-ente-2.1.3/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-04 04:22:53.491299 dt-authentication-ente-2.1.3/src/dt_authentication/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-07-04 04:22:46.000000 dt-authentication-ente-2.1.3/src/dt_authentication/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3980 2023-07-04 04:18:11.000000 dt-authentication-ente-2.1.3/src/dt_authentication/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      741 2023-06-07 13:33:39.000000 dt-authentication-ente-2.1.3/src/dt_authentication/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.3/src/dt_authentication/scope.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13504 2023-07-04 04:21:13.000000 dt-authentication-ente-2.1.3/src/dt_authentication/token.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-22 20:52:39.000000 dt-authentication-ente-2.1.3/src/dt_authentication/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-04 04:22:53.491299 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-07-04 04:22:53.000000 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-07-04 04:22:53.000000 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-07-04 04:22:53.000000 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2023-07-04 04:22:53.000000 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-07-04 04:22:53.000000 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-07-04 04:22:53.000000 dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/top_level.txt
```

### Comparing `dt-authentication-ente-2.1.2/setup.py` & `dt-authentication-ente-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.2/src/dt_authentication/cli.py` & `dt-authentication-ente-2.1.3/src/dt_authentication/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,16 @@
             token_s = args[0]
         else:
             msg = "Please enter token:\n> "
             token_s = builtins.input(msg)
 
         try:
             token = DuckietownToken.from_string(token_s)
-        except InvalidToken:
-            msg = "Invalid token format."
+        except InvalidToken as e:
+            msg = f"Invalid token: {e.args[0]}"
             logger.error(msg)
             sys.exit(1)
 
         _print_token_info(token)
         sys.exit(0)
     except Exception as e:
         logger.error(str(e))
@@ -48,38 +48,45 @@
     parser.add_argument("--uid", type=int, help="ID to sign")
     parser.add_argument("--key", type=str, help="Path to signing key")
     parser.add_argument("--ndays", type=int, default=0, help="Number of days for validity")
     parser.add_argument("--nhours", type=int, default=0, help="Number of hours for validity")
     parser.add_argument("--nminutes", type=int, default=0, help="Number of minutes for validity")
     parser.add_argument("--renewable", action="store_true", default=False, help="Make a renewable token")
     parser.add_argument("--scope", type=str, default=None, help="Scope as compact comma-separated list")
+    parser.add_argument("--version", type=str, default=None, help="Version of the token to generate")
 
     args = parser.parse_args(args=args)
 
     if args.key is None:
         msg = "Please supply --key "
         raise Exception(msg)
     if args.uid is None:
         msg = "Please supply --uid "
         raise Exception(msg)
 
+    # make sure the requested version is supported
+    if args.version not in [None, "dt1", "dt2"]:
+        msg = f"Token version '{args.version}' not recognized."
+        raise Exception(msg)
+
     # load private key
     with open(args.key, "r") as _:
         pem = _.read()
     sk = SigningKey.from_pem(pem)
 
     # generate token
     token: DuckietownToken = DuckietownToken.generate(
         key=sk,
         user_id=args.uid,
         days=args.ndays,
         hours=args.nhours,
         minutes=args.nminutes,
         scope=args.scope.split(",") if args.scope else None,
-        renewable=args.renewable
+        renewable=args.renewable,
+        version=args.version
     )
     _print_token_info(token)
 
 
 def cli_keygen(args=None):
     parser = argparse.ArgumentParser()
     parser.add_argument("--version", type=str, default="dt2", help="Version of the token")
@@ -112,15 +119,15 @@
 
 def _print_token_info(token: DuckietownToken):
     exp_info: str = "expired" if token.expired else \
         f"in {token.expiration and (token.expiration - datetime.datetime.utcnow()).days} days"
     print(f"""
 Payload:
 --------
-{token.payload_as_json(sort_keys=True, indent=4).strip("{}")}
+{token.payload_as_json(indent=4).strip("{}")}
 
 Expiration:
 --------\n
     Expired: {'Yes' if token.expired else 'No'}
     {token.expiration}    -    ({exp_info})
 
 Token:
```

### Comparing `dt-authentication-ente-2.1.2/src/dt_authentication/exceptions.py` & `dt-authentication-ente-2.1.3/src/dt_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.2/src/dt_authentication/scope.py` & `dt-authentication-ente-2.1.3/src/dt_authentication/scope.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.2/src/dt_authentication/token.py` & `dt-authentication-ente-2.1.3/src/dt_authentication/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         return self._payload['uid']
 
     @property
     def scope(self) -> List[Scope]:
         """
         The scope of this token.
         """
-        return self._payload.get("scope", DEFAULT_SCOPE)
+        scope = self._payload.get("scope", DEFAULT_SCOPE)
+        return [(s if isinstance(s, Scope) else Scope.parse(s)) for s in scope]
 
     @property
     def data(self) -> Optional[dict]:
         """
         The data baked into the token.
         """
         return self._payload.get("data", None)
@@ -159,19 +160,21 @@
         # compile token
         return f"{self._version}-{payload_base58}-{signature_base58}"
 
     def payload_as_json(self, sort_keys: bool = True, **kwargs) -> str:
         """
         The token's payload as JSON string.
         """
-        # encode scope
+        # get a copy of the payload dictionary
+        payload = copy.deepcopy(self._payload)
+        # replace parsed scope
         scope: List[Union[str, dict]] = [s.compact() for s in self.scope]
+        if "scope" in SUPPORTED_FIELDS[self.version]:
+            payload["scope"] = scope
         # encode payload into JSON
-        payload = copy.deepcopy(self._payload)
-        payload["scope"] = scope
         return json.dumps(payload, sort_keys=sort_keys, **kwargs)
 
     def grants(self, action: str, resource: Optional[str] = None, identifier: Optional[str] = None,
                service: Optional[str] = None) -> bool:
         """
         Checks whether this token grants the given scope.
 
@@ -372,13 +375,8 @@
             e = b"duckietown is a place of relaxed introspection, and hub extends this place a lot"
             return e[:numbytes]
 
         # compile payload
         payload_bytes = str.encode(json.dumps(payload, sort_keys=True))
         signature = key.sign(payload_bytes, entropy=entropy)
 
-        # - scope
-        if "scope" in fields:
-            # noinspection PyUnboundLocalVariable
-            payload["scope"] = scope_parsed
-
         return DuckietownToken(version, payload, signature)
```

### Comparing `dt-authentication-ente-2.1.2/src/dt_authentication/utils.py` & `dt-authentication-ente-2.1.3/src/dt_authentication/utils.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/SOURCES.txt` & `dt-authentication-ente-2.1.3/src/dt_authentication_ente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

