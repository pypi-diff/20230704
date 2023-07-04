# Comparing `tmp/pheme-21.4rc4.tar.gz` & `tmp/pheme-21.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheme-21.4rc4.tar", max compression
+gzip compressed data, was "pheme-21.5.0.tar", max compression
```

## Comparing `pheme-21.4rc4.tar` & `pheme-21.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2021-03-02 07:35:44.543759 pheme-21.4rc4/LICENSE
--rw-r--r--   0        0        0     3549 2021-03-02 07:35:44.543759 pheme-21.4rc4/README.md
--rw-r--r--   0        0        0      832 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/__init__.py
--rw-r--r--   0        0        0     3273 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/authentication.py
--rw-r--r--   0        0        0      950 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/datalink.py
--rw-r--r--   0        0        0      884 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/errors.py
--rw-r--r--   0        0        0     5152 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/parameter.py
--rw-r--r--   0        0        0      805 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/parser/__init__.py
--rw-r--r--   0        0        0     1833 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/parser/xml.py
--rw-r--r--   0        0        0     4193 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/renderer.py
--rw-r--r--   0        0        0     6087 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/settings.py
--rw-r--r--   0        0        0     1515 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/storage.py
--rw-r--r--   0        0        0      811 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/templatetags/__init__.py
--rw-r--r--   0        0        0     2896 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/templatetags/charts/__init__.py
--rw-r--r--   0        0        0     6760 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/templatetags/charts/h_bar.py
--rw-r--r--   0        0        0     4558 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/templatetags/charts/pie.py
--rw-r--r--   0        0        0     9928 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/templatetags/charts/treemap.py
--rw-r--r--   0        0        0     1714 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/templatetags/dynamic_template.py
--rw-r--r--   0        0        0      838 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/transformation/__init__.py
--rw-r--r--   0        0        0      853 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/transformation/scanreport/__init__.py
--rw-r--r--   0        0        0     8674 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/transformation/scanreport/gvmd.py
--rw-r--r--   0        0        0     5424 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/transformation/scanreport/model.py
--rw-r--r--   0        0        0     7536 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/transformation/scanreport/renderer.py
--rw-r--r--   0        0        0     2411 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/urls.py
--rw-r--r--   0        0        0      843 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/version/__init__.py
--rw-r--r--   0        0        0      104 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/version/__version__.py
--rw-r--r--   0        0        0     4533 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/views.py
--rw-r--r--   0        0        0     1181 2021-03-02 07:35:44.543759 pheme-21.4rc4/pheme/wsgi.py
--rw-r--r--   0        0        0     1793 2021-03-02 07:35:44.547759 pheme-21.4rc4/pyproject.toml
--rw-r--r--   0        0        0     4652 2021-03-02 07:36:02.907373 pheme-21.4rc4/setup.py
--rw-r--r--   0        0        0     4644 2021-03-02 07:36:02.907785 pheme-21.4rc4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-04 06:42:13.068205 pheme-21.5.0/LICENSE
+-rw-r--r--   0        0        0     3978 2023-07-04 06:42:13.068205 pheme-21.5.0/README.md
+-rw-r--r--   0        0        0      821 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/__init__.py
+-rw-r--r--   0        0        0     3263 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/authentication.py
+-rw-r--r--   0        0        0      929 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/datalink.py
+-rw-r--r--   0        0        0      873 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/errors.py
+-rw-r--r--   0        0        0     5048 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/parameter.py
+-rw-r--r--   0        0        0      794 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/parser/__init__.py
+-rw-r--r--   0        0        0     1822 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/parser/xml.py
+-rw-r--r--   0        0        0     4004 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/renderer.py
+-rw-r--r--   0        0        0     6780 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/settings.py
+-rw-r--r--   0        0        0     1495 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/storage.py
+-rw-r--r--   0        0        0      800 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/__init__.py
+-rw-r--r--   0        0        0     2888 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/charts/__init__.py
+-rw-r--r--   0        0        0     8041 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/charts/h_bar.py
+-rw-r--r--   0        0        0     4559 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/charts/pie.py
+-rw-r--r--   0        0        0     9920 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/charts/treemap.py
+-rw-r--r--   0        0        0     1703 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/dynamic_template.py
+-rw-r--r--   0        0        0     1643 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/templatetags/readable_timeformat.py
+-rw-r--r--   0        0        0      827 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/transformation/__init__.py
+-rw-r--r--   0        0        0      842 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/transformation/scanreport/__init__.py
+-rw-r--r--   0        0        0     8658 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/transformation/scanreport/gvmd.py
+-rw-r--r--   0        0        0     5356 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/transformation/scanreport/model.py
+-rw-r--r--   0        0        0     8911 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/transformation/scanreport/renderer.py
+-rw-r--r--   0        0        0     2369 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/urls.py
+-rw-r--r--   0        0        0      832 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/version/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/version/__version__.py
+-rw-r--r--   0        0        0     4443 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/views.py
+-rw-r--r--   0        0        0     1170 2023-07-04 06:42:13.068205 pheme-21.5.0/pheme/wsgi.py
+-rw-r--r--   0        0        0     1873 2023-07-04 06:42:13.072205 pheme-21.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5251 1970-01-01 00:00:00.000000 pheme-21.5.0/PKG-INFO
```

### Comparing `pheme-21.4rc4/LICENSE` & `pheme-21.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pheme-21.4rc4/README.md` & `pheme-21.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_logo_resilience_horizontal.png)
+![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # Pheme - Greenbone Static Report Generator <!-- omit in toc -->
 
+[![GitHub releases](https://img.shields.io/github/release-pre/greenbone/pheme.svg)](https://github.com/greenbone/pheme/releases)
+ [![PyPI release](https://img.shields.io/pypi/v/pheme.svg)](https://pypi.org/project/pheme/)
+ [![code test coverage](https://codecov.io/gh/greenbone/pheme/branch/main/graph/badge.svg)](https://codecov.io/gh/greenbone/pheme)
+ [![CircleCI](https://circleci.com/gh/greenbone/pheme/tree/main.svg?style=svg)](https://circleci.com/gh/greenbone/pheme/tree/main)
+ [![Build and test](https://github.com/greenbone/pheme/actions/workflows/ci-python.yml/badge.svg)](https://github.com/greenbone/pheme/actions/workflows/ci-python.yml)
+
 **pheme** is a service to create scan reports. It is maintained by [Greenbone Networks].
 
 [Pheme](https://en.wikipedia.org/wiki/Pheme) is the personification of fame and renown.
 
 Or in this case personification of a service to generate reports.
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Installation](#installation)
   - [Requirements](#requirements)
 - [Development](#development)
-- [API overview](#api-overview)
 - [Maintainer](#maintainer)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Installation
 
 ### Requirements
@@ -53,24 +58,14 @@
 
     poetry run autohooks activate
 
 Validate the activated git hooks by running
 
     poetry run autohooks check
 
-## API overview
-
-To get an overview of the API you can start this project
-
-```
-poetry run python manage.py runserver
-```
-
-and then go to [swagger](http://localhost:8000/docs/)
-
 ## Usage
 
 In order to prepare the data structure the XML report data needs to be posted to `pheme` with a grouping indicator (either by host or nvt).
 
 E.g.:
 
 ```
@@ -113,26 +108,26 @@
 
 ```
 > curl -v 'http://localhost:8000/report/scanreport-nvt-9a233b0d-713c-4f22-9e15-f6e5090873e3' -H 'Accept: application/pdf'
 ```
 
 ## Maintainer
 
-This project is maintained by [Greenbone Networks GmbH][Greenbone Networks]
+This project is maintained by [Greenbone AG][Greenbone Networks]
 
 ## Contributing
 
 Your contributions are highly appreciated. Please
 [create a pull request](https://github.com/greenbone/pheme/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/pheme/issues)
 first.
 
 ## License
 
-Copyright (C) 2020 [Greenbone Networks GmbH][Greenbone Networks]
+Copyright (C) 2020-2022 [Greenbone AG][Greenbone Networks]
 
 Licensed under the [GNU Affero General Public License v3.0 or later](LICENSE).
 
 [Greenbone Networks]: https://www.greenbone.net/
 [poetry]: https://python-poetry.org/
 [autohooks]: https://github.com/greenbone/autohooks
```

### Comparing `pheme-21.4rc4/pheme/__init__.py` & `pheme-21.5.0/pheme/version/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# pheme/__init__.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# pheme/version/__init__.py
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -12,9 +12,8 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from .version import __version__
+from .__version__ import __version__
```

### Comparing `pheme-21.4rc4/pheme/authentication.py` & `pheme-21.5.0/pheme/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -50,15 +50,15 @@
     return resp.get("login"), resp.get("role")
 
 
 def get_username_role(
     request: HttpRequest,
     *,
     gsad_url: str = settings.GSAD_URL,
-    get: Callable = requests.get
+    get: Callable = requests.get,
 ) -> Tuple[Union[str, None], Union[str, None]]:
     """
     returns a username and a role when it got found based on the request.
 
     So far only gsad is supported.
     Parameter:
         request: HttpRequest, the incoming request is used to get information
```

### Comparing `pheme-21.4rc4/pheme/datalink.py` & `pheme-21.5.0/pheme/templatetags/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# pheme/templatetags/__init__.py
+# Copyright (C) 2020-2021 Greenbone AG
 #
-# SPDX-License-Identifier: GPL-3.0-or-later
+# SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# GNU Affero General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import urllib
-import base64
-
-
-def as_datalink(data: bytes, file_format: str) -> str:
-    img = urllib.parse.quote(base64.b64encode(data))
-    return 'data:{};base64,{}'.format(file_format, img)
```

### Comparing `pheme-21.4rc4/pheme/errors.py` & `pheme-21.5.0/pheme/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `pheme-21.4rc4/pheme/parameter.py` & `pheme-21.5.0/pheme/parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -42,15 +42,15 @@
     """
     either loads json file from given_path or returns an empty dict when file
     does not exist.
 
     """
     param_file_obj = Path(from_path)
     return (
-        json.loads(param_file_obj.read_text())
+        json.loads(param_file_obj.read_text(encoding="utf-8"))
         if param_file_obj.exists()
         else {}
     )
 
 
 def load_params(
     system_parameter_path: str = settings.PARAMETER_FILE_ADDRESS,
@@ -66,107 +66,91 @@
     return {
         **__load_params(default_parameter_path),
         **__load_params(system_parameter_path),
     }
 
 
 def __store(params: Dict, *, from_path: str = None) -> Dict:
-    Path(from_path).write_text(json.dumps(params))
+    Path(from_path).write_text(json.dumps(params), encoding="utf-8")
     return params
 
 
 def __put(
     request: HttpRequest,
     func: Callable[[HttpRequest, Dict], Dict],
     *,
     from_path: str = settings.PARAMETER_FILE_ADDRESS,
-    store: Callable[[Dict, str], Dict] = __store
+    store: Callable[[Dict, str], Dict] = __store,
 ) -> Response:
     params = __load_params(from_path=from_path)
-    username = request.META.get('GVM_USERNAME')
+    username = request.META.get("GVM_USERNAME")
     if username:
-        all_user = params.get('user_specific', {})
+        all_user = params.get("user_specific", {})
         specific_user_params = all_user.get(username, {})
         specific_user_params = func(request, specific_user_params)
         all_user[username] = specific_user_params
-        params['user_specific'] = all_user
+        params["user_specific"] = all_user
         value = params
     else:
         value = func(request, params)
     return Response(store(value, from_path=from_path))
 
 
 def __process_form_data(request: HttpRequest, data: Dict) -> Dict:
     if not isinstance(request.data, dict):
         raise TypeError(
-            "Request data is expected to be a dict, but it is {}".format(
-                type(request.data)
-            )
+            "Request data is expected to be a dict, "
+            f"but it is {type(request.data)}"
         )
-    for (key, value) in request.data.items():
+    for key, value in request.data.items():
         if isinstance(value, UploadedFile):
             file_type, _ = mimetypes.guess_type(value.name)
             logger.info(
-                "uploading filetype %s/%s for %s",
-                file_type,
-                value.name,
-                key,
+                "uploading filetype %s/%s for %s", file_type, value.name, key
             )
-            if file_type and file_type.startswith('image'):
+            if file_type and file_type.startswith("image"):
                 data[key] = as_datalink(value.read(), file_type)
-            elif file_type and file_type.startswith('text'):
+            elif file_type and file_type.startswith("text"):
                 data[key] = value.read().decode()
             else:
                 raise ValueError("Only image or text is permitted")
         else:
             data[key] = value
     return data
 
 
 def __process_json_object(request: HttpRequest, data: Dict) -> Dict:
     return {**data, **request.data}
 
 
-@api_view(['PUT'])
+@api_view(["PUT"])
 @parser_classes([rest_framework.parsers.JSONParser])
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 @authentication_classes(
     [
         pheme.authentication.LoggedInAsAUser,
         pheme.authentication.SimpleApiKeyAuthentication,
     ]
 )
-def put_value(
-    request: HttpRequest,
-    key: str,
-) -> Response:
+def put_value(request: HttpRequest, key: str) -> Response:
     def __process_single_value(request: HttpRequest, data: Dict) -> Dict:
         data[key] = request.data
         return data
 
     return __put(request, __process_single_value)
 
 
-@api_view(['PUT'])
+@api_view(["PUT"])
 @parser_classes(
     [rest_framework.parsers.JSONParser, rest_framework.parsers.MultiPartParser]
 )
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 @authentication_classes(
     [
         pheme.authentication.LoggedInAsAUser,
         pheme.authentication.SimpleApiKeyAuthentication,
     ]
 )
 def put(request: HttpRequest) -> Response:
-
     if request.content_type == "application/json":
         return __put(request, __process_json_object)
     return __put(request, __process_form_data)
```

### Comparing `pheme-21.4rc4/pheme/parser/__init__.py` & `pheme-21.5.0/pheme/transformation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# pheme/parser/__init__.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# pheme/transformation/__init__.py
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -12,7 +12,8 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+from . import scanreport
```

### Comparing `pheme-21.4rc4/pheme/parser/xml.py` & `pheme-21.5.0/pheme/parser/xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/parser/xml.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -32,28 +32,28 @@
     XML parser based on xmltodict.
     """
 
     media_type = "multipart/form-data"
 
     def parse(self, stream, media_type=None, parser_context=None):
         for report in stream.FILES.values():
-            if report.content_type == 'text/xml':
+            if report.content_type == "text/xml":
                 return xmltodict.parse(
                     report.read(),
-                    attr_prefix='',
-                    cdata_key='text',
+                    attr_prefix="",
+                    cdata_key="text",
                     dict_constructor=dict,
                 )
         return None
 
 
 class XMLParser(BaseParser):
     """
     XML parser based on xmltodict.
     """
 
     media_type = "application/xml"
 
     def parse(self, stream, media_type=None, parser_context=None):
         return xmltodict.parse(
-            stream, attr_prefix='', cdata_key='text', dict_constructor=dict
+            stream, attr_prefix="", cdata_key="text", dict_constructor=dict
         )
```

### Comparing `pheme-21.4rc4/pheme/renderer.py` & `pheme-21.5.0/pheme/renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/renderer/xml.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -20,56 +20,56 @@
 from io import StringIO
 from csv import DictWriter
 from rest_framework.renderers import BaseRenderer
 import xmltodict
 
 
 class CSVRenderer(BaseRenderer):
-    media_type = 'text/csv'
-    format = 'text'
-    charset = 'utf-8'
+    media_type = "text/csv"
+    format = "text"
+    charset = "utf-8"
 
     def __flatten_per_result(
         self, data: Dict
     ) -> Generator[Union[List[str], Dict], None, None]:
         # for the case that results is there but it is None
-        results = data.pop('results', None) or []
+        results = data.pop("results", None) or []
         send_keys = True
         for host in results:
-            for result in host.get('results'):
+            for result in host.get("results"):
                 flatten = {
                     **data,
-                    "os": host.get('os'),
-                    **result.pop('nvt_tags_interpreted', {}),
+                    "os": host.get("os"),
+                    **result.pop("nvt_tags_interpreted", {}),
                     **result,
                 }
                 if send_keys:
                     yield flatten.keys()
                     send_keys = False
                 yield flatten
 
     def render(self, data, accepted_media_type=None, renderer_context=None):
         if data is None:
-            return ''
+            return ""
         try:
             generator = self.__flatten_per_result(data)
             result = StringIO()
             writer = DictWriter(result, next(generator))
             writer.writeheader()
             writer.writerows(generator)
             result.seek(0)
             return result.read()
         except StopIteration:
-            return ''
+            return ""
 
 
 class MarkDownTableRenderer(BaseRenderer):
-    media_type = 'text/markdown+table'
-    format = 'text'
-    charset = 'utf-8'
+    media_type = "text/markdown+table"
+    format = "text"
+    charset = "utf-8"
 
     def __as_md(self, previous_key, data):
         def append(value):
             return isinstance(value, str) or isinstance(value, int)
 
         if not (isinstance(data, dict) or isinstance(data, list)):
             return []
@@ -77,51 +77,45 @@
         result = []
 
         def to_new_key(key: str):
             if not previous_key:
                 return key
             if not key:
                 return previous_key
-            return "{}.{}".format(previous_key, key)
+            return f"{previous_key}.{key}"
 
         if isinstance(data, list):
             result.append(
-                "|{}|{}| a list of items|".format(
-                    previous_key,
-                    "{{% for item in {} %}} ... {{% endfor %}}".format(
-                        previous_key
-                    ),
-                )
+                f"|{previous_key}|{{% for item in {previous_key} %}} ..."
+                " {% endfor %}| a list of items|"
             )
-            previous_key = 'item'
+            previous_key = "item"
             items = [("", v) for v in data]
         else:
             items = data.items()
         for key, value in items:
             new_key = to_new_key(key)
             if append(value):
-                result.append(
-                    "|{}|{}|{}|".format(new_key, "{{ %s }}" % new_key, value)
-                )
+                result.append(f"|{new_key}|{{ {new_key} }}|{value}|")
             else:
                 result = result + self.__as_md(new_key, value)
         return result
 
     def render(self, data, accepted_media_type=None, renderer_context=None):
         if data is None:
-            return ''
+            return ""
         first_line = "|key|template_example|description|\n"
         table_indicator = "| :- | :--: | -: |\n"
         rest = "\n".join(self.__as_md("", data))
         return first_line + table_indicator + rest
 
 
 class XMLRenderer(BaseRenderer):
-    media_type = 'application/xml'
-    format = 'xml'
-    charset = 'utf-8'
+    media_type = "application/xml"
+    format = "xml"
+    charset = "utf-8"
 
     def render(self, data, accepted_media_type=None, renderer_context=None):
         if data is None:
-            return ''
+            return ""
 
         return xmltodict.unparse(data)
```

### Comparing `pheme-21.4rc4/pheme/settings.py` & `pheme-21.5.0/pheme/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/settings.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -41,42 +41,62 @@
 )
 STATIC_DIR = BASE_DIR / "static"
 TEMPLATE_DIR = BASE_DIR / "template"
 # set default to actual gos path instead of static dir
 
 GSAD_URL = os.environ.get("GSAD_URL", "https://localhost/gmp")
 
+SENTRY_DSN = os.environ.get("SENTRY_DSN_PHEME")
+
+# load sentry_sdk only when SENTRY_DSN_PHEME is set otherwise don't bother
+if SENTRY_DSN is not None:
+    # pylint: disable=import-error
+    import sentry_sdk
+    from sentry_sdk.integrations.django import DjangoIntegration
+
+    # pylint: disable=E0110
+    # Due to the MYPY handling within sentry_sdk.init, to have a nicer user
+    # experience than to have to look up lambdas, pylint detects this as an
+    # abstract class; which it is.
+    sentry_sdk.init(
+        SENTRY_DSN,
+        traces_sample_rate=1.0,
+        environment=os.environ.get("SENTRY_ENVIRONMENT"),
+        server_name=os.environ.get("SENTRY_SERVER_NAME"),
+        integrations=[DjangoIntegration()],
+    )
+
 DATA_UPLOAD_MAX_MEMORY_SIZE = None
 
 PHEME_CONFIGURATION_PATH = Path(
     os.environ.get(
         "PHEME_CONFIGURATION_PATH",
         "/var/lib/pheme" if Path("/var/lib/pheme").exists() else Path("/tmp/"),
     )
 )
 
 
 SECRET_KEY_LOCATION = PHEME_CONFIGURATION_PATH.joinpath("api_key")
 
 PARAMETER_FILE_ADDRESS = PHEME_CONFIGURATION_PATH.joinpath("parameter.json")
 DATA_OBJECT_PATH = "/opt/greenbone/feed/gvmd"
-GOS_VERSION = "21.04"
+GOS_VERSION = "22.04"
 DEFAULT_PARAMETER_ADDRESS = (
     os.environ.get("DEFAULT_PARAMETER_FILE_ADDRESS")
     or f"{DATA_OBJECT_PATH}/{GOS_VERSION}/pheme/default-parameter.json"
 )
 
 
 def __load_or_create_api_key() -> str:
     if SECRET_KEY_LOCATION.exists():
-        may_token = SECRET_KEY_LOCATION.read_text()
+        may_token = SECRET_KEY_LOCATION.read_text(encoding="utf-8")
         if len(may_token.strip()) > 0:
             return may_token
     token = secrets.token_urlsafe(50)
-    SECRET_KEY_LOCATION.write_text(token)
+    SECRET_KEY_LOCATION.write_text(token, encoding="utf-8")
     return token
 
 
 SECRET_KEY = os.environ.get("PHEME_API_KEY", __load_or_create_api_key())
 
 ENV_HOSTS = os.environ.get("ALLOWED_HOSTS", "*")
 DEBUG = os.environ.get("PHEME_DEBUG", "").lower() == "true"
@@ -105,27 +125,25 @@
 ]
 
 ROOT_URLCONF = "pheme.urls"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": [
-            TEMPLATE_DIR,
-        ],
+        "DIRS": [TEMPLATE_DIR],
         "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
                 "django.template.context_processors.debug",
                 "django.template.context_processors.request",
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
-            ],
+            ]
         },
-    },
+    }
 ]
 
 WSGI_APPLICATION = "pheme.wsgi.application"
 
 
 # Database
 # https://docs.djangoproject.com/en/3.1/ref/settings/#databases
@@ -153,30 +171,24 @@
 USE_TZ = True
 
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/3.1/howto/static-files/
 
 STATIC_URL = "/static/"
-STATICFILES_DIRS = [
-    STATIC_DIR,
-    TEMPLATE_DIR,
-]
+STATICFILES_DIRS = [STATIC_DIR, TEMPLATE_DIR]
 
 # Logging
 # https://docs.djangoproject.com/en/3.1/topics/logging/
 
 LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "handlers": {
-        "console": {
-            "class": "logging.StreamHandler",
-            "formatter": "standard",
-        },
+        "console": {"class": "logging.StreamHandler", "formatter": "standard"},
         "syslog": {
             "class": "logging.handlers.SysLogHandler",
             "formatter": "standard",
             "facility": "user",
             "address": "/dev/log",
         },
         "file": {
@@ -187,19 +199,19 @@
             else "/tmp/pheme.log",
         },
     },
     "formatters": {
         "standard": {
             "format": "{module}#{funcName} {levelname} {asctime}: {message}",
             "style": "{",
-        },
+        }
     },
     "root": {
         "handlers": [
-            "syslog" if Path("/dev/log").exists() else "console",
+            "syslog" if Path("/dev/log").exists() and not DEBUG else "console",
             "file",
         ],
         "level": os.getenv("DJANGO_LOG_LEVEL", "INFO"),
     },
 }
 # https://docs.djangoproject.com/en/3.1/topics/cache/
 CACHES = {
@@ -212,9 +224,9 @@
 
 # testing
 REST_FRAMEWORK = {
     "TEST_REQUEST_RENDERER_CLASSES": [
         "pheme.renderer.XMLRenderer",
         "rest_framework.renderers.JSONRenderer",
         "rest_framework.renderers.MultiPartRenderer",
-    ],
+    ]
 }
```

### Comparing `pheme-21.4rc4/pheme/storage.py` & `pheme-21.5.0/pheme/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/transformation/storage.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -27,26 +27,26 @@
 
 
 def __default_load_handler(name: str) -> Dict:
     return cache.get(name)
 
 
 def __default_id_generator(prefix: str) -> str:
-    return "{}-{}".format(prefix, uuid4())
+    return f"{prefix}-{uuid4()}"
 
 
 def load(name: str, *, handler=__default_load_handler) -> Dict:
     return handler(name)
 
 
 def store(
     prefix: str,
     value: Dict,
     *,
     handler=__default_store_handler,
-    id_generator=__default_id_generator
+    id_generator=__default_id_generator,
 ):
     name = id_generator(prefix)
     if isinstance(value, dict):
-        value['internal_name'] = name
+        value["internal_name"] = name
     handler(name, value)
     return name
```

### Comparing `pheme-21.4rc4/pheme/templatetags/__init__.py` & `pheme-21.5.0/pheme/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# pheme/templatetags/__init__.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# pheme/__init__.py
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -12,7 +12,9 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from .version import __version__
```

### Comparing `pheme-21.4rc4/pheme/templatetags/charts/__init__.py` & `pheme-21.5.0/pheme/templatetags/charts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -30,28 +30,28 @@
 __LEGEND_TEMPLATE = """
 <g transform="translate({x}, {y})">
 {legend}
 </g>
 """
 __LEGEND_ELEMENT = """
 <rect x="{x}" y="{y}" height="{font_size}" width="{font_size}" style="fill: {color};"></rect>
-<text style="font-size:{font_size};font-family:{font_family}" x="{text_x}" y="{text_y}" dominant-baseline="central">{label}</text>
+<text style="font-size:{font_size}px;font-family:{font_family}" x="{text_x}" y="{text_y}" dominant-baseline="central">{label}</text>
 """
 
 
 def calculate_legend_start_height(
     height: int, label_color: Dict, font_size: int
 ) -> int:
     return int(height / 2 - (len(label_color) * font_size) / 2)
 
 
 def build_legend(
     start_height: int,
     label_color: Dict,
-    font_family: str = "Droid Sans",
+    font_family: str = "Dejavu Sans",
     font_size: int = 10,
 ) -> str:
     """
     Generates a legend at     start_height y position and at
     width / 2 - last_x of element / 2 x position.
 
     By iterating through the the label_color dict and using the key as a label
```

### Comparing `pheme-21.4rc4/pheme/templatetags/charts/h_bar.py` & `pheme-21.5.0/pheme/templatetags/charts/h_bar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/templatetags/bar_chart.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -15,14 +15,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import itertools
 from typing import Dict
+from PIL import ImageFont
 from django.utils.safestring import SafeText
 from pheme.templatetags.charts import (
     register,
     _severity_class_colors,
     build_legend,
     calculate_legend_start_height,
 )
@@ -30,59 +31,79 @@
 
 __ORIENTATION_LINE_TEMPLATE = """
 <rect x="{x}" y="0" height="{height}" width="1" style="fill: #000000;"></rect>
 """
 
 __ORIENTATION_LINE_TEXT_TEMPLATE = """
 <text class="orientation label" y="22" x="{x}" fill="#4C4C4D" dominant-baseline="central"
-style="font-size:{font_size};font-family:{font_family};text-anchor: middle;" width="{width}">{label}
+style="font-size:{font_size}px;font-family:{font_family};text-anchor: middle;" width="{width}">{label}
 </text>
 """
+
+__X_AXIS_LABEL = """
+<text class="x axis label" y="{y}" x="{x}" fill="#000000"
+style="font-size:{font_size}px;font-family:{font_family};text-anchor: middle;">{axis_label}
+</text>
+"""
+
 __BAR_ELEMENT_TEMPLATE = """
 <rect x="{x}" y="17" height="10" width="{width}" style="fill: {color};"></rect>
 """
 
 __BAR_TEMPLATE = """
 <g class="entry" transform="translate(0, {y})">
 <text class="label category" y="22" x="87.5" fill="#4C4C4D" dominant-baseline="central"
-style="font-size:{font_size};font-family:{font_family};text-anchor: right;" width="{max_hostname_len}">{key}
+style="font-size:{font_size}px;font-family:{font_family};text-anchor: right;" width="{max_hostname_len}">{key}
 </text>
 <g transform="translate({max_hostname_len}, 0)">
 {orientation_lines}
 {bar_elements}
 </g>
 <g transform="translate({begin_total}, 0)">
 <text class="sum" y="22" x="10" fill="#4C4C4D" dominant-baseline="central"
-style="font-size:{font_size};font-family:{font_family};text-anchor: left;" width="100">{total}</text>
+style="font-size:{font_size}px;font-family:{font_family};text-anchor: left;" width="100">{total}</text>
 </g>
 </g>
 """
 __BAR_CHART_TEMPLATE = """
 <svg width="{width}" viewBox="0 0 {width} {height}" xmlns="http://www.w3.org/2000/svg">
 {bars}
+<g transform="translate(0, {bar_legend_y})">
+<text 
+    class="label category" 
+    y="22" x="87.5" 
+    fill="#4C4C4D" dominant-baseline="central"
+    style="font-size:{font_size}px;font-family:{font_family};text-anchor: right;" 
+    width="{max_hostname_len}">
+    {x_title}
+    </text>
+</g>
 <g transform="translate({max_hostname_len}, {bar_legend_y})">
 {bar_legend}
 </g>
 {legend}
+{x_axis_label}
 </svg>
 """
 
 
 @register.filter
+@register.simple_tag
 def h_bar_chart(
     chart_data: Dict[str, Dict[str, int]],
+    x_title: str = "",
     title_color=None,
     svg_width=800,
     bar_jump=44,
-    orientation_basis=20,
+    orientation_marker=6,
     limit=10,
-    font_family="Droid Sans",
+    font_family="Dejavu Sans",
+    font_file_name="DejaVuSans.ttf",
     font_size=10,
 ) -> SafeText:
-
     """
     Returns a stacked horizontal bar chart in svg.
 
     In order to function it needs a dict with label as key containing a dict
     with color key and amount.
 
     An example for valid input is:
@@ -97,64 +118,78 @@
 
     parameter:
         chart_data - The dict containing the values for the chart
         title_color - A colortable, defaulting to __severity_class_colors
         svg_width - The overall width of the output chart, default 800
         bar_jump - The amount of y pixels to jump from bar element to the next.
             Default is 44.
-        orientation_basis - if higher than 0 than there will be a vertical line
-            each orientation_basis.
+        orientation_marker - if higher than 0 than there will be a vertical line
+            each nth step.
         limit - limits the data by N first elements
         font_family - the font family used within text elements
         font_size - the font size used within text elements
+        x_title - the title of the x axis
     """
-
     data = dict(itertools.islice(chart_data.items(), limit))
     if not title_color:
         title_color = _severity_class_colors
     if not data.values():
         return SafeText("")
-    # multiply by 1.25 for kerning
-    max_hostname_len = max(len(k) for k in data.keys()) * font_size * 1.25
+    try:
+        font = ImageFont.truetype(font_file_name, font_size)
+        # add 87.5 + 10 for legend
+        max_hostname_len = (
+            max(
+                max(font.getlength(k) for k in data.keys()),
+                font.getlength(x_title),
+            )
+            + 87.5
+            + 10
+        )
+    except OSError:
+        # multiply by 1.25 for kerning and add 87.5 for legend
+        max_hostname_len = (
+            max(max(len(k) for k in data.keys()), len(x_title))
+            * font_size
+            * 1.25
+            + 87.5
+        )
     max_width = svg_width - max_hostname_len - 100  # key and total placeholder
     # highest sum of counts
     max_sum = max([sum(list(counts.values())) for counts in data.values()])
     if max_sum == 0:
         max_sum = 1
+
     orientation_lines = ""
     orientation_labels = ""
-
-    def __add_orientation(i: int, orientation_lines="", orientation_labels=""):
-        x_pos = i * orientation_basis / max_sum * max_width
-        label = str(i * orientation_basis)
-        orientation_lines += __ORIENTATION_LINE_TEMPLATE.format(
-            x=x_pos,
-            height=bar_jump + 10,
-            font_family=font_family,
-            font_size=font_size,
-        )
-        orientation_labels += __ORIENTATION_LINE_TEXT_TEMPLATE.format(
-            x=x_pos,
-            width=len(label),
-            label=label,
-            font_family=font_family,
-            font_size=font_size,
-        )
-        return orientation_lines, orientation_labels
-
-    if orientation_basis > 0:
+    orientation_basis = (
+        int(max_sum / orientation_marker) if orientation_marker > 0 else 0
+    )
+    if max_sum > orientation_basis and orientation_basis > 0:
         overhead = max_sum % orientation_basis
         # if it's already adjusted we don't need to add anything
         if overhead == 0:
             overhead = orientation_basis
         max_sum = max_sum + orientation_basis - overhead
 
         for i in range(int(max_sum / orientation_basis + 1)):
-            orientation_lines, orientation_labels = __add_orientation(
-                i, orientation_lines, orientation_labels
+            x_pos = i * orientation_basis / max_sum * max_width
+            label = str(i * orientation_basis)
+            orientation_lines += __ORIENTATION_LINE_TEMPLATE.format(
+                x=x_pos,
+                height=bar_jump + 10,
+                font_family=font_family,
+                font_size=font_size,
+            )
+            orientation_labels += __ORIENTATION_LINE_TEXT_TEMPLATE.format(
+                x=x_pos,
+                width=len(label),
+                label=label,
+                font_family=font_family,
+                font_size=font_size,
             )
 
     bars = ""
     for i, (key, counts) in enumerate(data.items()):
         element_x = 0
         elements = ""
         for category, count in counts.items():
@@ -177,23 +212,31 @@
             orientation_lines=orientation_lines,
             total=sum(counts.values()),
             font_family=font_family,
             font_size=font_size,
             max_hostname_len=max_hostname_len,
             begin_total=svg_width - 100,
         )
-    svg_element_lengths = len(data.keys()) * bar_jump + 50
+    svg_element_lengths = len(data.keys()) * bar_jump + 60 + font_size
     legend_start = calculate_legend_start_height(
         svg_element_lengths, title_color, font_size
     )
     svg_chart = __BAR_CHART_TEMPLATE.format(
         width=svg_width,
         height=svg_element_lengths,
         bars=bars,
         bar_legend=orientation_labels,
         bar_legend_y=len(data.keys()) * bar_jump + 20,
         legend=build_legend(legend_start, title_color),
         font_family=font_family,
         font_size=font_size,
         max_hostname_len=max_hostname_len,
+        x_axis_label=__X_AXIS_LABEL.format(
+            axis_label="Number of Vulnerabilities",
+            font_size=font_size,
+            font_family=font_family,
+            x=svg_width / 2,
+            y=svg_element_lengths,
+        ),
+        x_title=x_title,
     )
     return SafeText(svg_chart)
```

### Comparing `pheme-21.4rc4/pheme/templatetags/charts/pie.py` & `pheme-21.5.0/pheme/templatetags/charts/pie.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/templatetags/charts.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -34,27 +34,27 @@
 {legend}
 </svg>
 """
 
 __SLICE_TEMPLATE = """
 <g>
 <circle cx="{cx}" cy="{cy}" r="{radius}" stroke="{color}" stroke-width="{stroke_width}" stroke-dasharray="{d_array}" stroke-dashoffset="{s_offset}" transform="rotate({r_start}, {cx}, {cy})" fill="transparent"></circle>
-<text style="font-size:{font_size};font-family:{font_family}" x="{t_x}" y="{t_y}" text-anchor="middle">{label}</text>
+<text style="font-size:{font_size}px;font-family:{font_family}" x="{t_x}" y="{t_y}" text-anchor="middle">{label}</text>
 </g>
 """
 
 
 @register.filter
 def pie_chart(
     input_values: Dict,
     title_color: Dict = None,
     width: int = 390,
     border_size: int = 0,
     slice_width: int = 90,
-    font_family: str = "Droid Sans",
+    font_family: str = "Dejavu Sans",
     font_size: int = 10,
 ) -> SafeText:
     """
     creates a pie chart svg.
 
     The values parameter needs to be a dict with a categoryname: numeric_value.
     E.g.:
@@ -95,15 +95,15 @@
     cy = chart_size / 2  # shift y
     # need to cut out size of the slice_width, otherwise edges will be cut off
     radius = (chart_size - slice_width) / 2
     circumference = 2 * math.pi * radius
     dash_array = circumference - border_size
 
     donut = ""
-    for (category, amount) in input_values.items():
+    for category, amount in input_values.items():
         percent = amount / total
         color = title_color.get(category)
         dash_offset = circumference - percent * circumference
         degrees = angle_offset
         t_angle = (percent * 360) / 2 + angle_offset
         t_radians = t_angle * (math.pi / 180)
         t_x = radius * math.cos(t_radians) + cx
@@ -117,15 +117,15 @@
             color=color,
             stroke_width=slice_width,
             d_array=dash_array,
             s_offset=dash_offset,
             r_start=degrees,
             t_x=t_x,
             t_y=t_y,
-            label=f"{round(percent * 100)}%",
+            label=f"{amount} ({round(percent * 100)}%)",
             font_family=font_family,
             font_size=font_size,
         ).strip()
 
     legend_start = calculate_legend_start_height(
         chart_size, title_color, font_size
     )
```

### Comparing `pheme-21.4rc4/pheme/templatetags/charts/treemap.py` & `pheme-21.5.0/pheme/templatetags/charts/treemap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -37,15 +37,15 @@
     build_legend,
     calculate_legend_start_height,
 )
 
 __ELEMENT_TEMPLATE = """
 <g>
     <rect x="{x}" y="{y}" width="{width}" height="{height}" fill="{color}" stroke="{border_color}" strokeWidth="1" />
-    <text style="font-size:{font_size};font-family:{font_family}" x="{label_x}" y="{label_y}" width="{width}" height="{height}" dominant-baseline="central">{label}</text>
+    <text style="font-size:{font_size}px;font-family:{font_family}" x="{label_x}" y="{label_y}" width="{width}" height="{height}" dominant-baseline="central">{label}</text>
 </g>
 """
 
 __TEMPLATE = """
 <svg version="1.1"
      baseProfile="full"
      width="{width}" height="{height}"
@@ -236,15 +236,15 @@
 def treemap(
     data: List[Dict],
     width: int = 1024,
     height: int = 768,
     border_color: str = "#ffffff",
     title_color: Dict[str, str] = None,
     font_size: int = 10,
-    font_family: str = "Droid Sans",
+    font_family: str = "Dejavu Sans",
 ) -> SafeText:
     """
     Expects a sorted dict containing a str, and a dict with values in it.
 
     An example can be:
 
     {
```

### Comparing `pheme-21.4rc4/pheme/templatetags/dynamic_template.py` & `pheme-21.5.0/pheme/templatetags/dynamic_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/templatetags/dynamic_template.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `pheme-21.4rc4/pheme/transformation/__init__.py` & `pheme-21.5.0/pheme/transformation/scanreport/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# pheme/transformation/__init__.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# pheme/transformation/scanreport/__init__.py
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -12,8 +12,8 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from . import scanreport
+from . import gvmd, renderer
```

### Comparing `pheme-21.4rc4/pheme/transformation/scanreport/__init__.py` & `pheme-21.5.0/pheme/parser/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# pheme/transformation/scanreport/__init__.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# pheme/parser/__init__.py
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -12,8 +12,7 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from . import gvmd, renderer
```

### Comparing `pheme-21.4rc4/pheme/transformation/scanreport/gvmd.py` & `pheme-21.5.0/pheme/transformation/scanreport/gvmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/transformation/scanreport/gvmd.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -51,172 +51,173 @@
         return result
 
     return measure
 
 
 def __tansform_tags(item) -> Optional[Dict[str, str]]:
     if isinstance(item, str):
-        split = [i.split('=') for i in item.split('|')]
-        return {i[0]: i[1].replace('\n', ' ') for i in split if len(i) == 2}
+        split = [i.split("=") for i in item.split("|")]
+        return {i[0]: i[1].replace("\n", " ") for i in split if len(i) == 2}
     return None
 
 
 def __group_refs(refs: Dict[str, str]) -> Dict:
     refs_ref = {}
-    for ref in refs.get('ref', []):
+    for ref in refs.get("ref", []):
         if isinstance(ref, dict):
-            typus = ref.get('type', 'unknown')
-            refs_ref[typus] = refs_ref.get(typus, []) + [ref.get('id')]
+            typus = ref.get("type", "unknown")
+            refs_ref[typus] = refs_ref.get(typus, []) + [ref.get("id")]
     return refs_ref
 
 
 def __get_hostname_from_result(result) -> str:
     if isinstance(result, str):
         return result
     if isinstance(result, dict):
-        host = result.get('host', {})
+        host = result.get("host", {})
         if isinstance(host, dict):
-            return host.get('text', 'unknown')
+            return host.get("text", "unknown")
         return host
-    return 'unknown'
+    return "unknown"
 
 
 def __return_highest_threat(threats: List[int]) -> str:
     """
     returns the highest threat
     """
     for i, value in enumerate(threats):
         if value > 0:
             return __threats[i]
-    return 'NA'
+    return "NA"
 
 
-def __host_threat_overview(threat_count: List[int]) -> Dict:
+def __host_threat_overview(threat_count: Dict) -> Dict:
     """
     returns nvt statistics mostly used in the per host overview
     """
     result = {**threat_count}
-    result['total'] = sum(threat_count.values())
-    result['highest'] = __return_highest_threat(threat_count.values())
+    result["total"] = sum(threat_count.values())
+    result["highest"] = __return_highest_threat(threat_count.values())
     return result
 
 
 def __return_highest_severity(severities: List[int]) -> str:
     """
     returns the highest severity within a list
     """
     for i in range(len(severities) - 1, -1, -1):
         if severities[i] > 0:
             return str(i + 1)
-    return 'NA'
+    return "NA"
 
 
 def __host_severity_overview(nvt_count: List[int]) -> Dict:
     """
     returns nvt severity statistics mostly used in the per host overview
     """
     result = {str(i + 1): value for i, value in enumerate(nvt_count)}
-    result['total'] = sum(nvt_count)
-    result['highest'] = __return_highest_severity(nvt_count)
+    result["total"] = sum(nvt_count)
+    result["highest"] = __return_highest_severity(nvt_count)
     return result
 
 
 def __create_host_information_lookup(report: Dict) -> Dict:
     """
     created a lookup table for available host information
     """
     # lookup for host information name and dict name
-    information_key = {'best_os_txt': 'os'}
+    information_key = {"best_os_txt": "os"}
 
     def filter_per_host(host: Dict) -> Dict:
         information = {}
         found = 0
-        details = host.get('detail', [])
+        details = host.get("detail", [])
         for detail in details:
-            name = detail.get('name', '')
-            if name in information_key.keys():
-                information[information_key.get(name)] = detail.get('value')
+            name = detail.get("name", "")
+            if name in information_key:
+                information[information_key.get(name)] = detail.get("value")
                 found += 1
-            if found == len(information_key.keys()):
+            if found == len(information_key):
                 return information
         return information
 
     result = {}
-    hosts = report.get('host')
+    hosts = report.get("host")
     if isinstance(hosts, dict):
-        result[hosts.get('ip', 'unknown')] = filter_per_host(hosts)
+        result[hosts.get("ip", "unknown")] = filter_per_host(hosts)
     elif isinstance(hosts, list):
         # best_os_txt seems to be in the end
         for host in hosts[::-1]:
-            result[host.get('ip', 'unknown')] = filter_per_host(host)
+            result[host.get("ip", "unknown")] = filter_per_host(host)
     return result
 
 
 @measure_time
 def __create_results_per_host(report: Dict) -> List[Dict]:
     """
     creates the results dict used by a vulnerability-report based on a given
     gvmd report.
     """
     host_information_lookup = __create_host_information_lookup(report)
-    results = report.get('results', {}).get('result', [])
+    results = report.get("results", {}).get("result", [])
     by_host = {}
     host_threat_count = {}
     host_severity_count = {}
     threat_count = [0] * len(__threats)
 
     def transform_key(prefix: str, vic: Dict) -> Dict:
-        return {
-            "{}_{}".format(prefix, key): value for key, value in vic.items()
-        }
+        return {f"{prefix}_{key}": value for key, value in vic.items()}
 
     def per_result(result):
         hostname = __get_hostname_from_result(result)
         host_dict = by_host.get(hostname, {})
-        threat = result.get('threat', 'unknown')
-        port = result.get('port')
-        nvt = transform_key("nvt", result.get('nvt', {}))
-        nvt['nvt_tags_interpreted'] = __tansform_tags(nvt.get('nvt_tags', ''))
-        nvt['nvt_refs_ref'] = __group_refs(nvt.get('nvt_refs', {}))
-        qod = transform_key('qod', result.get('qod', {}))
-        severity = int(float(result.get('severity', '0.0')))
+        threat = result.get("threat", "unknown")
+        port = result.get("port")
+        nvt = transform_key("nvt", result.get("nvt", {}))
+        nvt["nvt_tags_interpreted"] = __tansform_tags(nvt.get("nvt_tags", ""))
+        nvt["nvt_refs_ref"] = __group_refs(nvt.get("nvt_refs", {}))
+        qod = transform_key("qod", result.get("qod", {}))
+        severity = float(result.get("severity", "0.0"))
         new_host_result = {
             "port": port,
             "threat": threat,
             "severity": severity,
-            "description": result.get('description'),
+            "description": result.get("description"),
             **nvt,
             **qod,
         }
-        host_results = host_dict.get('results', [])
+        host_results = host_dict.get("results", [])
         host_results.append(new_host_result)
-        equipment = host_dict.get('equipment', {})
-        equipment['ports'] = list(
-            dict.fromkeys(equipment.get('ports', []) + [port])
-        )
-        if not equipment.get('os'):
-            equipment['os'] = host_information_lookup.get(hostname, {}).get(
-                'os', 'unknown'
+        equipment = host_dict.get("equipment", {})
+        ports = list(dict.fromkeys(equipment.get("ports", [])))
+        if port and not port.startswith("general"):
+            ports = set(ports + [port])
+        equipment["ports"] = ports
+        if not equipment.get("os"):
+            equipment["os"] = host_information_lookup.get(hostname, {}).get(
+                "os", "unknown"
             )
 
         # needs hostname, high, medium, low
         host_threats = host_threat_count.get(
             hostname, {threat: 0 for threat in __threats}
         )
-        threat_index = __threat_index_lookup.get(threat, len(__threats) - 1)
+        threat_index = __threat_index_lookup.get(threat)
+        if threat_index is not None:
+            threat_count[threat_index] += 1
         if host_threats.get(threat) is not None:
             host_threats[threat] += 1
         host_threat_count[hostname] = host_threats
 
         # needs high, medium, low
-        threat_count[threat_index] += 1
 
         # severity 1 to 10
         host_severities = host_severity_count.get(hostname, [0] * 10)
-        host_severities[severity - 1] += 1
+        if severity > 0:
+            host_severities[int(severity) - 1] += 1
         host_severity_count[hostname] = host_severities
 
         by_host[hostname] = {
             "host": hostname,
             "threats": __host_threat_overview(host_threats),
             "severities": __host_severity_overview(host_severities),
             "equipment": equipment,
@@ -252,25 +253,21 @@
     """
     if not data:
         raise ValueError("Need data to process")
     report = data.get("report")
     # sometimes gvmd reports have .report.report sometimes just .report
     report = report.get("report", report)
 
-    task = report.get('task') or {}
-    gmp = report.get('gmp') or {}
+    task = report.get("task") or {}
     logger.info("data transformation")
     results, host_counts, nvts_counts = __create_results_per_host(report)
 
     return Report(
-        report.get('id'),
-        task.get('name'),
-        task.get('comment'),
-        gmp.get('version'),
-        report.get('scan_start'),
+        report.get("id"),
+        task.get("name"),
+        task.get("comment"),
+        report.get("scan_start"),
         Overview(
-            hosts=host_counts,
-            nvts=nvts_counts,
-            vulnerable_equipment=None,
+            hosts=host_counts, nvts=nvts_counts, vulnerable_equipment=None
         ),
         results,
     )
```

### Comparing `pheme-21.4rc4/pheme/transformation/scanreport/model.py` & `pheme-21.5.0/pheme/transformation/scanreport/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/transformation/scanreport/model.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -68,26 +68,24 @@
 
 
 @dataclass
 class Report:
     id: str
     name: str
     comment: str
-    version: str
     start: str
     overview: Overview
     results: List[Dict]
 
 
 def describe():
     return Report(
         id="str; identifier of a report",
         name="str; name of the scan",
         comment="str; comment of the scan",
-        version="str; version of gvmd",
         start="str; datetime of a scan start",
         overview=Overview(
             hosts=CountGraph(
                 name="host_top_ten",
                 chart="str; link to chart image (base64 encoded datalink)",
                 counts=[],
             ),
@@ -102,57 +100,57 @@
                 counts=[],
             ),
         ),
         results=[
             dict(
                 host="str; ip address of host",
                 threats={
-                    'high': 'int; amount of high nvts in host',
-                    'medium': 'int; amount of medium nvts in host',
-                    'low': 'int; amount of low nvts in host',
-                    'total': 'int; amount of nvts in host',
-                    'highest': 'str; highest threat within host',
+                    "high": "int; amount of high nvts in host",
+                    "medium": "int; amount of medium nvts in host",
+                    "low": "int; amount of low nvts in host",
+                    "total": "int; amount of nvts in host",
+                    "highest": "str; highest threat within host",
                 },
                 severities={
-                    '1': 'int; amount of 1 severities in host',
-                    '2': 'int; amount of 2 severities in host',
-                    '3': 'int; amount of 3 severities in host',
-                    '4': 'int; amount of 4 severities in host',
-                    '5': 'int; amount of 5 severities in host',
-                    '6': 'int; amount of 6 severities in host',
-                    '7': 'int; amount of 7 severities in host',
-                    '8': 'int; amount of 8 severities in host',
-                    '9': 'int; amount of 9 severities in host',
-                    '10': 'int; amount of 10 severities in host',
-                    'total': 'int; amount of nvts in host',
-                    'highest': 'str; highest severity within host',
+                    "1": "int; amount of 1 severities in host",
+                    "2": "int; amount of 2 severities in host",
+                    "3": "int; amount of 3 severities in host",
+                    "4": "int; amount of 4 severities in host",
+                    "5": "int; amount of 5 severities in host",
+                    "6": "int; amount of 6 severities in host",
+                    "7": "int; amount of 7 severities in host",
+                    "8": "int; amount of 8 severities in host",
+                    "9": "int; amount of 9 severities in host",
+                    "10": "int; amount of 10 severities in host",
+                    "total": "int; amount of nvts in host",
+                    "highest": "str; highest severity within host",
                 },
                 equipment=Equipment(
                     os="str; operating system", ports=["str; open ports"]
                 ),
                 results={
-                    'nvt.oid': 'str; nvt.oid; optional',
-                    'nvt.type': 'str; nvt.type; optional',
-                    'nvt.name': 'str; nvt.name; optional',
-                    'nvt.family': 'str; nvt.family; optional',
-                    'nvt.cvss_base': 'str; nvt.cvss_base; optional',
-                    'nvt.tags_interpreted': {
-                        'name_of_tag': 'str; value of a tag ()',
-                        'may_contain_multiple_tags': 'str; depends on xml',
-                        'solution': 'str; solution the fix the problem',
-                        'solution_type': 'str; solution type',
-                        'insight': 'str; insight into the problem',
-                        'vuldetect': 'str; ',
-                        'cvss_base_vector': 'str, cvss base vector',
+                    "nvt.oid": "str; nvt.oid; optional",
+                    "nvt.type": "str; nvt.type; optional",
+                    "nvt.name": "str; nvt.name; optional",
+                    "nvt.family": "str; nvt.family; optional",
+                    "nvt.cvss_base": "str; nvt.cvss_base; optional",
+                    "nvt.tags_interpreted": {
+                        "name_of_tag": "str; value of a tag ()",
+                        "may_contain_multiple_tags": "str; depends on xml",
+                        "solution": "str; solution the fix the problem",
+                        "solution_type": "str; solution type",
+                        "insight": "str; insight into the problem",
+                        "vuldetect": "str; ",
+                        "cvss_base_vector": "str, cvss base vector",
                     },
-                    'nvt.refs.ref': [{'name_of_ref': ["str; ref_vallue"]}],
-                    'nvt.solution.type': 'str; nvt.solution.type; optional',
-                    'nvt.solution.text': 'str; nvt.solution.text; optional',
-                    'port': 'str; port; optional',
-                    'severity': 'str; severity; optional',
-                    'qod.value': 'str; qod.value; optional',
-                    'qod.type': 'str; qod.type; optional',
-                    'description': 'str; description; optional',
+                    "nvt.refs.ref": [{"name_of_ref": ["str; ref_vallue"]}],
+                    "nvt.solution.type": "str; nvt.solution.type; optional",
+                    "nvt.solution.text": "str; nvt.solution.text; optional",
+                    "port": "str; port; optional",
+                    "severity": "str; severity; optional",
+                    "qod.value": "str; qod.value; optional",
+                    "qod.type": "str; qod.type; optional",
+                    "description": "str; description; optional",
                 },
             )
         ],
     )
```

### Comparing `pheme-21.4rc4/pheme/transformation/scanreport/renderer.py` & `pheme-21.5.0/pheme/transformation/scanreport/renderer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/transformation/scanreport/renderer.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -57,37 +57,38 @@
     renderer_context: Dict, request: Request
 ) -> str:
     resp = renderer_context["response"]
     resp.status_code = 404
     # pylint: disable=W0212
     path = request._request.path
     report_id = path[path.rfind("/") + 1 :]
-    return '"not data found for %s"' % report_id
+    return f'"not data found for {report_id}"'
 
 
 class Report(renderers.BaseRenderer):
     def render(self, data, accepted_media_type=None, renderer_context=None):
         request = _get_request(renderer_context)
         if not data:
             return _default_not_found_response(renderer_context, request)
 
         name = data.get("internal_name")
-        cache_key = "{}/{}".format(self.media_type, name) if name else None
+        cache_key = f"{self.media_type}/{name}" if name else None
         logger.debug("generating report %s", cache_key)
 
         if cache_key and not DEBUG:
             cached = cache.get(cache_key)
             if cached:
                 return cached
         params = load_params()
         # separate user specific parameter
         user_parameter = params.pop("user_specific", {})
         username, _ = get_username_role(request)
         if username:
             params = {**params, **user_parameter.get(username, {})}
+        data["version"] = params.get("version")
 
         result = self.apply(name, data, params)
         if cache_key:
             cache.set(cache_key, result)
         return result
 
     def apply(self, name: str, data: Dict, parameter: Dict):
@@ -136,40 +137,79 @@
         to_index = html.find(close_tag, from_index + len(open_tag))
         if to_index == -1:
             return html
         to_index += len(close_tag)
         to_encode = html[from_index:to_index]
         encoded = b64encode(to_encode.encode()).decode()
         img = (
-            '<img src="data:image/svg+xml;charset=utf-8;base64, {}" />'.format(
-                encoded
-            )
+            f'<img src="data:image/svg+xml;charset=utf-8;base64, {encoded}" />'
         )
         html = html[:from_index] + img + html[to_index:]
         from_index = to_index
 
 
+def enforce_limit(
+    data: Dict, parameter: Dict, format_type: str = "pdf"
+) -> Dict:
+    if not "results" in data:
+        return data
+
+    limits = parameter.get("limits", {}).get(format_type, {})
+    max_hosts = limits.get("hosts")
+    max_results_in_host = limits.get("results")
+    logger.debug(
+        "limit max_results %s and max_hosts %s", max_results_in_host, max_hosts
+    )
+    if not max_hosts and not max_results_in_host:
+        return data
+    host_cut = False
+    if max_hosts and len(data["results"]) > max_hosts:
+        data["results"] = data["results"][:max_hosts]
+        host_cut = True
+    result_cut = False
+    if max_results_in_host:
+        for result in data["results"]:
+            if len(result["results"]) > max_results_in_host:
+                result["results"] = result["results"][:max_results_in_host]
+                result_cut = True
+    if host_cut and not result_cut:
+        data["comment"] = limits.get(
+            "host_limit_msg", f"Host limit: {max_hosts}."
+        )
+    elif result_cut and not host_cut:
+        data["comment"] = limits.get(
+            "result_limit_msg", f"Result limit: {max_results_in_host}."
+        )
+    elif host_cut and result_cut:
+        data["comment"] = limits.get(
+            "host_result_limit_msg",
+            f"Host limit {max_hosts}; Result limit: {max_results_in_host}.",
+        )
+
+    return data
+
+
 class VulnerabilityPDFReport(Report):
     """
     Is used to generate vulnerability reports in PDF.
     It renders html and css templates given data struct and then translate
     the html document to PDF
     """
 
     __template = "vulnerability_report_pdf_template"
     __css_template = "vulnerability_report_pdf_css"
     media_type = "application/pdf"
     format = "binary"
 
     def apply(self, name: str, data: Dict, parameter: Dict):
-        logger.debug("got template: %s", self.__template)
+        data = enforce_limit(data, parameter)
         css = _load_template(self.__css_template, parameter).render(
             Context(parameter)
         )
-        html_template = _load_template(self.__template)
+        html_template = _load_template(self.__template, parameter)
         html = html_template.render(Context(_enrich(name, data, parameter)))
         html = _replace_inline_svg_with_img_tags(html)
         logger.debug("created html")
         pdf = HTML(string=html).write_pdf(stylesheets=[CSS(string=css)])
         logger.debug("created pdf")
         return pdf
```

### Comparing `pheme-21.4rc4/pheme/urls.py` & `pheme-21.5.0/pheme/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/urls.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -35,33 +35,29 @@
 from django.urls import path
 import pheme.version
 import pheme.views
 import pheme.parameter
 
 urlpatterns = [
     path(
-        'parameter/<str:key>',
+        "parameter/<str:key>",
         pheme.parameter.put_value,
-        name='put_value_parameters',
+        name="put_value_parameters",
     ),
+    path("parameter", pheme.parameter.put, name="put_parameter"),
+    path("cache/<str:key>", pheme.views.load_cache, name="load_cache"),
+    path("cache", pheme.views.store_cache, name="store_cache"),
+    path("unmodified", pheme.views.unmodified, name="unmodified"),
+    path("transform", pheme.views.transform, name="transform"),
+    path("transform/", pheme.views.transform),
     path(
-        'parameter',
-        pheme.parameter.put,
-        name='put_parameter',
-    ),
-    path('cache/<str:key>', pheme.views.load_cache, name='load_cache'),
-    path('cache', pheme.views.store_cache, name='store_cache'),
-    path('unmodified', pheme.views.unmodified, name='unmodified'),
-    path('transform', pheme.views.transform, name='transform'),
-    path('transform/', pheme.views.transform),
-    path(
-        'scanreport/data/description',
+        "scanreport/data/description",
         pheme.views.scanreport_data_description,
-        name='scanreport_data_description',
+        name="scanreport_data_description",
     ),
-    path('report/<str:name>', pheme.views.report, name='report'),
+    path("report/<str:name>", pheme.views.report, name="report"),
     path(
-        'template/elements/<str:name>',
+        "template/elements/<str:name>",
         pheme.views.template_elements,
-        name='template_elements',
+        name="template_elements",
     ),
 ]
```

### Comparing `pheme-21.4rc4/pheme/version/__init__.py` & `pheme-21.5.0/pheme/datalink.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- coding: utf-8 -*-
-# pheme/version/__init__.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from .__version__ import __version__
+import urllib
+import base64
+
+
+def as_datalink(data: bytes, file_format: str) -> str:
+    img = urllib.parse.quote(base64.b64encode(data))
+    return f"data:{file_format};base64,{img}"
```

### Comparing `pheme-21.4rc4/pheme/views.py` & `pheme-21.5.0/pheme/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/views.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -24,94 +24,75 @@
 
 
 from pheme.parser.xml import XMLFormParser, XMLParser
 from pheme.transformation import scanreport
 from pheme.storage import store, load
 from pheme.renderer import MarkDownTableRenderer, XMLRenderer, CSVRenderer
 from pheme.transformation.scanreport import model
+from pheme.version import __version__
 
 
-@api_view(['GET'])
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@api_view(["GET"])
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 def load_cache(request, key):
     return Response(load(key))
 
 
-@api_view(['POST'])
+@api_view(["POST"])
 @parser_classes([rest_framework.parsers.JSONParser])
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 def store_cache(request):
     key = request.data.get("key", "unknown")
-    data = request.data.get('value')
-    if request.data.get('append'):
+    data = request.data.get("value")
+    if request.data.get("append"):
         if isinstance(data, dict):
             cached = load(key) or {}
-            cached[data.get('name', 'unknown')] = data.get('content')
+            cached[data.get("name", "unknown")] = data.get("content")
             data = cached
     name = store(key, data, id_generator=str)
     return Response(name)
 
 
-@api_view(['POST'])
+@api_view(["POST"])
 @parser_classes([XMLParser, XMLFormParser])
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 def transform(request):
     name = store(
         "scanreport",
         dataclasses.asdict(scanreport.gvmd.transform(request.data)),
     )
     return Response(name)
 
 
-@api_view(['POST'])
+@api_view(["POST"])
 @parser_classes([XMLParser])
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 def unmodified(request):
     return Response(request.data)
 
 
-@api_view(['GET'])
-@renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-    ]
-)
+@api_view(["GET"])
+@renderer_classes([rest_framework.renderers.JSONRenderer])
 def template_elements(request: Request, name: str):
     def load_value_of(key) -> str:
         may_val = load(key) or {}
         return may_val
 
-    images = load_value_of("{}images".format(name))
+    images = load_value_of(f"{name}images")
     return Response(
         {
-            "template": load_value_of("{}html_template".format(name)),
-            "pdf_css": load_value_of("{}pdf_css".format(name)),
-            "html_css": load_value_of("{}html_css".format(name)),
+            "template": load_value_of(f"{name}html_template"),
+            "pdf_css": load_value_of(f"{name}pdf_css"),
+            "html_css": load_value_of(f"{name}html_css"),
             "images": images,
         }
     )
 
 
-@api_view(['GET'])
+@api_view(["GET"])
 @renderer_classes(
     [
         rest_framework.renderers.JSONRenderer,
         scanreport.renderer.ReportFormatPDFReport,
         scanreport.renderer.ReportFormatHTMLReport,
         scanreport.renderer.VulnerabilityHTMLReport,
         scanreport.renderer.VulnerabilityPDFReport,
@@ -121,36 +102,34 @@
 )
 def report(request: Request, name: str):
     def load_value_of(key) -> str:
         may_val = load(key) or {}
         return may_val
 
     if "report_format_editor" in request.accepted_media_type:
-        images = load_value_of("{}images".format(name))
+        images = load_value_of(f"{name}images")
         return Response(
             {
-                "template": load_value_of("{}html_template".format(name)),
+                "template": load_value_of(f"{name}html_template"),
                 "vulnerability_report": load(name),
-                "pdf_css": load_value_of("{}pdf_css".format(name)),
-                "html_css": load_value_of("{}html_css".format(name)),
+                "pdf_css": load_value_of(f"{name}pdf_css"),
+                "html_css": load_value_of(f"{name}html_css"),
                 "images": images,
             }
         )
     data = load(name)
-    if request.GET.get('without_overview'):
+    data["pheme_version"] = int("".join(filter(str.isdigit, __version__)))
+    if request.GET.get("without_overview"):
         # remove charts
-        data.pop('overview', None)
-    if request.META.get('HTTP_ACCEPT') == "application/xml":
+        data.pop("overview", None)
+    if request.META.get("HTTP_ACCEPT") == "application/xml":
         # XML needs exactly one root
-        data = {'report': data}
+        data = {"report": data}
     return Response(data)
 
 
-@api_view(['GET'])
+@api_view(["GET"])
 @renderer_classes(
-    [
-        rest_framework.renderers.JSONRenderer,
-        MarkDownTableRenderer,
-    ]
+    [rest_framework.renderers.JSONRenderer, MarkDownTableRenderer]
 )
 def scanreport_data_description(request):
     return Response(dataclasses.asdict(model.describe()))
```

### Comparing `pheme-21.4rc4/pheme/wsgi.py` & `pheme-21.5.0/pheme/wsgi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pheme/wsgi.py
-# Copyright (C) 2020-2021 Greenbone Networks GmbH
+# Copyright (C) 2020-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -25,10 +25,10 @@
 https://docs.djangoproject.com/en/3.1/howto/deployment/wsgi/
 """
 
 import os
 
 from django.core.wsgi import get_wsgi_application
 
-os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'pheme.settings')
+os.environ.setdefault("DJANGO_SETTINGS_MODULE", "pheme.settings")
 
 application = get_wsgi_application()
```

### Comparing `pheme-21.4rc4/pyproject.toml` & `pheme-21.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pheme"
-version = "21.4rc4"
-authors = ["Greenbone Networks GmbH <info@greenbone.net>"]
+version = "21.5.0"
+authors = ["Greenbone AG <info@greenbone.net>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 description = "report-generation-service"
 
 classifiers=[
   # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
   "Development Status :: 3 - Alpha",
@@ -16,41 +16,44 @@
   "Programming Language :: Python :: 3.8",
   "Operating System :: OS Independent",
   "Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-django = "=2.2.2"
-xmltodict = "^0.12.0"
-pyyaml = "^5.3.1"
-uritemplate = "^3.0.1"
-djangorestframework = "=3.9.0"
+django = "=2.2.28"
+xmltodict = ">=0.12,<0.14"
+pyyaml = ">=5.3.1,<7.0.0"
+uritemplate = ">=3.0.1,<5.0.0"
+djangorestframework = "=3.11.2"
 coreapi = "^2.3.3"
-weasyprint = ">=51,<53"
-rope = ">=0.17,<0.19"
+weasyprint = ">=51,<60"
+rope = ">=0.17,<1.10"
+sentry-sdk = { version="^1.1.0", optional=true}
 
 [tool.poetry.dev-dependencies]
-pylint = "^2.7.0"
-pylint-django = "^2.4.2"
-pytest = "^6.2.2"
-pytest-cov = "^2.11.1"
+pylint = "^2.13.9"
+pylint-django = "^2.5.3"
+pytest = "^7.4.0"
+pytest-cov = "^4.0.0"
 pytest-django = ">=3.9,<5.0"
-pytest-env = "^0.6.2"
-autohooks = "^2.2.0"
-autohooks-plugin-pylint = "^1.2.0"
-autohooks-plugin-black = {version = "^1.2.0", python = "^3.6"}
-black = {version = "20.8b1", python = "^3.6"}
-rope = ">=0.17,<0.19"
-pontos = "^0.3.0"
+pytest-env = "^0.8.1"
+autohooks = "^23.1.0"
+autohooks-plugin-pylint = "^22.8.1"
+autohooks-plugin-black = {version = "^22.11.0", python = "^3.6"}
+black = {version = "23.3.0", python = "^3.6"}
+rope = ">=0.17,<1.10"
+pontos = ">=21.6.3"
+
+[tool.poetry.extras]
+tracking = ["sentry-sdk"]
 
 [tool.black]
 line-length = 80
 target-version = ['py35', 'py36', 'py37', 'py38']
-skip-string-normalization = true
 exclude = '''
 /(
     \.git
   | \.hg
   | \.venv
   | \.circleci
   | \.github
```

### Comparing `pheme-21.4rc4/PKG-INFO` & `pheme-21.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 Metadata-Version: 2.1
 Name: pheme
-Version: 21.4rc4
+Version: 21.5.0
 Summary: report-generation-service
 License: AGPL-3.0-or-later
-Author: Greenbone Networks GmbH
+Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
+Provides-Extra: tracking
 Requires-Dist: coreapi (>=2.3.3,<3.0.0)
-Requires-Dist: django (==2.2.2)
-Requires-Dist: djangorestframework (==3.9.0)
-Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
-Requires-Dist: rope (>=0.17,<0.19)
-Requires-Dist: uritemplate (>=3.0.1,<4.0.0)
-Requires-Dist: weasyprint (>=51,<53)
-Requires-Dist: xmltodict (>=0.12.0,<0.13.0)
+Requires-Dist: django (==2.2.28)
+Requires-Dist: djangorestframework (==3.11.2)
+Requires-Dist: pyyaml (>=5.3.1,<7.0.0)
+Requires-Dist: rope (>=0.17,<1.10)
+Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0) ; extra == "tracking"
+Requires-Dist: uritemplate (>=3.0.1,<5.0.0)
+Requires-Dist: weasyprint (>=51,<60)
+Requires-Dist: xmltodict (>=0.12,<0.14)
 Description-Content-Type: text/markdown
 
-![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_logo_resilience_horizontal.png)
+![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # Pheme - Greenbone Static Report Generator <!-- omit in toc -->
 
+[![GitHub releases](https://img.shields.io/github/release-pre/greenbone/pheme.svg)](https://github.com/greenbone/pheme/releases)
+ [![PyPI release](https://img.shields.io/pypi/v/pheme.svg)](https://pypi.org/project/pheme/)
+ [![code test coverage](https://codecov.io/gh/greenbone/pheme/branch/main/graph/badge.svg)](https://codecov.io/gh/greenbone/pheme)
+ [![CircleCI](https://circleci.com/gh/greenbone/pheme/tree/main.svg?style=svg)](https://circleci.com/gh/greenbone/pheme/tree/main)
+ [![Build and test](https://github.com/greenbone/pheme/actions/workflows/ci-python.yml/badge.svg)](https://github.com/greenbone/pheme/actions/workflows/ci-python.yml)
+
 **pheme** is a service to create scan reports. It is maintained by [Greenbone Networks].
 
 [Pheme](https://en.wikipedia.org/wiki/Pheme) is the personification of fame and renown.
 
 Or in this case personification of a service to generate reports.
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Installation](#installation)
   - [Requirements](#requirements)
 - [Development](#development)
-- [API overview](#api-overview)
 - [Maintainer](#maintainer)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Installation
 
 ### Requirements
@@ -81,24 +90,14 @@
 
     poetry run autohooks activate
 
 Validate the activated git hooks by running
 
     poetry run autohooks check
 
-## API overview
-
-To get an overview of the API you can start this project
-
-```
-poetry run python manage.py runserver
-```
-
-and then go to [swagger](http://localhost:8000/docs/)
-
 ## Usage
 
 In order to prepare the data structure the XML report data needs to be posted to `pheme` with a grouping indicator (either by host or nvt).
 
 E.g.:
 
 ```
@@ -141,27 +140,27 @@
 
 ```
 > curl -v 'http://localhost:8000/report/scanreport-nvt-9a233b0d-713c-4f22-9e15-f6e5090873e3' -H 'Accept: application/pdf'
 ```
 
 ## Maintainer
 
-This project is maintained by [Greenbone Networks GmbH][Greenbone Networks]
+This project is maintained by [Greenbone AG][Greenbone Networks]
 
 ## Contributing
 
 Your contributions are highly appreciated. Please
 [create a pull request](https://github.com/greenbone/pheme/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/pheme/issues)
 first.
 
 ## License
 
-Copyright (C) 2020 [Greenbone Networks GmbH][Greenbone Networks]
+Copyright (C) 2020-2022 [Greenbone AG][Greenbone Networks]
 
 Licensed under the [GNU Affero General Public License v3.0 or later](LICENSE).
 
 [Greenbone Networks]: https://www.greenbone.net/
 [poetry]: https://python-poetry.org/
 [autohooks]: https://github.com/greenbone/autohooks
```

