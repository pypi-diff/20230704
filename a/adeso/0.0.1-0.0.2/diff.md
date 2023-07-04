# Comparing `tmp/adeso-0.0.1.tar.gz` & `tmp/adeso-0.0.2.tar.gz`

## Comparing `adeso-0.0.1.tar` & `adeso-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 adeso-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 adeso-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/__init__.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/adeso.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/about.html
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/favicon.png
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/index.html
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/robots.txt
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/steganography.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/version.json
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/0.fe90dd52.css
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/2.5529f161.css
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/4.ef1fb64e.css
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/_layout.b3d93ad9.css
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/_page.5529f161.css
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/_page.ef1fb64e.css
--rw-r--r--   0        0        0    77364 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
--rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
--rw-r--r--   0        0        0    15772 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
--rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
--rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
--rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/assets/github.1ea8d62e.svg
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/chunks/environment.9aa685ef.js
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/chunks/index.fcfb5454.js
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/chunks/scheduler.9254f691.js
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/chunks/singletons.5b0b2bfb.js
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/chunks/stores.b500bcea.js
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/entry/app.788394c9.js
--rw-r--r--   0        0        0    23995 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/entry/start.12349697.js
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/nodes/0.1a425b9e.js
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/nodes/1.5128def2.js
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/nodes/2.a3ea31da.js
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/nodes/3.d3ecf7d1.js
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 adeso-0.0.1/src/adeso/static/_app/immutable/nodes/4.fb178ad2.js
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 adeso-0.0.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 adeso-0.0.1/LICENSE
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 adeso-0.0.1/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 adeso-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 adeso-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 adeso-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 adeso-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/__init__.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/adeso.py
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/about.html
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/favicon.png
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/index.html
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/robots.txt
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/steganography.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/version.json
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/0.fe90dd52.css
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/2.5529f161.css
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/4.ef1fb64e.css
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/_layout.b3d93ad9.css
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/_page.5529f161.css
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/_page.ef1fb64e.css
+-rw-r--r--   0        0        0    77364 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
+-rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
+-rw-r--r--   0        0        0    15772 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
+-rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
+-rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/assets/github.1ea8d62e.svg
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/chunks/environment.9aa685ef.js
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/chunks/index.fcfb5454.js
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/chunks/scheduler.9254f691.js
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/chunks/singletons.5b0b2bfb.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/chunks/stores.b500bcea.js
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/entry/app.788394c9.js
+-rw-r--r--   0        0        0    23995 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/entry/start.12349697.js
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/nodes/0.1a425b9e.js
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/nodes/1.5128def2.js
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/nodes/2.a3ea31da.js
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/nodes/3.d3ecf7d1.js
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 adeso-0.0.2/src/adeso/static/_app/immutable/nodes/4.fb178ad2.js
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 adeso-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 adeso-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 adeso-0.0.2/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 adeso-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 adeso-0.0.2/PKG-INFO
```

### Comparing `adeso-0.0.1/requirements.txt` & `adeso-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/adeso.py` & `adeso-0.0.2/src/adeso/adeso.py`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/about.html` & `adeso-0.0.2/src/adeso/static/about.html`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/favicon.png` & `adeso-0.0.2/src/adeso/static/favicon.png`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/index.html` & `adeso-0.0.2/src/adeso/static/index.html`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/steganography.html` & `adeso-0.0.2/src/adeso/static/steganography.html`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/0.fe90dd52.css` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/0.fe90dd52.css`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/2.5529f161.css` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/2.5529f161.css`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/4.ef1fb64e.css` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/4.ef1fb64e.css`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/_layout.b3d93ad9.css` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/_layout.b3d93ad9.css`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/_page.5529f161.css` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/_page.5529f161.css`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/_page.ef1fb64e.css` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/_page.ef1fb64e.css`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/assets/github.1ea8d62e.svg` & `adeso-0.0.2/src/adeso/static/_app/immutable/assets/github.1ea8d62e.svg`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/chunks/index.fcfb5454.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/chunks/index.fcfb5454.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/chunks/scheduler.9254f691.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/chunks/scheduler.9254f691.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/chunks/singletons.5b0b2bfb.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/chunks/singletons.5b0b2bfb.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/entry/app.788394c9.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/entry/app.788394c9.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/entry/start.12349697.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/entry/start.12349697.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/nodes/0.1a425b9e.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/nodes/0.1a425b9e.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/nodes/1.5128def2.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/nodes/1.5128def2.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/nodes/2.a3ea31da.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/nodes/2.a3ea31da.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/nodes/3.d3ecf7d1.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/nodes/3.d3ecf7d1.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/src/adeso/static/_app/immutable/nodes/4.fb178ad2.js` & `adeso-0.0.2/src/adeso/static/_app/immutable/nodes/4.fb178ad2.js`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/.gitignore` & `adeso-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/LICENSE` & `adeso-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adeso-0.0.1/README.md` & `adeso-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,15 @@
  <ul style="margin-top: 5px;">
   <li>Large ciphertext and images can result in API lag or lockups for steganography.</li>
   <br>
   <li>The decode operation is done on the file selected, not the image displayed on the UI.</li>
  </ul>
  <h2 style="margin-top: 50px;"><b>Links:</b></h2>
  <p style="margin-top: 0px;">
- <br>
  <li><a href="https://wiki.bi0s.in/forensics/lsb/">Read the Docs</a></li>
  <br>
  <li><a href="https://wiki.bi0s.in/forensics/lsb/">PyPi Production</a></li>
  <br>
  <li><a href="https://wiki.bi0s.in/forensics/lsb/">PyPi Test</a></li>
  <h2 style="margin-top: 30px;"><b>Installation:</b></h2>
- <code style="margin-top: 5px;">
- <p><code>pip install adeso</code></p>
+ <code>pip install adeso</code>
 </div>
```

