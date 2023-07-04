# Comparing `tmp/quickbolt-0.1.2.tar.gz` & `tmp/quickbolt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbolt-0.1.2.tar", max compression
+gzip compressed data, was "quickbolt-0.1.3.tar", max compression
```

## Comparing `quickbolt-0.1.2.tar` & `quickbolt-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.2/LICENSE
--rw-r--r--   0        0        0     3947 2023-06-25 21:46:08.497591 quickbolt-0.1.2/README.md
--rw-r--r--   0        0        0     1238 2023-06-29 23:02:31.932187 quickbolt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.2/quickbolt/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.2/quickbolt/batch_generation/__init__.py
--rw-r--r--   0        0        0    10231 2023-06-29 16:19:50.859017 quickbolt-0.1.2/quickbolt/batch_generation/batch_generation.py
--rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.2/quickbolt/clients/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.2/quickbolt/clients/aio_requests.py
--rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.2/quickbolt/clients/httpx_requests.py
--rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.2/quickbolt/logging/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.2/quickbolt/logging/async_logger.py
--rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.2/quickbolt/pytest/__init__.py
--rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.2/quickbolt/pytest/core_pytest_base.py
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.2/quickbolt/reporting/__init__.py
--rw-r--r--   0        0        0     7244 2023-06-29 21:59:20.300359 quickbolt-0.1.2/quickbolt/reporting/response_csv.py
--rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.2/quickbolt/utils/__init__.py
--rw-r--r--   0        0        0     3859 2023-06-24 00:16:27.310243 quickbolt-0.1.2/quickbolt/utils/dictionary.py
--rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.2/quickbolt/utils/directory.py
--rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.2/quickbolt/utils/json.py
--rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.2/quickbolt/utils/sync_async.py
--rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.2/quickbolt/validations/__init__.py
--rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.2/quickbolt/validations/validations.py
--rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 quickbolt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.1.3/README.md
+-rw-r--r--   0        0        0     1238 2023-07-04 19:20:56.864321 quickbolt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.3/quickbolt/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.3/quickbolt/batch_generation/__init__.py
+-rw-r--r--   0        0        0    11241 2023-07-04 05:37:57.116510 quickbolt-0.1.3/quickbolt/batch_generation/batch_generation.py
+-rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.3/quickbolt/clients/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.3/quickbolt/clients/aio_requests.py
+-rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.3/quickbolt/clients/httpx_requests.py
+-rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.3/quickbolt/logging/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.3/quickbolt/logging/async_logger.py
+-rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.3/quickbolt/pytest/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.3/quickbolt/pytest/core_pytest_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.3/quickbolt/reporting/__init__.py
+-rw-r--r--   0        0        0     7394 2023-07-03 21:01:01.356118 quickbolt-0.1.3/quickbolt/reporting/response_csv.py
+-rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.3/quickbolt/utils/__init__.py
+-rw-r--r--   0        0        0     4266 2023-07-03 21:01:01.356324 quickbolt-0.1.3/quickbolt/utils/dictionary.py
+-rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.3/quickbolt/utils/directory.py
+-rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.3/quickbolt/utils/json.py
+-rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.3/quickbolt/utils/sync_async.py
+-rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.3/quickbolt/validations/__init__.py
+-rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.3/quickbolt/validations/validations.py
+-rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.1.3/PKG-INFO
```

### Comparing `quickbolt-0.1.2/LICENSE` & `quickbolt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/README.md` & `quickbolt-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 batch = generate_batch("get", ...)
 responses = aiohttp_requests.request(batch)
 responses = httpx_requests.request(batch)
 ```
 
 Note: Both clients have an awaitable request method called async_request e.g. **await aiohttp_requests.async_request(...)** or **await httpx_requests.async_request(...)**.
 
-Note: You can indicate where the batch generator will start looking for path parameters by placing a **semicolon (;)** where the path parameters start e.g. **https://httpbin.org/get;/param/value**.
+Note: You can indicate where the batch generator will start looking for path parameters by placing a **semicolon (;)** where the path parameters start (before a **/**) e.g. **https://httpbin.org/get;/param/value**.
 
 ### Validations
 
 After each **request**, a scrubbed copy of the csv history of the execution will be generated. This file (or the original) can be used to validate against executions over time. These files will have the same name as the running test, just with the **csv** extenstion instead. Any mismatches can be raised as errors and are reported in a separate csv. Historical csv files to be used as reference can be stored in a validations folder at the root level.
 
 ```python
 from quickbolt.validations import Validations
