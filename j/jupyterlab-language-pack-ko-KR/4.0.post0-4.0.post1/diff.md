# Comparing `tmp/jupyterlab_language_pack_ko_kr-4.0.post0.tar.gz` & `tmp/jupyterlab_language_pack_ko_kr-4.0.post1.tar.gz`

## Comparing `jupyterlab_language_pack_ko_kr-4.0.post0.tar` & `jupyterlab_language_pack_ko_kr-4.0.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/.copier-answers.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   229138 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   111809 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    53687 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/LICENSE.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/README.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/pyproject.toml
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/.copier-answers.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   240992 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   111809 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    54837 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/LICENSE.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/README.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.0.post1/PKG-INFO
```

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/CONTRIBUTORS.md` & `jupyterlab_language_pack_ko_kr-4.0.post1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ko\n"
 "X-Crowdin-File: /main/extensions/jupyter_collaboration/locale/jupyter_collaboration.pot\n"
 "X-Crowdin-File-ID: 229\n"
 "Language-Team: Korean\n"
 "Language: ko_KR\n"
-"PO-Revision-Date: 2023-05-21 14:17\n"
+"PO-Revision-Date: 2023-07-04 11:34\n"
 
 #: /packages/collaboration-extension/schema/shared-link.json:/description
 msgctxt "schema"
 msgid "Shared link settings"
 msgstr ""
 
 #: /packages/collaboration-extension/schema/shared-link.json:/title
@@ -30,38 +30,38 @@
 msgstr ""
 
 #: /packages/collaboration-extension/schema/user-menu-bar.json:/title
 msgctxt "schema"
 msgid "User Menu Bar"
 msgstr ""
 
-#: packages/collaboration-extension/src/collaboration.ts:151
+#: packages/collaboration-extension/src/collaboration.ts:144 packages/collaboration-extension/src/collaboration.ts:151
 msgid "Collaboration"
 msgstr ""
 
-#: packages/collaboration-extension/src/collaboration.ts:156
+#: packages/collaboration-extension/src/collaboration.ts:149 packages/collaboration-extension/src/collaboration.ts:156
 msgid "User info"
 msgstr "내 정보"
 
-#: packages/collaboration-extension/src/collaboration.ts:157
+#: packages/collaboration-extension/src/collaboration.ts:150 packages/collaboration-extension/src/collaboration.ts:157
 msgid "User information"
 msgstr "내 정보"
 
-#: packages/collaboration-extension/src/collaboration.ts:169
+#: packages/collaboration-extension/src/collaboration.ts:162 packages/collaboration-extension/src/collaboration.ts:169
 msgid "Online Collaborators"
 msgstr "접속중인 협업자"
 
 #: packages/collaboration-extension/src/filebrowser.ts:199 packages/collaboration-extension/src/filebrowser.ts:248
 msgid "Warning"
 msgstr ""
 
 #: packages/collaboration-extension/src/filebrowser.ts:249
 msgid "Two collaborative sessions are accessing the file %1 simultaneously.\n"
 "                \n"
-"'Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress."
+"Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress."
 msgstr ""
 
 #: packages/collaboration-extension/src/filebrowser.ts:254
 msgid "Ok"
 msgstr ""
 
 #: packages/collaboration-extension/src/sharedlink.ts:37
@@ -116,19 +116,11 @@
 msgid "Copy Link"
 msgstr ""
 
 #: packages/collaboration/src/sharedlink.ts:60
 msgid "Copy the link to the Jupyter Server"
 msgstr ""
 
-#: packages/docprovider/src/yprovider.ts:125
-msgid "Session expired"
-msgstr ""
-
-#: packages/docprovider/src/yprovider.ts:126
-msgid "The document session expired. You need to reload this browser tab."
-msgstr ""
-
-#: packages/docprovider/src/yprovider.ts:129
-msgid "Reload"
+#: packages/docprovider/src/yprovider.ts:124
+msgid "Document session error"
 msgstr ""
```

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ko\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: Korean\n"
 "Language: ko_KR\n"
-"PO-Revision-Date: 2023-05-24 03:45\n"
+"PO-Revision-Date: 2023-06-15 04:14\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "마크다운 뷰어 설정"
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -1069,14 +1069,24 @@
 msgstr "최근 수정된 열을 보여 줄지 여부"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showLastModifiedColumn/title
 msgctxt "settings"
 msgid "Show last modified column"
 msgstr "최근 수정된 열 보기"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/sortNotebooksFirst/description
+msgctxt "settings"
+msgid "Whether to group the notebooks away from files"
+msgstr ""
+
+#: /packages/filebrowser-extension/schema/browser.json:/properties/sortNotebooksFirst/title
+msgctxt "settings"
+msgid "When sorting by name, group notebooks before other files"
+msgstr ""
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/useFuzzyFilter/description
 msgctxt "settings"
 msgid "Whether to apply fuzzy algorithm while filtering on file names"
 msgstr "파일명을 필터링 할때 퍼지 알고리즘을 적용할지 여부."
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/useFuzzyFilter/title
 msgctxt "settings"
@@ -2134,14 +2144,24 @@
 msgstr ""
 
 #: /packages/toc-extension/schema/registry.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Table of Contents"
 msgstr "목차"
 
+#: /packages/toc-extension/schema/registry.json:/properties/baseNumbering/description
+msgctxt "settings"
+msgid "The number headings start at."
+msgstr ""
+
+#: /packages/toc-extension/schema/registry.json:/properties/baseNumbering/title
+msgctxt "settings"
+msgid "Base level for the highest headings"
+msgstr ""
+
 #: /packages/toc-extension/schema/registry.json:/properties/includeOutput/description
 msgctxt "settings"
 msgid "Whether to include cell output in headings or not."
 msgstr ""
 
 #: /packages/toc-extension/schema/registry.json:/properties/includeOutput/title
 msgctxt "settings"
@@ -2582,39 +2602,39 @@
 msgid "Hide notifications"
 msgstr "알림 숨기기"
 
 #: packages/apputils-extension/src/notificationplugin.tsx:229
 msgid "Dismiss notification"
 msgstr "알림 지우기"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:402
+#: packages/apputils-extension/src/notificationplugin.tsx:401 packages/apputils-extension/src/notificationplugin.tsx:402
 msgid "Emit a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:403
+#: packages/apputils-extension/src/notificationplugin.tsx:402 packages/apputils-extension/src/notificationplugin.tsx:403
 msgid "Notification is described by {message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:440
+#: packages/apputils-extension/src/notificationplugin.tsx:439 packages/apputils-extension/src/notificationplugin.tsx:440
 msgid "Update a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:441
+#: packages/apputils-extension/src/notificationplugin.tsx:440 packages/apputils-extension/src/notificationplugin.tsx:441
 msgid "Notification is described by {id: string, message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:480
+#: packages/apputils-extension/src/notificationplugin.tsx:479 packages/apputils-extension/src/notificationplugin.tsx:480
 msgid "Dismiss a notification"
 msgstr ""
 
-#: packages/apputils-extension/src/notificationplugin.tsx:601
+#: packages/apputils-extension/src/notificationplugin.tsx:600 packages/apputils-extension/src/notificationplugin.tsx:601
 msgid "Show Notifications"
 msgstr "알림 표시하기"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:688
+#: packages/apputils-extension/src/notificationplugin.tsx:688 packages/apputils-extension/src/notificationplugin.tsx:689
 msgid "Hide notification"
 msgstr "알림 숨기기"
 
 #: packages/apputils-extension/src/palette.ts:101
 msgid "Command Palette Section"
 msgstr "명령어 팔레트 섹션"
 
@@ -2634,19 +2654,19 @@
 msgid "SEARCH"
 msgstr "검색"
 
 #: packages/apputils-extension/src/palette.ts:42
 msgid "Command Palette"
 msgstr "명령어 팔레트"
 
-#: packages/apputils-extension/src/shortcuts.tsx:183
+#: packages/apputils-extension/src/shortcuts.tsx:183 packages/apputils-extension/src/shortcuts.tsx:193
 msgid "Keyboard Shortcuts"
 msgstr ""
 
-#: packages/apputils-extension/src/shortcuts.tsx:187 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/running-extension/src/opentabs.ts:86
+#: packages/apputils-extension/src/shortcuts.tsx:187 packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/filebrowser/src/listing.ts:1415 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr "닫기"
 
 #: packages/apputils-extension/src/themesplugins.ts:112
 msgid "Switch to the provided `theme`."
 msgstr ""
 
@@ -2698,43 +2718,43 @@
 msgid "Theme"
 msgstr "테마"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:181
 msgid "Workspace loader"
 msgstr "작업 공간 로더"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:272 packages/docmanager/src/widgetmanager.ts:436 packages/docregistry/src/context.ts:1019