#### html2text {}

```diff
@@ -29,15 +29,14 @@
 ***** Gotchas: *****
     * Large ciphertext and images can result in API lag or lockups for
       steganography.
     *
     * The decode operation is done on the file selected, not the image
       displayed on the UI.
 ***** Links: *****
-
 Read_the_Docs
 
 PyPi_Production
 
 PyPi_Test
 ***** Installation: *****
 pip install adeso
```

### Comparing `adeso-0.0.1/pyproject.toml` & `adeso-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "adeso"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eric Jay Hartman", email="ericjayhartman@gmail.com" },
 ]
 description = "Application for Decryption, Encryption and Steganographic Operations"
 readme = "README.md"
 requires-python = ">=3.11.1"
 classifiers = [
```

### Comparing `adeso-0.0.1/PKG-INFO` & `adeso-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adeso
-Version: 0.0.1
+Version: 0.0.2
 Summary: Application for Decryption, Encryption and Steganographic Operations
 Project-URL: Github, https://github.com/HartmanAnalytics/adeso
 Project-URL: Documentation, https://HartmanAnalytics.github.io/adeso/
 Author-email: Eric Jay Hartman <ericjayhartman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -84,17 +84,15 @@
  <ul style="margin-top: 5px;">
   <li>Large ciphertext and images can result in API lag or lockups for steganography.</li>
   <br>
   <li>The decode operation is done on the file selected, not the image displayed on the UI.</li>
  </ul>
  <h2 style="margin-top: 50px;"><b>Links:</b></h2>
  <p style="margin-top: 0px;">
- <br>
  <li><a href="https://wiki.bi0s.in/forensics/lsb/">Read the Docs</a></li>
  <br>
  <li><a href="https://wiki.bi0s.in/forensics/lsb/">PyPi Production</a></li>
  <br>
  <li><a href="https://wiki.bi0s.in/forensics/lsb/">PyPi Test</a></li>
  <h2 style="margin-top: 30px;"><b>Installation:</b></h2>
- <code style="margin-top: 5px;">
- <p><code>pip install adeso</code></p>
+ <code>pip install adeso</code>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adeso Version: 0.0.1 Summary: Application for
+Metadata-Version: 2.1 Name: adeso Version: 0.0.2 Summary: Application for
 Decryption, Encryption and Steganographic Operations Project-URL: Github,
 https://github.com/HartmanAnalytics/adeso Project-URL: Documentation, https://
 HartmanAnalytics.github.io/adeso/ Author-email: Eric Jay Hartman
 gmail.com> License-File: LICENSE Classifier: License :: OSI Approved :: GNU
 Affero General Public License v3 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.11.1
 Requires-Dist: bitarray==2.7.6 Requires-Dist: blinker==1.6.2 Requires-Dist:
@@ -52,15 +52,14 @@
 ***** Gotchas: *****
     * Large ciphertext and images can result in API lag or lockups for
       steganography.
     *
     * The decode operation is done on the file selected, not the image
       displayed on the UI.
 ***** Links: *****
-
 Read_the_Docs
 
 PyPi_Production
 
 PyPi_Test
 ***** Installation: *****
 pip install adeso
```