```

### Comparing `quickbolt-0.1.2/pyproject.toml` & `quickbolt-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbolt"
-version = "0.1.2"
+version = "0.1.3"
 description = "Asynchronously make and validate requests!"
 authors = ["Ashton Szabo <aszabo00@gmail.com>"]
 repository = "https://github.com/aszabo00/quickbolt"
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `quickbolt-0.1.2/quickbolt/batch_generation/batch_generation.py` & `quickbolt-0.1.3/quickbolt/batch_generation/batch_generation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,110 @@
 import itertools as it
 import re
-from copy import deepcopy
-from urllib.parse import urlparse
+from itertools import combinations
+from math import ceil
+from urllib.parse import parse_qs, urlencode, urlparse
 
+import quickbolt.utils.dictionary as dh
 import quickbolt.utils.json as jh
 
 
 def generate_batch(
     method: str,
-    headers: dict,
     url: str,
     description: str = "",
-    fr_pairs: None | list | list[list] = None,
-    bad_header_count: int = 1,
-    include_query_params: bool = True,
-    full: bool = False,
+    headers: None | dict = None,
     json: None | dict = None,
     data: None | dict = None,
+    bad_header_count: int = 1,
     unsafe_bodies: bool = False,
+    corrupt_query_params: bool = True,
+    min: bool = True,
+    corrupt_keys: bool = False,
 ) -> list[dict]:
     """
     This generates url batches to feed into the aio_requests.request loader.
 
     Args:
         method: The method of the request.
-        headers: The headers of the request.
         url: A 200 type url(a passing request).
         description: A description of the request.
-        fr_pairs: Forbidden swap out pairs e.g. [id, forbidden_id].
-        bad_header_count: The amount of bad header possibilities used.
-        include_query_params: Whether to include query params in the bad url generation.
-        full: Whether to generate bad values on all strings instead of strings with numbers.
+        headers: The headers of the request.
         json: A json (dict) body of the request.
         data: A data (dict) body of the request.
+        bad_header_count: The amount of bad header possibilities used.
         unsafe_bodies: Whether to include unsafe bodies in the batch.
+        corrupt_query_params: Whether to corrupt the query params.
+        min: Whether to give the minimum amount of corruptions.
+        corrupt_keys: Whether to corrupt the keys of a data set.
 
     Returns:
-        batch: The list of 200-500 url combinations.
+        batch: The list of 200-500 request corruptions.
     """
     method = method.lower()
     good_code = {
         "get": "200",
         "patch": "200",
         "post": "201",
         "put": "204",
         "delete": "204",
     }[method]
 
-    bad_headers = generate_bad_bodies(headers, "0", original_keys=True)[
-        :bad_header_count
-    ]
-
-    invalid_urls = generate_bad_urls(
-        url, "999", include_query_params=include_query_params, full=full
-    )
-    forbidden_urls = generate_bad_urls(
-        url, replacements=fr_pairs, include_query_params=include_query_params, full=full
-    )
+    invalid_sub_values = {"str": "aaa", "digit": "999"}
+    bad_headers = generate_bad_bodies(headers, min=min)[:bad_header_count]
+    invalid_urls = generate_bad_urls(url, invalid_sub_values, corrupt_query_params, min)
     not_found_urls = generate_bad_urls(
-        url, "0", include_query_params=include_query_params, full=full
+        url, corrupt_query_params=corrupt_query_params, min=min
     )
 
     clean_url = url.replace(";", "")
     if description:
         description += " "
 
     batch = [
-        [
+        *[
             {
                 "code": good_code,
                 "description": f"{description}good",
                 "method": method,
                 "headers": headers,
                 "url": clean_url,
             }
         ],
-        [
+        *[
             {
                 "code": "400",
                 "description": f"{description}invalid",
                 "method": method,
                 "headers": headers,
                 "url": u,
             }
             for u in invalid_urls
         ],
-        [
+        *[
             {
                 "code": "401",
                 "description": f"{description}not auth",
                 "method": method,
                 "headers": h,
                 "url": clean_url,
             }
             for h in bad_headers
         ],
-        [
-            {
-                "code": "403",
-                "description": f"{description}forbidden",
-                "method": method,
-                "headers": headers,
-                "url": u,
-            }
-            for u in forbidden_urls
-        ],
-        [
+        *[
             {
                 "code": "404",
                 "description": f"{description}not found",
                 "method": method,
                 "headers": headers,
                 "url": u,
             }
             for u in not_found_urls
         ],
     ]
-    batch = [i for b in batch for i in b]
 
     if json or data:
         body = json
         key = "json"
         if data:
             body = data
             key = "data"
@@ -132,188 +116,239 @@
             "code": good_code,
             "description": f"{description}good",
             "method": method,
             "headers": headers,
             "url": clean_url,
         }
 
-        extra_batch = [
-            {
-                **good_batch,
-                **{key: b, "description": f"{description}invalid"},
-                "code": "400",
-            }
-            for b in generate_bad_bodies(body, "999")
-        ]
-        batch.extend(extra_batch)
-
-        extra_batch = [
-            {
-                **good_batch,
-                **{key: b, "description": f"{description}not found"},
-                "code": "404",
-            }
-            for b in generate_bad_bodies(body, "0")
+        bad_bodies_batch = [
+            *[
+                {
+                    **good_batch,
+                    **{key: b, "description": f"{description}invalid"},
+                    "code": "400",
+                }
+                for b in generate_bad_bodies(
+                    body, invalid_sub_values, min=min, corrupt_keys=corrupt_keys
+                )
+            ],
+            *[
+                {
+                    **good_batch,
+                    **{key: b, "description": f"{description}not found"},
+                    "code": "404",
+                }
+                for b in generate_bad_bodies(body, min=min, corrupt_keys=corrupt_keys)
+            ],
         ]
-        batch.extend(extra_batch)
 
         if unsafe_bodies:
             extra_batch = [
                 {
                     **good_batch,
                     **{key: b, "description": f"{description}unsafe bodies"},
                     "code": "???",
                 }
                 for b in generate_unsafe_bodies(body)
             ]
-            batch.extend(extra_batch)
+            bad_bodies_batch.extend(extra_batch)
+
+        batch.extend(bad_bodies_batch)
+        batch.sort(key=lambda k: k["code"].split("|")[0])
 
-    return [batch[0]] + sorted(batch[1:], key=lambda k: k["code"].split("|")[0])
+    return batch
 
 
 def generate_bad_urls(
-    data: str,
-    sub_value: None | str = None,
-    replacements: None | list | list[list] = None,
-    include_query_params: bool = True,
-    full: bool = False,
+    url: str,
+    sub_values: None | dict = None,
+    corrupt_query_params: bool = True,
+    min: bool = True,
 ) -> list:
     """
     This generates a list of bad urls e.g. path params and query params.
 
     Args:
         data: A 200 type url.
-        sub_value: A numerical substitute value for invalidating(i.e. '999')
-                   or converting to not found(i.e. '0').
-        replacements: Forbidden swap out pairs e.g. [id, forbidden_id].
-        include_query_params: Whether to include bad generations of query params.
-        full: Whether to generate bad values on all strings instead of strings with numbers.
+        sub_values: Regex type substitutes for char type replacements.
+        corrupt_query_params: Whether to corrupt the query params.
+        min: Whether to give the minimum amount of corruptions.
 
     Returns:
-        bad_datas: The list of bad datas for the request.
+        bad_urls: The list of bad urls for the request.
     """
-    if not sub_value and not replacements:
-        return []
-
-    _data = data[:]
-    parsed = urlparse(_data)
-    _data = _data.replace(";", "")
+    parsed = urlparse(url)
 
     query = parsed.query
-    if not include_query_params:
-        query = ""
+    query_dict = {"query": parse_qs(query) or ""}
 
+    marked_url = url
     path = parsed.path
     if ";" not in parsed.path:
-        path = f";{path}"
+        marked_path = f";{path}"
+        marked_url = marked_url.replace(path, marked_path)
+        path = marked_path
+
+    _, params = path.split(";")
+    params_split = params.lstrip("/").split("/")
+
+    corruptables = {"params": dict(zip(params_split, params_split))}
+    if corrupt_query_params:
+        corruptables.update(query_dict)
+    corruptables = dh.flatten(corruptables)
+    corruptables_ser = jh.serialize(corruptables)
 
-    path, params = path.split(";")
-    params += "/" + re.sub(r"[?=&]", "/", query)
+    bad_combos_des = generate_bad_data(corruptables_ser, corruptables, sub_values, min)
+    bad_combos_unfl = [dh.unflatten(b) for b in bad_combos_des]
 
-    return generate_bad_data(sub_value, replacements, full, _data, params)
+    bad_urls = []
+    clean_url = url.replace(";", "")
+    base_url = marked_url.split(";")[0].lstrip("/").rstrip("/")
+    for bad_combo in bad_combos_unfl:
+        query = bad_combo.get("query", "") or query_dict.get("query", "")
+        if query:
+            query = urlencode(query, doseq=True)
+            query = f"?{query}"
+
+        params = bad_combo.get("params", "")
+        if params:
+            params = "/".join(params.values()).rstrip("/")
+
+        bad_url = f"{base_url}/{params + query}"
+        if bad_url != clean_url:
+            bad_urls.append(bad_url)
+
+    return list(dict.fromkeys(bad_urls))
 
 
 def generate_bad_bodies(
     data: dict,
-    sub_value: None | str = None,
-    replacements: None | list | list[list] = None,
-    full: bool = False,
-    original_keys: bool = False,
-) -> list:
+    sub_values: None | dict = None,
+    min: bool = True,
+    corrupt_keys: bool = False,
+) -> list[dict]:
     """
     This generates a list of bad bodies.
 
     Args:
         data: A 200 type body.
-        sub_value: A numerical substitute value for invalidating(i.e. '999')
-                   or converting to not found(i.e. '0').
-        replacements: Forbidden swap out pairs e.g. [id, forbidden_id].
-        full: Whether to generate bad values on all strings instead of strings with numbers.
-        original_keys: Whether to keep the bad bodies with their original keys.
+        sub_values: Regex type substitutes for char type replacements.
+        min: Whether to give the minimum amount of corruptions.
+        corrupt_keys: Whether to corrupt the keys of a data set.
 
     Returns:
-        bad_data: The list of bad datas for the request.
+        bad_data: The unflattened list of bad data for the request.
     """
-    if not sub_value and not replacements:
-        return []
-
-    _data = deepcopy(data)
-    incorruptible_data = {}
-    for key, value in data.items():
-        if "file" in key or not isinstance(value, (int, float, str, dict)):
-            incorruptible_data[key] = _data.pop(key)
-
-    _data = jh.serialize(_data)
-    params = "/".join(f"{k}/{v}" for k, v in data.items())
+    data_copy_flat = dh.flatten(data)
 
-    bad_data = generate_bad_data(sub_value, replacements, full, _data, params)
-    bad_data = [jh.deserialize(b) for b in bad_data]
+    corruptables = {}
+    incorruptibles = {}
+    for key, value in data_copy_flat.items():
+        if "file" in key or not isinstance(value, (int, float, str)):
+            incorruptibles[key] = value
+        else:
+            corruptables[key] = value
+    data_copy_flat_ser = jh.serialize(corruptables)
 
-    if original_keys:
-        original_keys_set = set(data.keys())
-        bad_data = [b for b in bad_data if original_keys_set.issuperset(b)]
+    bad_combos_des = generate_bad_data(
+        data_copy_flat_ser, corruptables, sub_values, min, corrupt_keys
+    )
 
-    for b in bad_data:
-        b.update(incorruptible_data)
+    if incorruptibles:
+        for bad_combo in bad_combos_des:
+            bad_combo.update(incorruptibles)
+
+    bad_combos_unfl = [dh.unflatten(b) for b in bad_combos_des]
+
+    seen = []
+    unique_dicts = []
+    for bad_combo in bad_combos_unfl:
+        t = tuple(bad_combo.items())
+        if t not in seen:
+            unique_dicts.append(bad_combo)
+            seen.append(t)
 
-    return bad_data
+    return unique_dicts
 
 
 def generate_bad_data(
-    sub_value: str, replacements: list | list[list], full: bool, data: str, params: str
-):
+    data_flat_ser: str,
+    corruptables: dict,
+    sub_values: dict,
+    min: bool = True,
+    corrupt_keys: bool = False,
+) -> list[dict]:
     """
-    This generates a list of bad data.
+    This creates the corrupted combinations.
 
     Args:
-        sub_value: A numerical substitute value for invalidating(i.e. '999')
-                   or converting to not found(i.e. '0').
-        replacements: Forbidden swap out pairs e.g. [id, forbidden_id].
-        full: Whether to generate bad values on all strings instead of strings with numbers.
-        data: The original 200 type data object (str url or json).
-        params: The parameters to corrupt.
+        data_flat_ser: A flat, serialized version of the data being corrupted.
+        corruptables: The values to target for corruption.
+        sub_values: Regex type substitutes for char type replacements.
+        min: Whether to give the minimum amount of corruptions.
+        corrupt_keys: Whether to corrupt the keys of a data set.
 
     Returns:
-        bad_datas: The list of bad datas for the request.
+        bad_combos_des: The list of deserialized bad data for the request.
     """
 
-    if sub_value:
-        replacements = [
-            [p, re.sub(r"[a-zA-Z]", "a", re.sub(r"\d", sub_value, p))]
-            for p in params.split("/")
-            if full or re.findall(r"\d+", p)
-        ]
-        if not replacements:
-            return []
-    elif replacements and not isinstance(replacements[0], list):
-        replacements = [replacements]
-
-    # restricts the generated combinations
-    num_combinations = len(set([r[0] for r in replacements]))
-    combinations = [
-        c
-        for c in it.combinations(replacements, num_combinations)
-        if len(set([i[0] for i in c])) > num_combinations - 1
-    ]
-
-    bad_datas = []
-    for comb in combinations:
-        bad_data = data.rstrip("/")
-        for c in comb:
-            bad_data = bad_data.replace(c[0], c[1])
-            if sub_value:
-                _bad_data = data.rstrip("/")
-                _bad_data = re.sub(rf"\b{c[0]}\b", c[1], _bad_data)
-                if _bad_data != data and _bad_data not in bad_datas:
-                    bad_datas.append(_bad_data)
+    def corruption_regex(value_str, active_sub_values):
+        corrupt_value = value_str
 
-        if bad_data not in bad_datas:
-            bad_datas.append(bad_data)
+        str_sub = active_sub_values.get("str")
+        if str_sub:
+            corrupt_value = re.sub(r"[a-zA-Z]", str_sub, corrupt_value)
+
+        digit_sub = active_sub_values.get("digit")
+        if digit_sub:
+            corrupt_value = re.sub(r"\d", digit_sub, corrupt_value)
+
+        return corrupt_value
+
+    active_sub_values = {"str": "a", "digit": "0"}
+    if isinstance(sub_values, dict):
+        active_sub_values.update(sub_values)
+
+    num_of_combos = 1
+    if not min:
+        num_of_combos = ceil(len(corruptables) / 3)
+
+    combos = list(combinations(corruptables.items(), num_of_combos))
+    combos.append(tuple(corruptables.items()))
+
+    bad_combos = []
+    for combo in combos:
+        bad_combo_value = data_flat_ser
+        bad_combo_key = data_flat_ser
+
+        for key, value in combo:
+            key_str = f'"{key}"'
+
+            if isinstance(value, str):
+                value_str = f'"{value}"'
+            else:
+                value_str = str(value)
+
+            corrupt_value = corruption_regex(value_str, active_sub_values)
+            bad_combo_value = bad_combo_value.replace(
+                f"{key_str}: {value_str}", f"{key_str}: {corrupt_value}"
+            )
+
+            corrupt_key = None
+            if corrupt_keys and len(corruptables) != len(combo):
+                corrupt_key = corruption_regex(key_str, {"str": "a"})
+                bad_combo_key = bad_combo_key.replace(
+                    f"{key_str}: {value_str}", f"{corrupt_key}: {value_str}"
+                )
+
+        bad_combos.append(bad_combo_value)
+        if corrupt_keys and corrupt_key:
+            bad_combos.append(bad_combo_key)
 
-    return bad_datas
+    return [jh.deserialize(b) for b in bad_combos]
 
 
 def generate_unsafe_bodies(body: dict) -> list[dict]:
     """
     This creates an unsafe body from a good one.
 
     Args:
```