+#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:267 packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:275 packages/docmanager/src/widgetmanager.ts:436 packages/docmanager/src/widgetmanager.ts:442 packages/docregistry/src/context.ts:1015 packages/docregistry/src/context.ts:1019
 msgid "Save"
 msgstr "저장"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:79
+#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:79
 msgid "Save Current Workspace As…"
 msgstr "다른 이름으로 저장"
 
+#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:93
+msgid "Save Current Workspace"
+msgstr "저장"
+
 #: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr "JupyterLab 작업 공간 파일"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:93
-msgid "Save Current Workspace"
-msgstr "저장"
-
 #: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr "취소"
 
-#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:862 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147
+#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:862 packages/apputils/src/dialog.tsx:870 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147
 msgid "Cancel"
 msgstr "취소"
 
-#: packages/apputils/src/dialog.tsx:763 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/settingeditor/src/plugineditor.ts:133
+#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:770 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr "확인"
 
-#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:631
+#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:1757 packages/apputils/src/sessioncontext.tsx:631
 msgid "No Kernel"
 msgstr "커널 선택 안함"
 
 #: packages/apputils/src/kernelstatuses.tsx:29
 msgid "Unknown"
 msgstr "알 수 없음"
 
@@ -2798,75 +2818,87 @@
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr "%1개의 터미널, %2개의 커널 세션"
 
 #: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr "커널 시작 오류"
 
-#: packages/apputils/src/sessioncontext.tsx:1341 packages/filebrowser/src/opendialog.ts:83
+#: packages/apputils/src/sessioncontext.tsx:1341 packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:83
 msgid "Select"
 msgstr "선택"
 
-#: packages/apputils/src/sessioncontext.tsx:1348
+#: packages/apputils/src/sessioncontext.tsx:1345 packages/apputils/src/sessioncontext.tsx:1348 packages/apputils/src/sessioncontext.tsx:1353
 msgid "Select Kernel"
 msgstr "커널 선택"
 
-#: packages/apputils/src/sessioncontext.tsx:1353
+#: packages/apputils/src/sessioncontext.tsx:1353 packages/apputils/src/sessioncontext.tsx:1358
 msgid "Always start the preferred kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1354
+#: packages/apputils/src/sessioncontext.tsx:1354 packages/apputils/src/sessioncontext.tsx:1359
 msgid "Remember my choice and always start the preferred kernel"
 msgstr ""
 
-#: packages/apputils/src/sessioncontext.tsx:1415
+#: packages/apputils/src/sessioncontext.tsx:1415 packages/apputils/src/sessioncontext.tsx:1423
 msgid "Restart Kernel?"
 msgstr "커널을 재시작할까요?"
 
-#: packages/apputils/src/sessioncontext.tsx:1416
+#: packages/apputils/src/sessioncontext.tsx:1416 packages/apputils/src/sessioncontext.tsx:1424
 msgid "Do you want to restart the kernel of %1? All variables will be lost."
 msgstr "%1의 커널을 재시작합니다. 저장된 모든 변수가 초기화됩니다."
 
-#: packages/apputils/src/sessioncontext.tsx:1473
+#: packages/apputils/src/sessioncontext.tsx:1419 packages/hub-extension/src/index.ts:172
+msgid "Restart"
+msgstr "재시작"
+
+#: packages/apputils/src/sessioncontext.tsx:1420
+msgid "Confirm Kernel Restart"
+msgstr ""
+
+#: packages/apputils/src/sessioncontext.tsx:1429
+msgid "Cancel Kernel Restart"
+msgstr ""
+
+#: packages/apputils/src/sessioncontext.tsx:1473 packages/apputils/src/sessioncontext.tsx:1484
 msgid "Select kernel for:"
 msgstr "커널을 선택하세요:"
 
-#: packages/apputils/src/sessioncontext.tsx:1607
+#: packages/apputils/src/sessioncontext.tsx:1607 packages/apputils/src/sessioncontext.tsx:1618
 msgid "Start Preferred Kernel"
 msgstr "선호하는 커널 시작"
 
-#: packages/apputils/src/sessioncontext.tsx:1622
+#: packages/apputils/src/sessioncontext.tsx:1622 packages/apputils/src/sessioncontext.tsx:1633
 msgid "Start Other Kernel"
 msgstr "다른 커널 시작"
 
-#: packages/apputils/src/sessioncontext.tsx:1679
+#: packages/apputils/src/sessioncontext.tsx:1679 packages/apputils/src/sessioncontext.tsx:1690
 msgid "Use Kernel from Preferred Session"
 msgstr "선호하는 세션의 커널 사용"
 
-#: packages/apputils/src/sessioncontext.tsx:1694
+#: packages/apputils/src/sessioncontext.tsx:1694 packages/apputils/src/sessioncontext.tsx:1705
 msgid "Use Kernel from Other Session"
 msgstr "다른 세션의 커널 사용"
 
-#: packages/apputils/src/sessioncontext.tsx:1744
+#: packages/apputils/src/sessioncontext.tsx:1744 packages/apputils/src/sessioncontext.tsx:1755
 msgid "Use No Kernel"
 msgstr "커널 사용하지 않음"
 
-#: packages/apputils/src/sessioncontext.tsx:1768
+#: packages/apputils/src/sessioncontext.tsx:1768 packages/apputils/src/sessioncontext.tsx:1779
 msgid "Path:"
 msgstr "경로:"
 
-#: packages/apputils/src/sessioncontext.tsx:1769
+#: packages/apputils/src/sessioncontext.tsx:1769 packages/apputils/src/sessioncontext.tsx:1780
 msgid "Name:"
 msgstr "이름:"
 
-#: packages/apputils/src/sessioncontext.tsx:1770
+#: packages/apputils/src/sessioncontext.tsx:1770 packages/apputils/src/sessioncontext.tsx:1781
 msgid "Kernel Name:"
 msgstr "커널 이름:"
 
-#: packages/apputils/src/sessioncontext.tsx:1771
+#: packages/apputils/src/sessioncontext.tsx:1771 packages/apputils/src/sessioncontext.tsx:1782
 msgid "Kernel Id:"
 msgstr "커널 Id:"
 
 #: packages/apputils/src/thememanager.ts:371
 msgid "Neither theme %1 nor default %2 loaded."
 msgstr "테마 %1 혹은 기본 %2 모두 로딩되지 않았습니다."
 
@@ -3703,15 +3735,15 @@
 msgid "HTTP"
 msgstr ""
 
 #: packages/codemirror/src/language.ts:996
 msgid "IDL"
 msgstr ""
 
-#: packages/codemirror/src/theme.ts:215
+#: packages/codemirror/src/theme.ts:215 packages/codemirror/src/theme.ts:225
 msgid "codemirror"
 msgstr "codeMirror"
 
 #: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr "콘솔"
 
@@ -3771,39 +3803,47 @@
 msgid "Shut down the console?"
 msgstr "콘솔을 종료 하겠습니까?"
 
 #: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2357
 msgid "Are you sure you want to close \"%1\"?"
 msgstr "\"%1\"을 닫으시겠습니까?"
 
-#: packages/console-extension/src/index.ts:684
+#: packages/console-extension/src/index.ts:668
+msgid "Cancel console Shut Down"
+msgstr ""
+
+#: packages/console-extension/src/index.ts:671
+msgid "Confirm console Shut Down"
+msgstr ""
+
+#: packages/console-extension/src/index.ts:684 packages/console-extension/src/index.ts:691
 msgid "Inject some code in a console."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:705 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059
+#: packages/console-extension/src/index.ts:705 packages/console-extension/src/index.ts:712 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059
 msgid "Change Kernel…"
 msgstr "커널 변경"
 
-#: packages/console-extension/src/index.ts:717 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070
+#: packages/console-extension/src/index.ts:717 packages/console-extension/src/index.ts:724 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070
 msgid "Get Kernel"
 msgstr ""
 
-#: packages/console-extension/src/index.ts:799
+#: packages/console-extension/src/index.ts:799 packages/console-extension/src/index.ts:806
 msgid "Execute with Shift+Enter"
 msgstr "Shift+Enter 로 실행"
 
-#: packages/console-extension/src/index.ts:800
+#: packages/console-extension/src/index.ts:800 packages/console-extension/src/index.ts:807
 msgid "Execute with Enter"
 msgstr "Enter 로 실행"
 
-#: packages/console-extension/src/index.ts:844 packages/fileeditor-extension/src/commands.ts:1005 packages/notebook-extension/src/index.ts:1974
+#: packages/console-extension/src/index.ts:844 packages/console-extension/src/index.ts:851 packages/fileeditor-extension/src/commands.ts:1005 packages/notebook-extension/src/index.ts:1974
 msgid "Display the completion helper."
 msgstr ""
 
-#: packages/console-extension/src/index.ts:855 packages/fileeditor-extension/src/commands.ts:1016 packages/notebook-extension/src/index.ts:1984
+#: packages/console-extension/src/index.ts:855 packages/console-extension/src/index.ts:862 packages/fileeditor-extension/src/commands.ts:1016 packages/notebook-extension/src/index.ts:1984
 msgid "Select the completion suggestion."
 msgstr ""
 
 #: packages/console/src/panel.ts:316
 msgid "Name: %1\n"
 msgstr "이름: %1\n"
 
@@ -4019,15 +4059,15 @@
 msgid "Type"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr ""
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258 packages/filebrowser/src/listing.ts:2275
 msgid "Name"
 msgstr "이름"
 
 #: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr "변수"
 
@@ -4051,55 +4091,59 @@
 msgid "Render variable: %1"
 msgstr ""
 
 #: packages/debugger/src/service.ts:378
 msgid "Globals"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1060
+#: packages/docmanager-extension/src/index.tsx:1002 packages/docmanager-extension/src/index.tsx:999
+msgid "Autosave Documents"
+msgstr "문서 자동 저장"
+
+#: packages/docmanager-extension/src/index.tsx:1060 packages/docmanager-extension/src/index.tsx:1063
 msgid "New View for %1"
 msgstr "새로운 %1 뷰포트 열기"
 
-#: packages/docmanager-extension/src/index.tsx:1084
+#: packages/docmanager-extension/src/index.tsx:1084 packages/docmanager-extension/src/index.tsx:1087
 msgid "Rename%1…"
 msgstr "이름변경 %1..."
 
-#: packages/docmanager-extension/src/index.tsx:1098
+#: packages/docmanager-extension/src/index.tsx:1098 packages/docmanager-extension/src/index.tsx:1101
 msgid "Duplicate %1"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1113
+#: packages/docmanager-extension/src/index.tsx:1113 packages/docmanager-extension/src/index.tsx:1116
 msgid "Delete %1"
 msgstr "%1 삭제"
 
-#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1127 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430
+#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1126 packages/docmanager-extension/src/index.tsx:1127 packages/docmanager-extension/src/index.tsx:1130 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser-extension/src/index.ts:926 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:434
 msgid "Delete"
 msgstr "삭제"
 
-#: packages/docmanager-extension/src/index.tsx:1124
+#: packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:1127
 msgid "Are you sure you want to delete %1"
 msgstr "정말로 %1를 삭제하시겠습니까?"
 
-#: packages/docmanager-extension/src/index.tsx:1141
+#: packages/docmanager-extension/src/index.tsx:1141 packages/docmanager-extension/src/index.tsx:1144
 msgid "Show in File Browser"
 msgstr "파일 탐색기에서 보기"
 
-#: packages/docmanager-extension/src/index.tsx:1207
+#: packages/docmanager-extension/src/index.tsx:1207 packages/docmanager-extension/src/index.tsx:1210
 msgid "Are you sure you want to revert the %1 to checkpoint? "
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1213
+#: packages/docmanager-extension/src/index.tsx:1213 packages/docmanager-extension/src/index.tsx:1216
 msgid "This cannot be undone."
 msgstr "이 작업은 되돌릴 수 없습니다."
 
-#: packages/docmanager-extension/src/index.tsx:1220
+#: packages/docmanager-extension/src/index.tsx:1220 packages/docmanager-extension/src/index.tsx:1223
 msgid "The checkpoint was last updated at: "
 msgstr "체크 포인트가 갱신됨: "
 
-#: packages/docmanager-extension/src/index.tsx:1254
+#: packages/docmanager-extension/src/index.tsx:1254 packages/docmanager-extension/src/index.tsx:1257
 msgid "Choose a checkpoint"
 msgstr ""
 
 #: packages/docmanager-extension/src/index.tsx:344
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
@@ -4119,39 +4163,39 @@
 "만일 존재하지 않는 파일 유형이나 뷰어를 지정하거나, 혹은 뷰어가 주어진 파일 유형에서 \n"
 "파일을 열수 없는 경우, 이러한 재정의는 작동하지 않는다. \n\n"
 "사용가능한 뷰어:\n"
 "%1\n\n"
 "사용가능한 파일 유형:\n"
 "%2"
 
-#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367
+#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367 packages/filebrowser-extension/src/index.ts:371
 msgid "Download"
 msgstr "다운로드"
 
 #: packages/docmanager-extension/src/index.tsx:475
 msgid "Download the file to your computer"
 msgstr "파일을 당신의 컴퓨터에 다운로드"
 
 #: packages/docmanager-extension/src/index.tsx:483
 msgid "Cannot Download"
 msgstr "다운로드할 수 없음"
 
-#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:968
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:847 packages/docmanager-extension/src/index.tsx:968 packages/docmanager-extension/src/index.tsx:971
 msgid "No context found for current widget!"
 msgstr "현재 위젯에서는 컨텍스트를 찾을 수 없습니다!"
 
-#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:892 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1078 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:570 packages/filebrowser-extension/src/index.ts:892 packages/filebrowser-extension/src/index.ts:896 packages/htmlviewer-extension/src/index.tsx:206
 msgid "File Operations"
 msgstr "파일 명령"
 
-#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772
+#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772 packages/filebrowser-extension/src/index.ts:776
 msgid "Open in New Browser Tab"
 msgstr "새로운 탐색 창에서 열기"
 
-#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/logconsole-extension/src/index.tsx:376
+#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/filebrowser/src/browser.ts:252 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr "오류"
 
 #: packages/docmanager-extension/src/index.tsx:704
 msgid "Open the provided `path`."
 msgstr ""
 
@@ -4191,107 +4235,111 @@
 msgid "No checkpoints are available for this %1."
 msgstr ""
 
 #: packages/docmanager-extension/src/index.tsx:793
 msgid "Revert %1 to checkpoint"
 msgstr "체크포인트로 %1 되돌리기"
 
-#: packages/docmanager-extension/src/index.tsx:797 packages/docregistry/src/context.ts:805
+#: packages/docmanager-extension/src/index.tsx:797 packages/docmanager-extension/src/index.tsx:798 packages/docregistry/src/context.ts:801 packages/docregistry/src/context.ts:805
 msgid "Revert"
 msgstr "되돌리기"
 
-#: packages/docmanager-extension/src/index.tsx:820
+#: packages/docmanager-extension/src/index.tsx:799
+msgid "Revert to Checkpoint"
+msgstr ""
+
+#: packages/docmanager-extension/src/index.tsx:820 packages/docmanager-extension/src/index.tsx:823
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:826
+#: packages/docmanager-extension/src/index.tsx:826 packages/docmanager-extension/src/index.tsx:829
 msgid "Save and create checkpoint"
 msgstr "저장"
 
-#: packages/docmanager-extension/src/index.tsx:832
+#: packages/docmanager-extension/src/index.tsx:832 packages/docmanager-extension/src/index.tsx:835
 msgid "Save %1"
 msgstr "%1 저장"
 
-#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:967 packages/notebook/src/default-toolbar.tsx:68
+#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:846 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:857 packages/docmanager-extension/src/index.tsx:967 packages/docmanager-extension/src/index.tsx:970 packages/notebook/src/default-toolbar.tsx:68
 msgid "Cannot Save"
 msgstr "저장 불가"
 
-#: packages/docmanager-extension/src/index.tsx:855 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:855 packages/docmanager-extension/src/index.tsx:858 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr "읽기 전용 문서입니다"
 
-#: packages/docmanager-extension/src/index.tsx:870
+#: packages/docmanager-extension/src/index.tsx:870 packages/docmanager-extension/src/index.tsx:873
 msgid "Rename file"
 msgstr "파일 이름 변경"
 
-#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager/src/dialogs.ts:57 packages/filebrowser-extension/src/index.ts:1197
+#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:874 packages/docmanager/src/dialogs.ts:57 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1197 packages/filebrowser-extension/src/index.ts:1201
 msgid "Rename"
 msgstr "이름 변경"
 
-#: packages/docmanager-extension/src/index.tsx:872
+#: packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:875
 msgid "File name"
 msgstr "파일 이름"
 
-#: packages/docmanager-extension/src/index.tsx:876 packages/docmanager/src/widgetmanager.ts:414
+#: packages/docmanager-extension/src/index.tsx:876 packages/docmanager-extension/src/index.tsx:879 packages/docmanager/src/widgetmanager.ts:414 packages/docmanager/src/widgetmanager.ts:420
 msgid "Do not ask me again."
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:877
+#: packages/docmanager-extension/src/index.tsx:877 packages/docmanager-extension/src/index.tsx:880
 msgid "If checked, you will not be asked to rename future untitled files when saving them."
 msgstr "활성화되면, untitled 파일을 저장할 때 이름을 바꿀것을 요청하지 않는다."
 