### Comparing `quickbolt-0.1.2/quickbolt/clients/aio_requests.py` & `quickbolt-0.1.3/quickbolt/clients/aio_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/quickbolt/clients/httpx_requests.py` & `quickbolt-0.1.3/quickbolt/clients/httpx_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/quickbolt/logging/async_logger.py` & `quickbolt-0.1.3/quickbolt/logging/async_logger.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/quickbolt/pytest/core_pytest_base.py` & `quickbolt-0.1.3/quickbolt/pytest/core_pytest_base.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/quickbolt/reporting/response_csv.py` & `quickbolt-0.1.3/quickbolt/reporting/response_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,28 +130,32 @@
     """
     responses = _return["responses"]
 
     for r in responses:
         r["server_headers"] = {k: v for k, v in r["server_headers"].items()}
 
         kwargs = r.get("kwargs", {})
-        r["body"] = kwargs.pop("message", {}) or kwargs.pop("data", {})
+        r["body"] = kwargs.pop("json", {}) or kwargs.pop("data", {})
         if "FormData" in str(type(r["body"])):
             r["body"] = {f[0]["name"]: f[2] for f in r["body"]._fields}
         elif isinstance(r["body"], dict):
             update = {
                 k: v.name
                 for k, v in r["body"].items()
                 if "BufferedReader" in str(type(v))
             }
             r["body"].update(update)
 
         r["response_seconds"] = r.pop("response_seconds")
         r["delay_seconds"] = r.pop("delay_seconds")
 
+        for key, value in kwargs.items():
+            if not isinstance(value, (str, int, float, list, dict)):
+                kwargs[key] = str(value)
+
     col_titles = [""]
     if not await aos.path.exists(csv_path):
         col_titles = [[key.upper() for key in responses[0].keys()]]
 
     csv_data = col_titles + [list(r.values()) for r in responses]
     await add_rows_to_csv_report(csv_path, csv_data)
```

### Comparing `quickbolt-0.1.2/quickbolt/utils/dictionary.py` & `quickbolt-0.1.3/quickbolt/utils/dictionary.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,48 +23,56 @@
             obj[parent_key] = value
 
     obj = {}
     recurse(d)
     return obj
 
 
-def unflatten(d: dict | list) -> dict:
+def unflatten(flat_dict: dict) -> dict | list:
     """
     This unflattens a flattened dictionary.
 
     Args:
-        d: The object to flatten.
+        flat_dict: The flat dictionary to unflatten.
 
     Returns:
-        items: The unflattened object.
+        unflattened_dict: The unflattened dict.
     """
-    items = {}
-    for k, v in d.items():
-        keys = k.split(".")
-        sub_items = items
-
-        index = None
-        if keys[-1].isdigit():
-            index = int(keys[-1])
-        list_action = isinstance(index, int)
-
-        for ki in keys[:-1]:
-            try:
-                sub_items = sub_items[ki]
-            except KeyError:
-                if list_action:
-                    sub_items[ki] = []
-                else:
-                    sub_items[ki] = {}
-                sub_items = sub_items[ki]
-        if list_action:
-            sub_items.insert(index, v)
+    unflattened_dict = {}
+
+    def assign(keys, value, d):
+        key = keys.pop(0)
+        if len(keys) == 0:
+            if key.isdigit():
+                while len(d) <= int(key):
+                    d.append(None)
+                d[int(key)] = value
+            else:
+                d[key] = value
         else:
-            sub_items[keys[-1]] = v
-    return items
+            if key.isdigit():
+                if int(key) < len(d):
+                    assign(keys, value, d[int(key)])
+                else:
+                    while len(d) < int(key):
+                        d.append({})
+                    d.append({})
+                    assign(keys, value, d[int(key)])
+            else:
+                if key in d.keys():
+                    assign(keys, value, d[key])
+                else:
+                    d[key] = [{}] if keys[0].isdigit() else {}
+                    assign(keys, value, d[key])
+
+    for flat_key, value in flat_dict.items():
+        keys = flat_key.split(".")
+        assign(keys, value, unflattened_dict)
+
+    return unflattened_dict
 
 
 def compare_dictionaries(
     d1: dict,
     d2: dict,
     skipped_keys: None | list = None,
     exclusive_keys: None | list = None,
```

### Comparing `quickbolt-0.1.2/quickbolt/utils/directory.py` & `quickbolt-0.1.3/quickbolt/utils/directory.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/quickbolt/utils/json.py` & `quickbolt-0.1.3/quickbolt/utils/json.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/quickbolt/validations/validations.py` & `quickbolt-0.1.3/quickbolt/validations/validations.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.2/PKG-INFO` & `quickbolt-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbolt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronously make and validate requests!
 Home-page: https://github.com/aszabo00/quickbolt
 License: MIT
 Author: Ashton Szabo
 Author-email: aszabo00@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
@@ -78,15 +78,15 @@
 batch = generate_batch("get", ...)
 responses = aiohttp_requests.request(batch)
 responses = httpx_requests.request(batch)
 ```
 
 Note: Both clients have an awaitable request method called async_request e.g. **await aiohttp_requests.async_request(...)** or **await httpx_requests.async_request(...)**.
 
-Note: You can indicate where the batch generator will start looking for path parameters by placing a **semicolon (;)** where the path parameters start e.g. **https://httpbin.org/get;/param/value**.
+Note: You can indicate where the batch generator will start looking for path parameters by placing a **semicolon (;)** where the path parameters start (before a **/**) e.g. **https://httpbin.org/get;/param/value**.
 
 ### Validations
 
 After each **request**, a scrubbed copy of the csv history of the execution will be generated. This file (or the original) can be used to validate against executions over time. These files will have the same name as the running test, just with the **csv** extenstion instead. Any mismatches can be raised as errors and are reported in a separate csv. Historical csv files to be used as reference can be stored in a validations folder at the root level.
 
 ```python
 from quickbolt.validations import Validations
```