-#: packages/docmanager-extension/src/index.tsx:934
+#: packages/docmanager-extension/src/index.tsx:934 packages/docmanager-extension/src/index.tsx:937
 msgid "Save All"
 msgstr "모두 저장"
 
-#: packages/docmanager-extension/src/index.tsx:935
+#: packages/docmanager-extension/src/index.tsx:935 packages/docmanager-extension/src/index.tsx:938
 msgid "Save all open documents"
 msgstr "열린 문서 모두 저장하기"
 
-#: packages/docmanager-extension/src/index.tsx:958
+#: packages/docmanager-extension/src/index.tsx:958 packages/docmanager-extension/src/index.tsx:961
 msgid "Save %1 As…"
 msgstr "%1 다른 이름으로 저장..."
 
-#: packages/docmanager-extension/src/index.tsx:959
+#: packages/docmanager-extension/src/index.tsx:959 packages/docmanager-extension/src/index.tsx:962
 msgid "Save with new path"
 msgstr "새로운 경로에 저장"
 
-#: packages/docmanager-extension/src/index.tsx:999
-msgid "Autosave Documents"
-msgstr "문서 자동 저장"
-
-#: packages/docmanager/src/dialogs.ts:114
+#: packages/docmanager/src/dialogs.ts:114 packages/docmanager/src/dialogs.ts:117
 msgid "Overwrite file?"
 msgstr "덮어쓰시겠습니까?"
 
-#: packages/docmanager/src/dialogs.ts:115
+#: packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:118
 msgid "\"%1\" already exists, overwrite?"
 msgstr "\"%1\" 파일이 이미 있습니다. 덮어쓸까요?"
 
-#: packages/docmanager/src/dialogs.ts:118 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
+#: packages/docmanager/src/dialogs.ts:118 packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:805 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:841 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
 msgid "Overwrite"
 msgstr "덮어쓰기"
 
-#: packages/docmanager/src/dialogs.ts:182
+#: packages/docmanager/src/dialogs.ts:123
+msgid "Overwrite Existing File"
+msgstr ""
+
+#: packages/docmanager/src/dialogs.ts:182 packages/docmanager/src/dialogs.ts:188
 msgid "File Path"
 msgstr "파일 경로"
 
-#: packages/docmanager/src/dialogs.ts:187
+#: packages/docmanager/src/dialogs.ts:187 packages/docmanager/src/dialogs.ts:193
 msgid "New Name"
 msgstr "새 이름"
 
-#: packages/docmanager/src/dialogs.ts:52
+#: packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/dialogs.ts:59
 msgid "Rename File"
 msgstr "파일 이름 변경"
 
-#: packages/docmanager/src/dialogs.ts:65 packages/filebrowser/src/listing.ts:1875
+#: packages/docmanager/src/dialogs.ts:65 packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1875 packages/filebrowser/src/listing.ts:1891
 msgid "Rename Error"
 msgstr "이름 변경 에러"
 
-#: packages/docmanager/src/dialogs.ts:67
+#: packages/docmanager/src/dialogs.ts:67 packages/docmanager/src/dialogs.ts:70
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" 은 파일명으로 유효하지 않습니다. 이름은 한글자 이상이어야 하고, \"/\", \"\\\", \":\" 을 포함하지 않아야 합니다."
 
 #: packages/docmanager/src/savingstatus.tsx:58
 msgid "Saving completed"
 msgstr "저장 완료"
 
@@ -4321,75 +4369,91 @@
 msgid "Last Checkpoint: %1"
 msgstr "최근 체크포인트: %1"
 
 #: packages/docmanager/src/widgetmanager.ts:397
 msgid "Close and save"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:404
+#: packages/docmanager/src/widgetmanager.ts:399
+msgid "Close and save Document"
+msgstr ""
+
+#: packages/docmanager/src/widgetmanager.ts:400
+msgid "Close Document"
+msgstr ""
+
+#: packages/docmanager/src/widgetmanager.ts:404 packages/docmanager/src/widgetmanager.ts:408
 msgid "Close without saving"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:409 packages/notebook/src/searchprovider.ts:509
+#: packages/docmanager/src/widgetmanager.ts:409
+msgid "Close Document without saving"
+msgstr ""
+
+#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:415 packages/notebook/src/searchprovider.ts:509
 msgid "Confirmation"
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:410
+#: packages/docmanager/src/widgetmanager.ts:410 packages/docmanager/src/widgetmanager.ts:416
 msgid "Please confirm you want to close \"%1\"."
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:415
+#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:421
 msgid "If checked, no confirmation to close a document will be asked in the future."
 msgstr ""
 
-#: packages/docmanager/src/widgetmanager.ts:437
+#: packages/docmanager/src/widgetmanager.ts:437 packages/docmanager/src/widgetmanager.ts:443
 msgid "Save as"
 msgstr "다른 이름으로 저장"
 
-#: packages/docmanager/src/widgetmanager.ts:439
+#: packages/docmanager/src/widgetmanager.ts:439 packages/docmanager/src/widgetmanager.ts:445
 msgid "Save your work"
 msgstr "저장하시겠습니까?"
 
-#: packages/docmanager/src/widgetmanager.ts:440
+#: packages/docmanager/src/widgetmanager.ts:440 packages/docmanager/src/widgetmanager.ts:446
 msgid "Save changes in \"%1\" before closing?"
 msgstr "\"%1\"에 대한 변경 내용을 저장할까요?"
 
-#: packages/docmanager/src/widgetmanager.ts:443
+#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:450
 msgid "Discard"
 msgstr "버리기"
 
-#: packages/docregistry/src/context.ts:1021
+#: packages/docmanager/src/widgetmanager.ts:451
+msgid "Discard changes to file"
+msgstr ""
+
+#: packages/docregistry/src/context.ts:1017 packages/docregistry/src/context.ts:1021
 msgid "Save File As…"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:894
+#: packages/docregistry/src/context.ts:627 packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:890 packages/docregistry/src/context.ts:894
 msgid "File Save Error for %1"
 msgstr "파일 저장 오류 %1"
 
-#: packages/docregistry/src/context.ts:695
+#: packages/docregistry/src/context.ts:691 packages/docregistry/src/context.ts:695
 msgid "File Load Error for %1"
 msgstr "파일 로딩 오류 %1"
 
-#: packages/docregistry/src/context.ts:798
+#: packages/docregistry/src/context.ts:794 packages/docregistry/src/context.ts:798
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr "\"%1\"이 가장 최근에 열거나 저장된 이후에 디스크에서 변경되었습니다. \n"
 "디스크의 파일에 지금 열려있는 버전으로 덮어 쓰겠습니까? 아니면\n"
 "디스크의 버전을 가져와 현재 파일을 되돌리겠습니까?"
 
-#: packages/docregistry/src/context.ts:814
+#: packages/docregistry/src/context.ts:810 packages/docregistry/src/context.ts:814
 msgid "File Changed"
 msgstr "파일 변경됨"
 
-#: packages/docregistry/src/context.ts:840
+#: packages/docregistry/src/context.ts:836 packages/docregistry/src/context.ts:840
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "'%1\"가 이미 존재합니다. 바꾸시겠습니까?"
 
-#: packages/docregistry/src/context.ts:849
+#: packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:849
 msgid "File Overwrite?"
 msgstr "파일을 덮어 쓰겠습니까?"
 
 #: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr "렌더링 실패: %1"
 
@@ -4693,192 +4757,196 @@
 msgid "Version: %1"
 msgstr ""
 
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1014
-msgid "Open from Path…"
-msgstr "열기"
-
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839
+#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:1018 packages/filebrowser-extension/src/index.ts:1020 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:841 packages/filebrowser-extension/src/index.ts:843
 msgid "Open %1"
 msgstr "%1 열기"
 
-#: packages/filebrowser-extension/src/index.ts:1016
+#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1018
+msgid "Open from Path…"
+msgstr "열기"
+
+#: packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:1020
 msgid "Open from path"
 msgstr "경로에서 열기"
 
-#: packages/filebrowser-extension/src/index.ts:1025
+#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:1029
 msgid "Path"
 msgstr "경로"
 
-#: packages/filebrowser-extension/src/index.ts:1027
+#: packages/filebrowser-extension/src/index.ts:1027 packages/filebrowser-extension/src/index.ts:1031
 msgid "Open Path"
 msgstr "경로 열기"
 
-#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:849
+#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1032 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:1121 packages/filebrowser-extension/src/index.ts:849 packages/filebrowser-extension/src/index.ts:853
 msgid "Open"
 msgstr "열기"
 
-#: packages/filebrowser-extension/src/index.ts:1063
+#: packages/filebrowser-extension/src/index.ts:1063 packages/filebrowser-extension/src/index.ts:1067
 msgid "Could not find path: %1"
 msgstr "다음 경로를 찾을 수 없습니다:%1"
 
-#: packages/filebrowser-extension/src/index.ts:1065
+#: packages/filebrowser-extension/src/index.ts:1065 packages/filebrowser-extension/src/index.ts:1069
 msgid "Cannot open"
 msgstr "열 수 없음"
 
-#: packages/filebrowser-extension/src/index.ts:1130 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488
+#: packages/filebrowser-extension/src/index.ts:1130 packages/filebrowser-extension/src/index.ts:1134 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488 packages/terminal-extension/src/index.ts:494
 msgid "Paste"
 msgstr "붙여넣기"
 
-#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser/src/opendialog.ts:153
+#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser-extension/src/index.ts:1147 packages/filebrowser/src/opendialog.ts:153
 msgid "New Folder"
 msgstr "새 폴더"
 
-#: packages/filebrowser-extension/src/index.ts:1155
+#: packages/filebrowser-extension/src/index.ts:1155 packages/filebrowser-extension/src/index.ts:1159
 msgid "New File"
 msgstr "새 파일"
 
-#: packages/filebrowser-extension/src/index.ts:1167 packages/fileeditor-extension/src/commands.ts:809
+#: packages/filebrowser-extension/src/index.ts:1167 packages/filebrowser-extension/src/index.ts:1171 packages/fileeditor-extension/src/commands.ts:809
 msgid "New Markdown File"
 msgstr "새 마크다운 파일"
 
-#: packages/filebrowser-extension/src/index.ts:1179
+#: packages/filebrowser-extension/src/index.ts:1179 packages/filebrowser-extension/src/index.ts:1183
 msgid "Refresh the file browser."
 msgstr "파일 탐색창 새로고침"
 
-#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser/src/opendialog.ts:168
+#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser-extension/src/index.ts:1184 packages/filebrowser/src/opendialog.ts:168
 msgid "Refresh File List"
 msgstr "파일 목록 새로 고침"
 
-#: packages/filebrowser-extension/src/index.ts:1220
+#: packages/filebrowser-extension/src/index.ts:1220 packages/filebrowser-extension/src/index.ts:1224
 msgid "Copy Path"
 msgstr "경로 복사"
 
-#: packages/filebrowser-extension/src/index.ts:1232 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1232 packages/filebrowser-extension/src/index.ts:1236 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
 msgid "Shut Down Kernel"
 msgstr "커널 종료"
 
-#: packages/filebrowser-extension/src/index.ts:1236
+#: packages/filebrowser-extension/src/index.ts:1236 packages/filebrowser-extension/src/index.ts:1240
 msgid "Show Last Modified Column"
 msgstr "최근 수정된 열 보기"
 
-#: packages/filebrowser-extension/src/index.ts:1252
+#: packages/filebrowser-extension/src/index.ts:1252 packages/filebrowser-extension/src/index.ts:1272
 msgid "Show File Size Column"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1268
+#: packages/filebrowser-extension/src/index.ts:1256
+msgid "Sort Notebooks Above Files"
+msgstr ""
+
+#: packages/filebrowser-extension/src/index.ts:1268 packages/filebrowser-extension/src/index.ts:1288
 msgid "Show Hidden Files"
 msgstr "숨긴 파일 표시"
 
-#: packages/filebrowser-extension/src/index.ts:1285
+#: packages/filebrowser-extension/src/index.ts:1285 packages/filebrowser-extension/src/index.ts:1305
 msgid "Show File Checkboxes"
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:1301
+#: packages/filebrowser-extension/src/index.ts:1301 packages/filebrowser-extension/src/index.ts:1321
 msgid "Search on File Names"
 msgstr "파일 이름으로 검색"
 
-#: packages/filebrowser-extension/src/index.ts:1370
+#: packages/filebrowser-extension/src/index.ts:1370 packages/filebrowser-extension/src/index.ts:1390
 msgid "No browser for path"
 msgstr "경로의 탐색기가 없습니다."
 
-#: packages/filebrowser-extension/src/index.ts:389
+#: packages/filebrowser-extension/src/index.ts:389 packages/filebrowser-extension/src/index.ts:393
 msgid "Copy Download Link"
 msgstr "다운로드 링크 복사"
 
-#: packages/filebrowser-extension/src/index.ts:432
+#: packages/filebrowser-extension/src/index.ts:432 packages/filebrowser-extension/src/index.ts:436
 msgid "File Browser Section"
 msgstr "파일 탐색기 섹션"
 
-#: packages/filebrowser-extension/src/index.ts:443
+#: packages/filebrowser-extension/src/index.ts:443 packages/filebrowser-extension/src/index.ts:447
 msgid "File Browser (%1)"
 msgstr "파일 탐색기 (%1)"
 
-#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser/src/browser.ts:75
+#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:449 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser-extension/src/index.ts:501 packages/filebrowser/src/browser.ts:75
 msgid "File Browser"
 msgstr "파일 탐색기"
 
-#: packages/filebrowser-extension/src/index.ts:475
+#: packages/filebrowser-extension/src/index.ts:475 packages/filebrowser-extension/src/index.ts:479
 msgid "Filter files by name"
 msgstr "이름으로 파일 검색"
 
-#: packages/filebrowser-extension/src/index.ts:508
+#: packages/filebrowser-extension/src/index.ts:508 packages/filebrowser-extension/src/index.ts:512
 msgid "Open the file browser for the provided `path`."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:540
+#: packages/filebrowser-extension/src/index.ts:540 packages/filebrowser-extension/src/index.ts:544
 msgid "Hide the file browser."
 msgstr ""
 
-#: packages/filebrowser-extension/src/index.ts:550
+#: packages/filebrowser-extension/src/index.ts:550 packages/filebrowser-extension/src/index.ts:554
 msgid "Show Active File in File Browser"
 msgstr "활성화된 파일 보이기"
 
-#: packages/filebrowser-extension/src/index.ts:647
+#: packages/filebrowser-extension/src/index.ts:647 packages/filebrowser-extension/src/index.ts:651
 msgid "Copy Shareable Link"
 msgstr "공유 가능한 링크 복사"
 
-#: packages/filebrowser-extension/src/index.ts:771
+#: packages/filebrowser-extension/src/index.ts:771 packages/filebrowser-extension/src/index.ts:775
 msgid "Open in Simple Mode"
 msgstr "단순 모드로 열기"
 
-#: packages/filebrowser-extension/src/index.ts:837
+#: packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:841
 msgid "Open from URL…"
 msgstr "URL에서 열기..."
 
-#: packages/filebrowser-extension/src/index.ts:839
+#: packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:843
 msgid "Open from URL"
 msgstr "URL에서 열기"
 
-#: packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:850
 msgid "URL"
 msgstr "URL"
 
-#: packages/filebrowser-extension/src/index.ts:848
+#: packages/filebrowser-extension/src/index.ts:848 packages/filebrowser-extension/src/index.ts:852
 msgid "Open URL"
 msgstr "URL 열기"
 
-#: packages/filebrowser-extension/src/index.ts:867
+#: packages/filebrowser-extension/src/index.ts:867 packages/filebrowser-extension/src/index.ts:871
 msgid "Could not open URL: %1"
 msgstr "다음 URL을 열 수 없습니다:%1"
 
-#: packages/filebrowser-extension/src/index.ts:869
+#: packages/filebrowser-extension/src/index.ts:869 packages/filebrowser-extension/src/index.ts:873
 msgid "Cannot fetch"
 msgstr "가져올 수 없음"
 
-#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser-extension/src/index.ts:886 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr "업로드 에러"
 
-#: packages/filebrowser-extension/src/index.ts:935 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463
+#: packages/filebrowser-extension/src/index.ts:935 packages/filebrowser-extension/src/index.ts:939 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463 packages/terminal-extension/src/index.ts:469
 msgid "Copy"
 msgstr "복사하기"
 
-#: packages/filebrowser-extension/src/index.ts:948 packages/fileeditor-extension/src/commands.ts:913
+#: packages/filebrowser-extension/src/index.ts:948 packages/filebrowser-extension/src/index.ts:952 packages/fileeditor-extension/src/commands.ts:913
 msgid "Cut"
 msgstr "잘라내기"
 
-#: packages/filebrowser-extension/src/index.ts:960
+#: packages/filebrowser-extension/src/index.ts:960 packages/filebrowser-extension/src/index.ts:964
 msgid "Duplicate"
 msgstr "복제하기"
 
-#: packages/filebrowser-extension/src/index.ts:964
+#: packages/filebrowser-extension/src/index.ts:964 packages/filebrowser-extension/src/index.ts:968
 msgid "Update the file browser to display the provided `path`."
 msgstr ""
 
-#: packages/filebrowser/src/browser.ts:372
+#: packages/filebrowser/src/browser.ts:372 packages/filebrowser/src/browser.ts:388
 msgid "Directory not found"
 msgstr "디렉토리를 찾지 못했습니다"
 
-#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/model.ts:298
+#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/browser.ts:389 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr "디렉토리를 찾지 못했습니다: \"%1\""
 
 #: packages/filebrowser/src/browser.ts:69
 msgid "file browser"
 msgstr "파일 탐색기"
 
@@ -4886,147 +4954,147 @@
 msgid "Open Error"
 msgstr "열기 오류"
 
 #: packages/filebrowser/src/crumbs.ts:302
 msgid "Move Error"
 msgstr "이동 오류"
 
-#: packages/filebrowser/src/listing.ts:1120
+#: packages/filebrowser/src/listing.ts:1120 packages/filebrowser/src/listing.ts:1136
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr "디렉토리 열기"
 
-#: packages/filebrowser/src/listing.ts:1395
+#: packages/filebrowser/src/listing.ts:1395 packages/filebrowser/src/listing.ts:1411
 msgid "Error Uploading Folder"
 msgstr "폴더 업로드 오류"
 
-#: packages/filebrowser/src/listing.ts:1396
+#: packages/filebrowser/src/listing.ts:1396 packages/filebrowser/src/listing.ts:1412
 msgid "Drag and Drop is currently not supported for folders"
 msgstr "폴더에 대해서는 드래그 앤 드랍이 현재 지원되지 않습니다."
 
-#: packages/filebrowser/src/listing.ts:1515
+#: packages/filebrowser/src/listing.ts:1515 packages/filebrowser/src/listing.ts:1531
 msgctxt "showErrorMessage"
 msgid "Error while copying/moving files"
 msgstr "파일 복사/이동 중 오류 발생"
 
-#: packages/filebrowser/src/listing.ts:1814
+#: packages/filebrowser/src/listing.ts:1814 packages/filebrowser/src/listing.ts:1830
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr "삭제 실패"
 
-#: packages/filebrowser/src/listing.ts:1877
+#: packages/filebrowser/src/listing.ts:1877 packages/filebrowser/src/listing.ts:1893
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" 은 파일명으로 유효하지 않습니다. 이름은 한글자 이상이어야 하고, \"/\", \"\\\", \":\" 을 포함하지 않아야 합니다."
 
-#: packages/filebrowser/src/listing.ts:1896
+#: packages/filebrowser/src/listing.ts:1896 packages/filebrowser/src/listing.ts:1912
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr "이름 변경 에러"
 
-#: packages/filebrowser/src/listing.ts:2260
+#: packages/filebrowser/src/listing.ts:2260 packages/filebrowser/src/listing.ts:2277
 msgid "Last Modified"
 msgstr "마지막 수정"
 
-#: packages/filebrowser/src/listing.ts:2261
+#: packages/filebrowser/src/listing.ts:2261 packages/filebrowser/src/listing.ts:2278
 msgid "File Size"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2549
+#: packages/filebrowser/src/listing.ts:2549 packages/filebrowser/src/listing.ts:2566
 msgid "Name: %1"
 msgstr "이름: %1"
 
-#: packages/filebrowser/src/listing.ts:2555
+#: packages/filebrowser/src/listing.ts:2555 packages/filebrowser/src/listing.ts:2572
 msgid "\n"
 "Size: %1"
 msgstr "\n"
 "크기: %1"
 
-#: packages/filebrowser/src/listing.ts:2565
+#: packages/filebrowser/src/listing.ts:2565 packages/filebrowser/src/listing.ts:2582
 msgid "\n"
 "Path: %1"
 msgstr "\n"
 "경로: %1"
 
-#: packages/filebrowser/src/listing.ts:2572
+#: packages/filebrowser/src/listing.ts:2572 packages/filebrowser/src/listing.ts:2589
 msgid "\n"
 "Created: %1"
 msgstr "\n"
 "생성: %1"
 
-#: packages/filebrowser/src/listing.ts:2578
+#: packages/filebrowser/src/listing.ts:2578 packages/filebrowser/src/listing.ts:2595
 msgid "\n"
 "Modified: %1"
 msgstr "\n"
 "수정: %1"
 
-#: packages/filebrowser/src/listing.ts:2583
+#: packages/filebrowser/src/listing.ts:2583 packages/filebrowser/src/listing.ts:2600
 msgid "\n"
 "Writable: %1"
 msgstr "\n"
 "수정가능: %1"
 
-#: packages/filebrowser/src/listing.ts:2608
+#: packages/filebrowser/src/listing.ts:2608 packages/filebrowser/src/listing.ts:2625
 msgid "Deselect directory \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2609
+#: packages/filebrowser/src/listing.ts:2609 packages/filebrowser/src/listing.ts:2626
 msgid "Select directory \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2612
+#: packages/filebrowser/src/listing.ts:2612 packages/filebrowser/src/listing.ts:2629
 msgid "Deselect file \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2613
+#: packages/filebrowser/src/listing.ts:2613 packages/filebrowser/src/listing.ts:2630
 msgid "Select file \"%1\""
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:2687
+#: packages/filebrowser/src/listing.ts:2687 packages/filebrowser/src/listing.ts:2704
 msgid "%1 Item"
 msgid_plural "%1 Items"
 msgstr[0] "%1 항목"
 
-#: packages/filebrowser/src/listing.ts:396
+#: packages/filebrowser/src/listing.ts:396 packages/filebrowser/src/listing.ts:400
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr "붙여넣기 오류"
 
-#: packages/filebrowser/src/listing.ts:416
+#: packages/filebrowser/src/listing.ts:416 packages/filebrowser/src/listing.ts:420
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr "정말 %1를 영구적으로 삭제하시겠습니까?"
 
-#: packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420 packages/filebrowser/src/listing.ts:424
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] "%1 개의 선택한 아이템을 영구적으로 삭제하시겠습니까?"
 
-#: packages/filebrowser/src/listing.ts:472
+#: packages/filebrowser/src/listing.ts:472 packages/filebrowser/src/listing.ts:476
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr "중복 파일"
 
-#: packages/filebrowser/src/listing.ts:512
+#: packages/filebrowser/src/listing.ts:512 packages/filebrowser/src/listing.ts:516
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr "커널 종료"
 
-#: packages/filebrowser/src/listing.ts:852
+#: packages/filebrowser/src/listing.ts:852 packages/filebrowser/src/listing.ts:856
 msgid "Deselect all files and directories"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:853
+#: packages/filebrowser/src/listing.ts:853 packages/filebrowser/src/listing.ts:857
 msgid "Select all files and directories"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:906
+#: packages/filebrowser/src/listing.ts:906 packages/filebrowser/src/listing.ts:910
 msgid "unknown"
 msgstr ""
 
-#: packages/filebrowser/src/listing.ts:908
+#: packages/filebrowser/src/listing.ts:908 packages/filebrowser/src/listing.ts:912
 msgid "%1\n"
 "Kernel: %2"
 msgstr "%1\n"
 "커널: %2"
 
 #: packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
@@ -5378,18 +5446,14 @@
 msgstr "서버에 접근할 수 없습니다"
 
 #: packages/hub-extension/src/index.ts:167
 msgid "Your server at %1 is not running.\n"
 "Would you like to restart it?"
 msgstr "%1 서버가 실행되고 있지 않습니다. 재시작 할까요?"
 
-#: packages/hub-extension/src/index.ts:172
-msgid "Restart"
-msgstr "재시작"
-
 #: packages/hub-extension/src/index.ts:67
 msgid "Restart Server"
 msgstr "서버 재시작"
 
 #: packages/hub-extension/src/index.ts:68
 msgid "Request that the Hub restart this server"
 msgstr "허브가 이 이서버를 재시작 하도록 요청"
@@ -6219,33 +6283,37 @@
 msgid "Notebook is already trusted"
 msgstr "노트북은 이미 신뢰함 상태임"
 
 #: packages/notebook/src/actions.tsx:2061
 msgid "Trust this notebook?"
 msgstr "이 노트북을 신뢰함으로 설정하겠습니까?"
 
-#: packages/notebook/src/actions.tsx:2064
+#: packages/notebook/src/actions.tsx:2064 packages/notebook/src/actions.tsx:2065
 msgid "Trust"
 msgstr ""
 
-#: packages/notebook/src/actions.tsx:2279
+#: packages/notebook/src/actions.tsx:2066
+msgid "Confirm Trusting this notebook"
+msgstr ""
+
+#: packages/notebook/src/actions.tsx:2279 packages/notebook/src/actions.tsx:2282
 msgid "Kernel Terminating"
 msgstr "커널 종료"
 
-#: packages/notebook/src/actions.tsx:2280
+#: packages/notebook/src/actions.tsx:2280 packages/notebook/src/actions.tsx:2283
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr "%1에 대한 커널이 종료된 것으로 보입니다. 지금은 어떤 셀도 실행할 수 없습니다."
 
-#: packages/notebook/src/actions.tsx:2290
+#: packages/notebook/src/actions.tsx:2290 packages/notebook/src/actions.tsx:2293
 msgid "Cell not executed due to pending input"
-msgstr "이전 실행이 예기치 못하게 종료되었습니다"
+msgstr "대기 중인 입력이 있어 실행이 취소되었습니다"
 
-#: packages/notebook/src/actions.tsx:2291
+#: packages/notebook/src/actions.tsx:2291 packages/notebook/src/actions.tsx:2294
 msgid "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again."
-msgstr "이전 실행을 제출하고 다시 시도해보십시오."
+msgstr "대기 중인 입력이 있어 교착 상태를 방지하기 위해 실행을 취소했습니다. 대기 중인 입력을 마무리하고 다시 시도해주세요."
 
 #: packages/notebook/src/default-toolbar.tsx:141
 msgid "Cut the selected cells"
 msgstr "선택한 셀 잘라내기"
 
 #: packages/notebook/src/default-toolbar.tsx:161
 msgid "Copy the selected cells"
@@ -6419,15 +6487,15 @@
 msgid "Handle Local Link"
 msgstr "로컬 링크 핸들"
 
 #: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "이 HTML 출력은 인라인 스크립트를 갖고 있습니다. 당신의 JupyterLab 세션에서 이러한 Javascript 코드를 실행하시겠습니까?"
 
-#: packages/rendermime/src/widgets.ts:428
+#: packages/rendermime/src/widgets.ts:428 packages/rendermime/src/widgets.ts:446
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr "JavaScript 출력이 JupyterLab에서 비활성화 되었습니다."
 
 #: packages/running-extension/src/index.ts:66
 msgid "Running Terminals and Kernels"
 msgstr "현재 실행중인 탭"
 
@@ -6708,23 +6776,23 @@
 msgstr "터미널"
 
 #: packages/terminal-extension/src/index.ts:191
 msgctxt "menu"
 msgid "Terminal Theme"
 msgstr "터미널 테마"
 
-#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534
+#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534 packages/terminal-extension/src/index.ts:540
 msgid "Inherit"
 msgstr "시스템 설정 사용"
 
-#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535
+#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535 packages/terminal-extension/src/index.ts:541
 msgid "Light"
 msgstr "라이트"
 
-#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536
+#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536 packages/terminal-extension/src/index.ts:542
 msgid "Dark"
 msgstr "다크"
 
 #: packages/terminal-extension/src/index.ts:316
 msgid "Terminals"
 msgstr "터미널"
 
@@ -6736,47 +6804,47 @@
 msgid "New Terminal"
 msgstr "새 터미널"
 
 #: packages/terminal-extension/src/index.ts:351
 msgid "Start a new terminal session"
 msgstr "새 터미널 세션 시작"
 
-#: packages/terminal-extension/src/index.ts:389
+#: packages/terminal-extension/src/index.ts:389 packages/terminal-extension/src/index.ts:395
 msgid "Open a terminal by its `name`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:407
+#: packages/terminal-extension/src/index.ts:407 packages/terminal-extension/src/index.ts:413
 msgid "Refresh Terminal"
 msgstr "터미널 새로 고침"
 
-#: packages/terminal-extension/src/index.ts:408
+#: packages/terminal-extension/src/index.ts:408 packages/terminal-extension/src/index.ts:414
 msgid "Refresh the current terminal session"
 msgstr "현재 터미널 세션 새로 고침"
 
-#: packages/terminal-extension/src/index.ts:492
+#: packages/terminal-extension/src/index.ts:492 packages/terminal-extension/src/index.ts:498
 msgid "Shutdown Terminal"
 msgstr "터미널 종료"
 
-#: packages/terminal-extension/src/index.ts:506
+#: packages/terminal-extension/src/index.ts:506 packages/terminal-extension/src/index.ts:512
 msgid "Increase Terminal Font Size"
 msgstr "터미널 글자 크기 크게"
 
-#: packages/terminal-extension/src/index.ts:520
+#: packages/terminal-extension/src/index.ts:520 packages/terminal-extension/src/index.ts:526
 msgid "Decrease Terminal Font Size"
 msgstr "터미널 글자 크기 작게"
 
-#: packages/terminal-extension/src/index.ts:542
+#: packages/terminal-extension/src/index.ts:542 packages/terminal-extension/src/index.ts:548
 msgid "Set terminal theme to the provided `theme`."
 msgstr ""
 
-#: packages/terminal-extension/src/index.ts:550
+#: packages/terminal-extension/src/index.ts:550 packages/terminal-extension/src/index.ts:556
 msgid "Use Terminal Theme: %1"
 msgstr "터미널 테마 사용: %1"
 
-#: packages/terminal-extension/src/index.ts:553
+#: packages/terminal-extension/src/index.ts:553 packages/terminal-extension/src/index.ts:559
 msgid "Set the terminal theme"
 msgstr "터미널 테마 설정"
 
 #: packages/terminal/src/widget.ts:345
 msgid "Terminal %1"
 msgstr "터미널 %1"
```

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ko\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_lsp/locale/jupyterlab_lsp.pot\n"
 "X-Crowdin-File-ID: 199\n"
 "Language-Team: Korean\n"
 "Language: ko_KR\n"
-"PO-Revision-Date: 2023-04-27 12:40\n"
+"PO-Revision-Date: 2023-05-29 08:42\n"
 
 #: /packages/jupyterlab-lsp/schema/completion.json:/description
 msgctxt "schema"
 msgid "LSP Completion settings."
 msgstr "LSP 자동 완성 설정"
 
 #: /packages/jupyterlab-lsp/schema/completion.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/diagnostics.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/highlights.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/hover.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/jump_to.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/rename.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/signature.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/syntax_highlighting.json:/jupyter.lab.setting-icon-label
@@ -220,14 +220,24 @@
 msgstr "패널에 표시하거나 편집기에서 강조 표시해서는 안 되는 진단 메시지와 일치하는 정규식입니다."
 
 #: /packages/jupyterlab-lsp/schema/diagnostics.json:/properties/ignoreMessagesPatterns/title
 msgctxt "settings"
 msgid "Diagnostic messages to ignore"
 msgstr "무시할 진단 메시지"
 
+#: /packages/jupyterlab-lsp/schema/diagnostics.json:/properties/ignoreSeverities/description
+msgctxt "settings"
+msgid "Severities of diagnostics which should not be shown in the panel nor highlighted in the editor."
+msgstr ""
+
+#: /packages/jupyterlab-lsp/schema/diagnostics.json:/properties/ignoreSeverities/title
+msgctxt "settings"
+msgid "Diagnostic severity levels to ignore"
+msgstr ""
+
 #: /packages/jupyterlab-lsp/schema/diagnostics.json:/title
 msgctxt "schema"
 msgid "Code Diagnostics"
 msgstr "진단 코드"
 
 #: /packages/jupyterlab-lsp/schema/highlights.json:/description
 msgctxt "schema"
@@ -405,14 +415,44 @@
 "  serverSettings: {\n"
 "    \"pyls.plugins.pydocstyle.enabled\": true,\n"
 "    \"pyls.plugins.pyflakes.enabled\": false,\n"
 "    \"pyls.plugins.flake8.enabled\": true\n"
 "  }\n"
 "}"
 
+#: /packages/jupyterlab-lsp/schema/plugin.json:/properties/language_servers/description
+msgctxt "settings"
+msgid "Language-server specific configuration, keyed by implementation, e.g: \n\n"
+"pyls: {\n"
+"  serverSettings: {\n"
+"    pyls: {\n"
+"      plugins: {\n"
+"        pydocstyle: {\n"
+"          enabled: true\n"
+"        },\n"
+"        pyflakes: {\n"
+"          enabled: false\n"
+"        },\n"
+"        flake8: {\n"
+"          enabled: true\n"
+"        }\n"
+"      }\n"
+"    }\n"
+"  }\n"
+"}\n\n"
+"Alternatively, using dotted naming convention:\n\n"
+"pyls: {\n"
+"  serverSettings: {\n"
+"    \"pyls.plugins.pydocstyle.enabled\": true,\n"
+"    \"pyls.plugins.pyflakes.enabled\": false,\n"
+"    \"pyls.plugins.flake8.enabled\": true\n"
+"  }\n"
+"}"
+msgstr ""
+
 #: /packages/jupyterlab-lsp/schema/plugin.json:/properties/language_servers/title
 msgctxt "settings"
 msgid "Language Server"
 msgstr "언어 서버"
 
 #: /packages/jupyterlab-lsp/schema/plugin.json:/properties/logAllCommunication/description
 msgctxt "settings"
```

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: ko\n"
 "X-Crowdin-File: /main/extensions/notebook/locale/notebook.pot\n"
 "X-Crowdin-File-ID: 231\n"
 "Language-Team: Korean\n"
 "Language: ko_KR\n"
-"PO-Revision-Date: 2023-05-21 14:18\n"
+"PO-Revision-Date: 2023-07-04 11:34\n"
 
 #: /packages/application-extension/schema/menus.json:/description /packages/application-extension/schema/menus.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Menu Entries"
 msgstr ""
 
 #: /packages/application-extension/schema/menus.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
@@ -25,14 +25,34 @@
 msgstr ""
 
 #: /packages/application-extension/schema/pages.json:/description /packages/application-extension/schema/pages.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Pages"
 msgstr ""
 
+#: /packages/application-extension/schema/shell.json:/description
+msgctxt "schema"
+msgid "Notebook Shell layout settings."
+msgstr ""
+
+#: /packages/application-extension/schema/shell.json:/properties/layout/description
+msgctxt "settings"
+msgid "Overrides default widget position in the application layout"
+msgstr ""
+
+#: /packages/application-extension/schema/shell.json:/properties/layout/title
+msgctxt "settings"
+msgid "Customize shell widget positioning"
+msgstr ""
+
+#: /packages/application-extension/schema/shell.json:/title
+msgctxt "schema"
+msgid "Notebook Shell"
+msgstr ""
+
 #: /packages/application-extension/schema/title.json:/description /packages/application-extension/schema/title.json:/title
 msgctxt "schema"
 msgid "Title widget"
 msgstr ""
 
 #: /packages/application-extension/schema/top.json:/description
 msgctxt "schema"
@@ -60,19 +80,14 @@
 msgstr ""
 
 #: /packages/application-extension/schema/zen.json:/description /packages/application-extension/schema/zen.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Zen Mode"
 msgstr ""
 
-#: /packages/documentsearch-extension/schema/notebookShellWidgetListener.json:/description /packages/documentsearch-extension/schema/notebookShellWidgetListener.json:/title
-msgctxt "schema"
-msgid "Jupyter Notebook DocumentSearch Settings"
-msgstr ""
-
 #: /packages/help-extension/schema/open.json:/description /packages/help-extension/schema/open.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Help Menu Entries"
 msgstr ""
 
 #: /packages/lab-extension/schema/interface-switcher.json:/description
 msgctxt "schema"
@@ -130,14 +145,24 @@
 msgstr ""
 
 #: /packages/notebook-extension/schema/scroll-output.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Notebook"
 msgstr ""
 
+#: /packages/tree-extension/schema/file-actions.json:/description
+msgctxt "schema"
+msgid "File Browser widget - File Actions settings."
+msgstr ""
+
+#: /packages/tree-extension/schema/file-actions.json:/title
+msgctxt "schema"
+msgid "File Browser Widget - File Actions"
+msgstr ""
+
 #: /packages/tree-extension/schema/widget.json:/definitions/toolbarItem/properties/args/title
 msgctxt "settings"
 msgid "Command arguments"
 msgstr ""
 
 #: /packages/tree-extension/schema/widget.json:/definitions/toolbarItem/properties/command/title
 msgctxt "settings"
@@ -211,60 +236,64 @@
 msgstr ""
 
 #: /packages/tree-extension/schema/widget.json:/title
 msgctxt "schema"
 msgid "File Browser Widget"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:119
+#: packages/application-extension/src/index.ts:1058
+msgid "Toggle Zen Mode"
+msgstr ""
+
+#: packages/application-extension/src/index.ts:141
 msgid "Are you sure you want to exit Jupyter Notebook?\n\n"
 "Any unsaved changes will be lost."
 msgstr ""
 
-#: packages/application-extension/src/index.ts:258
+#: packages/application-extension/src/index.ts:310
 msgid "Open JupyterLab"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:266
+#: packages/application-extension/src/index.ts:318
 msgid "File Browser"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:415
+#: packages/application-extension/src/index.ts:376
+msgid "Handle Local Link"
+msgstr ""
+
+#: packages/application-extension/src/index.ts:586
 msgid "Rename…"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:481
+#: packages/application-extension/src/index.ts:652
 msgid "Show Header"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:571
+#: packages/application-extension/src/index.ts:742
 msgid "Show %1 in the left sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:576
+#: packages/application-extension/src/index.ts:747
 msgid "Show %1 in the right sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:581
+#: packages/application-extension/src/index.ts:752
 msgid "Show %1 in the sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:696
+#: packages/application-extension/src/index.ts:867
 msgid "Left Sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:698
+#: packages/application-extension/src/index.ts:869
 msgid "Right Sidebar"
 msgstr ""
 
-#: packages/application-extension/src/index.ts:887
-msgid "Toggle Zen Mode"
-msgstr ""
-
-#: packages/application/src/shell.ts:203 packages/application/src/shell.ts:207
+#: packages/application/src/shell.ts:238 packages/application/src/shell.ts:242
 msgid "Collapse %1 side panel"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:114
 msgid "Version: %1"
 msgstr ""
 
@@ -272,15 +301,15 @@
 msgid "© 2021-2023 Jupyter Notebook Contributors"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:131
 msgid "Dismiss"
 msgstr ""
 
-#: packages/help-extension/src/index.tsx:77 packages/lab-extension/src/index.ts:178
+#: packages/help-extension/src/index.tsx:77 packages/lab-extension/src/index.ts:221
 msgid "Help"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:80
 msgid "About %1"
 msgstr ""
 
@@ -288,38 +317,46 @@
 msgid "JUPYTER NOTEBOOK ON GITHUB"
 msgstr ""
 
 #: packages/help-extension/src/index.tsx:93
 msgid "CONTRIBUTOR LIST"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:131
-msgid "Notebook"
+#: packages/lab-extension/src/index.ts:104
+msgid "JupyterLab"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:132 packages/lab-extension/src/index.ts:142
+#: packages/lab-extension/src/index.ts:105 packages/lab-extension/src/index.ts:115 packages/lab-extension/src/index.ts:95
 msgid "Open in %1"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:141
-msgid "JupyterLab"
+#: packages/lab-extension/src/index.ts:114
+msgid "NbClassic"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:181
+#: packages/lab-extension/src/index.ts:184
+msgid "Open in..."
+msgstr ""
+
+#: packages/lab-extension/src/index.ts:224
 msgid "Launch Jupyter Notebook File Browser"
 msgstr ""
 
-#: packages/lab-extension/src/index.ts:82
-msgid "Open in..."
+#: packages/lab-extension/src/index.ts:94
+msgid "Notebook"
 msgstr ""
 
-#: packages/notebook-extension/src/index.ts:107
+#: packages/notebook-extension/src/index.ts:109
 msgid "Last Checkpoint: %1"
 msgstr ""
 
+#: packages/notebook-extension/src/index.ts:150
+msgid "Close and Shut Down Notebook"
+msgstr ""
+
 #: packages/notebook-extension/src/trusted.tsx:75
 msgid "JavaScript enabled for notebook display"
 msgstr ""
 
 #: packages/notebook-extension/src/trusted.tsx:76
 msgid "JavaScript disabled for notebook display"
 msgstr ""
@@ -328,31 +365,35 @@
 msgid "Not Trusted"
 msgstr ""
 
 #: packages/notebook-extension/src/trusted.tsx:79
 msgid "Trusted"
 msgstr ""
 
-#: packages/tree-extension/src/index.ts:232
+#: packages/tree-extension/src/fileactions.tsx:39
+msgid "Select items to perform actions on them."
+msgstr ""
+
+#: packages/tree-extension/src/index.ts:284
 msgid "Files"
 msgstr ""
 
-#: packages/tree-extension/src/index.ts:234
+#: packages/tree-extension/src/index.ts:286
 msgid "File Browser Section"
 msgstr ""
 
-#: packages/tree-extension/src/index.ts:249
+#: packages/tree-extension/src/index.ts:300
 msgid "Upload"
 msgstr ""
 
-#: packages/tree-extension/src/index.ts:267
+#: packages/tree-extension/src/index.ts:318
 msgid "Filter files by name"
 msgstr ""
 
-#: packages/tree-extension/src/index.ts:289
+#: packages/tree-extension/src/index.ts:340
 msgid "Running"
 msgstr ""
 
-#: packages/tree-extension/src/index.ts:91
+#: packages/tree-extension/src/index.ts:95
 msgid "New"
 msgstr ""
```

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_ko_kr-4.0.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/.gitignore` & `jupyterlab_language_pack_ko_kr-4.0.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/LICENSE.txt` & `jupyterlab_language_pack_ko_kr-4.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/pyproject.toml` & `jupyterlab_language_pack_ko_kr-4.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.0.post0/PKG-INFO` & `jupyterlab_language_pack_ko_kr-4.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-ko-KR
-Version: 4.0.post0
+Version: 4.0.post1
 Summary: JupyterLab Korean (South Korea) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

