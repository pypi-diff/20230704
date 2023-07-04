# Comparing `tmp/jupyterlab_language_pack_fr_fr-4.0.post0.tar.gz` & `tmp/jupyterlab_language_pack_fr_fr-4.0.post1.tar.gz`

## Comparing `jupyterlab_language_pack_fr_fr-4.0.post0.tar` & `jupyterlab_language_pack_fr_fr-4.0.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/.copier-answers.yml
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   250015 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   112963 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    56212 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/LICENSE.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/README.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/pyproject.toml
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/.copier-answers.yml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   262371 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   112963 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    58181 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0    13537 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/LICENSE.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/README.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlab_language_pack_fr_fr-4.0.post1/PKG-INFO
```

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/CONTRIBUTORS.md` & `jupyterlab_language_pack_fr_fr-4.0.post1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_collaboration.po`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: fr\n"
 "X-Crowdin-File: /main/extensions/jupyter_collaboration/locale/jupyter_collaboration.pot\n"
 "X-Crowdin-File-ID: 229\n"
 "Language-Team: French\n"
 "Language: fr_FR\n"
-"PO-Revision-Date: 2023-05-21 14:17\n"
+"PO-Revision-Date: 2023-07-04 11:34\n"
 
 #: /packages/collaboration-extension/schema/shared-link.json:/description
 msgctxt "schema"
 msgid "Shared link settings"
 msgstr "Paramètres du lien partagé"
 
 #: /packages/collaboration-extension/schema/shared-link.json:/title
@@ -30,38 +30,38 @@
 msgstr "Paramètres de la barre de menu utilisateur."
 
 #: /packages/collaboration-extension/schema/user-menu-bar.json:/title
 msgctxt "schema"
 msgid "User Menu Bar"
 msgstr "Barre de menu utilisateur"
 
-#: packages/collaboration-extension/src/collaboration.ts:151
+#: packages/collaboration-extension/src/collaboration.ts:144 packages/collaboration-extension/src/collaboration.ts:151
 msgid "Collaboration"
 msgstr "Collaboration"
 
-#: packages/collaboration-extension/src/collaboration.ts:156
+#: packages/collaboration-extension/src/collaboration.ts:149 packages/collaboration-extension/src/collaboration.ts:156
 msgid "User info"
 msgstr "Informations utilisateur"
 
-#: packages/collaboration-extension/src/collaboration.ts:157
+#: packages/collaboration-extension/src/collaboration.ts:150 packages/collaboration-extension/src/collaboration.ts:157
 msgid "User information"
 msgstr "Informations de l'utilisateur"
 
-#: packages/collaboration-extension/src/collaboration.ts:169
+#: packages/collaboration-extension/src/collaboration.ts:162 packages/collaboration-extension/src/collaboration.ts:169
 msgid "Online Collaborators"
 msgstr "Collaborateurs en ligne"
 
 #: packages/collaboration-extension/src/filebrowser.ts:199 packages/collaboration-extension/src/filebrowser.ts:248
 msgid "Warning"
 msgstr "Avertissement"
 
 #: packages/collaboration-extension/src/filebrowser.ts:249
 msgid "Two collaborative sessions are accessing the file %1 simultaneously.\n"
 "                \n"
-"'Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress."
+"Opening a document with multiple views simultaneously is not supported. Please close one view; otherwise, you might lose some of your progress."
 msgstr "Deux sessions collaboratives accèdent simultanément au fichier %1 .\n"
 "                \n"
 "Ouvrir un document avec des vues multiples simultanément n'est pas pris en charge. Veuillez fermer une vue; sinon, vous risquez de perdre une partie de vos modifications."
 
 #: packages/collaboration-extension/src/filebrowser.ts:254
 msgid "Ok"
 msgstr "Ok"
@@ -118,19 +118,11 @@
 msgid "Copy Link"
 msgstr "Copier le lien"
 
 #: packages/collaboration/src/sharedlink.ts:60
 msgid "Copy the link to the Jupyter Server"
 msgstr "Copier le lien vers le serveur Jupyter"
 
-#: packages/docprovider/src/yprovider.ts:125
-msgid "Session expired"
-msgstr "Session expirée"
-
-#: packages/docprovider/src/yprovider.ts:126
-msgid "The document session expired. You need to reload this browser tab."
-msgstr "La session du document a expiré. Vous devez recharger cet onglet du navigateur."
-
-#: packages/docprovider/src/yprovider.ts:129
-msgid "Reload"
-msgstr "Recharger"
+#: packages/docprovider/src/yprovider.ts:124
+msgid "Document session error"
+msgstr "Erreur de session du document"
```

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: fr\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: French\n"
 "Language: fr_FR\n"
-"PO-Revision-Date: 2023-05-21 14:17\n"
+"PO-Revision-Date: 2023-05-31 11:17\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "Paramètres du visualiseur Markdown."
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -1069,14 +1069,24 @@
 msgstr "Afficher/Masquer la dernière colonne modifiée"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showLastModifiedColumn/title
 msgctxt "settings"
 msgid "Show last modified column"
 msgstr "Afficher la dernière colonne modifiée"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/sortNotebooksFirst/description
+msgctxt "settings"
+msgid "Whether to group the notebooks away from files"
+msgstr "Regrouper ou non les notebooks séparément des autres fichiers"
+
+#: /packages/filebrowser-extension/schema/browser.json:/properties/sortNotebooksFirst/title
+msgctxt "settings"
+msgid "When sorting by name, group notebooks before other files"
+msgstr "Lors du tri par nom, regroupe les notebooks avant les autres fichiers"
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/useFuzzyFilter/description
 msgctxt "settings"
 msgid "Whether to apply fuzzy algorithm while filtering on file names"
 msgstr "Appliquer ou non un algorithme flou lors du filtrage sur les noms de fichiers"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/useFuzzyFilter/title
 msgctxt "settings"
@@ -2132,14 +2142,24 @@
 msgstr "Paramètres par défaut de la table des matières."
 
 #: /packages/toc-extension/schema/registry.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "Table of Contents"
 msgstr "Table des Matières"
 
+#: /packages/toc-extension/schema/registry.json:/properties/baseNumbering/description
+msgctxt "settings"
+msgid "The number headings start at."
+msgstr "L'index des titres commence à."
+
+#: /packages/toc-extension/schema/registry.json:/properties/baseNumbering/title
+msgctxt "settings"
+msgid "Base level for the highest headings"
+msgstr "Index de base pour les titres les plus élevés"
+
 #: /packages/toc-extension/schema/registry.json:/properties/includeOutput/description
 msgctxt "settings"
 msgid "Whether to include cell output in headings or not."
 msgstr "Inclure ou non la sortie des cellules dans les titres."
 
 #: /packages/toc-extension/schema/registry.json:/properties/includeOutput/title
 msgctxt "settings"
@@ -2582,39 +2602,39 @@
 msgid "Hide notifications"
 msgstr "Masquer les notifications"
 
 #: packages/apputils-extension/src/notificationplugin.tsx:229
 msgid "Dismiss notification"
 msgstr "Effacer la notification"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:402
+#: packages/apputils-extension/src/notificationplugin.tsx:401 packages/apputils-extension/src/notificationplugin.tsx:402
 msgid "Emit a notification"
 msgstr "Émettre une notification"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:403
+#: packages/apputils-extension/src/notificationplugin.tsx:402 packages/apputils-extension/src/notificationplugin.tsx:403
 msgid "Notification is described by {message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr "Une notification est décrite par {message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args? ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 
-#: packages/apputils-extension/src/notificationplugin.tsx:440
+#: packages/apputils-extension/src/notificationplugin.tsx:439 packages/apputils-extension/src/notificationplugin.tsx:440
 msgid "Update a notification"
 msgstr "Mise à jour d'une notification"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:441
+#: packages/apputils-extension/src/notificationplugin.tsx:440 packages/apputils-extension/src/notificationplugin.tsx:441
 msgid "Notification is described by {id: string, message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args?: ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 msgstr "Une notification est décrite par {message: string, type?: string, options?: {autoClose?: number | false, actions: {label: string, commandId: string, args? ReadOnlyJSONObject, caption?: string, className?: string}[], data?: ReadOnlyJSONValue}}."
 
-#: packages/apputils-extension/src/notificationplugin.tsx:480
+#: packages/apputils-extension/src/notificationplugin.tsx:479 packages/apputils-extension/src/notificationplugin.tsx:480
 msgid "Dismiss a notification"
 msgstr "Effacer une notification"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:601
+#: packages/apputils-extension/src/notificationplugin.tsx:600 packages/apputils-extension/src/notificationplugin.tsx:601
 msgid "Show Notifications"
 msgstr "Afficher les notifications"
 
-#: packages/apputils-extension/src/notificationplugin.tsx:688
+#: packages/apputils-extension/src/notificationplugin.tsx:688 packages/apputils-extension/src/notificationplugin.tsx:689
 msgid "Hide notification"
 msgstr "Masquer les notifications"
 
 #: packages/apputils-extension/src/palette.ts:101
 msgid "Command Palette Section"
 msgstr "Paramètres de la palette de commandes"
 
@@ -2634,19 +2654,19 @@
 msgid "SEARCH"
 msgstr "RECHERCHER"
 
 #: packages/apputils-extension/src/palette.ts:42
 msgid "Command Palette"
 msgstr "Palette de commandes"
 
-#: packages/apputils-extension/src/shortcuts.tsx:183
+#: packages/apputils-extension/src/shortcuts.tsx:183 packages/apputils-extension/src/shortcuts.tsx:193
 msgid "Keyboard Shortcuts"
 msgstr "Raccourcis clavier"
 
-#: packages/apputils-extension/src/shortcuts.tsx:187 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/running-extension/src/opentabs.ts:86
+#: packages/apputils-extension/src/shortcuts.tsx:187 packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1399 packages/filebrowser/src/listing.ts:1415 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr "Fermer"
 
 #: packages/apputils-extension/src/themesplugins.ts:112
 msgid "Switch to the provided `theme`."
 msgstr "Basculer vers le thème choisi."
 
@@ -2698,43 +2718,43 @@
 msgid "Theme"
 msgstr "Thème"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:181
 msgid "Workspace loader"
 msgstr "Chargeur d'espace de travail"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:272 packages/docmanager/src/widgetmanager.ts:436 packages/docregistry/src/context.ts:1019
+#: packages/apputils-extension/src/workspacesplugin.ts:266 packages/apputils-extension/src/workspacesplugin.ts:267 packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:275 packages/docmanager/src/widgetmanager.ts:436 packages/docmanager/src/widgetmanager.ts:442 packages/docregistry/src/context.ts:1015 packages/docregistry/src/context.ts:1019
 msgid "Save"
 msgstr "Sauvegarder"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:79
+#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:79
 msgid "Save Current Workspace As…"
 msgstr "Enregistrer l'espace de travail actuel sous…"
 
+#: packages/apputils-extension/src/workspacesplugin.ts:268 packages/apputils-extension/src/workspacesplugin.ts:93
+msgid "Save Current Workspace"
+msgstr "Enregistrer l'espace de travail actuel"
+
 #: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr "Fichier d'espace de travail JupyterLab"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:93
-msgid "Save Current Workspace"
-msgstr "Enregistrer l'espace de travail actuel"
-
 #: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:404 packages/hub-extension/src/index.ts:173 packages/lsp/src/adapters/adapter.ts:470 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr "Ignorer"
 
-#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:862 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147
+#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:862 packages/apputils/src/dialog.tsx:870 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:696 packages/filebrowser/src/listing.ts:429 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:514 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:147
 msgid "Cancel"
 msgstr "Annuler"
 
-#: packages/apputils/src/dialog.tsx:763 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/settingeditor/src/plugineditor.ts:133
+#: packages/apputils/src/dialog.tsx:763 packages/apputils/src/dialog.tsx:770 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:508 packages/extensionmanager/src/model.ts:531 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:234 packages/notebook/src/searchprovider.ts:515 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr "Ok"
 
-#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:631
+#: packages/apputils/src/kernelstatuses.tsx:210 packages/apputils/src/sessioncontext.tsx:1746 packages/apputils/src/sessioncontext.tsx:1757 packages/apputils/src/sessioncontext.tsx:631
 msgid "No Kernel"
 msgstr "Aucun noyau"
 
 #: packages/apputils/src/kernelstatuses.tsx:29
 msgid "Unknown"
 msgstr "Inconnu"
 
@@ -2798,75 +2818,87 @@
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr "%1 terminaux, %2 sessions de noyau"
 
 #: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr "Erreur lors du démarrage du noyau"
 
-#: packages/apputils/src/sessioncontext.tsx:1341 packages/filebrowser/src/opendialog.ts:83
+#: packages/apputils/src/sessioncontext.tsx:1341 packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:83
 msgid "Select"
 msgstr "Sélectionner"
 
-#: packages/apputils/src/sessioncontext.tsx:1348
+#: packages/apputils/src/sessioncontext.tsx:1345 packages/apputils/src/sessioncontext.tsx:1348 packages/apputils/src/sessioncontext.tsx:1353
 msgid "Select Kernel"
 msgstr "Sélectionnez le noyau"
 
-#: packages/apputils/src/sessioncontext.tsx:1353
+#: packages/apputils/src/sessioncontext.tsx:1353 packages/apputils/src/sessioncontext.tsx:1358
 msgid "Always start the preferred kernel"
 msgstr "Toujours démarrer le noyau d'exécution préféré"
 
-#: packages/apputils/src/sessioncontext.tsx:1354
+#: packages/apputils/src/sessioncontext.tsx:1354 packages/apputils/src/sessioncontext.tsx:1359
 msgid "Remember my choice and always start the preferred kernel"
 msgstr "Mémoriser mon choix et toujours démarrer le noyau préféré"
 
-#: packages/apputils/src/sessioncontext.tsx:1415
+#: packages/apputils/src/sessioncontext.tsx:1415 packages/apputils/src/sessioncontext.tsx:1423
 msgid "Restart Kernel?"
 msgstr "Redémarrer le noyau ?"
 
-#: packages/apputils/src/sessioncontext.tsx:1416
+#: packages/apputils/src/sessioncontext.tsx:1416 packages/apputils/src/sessioncontext.tsx:1424
 msgid "Do you want to restart the kernel of %1? All variables will be lost."
 msgstr "Voulez-vous redémarrer le noyau actuel pour %1? Toutes les variables seront perdues."
 
-#: packages/apputils/src/sessioncontext.tsx:1473
+#: packages/apputils/src/sessioncontext.tsx:1419 packages/hub-extension/src/index.ts:172
+msgid "Restart"
+msgstr "Redémarrer"
+
+#: packages/apputils/src/sessioncontext.tsx:1420
+msgid "Confirm Kernel Restart"
+msgstr "Confirmer le redémarrage du noyau"
+
+#: packages/apputils/src/sessioncontext.tsx:1429
+msgid "Cancel Kernel Restart"
+msgstr "Annuler le redémarrage du noyau"
+
+#: packages/apputils/src/sessioncontext.tsx:1473 packages/apputils/src/sessioncontext.tsx:1484
 msgid "Select kernel for:"
 msgstr "Sélectionnez le noyau pour:"
 
-#: packages/apputils/src/sessioncontext.tsx:1607
+#: packages/apputils/src/sessioncontext.tsx:1607 packages/apputils/src/sessioncontext.tsx:1618
 msgid "Start Preferred Kernel"
 msgstr "Démarrer le noyau préféré"
 
-#: packages/apputils/src/sessioncontext.tsx:1622
+#: packages/apputils/src/sessioncontext.tsx:1622 packages/apputils/src/sessioncontext.tsx:1633
 msgid "Start Other Kernel"
 msgstr "Démarrer un autre noyau"
 
-#: packages/apputils/src/sessioncontext.tsx:1679
+#: packages/apputils/src/sessioncontext.tsx:1679 packages/apputils/src/sessioncontext.tsx:1690
 msgid "Use Kernel from Preferred Session"
 msgstr "Utiliser le noyau de la session préférée"
 
-#: packages/apputils/src/sessioncontext.tsx:1694
+#: packages/apputils/src/sessioncontext.tsx:1694 packages/apputils/src/sessioncontext.tsx:1705
 msgid "Use Kernel from Other Session"
 msgstr "Utiliser le noyau d'une autre session"
 
-#: packages/apputils/src/sessioncontext.tsx:1744
+#: packages/apputils/src/sessioncontext.tsx:1744 packages/apputils/src/sessioncontext.tsx:1755
 msgid "Use No Kernel"
 msgstr "Ne pas utiliser de noyau"
 
-#: packages/apputils/src/sessioncontext.tsx:1768
+#: packages/apputils/src/sessioncontext.tsx:1768 packages/apputils/src/sessioncontext.tsx:1779
 msgid "Path:"
 msgstr "Chemin d'accès:"
 
-#: packages/apputils/src/sessioncontext.tsx:1769
+#: packages/apputils/src/sessioncontext.tsx:1769 packages/apputils/src/sessioncontext.tsx:1780
 msgid "Name:"
 msgstr "Nom:"
 
-#: packages/apputils/src/sessioncontext.tsx:1770
+#: packages/apputils/src/sessioncontext.tsx:1770 packages/apputils/src/sessioncontext.tsx:1781
 msgid "Kernel Name:"
 msgstr "Nom du noyau :"
 
-#: packages/apputils/src/sessioncontext.tsx:1771
+#: packages/apputils/src/sessioncontext.tsx:1771 packages/apputils/src/sessioncontext.tsx:1782
 msgid "Kernel Id:"
 msgstr "Identifiant du noyau:"
 
 #: packages/apputils/src/thememanager.ts:371
 msgid "Neither theme %1 nor default %2 loaded."
 msgstr "Ni le thème %1 ni le thème par défaut %2 n'ont été chargés."
 
@@ -3704,15 +3736,15 @@
 msgid "HTTP"
 msgstr "HTTP"
 
 #: packages/codemirror/src/language.ts:996
 msgid "IDL"
 msgstr "IDL"
 
-#: packages/codemirror/src/theme.ts:215
+#: packages/codemirror/src/theme.ts:215 packages/codemirror/src/theme.ts:225
 msgid "codemirror"
 msgstr "codemirror"
 
 #: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr "Console"
 
@@ -3772,39 +3804,47 @@
 msgid "Shut down the console?"
 msgstr "Arrêter la console ?"
 
 #: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2357
 msgid "Are you sure you want to close \"%1\"?"
 msgstr "Êtes-vous sûr de vouloir fermer \"%1\"?"
 
-#: packages/console-extension/src/index.ts:684
+#: packages/console-extension/src/index.ts:668
+msgid "Cancel console Shut Down"
+msgstr "Annuler l'arrêt de la console"
+
+#: packages/console-extension/src/index.ts:671
+msgid "Confirm console Shut Down"
+msgstr "Confirmer l'arrêt de la console"
+
+#: packages/console-extension/src/index.ts:684 packages/console-extension/src/index.ts:691
 msgid "Inject some code in a console."
 msgstr "Copie du code dans une console."
 
-#: packages/console-extension/src/index.ts:705 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059
+#: packages/console-extension/src/index.ts:705 packages/console-extension/src/index.ts:712 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3059
 msgid "Change Kernel…"
 msgstr "Changer de noyau…"
 
-#: packages/console-extension/src/index.ts:717 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070
+#: packages/console-extension/src/index.ts:717 packages/console-extension/src/index.ts:724 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3070
 msgid "Get Kernel"
 msgstr "Fournit le noyau d'exécution"
 
-#: packages/console-extension/src/index.ts:799
+#: packages/console-extension/src/index.ts:799 packages/console-extension/src/index.ts:806
 msgid "Execute with Shift+Enter"
 msgstr "Exécuter avec Maj + Entrée"
 
-#: packages/console-extension/src/index.ts:800
+#: packages/console-extension/src/index.ts:800 packages/console-extension/src/index.ts:807
 msgid "Execute with Enter"
 msgstr "Exécuter avec Entrée"
 
-#: packages/console-extension/src/index.ts:844 packages/fileeditor-extension/src/commands.ts:1005 packages/notebook-extension/src/index.ts:1974
+#: packages/console-extension/src/index.ts:844 packages/console-extension/src/index.ts:851 packages/fileeditor-extension/src/commands.ts:1005 packages/notebook-extension/src/index.ts:1974
 msgid "Display the completion helper."
 msgstr "Afficher l'aide de complétion."
 
-#: packages/console-extension/src/index.ts:855 packages/fileeditor-extension/src/commands.ts:1016 packages/notebook-extension/src/index.ts:1984
+#: packages/console-extension/src/index.ts:855 packages/console-extension/src/index.ts:862 packages/fileeditor-extension/src/commands.ts:1016 packages/notebook-extension/src/index.ts:1984
 msgid "Select the completion suggestion."
 msgstr "Sélectionne la suggestion de complétion."
 
 #: packages/console/src/panel.ts:316
 msgid "Name: %1\n"
 msgstr "Nom: %1\n"
 
@@ -4020,15 +4060,15 @@
 msgid "Type"
 msgstr "Type"
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr "Valeur"
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2258 packages/filebrowser/src/listing.ts:2275
 msgid "Name"
 msgstr "Nom"
 
 #: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr "Variables"
 
@@ -4052,55 +4092,59 @@
 msgid "Render variable: %1"
 msgstr "Rendre la variable : %1"
 
 #: packages/debugger/src/service.ts:378
 msgid "Globals"
 msgstr "Variables globales"
 
-#: packages/docmanager-extension/src/index.tsx:1060
+#: packages/docmanager-extension/src/index.tsx:1002 packages/docmanager-extension/src/index.tsx:999
+msgid "Autosave Documents"
+msgstr "Enregistrement automatique des documents"
+
+#: packages/docmanager-extension/src/index.tsx:1060 packages/docmanager-extension/src/index.tsx:1063
 msgid "New View for %1"
 msgstr "Nouvelle vue pour %1"
 
-#: packages/docmanager-extension/src/index.tsx:1084
+#: packages/docmanager-extension/src/index.tsx:1084 packages/docmanager-extension/src/index.tsx:1087
 msgid "Rename%1…"
 msgstr "Renommer %1…"
 
-#: packages/docmanager-extension/src/index.tsx:1098
+#: packages/docmanager-extension/src/index.tsx:1098 packages/docmanager-extension/src/index.tsx:1101
 msgid "Duplicate %1"
 msgstr "Dupliquer %1"
 
-#: packages/docmanager-extension/src/index.tsx:1113
+#: packages/docmanager-extension/src/index.tsx:1113 packages/docmanager-extension/src/index.tsx:1116
 msgid "Delete %1"
 msgstr "Supprimer %1"
 
-#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1127 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430
+#: packages/docmanager-extension/src/index.tsx:1123 packages/docmanager-extension/src/index.tsx:1126 packages/docmanager-extension/src/index.tsx:1127 packages/docmanager-extension/src/index.tsx:1130 packages/filebrowser-extension/src/index.ts:922 packages/filebrowser-extension/src/index.ts:926 packages/filebrowser/src/listing.ts:426 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:434
 msgid "Delete"
 msgstr "Supprimer"
 
-#: packages/docmanager-extension/src/index.tsx:1124
+#: packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:1127
 msgid "Are you sure you want to delete %1"
 msgstr "Êtes-vous sûr de vouloir supprimer %1"
 
-#: packages/docmanager-extension/src/index.tsx:1141
+#: packages/docmanager-extension/src/index.tsx:1141 packages/docmanager-extension/src/index.tsx:1144
 msgid "Show in File Browser"
 msgstr "Ouvrir dans l'explorateur de fichier"
 
-#: packages/docmanager-extension/src/index.tsx:1207
+#: packages/docmanager-extension/src/index.tsx:1207 packages/docmanager-extension/src/index.tsx:1210
 msgid "Are you sure you want to revert the %1 to checkpoint? "
 msgstr "Êtes-vous sûr de vouloir revenir au point de contrôle pour %1? "
 
-#: packages/docmanager-extension/src/index.tsx:1213
+#: packages/docmanager-extension/src/index.tsx:1213 packages/docmanager-extension/src/index.tsx:1216
 msgid "This cannot be undone."
 msgstr "Cela ne peut pas être annulé."
 
-#: packages/docmanager-extension/src/index.tsx:1220
+#: packages/docmanager-extension/src/index.tsx:1220 packages/docmanager-extension/src/index.tsx:1223
 msgid "The checkpoint was last updated at: "
 msgstr "Le point de contrôle a été mis à jour pour la dernière fois à: "
 
-#: packages/docmanager-extension/src/index.tsx:1254
+#: packages/docmanager-extension/src/index.tsx:1254 packages/docmanager-extension/src/index.tsx:1257
 msgid "Choose a checkpoint"
 msgstr "Choisir un point de contrôle"
 
 #: packages/docmanager-extension/src/index.tsx:344
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
@@ -4120,39 +4164,39 @@
 "Si vous spécifiez des types de fichiers ou des visionneuses inexistants, ou si une visionneuse ne peut pas\n"
 "ouvrir un type de fichier donné, la substitution ne fonctionnera pas.\n\n"
 "Visionneuses disponibles :\n"
 "%1\n\n"
 "Types de fichiers disponibles :\n"
 "%2"
 
-#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367
+#: packages/docmanager-extension/src/index.tsx:474 packages/filebrowser-extension/src/index.ts:367 packages/filebrowser-extension/src/index.ts:371
 msgid "Download"
 msgstr "Télécharger"
 
 #: packages/docmanager-extension/src/index.tsx:475
 msgid "Download the file to your computer"
 msgstr "Télécharger le fichier sur votre ordinateur"
 
 #: packages/docmanager-extension/src/index.tsx:483
 msgid "Cannot Download"
 msgstr "Téléchargement impossible"
 
-#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:968
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:726 packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:844 packages/docmanager-extension/src/index.tsx:847 packages/docmanager-extension/src/index.tsx:968 packages/docmanager-extension/src/index.tsx:971
 msgid "No context found for current widget!"
 msgstr "Aucun contexte trouvé pour le widget actuel!"
 
-#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:892 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:493 packages/docmanager-extension/src/index.tsx:634 packages/filebrowser-extension/src/index.ts:1074 packages/filebrowser-extension/src/index.ts:1078 packages/filebrowser-extension/src/index.ts:566 packages/filebrowser-extension/src/index.ts:570 packages/filebrowser-extension/src/index.ts:892 packages/filebrowser-extension/src/index.ts:896 packages/htmlviewer-extension/src/index.tsx:206
 msgid "File Operations"
 msgstr "Opérations sur les fichiers"
 
-#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772
+#: packages/docmanager-extension/src/index.tsx:542 packages/filebrowser-extension/src/index.ts:772 packages/filebrowser-extension/src/index.ts:776
 msgid "Open in New Browser Tab"
 msgstr "Ouvrir dans un nouvel onglet de navigation"
 
-#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/logconsole-extension/src/index.tsx:376
+#: packages/docmanager-extension/src/index.tsx:670 packages/filebrowser/src/browser.ts:236 packages/filebrowser/src/browser.ts:252 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr "Erreur"
 
 #: packages/docmanager-extension/src/index.tsx:704
 msgid "Open the provided `path`."
 msgstr "Ouvrir le chemin (`path`) fourni."
 
@@ -4192,107 +4236,111 @@
 msgid "No checkpoints are available for this %1."
 msgstr "Aucun point de contrôle n'est disponible pour ce %1."
 
 #: packages/docmanager-extension/src/index.tsx:793
 msgid "Revert %1 to checkpoint"
 msgstr "Rétablir %1 au Point de Contrôle"
 
-#: packages/docmanager-extension/src/index.tsx:797 packages/docregistry/src/context.ts:805
+#: packages/docmanager-extension/src/index.tsx:797 packages/docmanager-extension/src/index.tsx:798 packages/docregistry/src/context.ts:801 packages/docregistry/src/context.ts:805
 msgid "Revert"
 msgstr "Rétablir"
 
-#: packages/docmanager-extension/src/index.tsx:820
+#: packages/docmanager-extension/src/index.tsx:799
+msgid "Revert to Checkpoint"
+msgstr "Revenir au point de contrôle"
+
+#: packages/docmanager-extension/src/index.tsx:820 packages/docmanager-extension/src/index.tsx:823
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr "En mode collaboratif, le document est sauvegardé automatiquement après chaque modification"
 
-#: packages/docmanager-extension/src/index.tsx:826
+#: packages/docmanager-extension/src/index.tsx:826 packages/docmanager-extension/src/index.tsx:829
 msgid "Save and create checkpoint"
 msgstr "Enregistrer et créer un point de contrôle"
 
-#: packages/docmanager-extension/src/index.tsx:832
+#: packages/docmanager-extension/src/index.tsx:832 packages/docmanager-extension/src/index.tsx:835
 msgid "Save %1"
 msgstr "Sauvegarder %1"
 
-#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:967 packages/notebook/src/default-toolbar.tsx:68
+#: packages/docmanager-extension/src/index.tsx:843 packages/docmanager-extension/src/index.tsx:846 packages/docmanager-extension/src/index.tsx:854 packages/docmanager-extension/src/index.tsx:857 packages/docmanager-extension/src/index.tsx:967 packages/docmanager-extension/src/index.tsx:970 packages/notebook/src/default-toolbar.tsx:68
 msgid "Cannot Save"
 msgstr "Enregistrement impossible"
 
-#: packages/docmanager-extension/src/index.tsx:855 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:855 packages/docmanager-extension/src/index.tsx:858 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr "Le document est en lecture seule"
 
-#: packages/docmanager-extension/src/index.tsx:870
+#: packages/docmanager-extension/src/index.tsx:870 packages/docmanager-extension/src/index.tsx:873
 msgid "Rename file"
 msgstr "Renommer le fichier"
 
-#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager/src/dialogs.ts:57 packages/filebrowser-extension/src/index.ts:1197
+#: packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:874 packages/docmanager/src/dialogs.ts:57 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1197 packages/filebrowser-extension/src/index.ts:1201
 msgid "Rename"
 msgstr "Renommer"
 
-#: packages/docmanager-extension/src/index.tsx:872
+#: packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:875
 msgid "File name"
 msgstr "Nom du fichier"
 
-#: packages/docmanager-extension/src/index.tsx:876 packages/docmanager/src/widgetmanager.ts:414
+#: packages/docmanager-extension/src/index.tsx:876 packages/docmanager-extension/src/index.tsx:879 packages/docmanager/src/widgetmanager.ts:414 packages/docmanager/src/widgetmanager.ts:420
 msgid "Do not ask me again."
 msgstr "Ne plus demander."
 
-#: packages/docmanager-extension/src/index.tsx:877
+#: packages/docmanager-extension/src/index.tsx:877 packages/docmanager-extension/src/index.tsx:880
 msgid "If checked, you will not be asked to rename future untitled files when saving them."
 msgstr "Si coché, il ne vous sera plus demandé de renommer les fichiers sans titre lors de leur sauvegarde."
 
-#: packages/docmanager-extension/src/index.tsx:934
+#: packages/docmanager-extension/src/index.tsx:934 packages/docmanager-extension/src/index.tsx:937
 msgid "Save All"
 msgstr "Tout enregistrer"
 
-#: packages/docmanager-extension/src/index.tsx:935
+#: packages/docmanager-extension/src/index.tsx:935 packages/docmanager-extension/src/index.tsx:938
 msgid "Save all open documents"
 msgstr "Enregistrer tous les documents ouverts"
 
-#: packages/docmanager-extension/src/index.tsx:958
+#: packages/docmanager-extension/src/index.tsx:958 packages/docmanager-extension/src/index.tsx:961
 msgid "Save %1 As…"
 msgstr "Enregistrer %1 sous…"
 
-#: packages/docmanager-extension/src/index.tsx:959
+#: packages/docmanager-extension/src/index.tsx:959 packages/docmanager-extension/src/index.tsx:962
 msgid "Save with new path"
 msgstr "Enregistrer avec un nouveau chemin"
 
-#: packages/docmanager-extension/src/index.tsx:999
-msgid "Autosave Documents"
-msgstr "Enregistrement automatique des documents"
-
-#: packages/docmanager/src/dialogs.ts:114
+#: packages/docmanager/src/dialogs.ts:114 packages/docmanager/src/dialogs.ts:117
 msgid "Overwrite file?"
 msgstr "Écraser le fichier ?"
 
-#: packages/docmanager/src/dialogs.ts:115
+#: packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:118
 msgid "\"%1\" already exists, overwrite?"
 msgstr "\"%1\" existe déjà, remplacer?"
 
-#: packages/docmanager/src/dialogs.ts:118 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
+#: packages/docmanager/src/dialogs.ts:118 packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:805 packages/docregistry/src/context.ts:809 packages/docregistry/src/context.ts:841 packages/docregistry/src/context.ts:845 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
 msgid "Overwrite"
 msgstr "Écraser"
 
-#: packages/docmanager/src/dialogs.ts:182
+#: packages/docmanager/src/dialogs.ts:123
+msgid "Overwrite Existing File"
+msgstr "Remplacer le fichier existant"
+
+#: packages/docmanager/src/dialogs.ts:182 packages/docmanager/src/dialogs.ts:188
 msgid "File Path"
 msgstr "Chemin du fichier"
 
-#: packages/docmanager/src/dialogs.ts:187
+#: packages/docmanager/src/dialogs.ts:187 packages/docmanager/src/dialogs.ts:193
 msgid "New Name"
 msgstr "Nouveau nom"
 
-#: packages/docmanager/src/dialogs.ts:52
+#: packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/dialogs.ts:59
 msgid "Rename File"
 msgstr "Renommer le fichier"
 
-#: packages/docmanager/src/dialogs.ts:65 packages/filebrowser/src/listing.ts:1875
+#: packages/docmanager/src/dialogs.ts:65 packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1875 packages/filebrowser/src/listing.ts:1891
 msgid "Rename Error"
 msgstr "Erreur lors du renommage"
 
-#: packages/docmanager/src/dialogs.ts:67
+#: packages/docmanager/src/dialogs.ts:67 packages/docmanager/src/dialogs.ts:70
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" n'est pas un nom valide pour un fichier. Les noms doivent avoir une longueur non nulle, et ne peuvent pas inclure \"/\", \"\\\", ou \":\""
 
 #: packages/docmanager/src/savingstatus.tsx:58
 msgid "Saving completed"
 msgstr "Enregistrement effectué"
 
@@ -4322,75 +4370,91 @@
 msgid "Last Checkpoint: %1"
 msgstr "Dernier point de contrôle : %1"
 
 #: packages/docmanager/src/widgetmanager.ts:397
 msgid "Close and save"
 msgstr "Fermer et sauvegarder"
 
-#: packages/docmanager/src/widgetmanager.ts:404
+#: packages/docmanager/src/widgetmanager.ts:399
+msgid "Close and save Document"
+msgstr "Fermer et enregistrer le document"
+
+#: packages/docmanager/src/widgetmanager.ts:400
+msgid "Close Document"
+msgstr "Fermer le document"
+
+#: packages/docmanager/src/widgetmanager.ts:404 packages/docmanager/src/widgetmanager.ts:408
 msgid "Close without saving"
 msgstr "Fermer sans sauvegarder"
 
-#: packages/docmanager/src/widgetmanager.ts:409 packages/notebook/src/searchprovider.ts:509
+#: packages/docmanager/src/widgetmanager.ts:409
+msgid "Close Document without saving"
+msgstr "Fermer le document sans sauvegarder"
+
+#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:415 packages/notebook/src/searchprovider.ts:509
 msgid "Confirmation"
 msgstr "Confirmation"
 
-#: packages/docmanager/src/widgetmanager.ts:410
+#: packages/docmanager/src/widgetmanager.ts:410 packages/docmanager/src/widgetmanager.ts:416
 msgid "Please confirm you want to close \"%1\"."
 msgstr "Veuillez confirmer que vous voulez fermer \"%1\"."
 
-#: packages/docmanager/src/widgetmanager.ts:415
+#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:421
 msgid "If checked, no confirmation to close a document will be asked in the future."
 msgstr "Si coché, aucune confirmation de fermeture d'un document ne sera demandée dans le futur."
 
-#: packages/docmanager/src/widgetmanager.ts:437
+#: packages/docmanager/src/widgetmanager.ts:437 packages/docmanager/src/widgetmanager.ts:443
 msgid "Save as"
 msgstr "Enregistrer sous"
 
-#: packages/docmanager/src/widgetmanager.ts:439
+#: packages/docmanager/src/widgetmanager.ts:439 packages/docmanager/src/widgetmanager.ts:445
 msgid "Save your work"
 msgstr "Enregistrer votre travail"
 
-#: packages/docmanager/src/widgetmanager.ts:440
+#: packages/docmanager/src/widgetmanager.ts:440 packages/docmanager/src/widgetmanager.ts:446
 msgid "Save changes in \"%1\" before closing?"
 msgstr "Enregistrer les modifications dans \"%1\" avant de fermer ?"
 
-#: packages/docmanager/src/widgetmanager.ts:443
+#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:450
 msgid "Discard"
 msgstr "Abandonner"
 
-#: packages/docregistry/src/context.ts:1021
+#: packages/docmanager/src/widgetmanager.ts:451
+msgid "Discard changes to file"
+msgstr "Ignorer les modifications apportées au fichier"
+
+#: packages/docregistry/src/context.ts:1017 packages/docregistry/src/context.ts:1021
 msgid "Save File As…"
 msgstr "Enregistrer le fichier sous…"
 
-#: packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:894
+#: packages/docregistry/src/context.ts:627 packages/docregistry/src/context.ts:631 packages/docregistry/src/context.ts:890 packages/docregistry/src/context.ts:894
 msgid "File Save Error for %1"
 msgstr "Erreur d'enregistrement du fichier pour %1"
 
-#: packages/docregistry/src/context.ts:695
+#: packages/docregistry/src/context.ts:691 packages/docregistry/src/context.ts:695
 msgid "File Load Error for %1"
 msgstr "Erreur de chargement de fichier pour %1"
 
-#: packages/docregistry/src/context.ts:798
+#: packages/docregistry/src/context.ts:794 packages/docregistry/src/context.ts:798
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr "\"%1\" a changé sur le disque depuis la dernière fois qu'il a été ouvert ou enregistré.\n"
 "Voulez-vous remplacer le fichier sur le disque avec la version ouverte ici,\n"
 "ou charger la version sur le disque (rétablir) ?"
 
-#: packages/docregistry/src/context.ts:814
+#: packages/docregistry/src/context.ts:810 packages/docregistry/src/context.ts:814
 msgid "File Changed"
 msgstr "Fichier modifié"
 
-#: packages/docregistry/src/context.ts:840
+#: packages/docregistry/src/context.ts:836 packages/docregistry/src/context.ts:840
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "\"%1\" existe déjà. Voulez-vous le remplacer?"
 
-#: packages/docregistry/src/context.ts:849
+#: packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:849
 msgid "File Overwrite?"
 msgstr "Écraser le fichier ?"
 
 #: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr "Échec du rendu : %1"
 
@@ -4702,192 +4766,196 @@
 msgid "Version: %1"
 msgstr "Version : %1"
 
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr "L'extension %1 n'est plus autorisée. Veuillez la désinstaller immédiatement ou contacter votre administrateur."
 
-#: packages/filebrowser-extension/src/index.ts:1014
-msgid "Open from Path…"
-msgstr "Ouvrir à partir du chemin…"
-
-#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839
+#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:1018 packages/filebrowser-extension/src/index.ts:1020 packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:841 packages/filebrowser-extension/src/index.ts:843
 msgid "Open %1"
 msgstr "Ouvrir %1"
 
-#: packages/filebrowser-extension/src/index.ts:1016
+#: packages/filebrowser-extension/src/index.ts:1014 packages/filebrowser-extension/src/index.ts:1018
+msgid "Open from Path…"
+msgstr "Ouvrir à partir du chemin…"
+
+#: packages/filebrowser-extension/src/index.ts:1016 packages/filebrowser-extension/src/index.ts:1020
 msgid "Open from path"
 msgstr "Ouvrir depuis le chemin d'accès"
 
-#: packages/filebrowser-extension/src/index.ts:1025
+#: packages/filebrowser-extension/src/index.ts:1025 packages/filebrowser-extension/src/index.ts:1029
 msgid "Path"
 msgstr "Chemin d'accès"
 
-#: packages/filebrowser-extension/src/index.ts:1027
+#: packages/filebrowser-extension/src/index.ts:1027 packages/filebrowser-extension/src/index.ts:1031
 msgid "Open Path"
 msgstr "Ouvrir le Chemin"
 
-#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:849
+#: packages/filebrowser-extension/src/index.ts:1028 packages/filebrowser-extension/src/index.ts:1032 packages/filebrowser-extension/src/index.ts:1117 packages/filebrowser-extension/src/index.ts:1121 packages/filebrowser-extension/src/index.ts:849 packages/filebrowser-extension/src/index.ts:853
 msgid "Open"
 msgstr "Ouvrir"
 
-#: packages/filebrowser-extension/src/index.ts:1063
+#: packages/filebrowser-extension/src/index.ts:1063 packages/filebrowser-extension/src/index.ts:1067
 msgid "Could not find path: %1"
 msgstr "Impossible de trouver le chemin : %1"
 
-#: packages/filebrowser-extension/src/index.ts:1065
+#: packages/filebrowser-extension/src/index.ts:1065 packages/filebrowser-extension/src/index.ts:1069
 msgid "Cannot open"
 msgstr "Ouverture impossible"
 
-#: packages/filebrowser-extension/src/index.ts:1130 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488
+#: packages/filebrowser-extension/src/index.ts:1130 packages/filebrowser-extension/src/index.ts:1134 packages/fileeditor-extension/src/commands.ts:974 packages/terminal-extension/src/index.ts:488 packages/terminal-extension/src/index.ts:494
 msgid "Paste"
 msgstr "Coller"
 
-#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser/src/opendialog.ts:153
+#: packages/filebrowser-extension/src/index.ts:1143 packages/filebrowser-extension/src/index.ts:1147 packages/filebrowser/src/opendialog.ts:153
 msgid "New Folder"
 msgstr "Nouveau dossier"
 
-#: packages/filebrowser-extension/src/index.ts:1155
+#: packages/filebrowser-extension/src/index.ts:1155 packages/filebrowser-extension/src/index.ts:1159
 msgid "New File"
 msgstr "Nouveau fichier"
 
-#: packages/filebrowser-extension/src/index.ts:1167 packages/fileeditor-extension/src/commands.ts:809
+#: packages/filebrowser-extension/src/index.ts:1167 packages/filebrowser-extension/src/index.ts:1171 packages/fileeditor-extension/src/commands.ts:809
 msgid "New Markdown File"
 msgstr "Nouveau fichier Markdown"
 
-#: packages/filebrowser-extension/src/index.ts:1179
+#: packages/filebrowser-extension/src/index.ts:1179 packages/filebrowser-extension/src/index.ts:1183
 msgid "Refresh the file browser."
 msgstr "Rafraîchir le navigateur de fichiers."
 
-#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser/src/opendialog.ts:168
+#: packages/filebrowser-extension/src/index.ts:1180 packages/filebrowser-extension/src/index.ts:1184 packages/filebrowser/src/opendialog.ts:168
 msgid "Refresh File List"
 msgstr "Actualiser la liste des fichiers"
 
-#: packages/filebrowser-extension/src/index.ts:1220
+#: packages/filebrowser-extension/src/index.ts:1220 packages/filebrowser-extension/src/index.ts:1224
 msgid "Copy Path"
 msgstr "Copier le chemin"
 
-#: packages/filebrowser-extension/src/index.ts:1232 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1232 packages/filebrowser-extension/src/index.ts:1236 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2332 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
 msgid "Shut Down Kernel"
 msgstr "Arrêter le noyau"
 
-#: packages/filebrowser-extension/src/index.ts:1236
+#: packages/filebrowser-extension/src/index.ts:1236 packages/filebrowser-extension/src/index.ts:1240
 msgid "Show Last Modified Column"
 msgstr "Afficher la dernière colonne modifiée"
 
-#: packages/filebrowser-extension/src/index.ts:1252
+#: packages/filebrowser-extension/src/index.ts:1252 packages/filebrowser-extension/src/index.ts:1272
 msgid "Show File Size Column"
 msgstr "Afficher la colonne de taille de fichier"
 
-#: packages/filebrowser-extension/src/index.ts:1268
+#: packages/filebrowser-extension/src/index.ts:1256
+msgid "Sort Notebooks Above Files"
+msgstr "Grouper les notebooks au-dessus des fichiers"
+
+#: packages/filebrowser-extension/src/index.ts:1268 packages/filebrowser-extension/src/index.ts:1288
 msgid "Show Hidden Files"
 msgstr "Afficher les fichiers cachés"
 
-#: packages/filebrowser-extension/src/index.ts:1285
+#: packages/filebrowser-extension/src/index.ts:1285 packages/filebrowser-extension/src/index.ts:1305
 msgid "Show File Checkboxes"
 msgstr "Afficher les cases à cocher des fichiers"
 
-#: packages/filebrowser-extension/src/index.ts:1301
+#: packages/filebrowser-extension/src/index.ts:1301 packages/filebrowser-extension/src/index.ts:1321
 msgid "Search on File Names"
 msgstr "Rechercher dans les noms de fichiers"
 
-#: packages/filebrowser-extension/src/index.ts:1370
+#: packages/filebrowser-extension/src/index.ts:1370 packages/filebrowser-extension/src/index.ts:1390
 msgid "No browser for path"
 msgstr "Aucun navigateur pour le chemin"
 
-#: packages/filebrowser-extension/src/index.ts:389
+#: packages/filebrowser-extension/src/index.ts:389 packages/filebrowser-extension/src/index.ts:393
 msgid "Copy Download Link"
 msgstr "Copier le lien de téléchargement"
 
-#: packages/filebrowser-extension/src/index.ts:432
+#: packages/filebrowser-extension/src/index.ts:432 packages/filebrowser-extension/src/index.ts:436
 msgid "File Browser Section"
 msgstr "Section du navigateur de fichiers"
 
-#: packages/filebrowser-extension/src/index.ts:443
+#: packages/filebrowser-extension/src/index.ts:443 packages/filebrowser-extension/src/index.ts:447
 msgid "File Browser (%1)"
 msgstr "Explorateur de fichiers (%1)"
 
-#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser/src/browser.ts:75
+#: packages/filebrowser-extension/src/index.ts:445 packages/filebrowser-extension/src/index.ts:449 packages/filebrowser-extension/src/index.ts:497 packages/filebrowser-extension/src/index.ts:501 packages/filebrowser/src/browser.ts:75
 msgid "File Browser"
 msgstr "Explorateur de fichiers"
 
-#: packages/filebrowser-extension/src/index.ts:475
+#: packages/filebrowser-extension/src/index.ts:475 packages/filebrowser-extension/src/index.ts:479
 msgid "Filter files by name"
 msgstr "Filtrer les fichiers par nom"
 
-#: packages/filebrowser-extension/src/index.ts:508
+#: packages/filebrowser-extension/src/index.ts:508 packages/filebrowser-extension/src/index.ts:512
 msgid "Open the file browser for the provided `path`."
 msgstr "Ouvrez le navigateur de fichiers pour le chemin (`path`) fourni."
 
-#: packages/filebrowser-extension/src/index.ts:540
+#: packages/filebrowser-extension/src/index.ts:540 packages/filebrowser-extension/src/index.ts:544
 msgid "Hide the file browser."
 msgstr "Masquer le navigateur de fichiers."
 
-#: packages/filebrowser-extension/src/index.ts:550
+#: packages/filebrowser-extension/src/index.ts:550 packages/filebrowser-extension/src/index.ts:554
 msgid "Show Active File in File Browser"
 msgstr "Afficher le fichier actif dans le navigateur de fichiers"
 
-#: packages/filebrowser-extension/src/index.ts:647
+#: packages/filebrowser-extension/src/index.ts:647 packages/filebrowser-extension/src/index.ts:651
 msgid "Copy Shareable Link"
 msgstr "Copier le lien partageable"
 
-#: packages/filebrowser-extension/src/index.ts:771
+#: packages/filebrowser-extension/src/index.ts:771 packages/filebrowser-extension/src/index.ts:775
 msgid "Open in Simple Mode"
 msgstr "Ouvrir en Mode Simple"
 
-#: packages/filebrowser-extension/src/index.ts:837
+#: packages/filebrowser-extension/src/index.ts:837 packages/filebrowser-extension/src/index.ts:841
 msgid "Open from URL…"
 msgstr "Ouvrir depuis l'URL…"
 
-#: packages/filebrowser-extension/src/index.ts:839
+#: packages/filebrowser-extension/src/index.ts:839 packages/filebrowser-extension/src/index.ts:843
 msgid "Open from URL"
 msgstr "Ouvrir depuis l'URL"
 
-#: packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:850
 msgid "URL"
 msgstr "URL"
 
-#: packages/filebrowser-extension/src/index.ts:848
+#: packages/filebrowser-extension/src/index.ts:848 packages/filebrowser-extension/src/index.ts:852
 msgid "Open URL"
 msgstr "Ouvrir l'URL"
 
-#: packages/filebrowser-extension/src/index.ts:867
+#: packages/filebrowser-extension/src/index.ts:867 packages/filebrowser-extension/src/index.ts:871
 msgid "Could not open URL: %1"
 msgstr "Impossible d'ouvrir l'URL: %1"
 
-#: packages/filebrowser-extension/src/index.ts:869
+#: packages/filebrowser-extension/src/index.ts:869 packages/filebrowser-extension/src/index.ts:873
 msgid "Cannot fetch"
 msgstr "Impossible de récupérer"
 
-#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:882 packages/filebrowser-extension/src/index.ts:886 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr "Erreur lors du téléversement"
 
-#: packages/filebrowser-extension/src/index.ts:935 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463
+#: packages/filebrowser-extension/src/index.ts:935 packages/filebrowser-extension/src/index.ts:939 packages/fileeditor-extension/src/commands.ts:947 packages/terminal-extension/src/index.ts:463 packages/terminal-extension/src/index.ts:469
 msgid "Copy"
 msgstr "Copier"
 
-#: packages/filebrowser-extension/src/index.ts:948 packages/fileeditor-extension/src/commands.ts:913
+#: packages/filebrowser-extension/src/index.ts:948 packages/filebrowser-extension/src/index.ts:952 packages/fileeditor-extension/src/commands.ts:913
 msgid "Cut"
 msgstr "Couper"
 
-#: packages/filebrowser-extension/src/index.ts:960
+#: packages/filebrowser-extension/src/index.ts:960 packages/filebrowser-extension/src/index.ts:964
 msgid "Duplicate"
 msgstr "Dupliquer"
 
-#: packages/filebrowser-extension/src/index.ts:964
+#: packages/filebrowser-extension/src/index.ts:964 packages/filebrowser-extension/src/index.ts:968
 msgid "Update the file browser to display the provided `path`."
 msgstr "Mettez à jour le navigateur de fichiers pour afficher le chemin (`path`) fourni."
 
-#: packages/filebrowser/src/browser.ts:372
+#: packages/filebrowser/src/browser.ts:372 packages/filebrowser/src/browser.ts:388
 msgid "Directory not found"
 msgstr "Dossier introuvable"
 
-#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/model.ts:298
+#: packages/filebrowser/src/browser.ts:373 packages/filebrowser/src/browser.ts:389 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr "Répertoire introuvable: \"%1\""
 
 #: packages/filebrowser/src/browser.ts:69
 msgid "file browser"
 msgstr "explorateur de fichiers"
 
@@ -4895,149 +4963,149 @@
 msgid "Open Error"
 msgstr "Erreur lors de l'ouverture"
 
 #: packages/filebrowser/src/crumbs.ts:302
 msgid "Move Error"
 msgstr "Erreur lors du déplacement"
 
-#: packages/filebrowser/src/listing.ts:1120
+#: packages/filebrowser/src/listing.ts:1120 packages/filebrowser/src/listing.ts:1136
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr "Ouvrir le dossier"
 
-#: packages/filebrowser/src/listing.ts:1395
+#: packages/filebrowser/src/listing.ts:1395 packages/filebrowser/src/listing.ts:1411
 msgid "Error Uploading Folder"
 msgstr "Erreur lors du téléversement du dossier"
 
-#: packages/filebrowser/src/listing.ts:1396
+#: packages/filebrowser/src/listing.ts:1396 packages/filebrowser/src/listing.ts:1412
 msgid "Drag and Drop is currently not supported for folders"
 msgstr "Glisser-déposer n'est actuellement pas pris en charge pour les dossiers"
 
-#: packages/filebrowser/src/listing.ts:1515
+#: packages/filebrowser/src/listing.ts:1515 packages/filebrowser/src/listing.ts:1531
 msgctxt "showErrorMessage"
 msgid "Error while copying/moving files"
 msgstr "Erreur lors de la copie/déplacement des fichiers"
 
-#: packages/filebrowser/src/listing.ts:1814
+#: packages/filebrowser/src/listing.ts:1814 packages/filebrowser/src/listing.ts:1830
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr "Echec de la Suppression"
 
-#: packages/filebrowser/src/listing.ts:1877
+#: packages/filebrowser/src/listing.ts:1877 packages/filebrowser/src/listing.ts:1893
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "\"%1\" n'est pas un nom valide pour un fichier. Les noms doivent avoir une longueur non nulle, et ne peuvent pas inclure \"/\", \"\\\", ou \":\""
 
-#: packages/filebrowser/src/listing.ts:1896
+#: packages/filebrowser/src/listing.ts:1896 packages/filebrowser/src/listing.ts:1912
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr "Erreur lors du renommage"
 
-#: packages/filebrowser/src/listing.ts:2260
+#: packages/filebrowser/src/listing.ts:2260 packages/filebrowser/src/listing.ts:2277
 msgid "Last Modified"
 msgstr "Dernière Modification"
 
-#: packages/filebrowser/src/listing.ts:2261
+#: packages/filebrowser/src/listing.ts:2261 packages/filebrowser/src/listing.ts:2278
 msgid "File Size"
 msgstr "Taille du fichier"
 
-#: packages/filebrowser/src/listing.ts:2549
+#: packages/filebrowser/src/listing.ts:2549 packages/filebrowser/src/listing.ts:2566
 msgid "Name: %1"
 msgstr "Nom: %1"
 
-#: packages/filebrowser/src/listing.ts:2555
+#: packages/filebrowser/src/listing.ts:2555 packages/filebrowser/src/listing.ts:2572
 msgid "\n"
 "Size: %1"
 msgstr "\n"
 "Taille: %1"
 
-#: packages/filebrowser/src/listing.ts:2565
+#: packages/filebrowser/src/listing.ts:2565 packages/filebrowser/src/listing.ts:2582
 msgid "\n"
 "Path: %1"
 msgstr "\n"
 "Chemin : %1"
 
-#: packages/filebrowser/src/listing.ts:2572
+#: packages/filebrowser/src/listing.ts:2572 packages/filebrowser/src/listing.ts:2589
 msgid "\n"
 "Created: %1"
 msgstr "\n"
 "Créé: %1"
 
-#: packages/filebrowser/src/listing.ts:2578
+#: packages/filebrowser/src/listing.ts:2578 packages/filebrowser/src/listing.ts:2595
 msgid "\n"
 "Modified: %1"
 msgstr "\n"
 "Modifié le : %1"
 
-#: packages/filebrowser/src/listing.ts:2583
+#: packages/filebrowser/src/listing.ts:2583 packages/filebrowser/src/listing.ts:2600
 msgid "\n"
 "Writable: %1"
 msgstr "\n"
 "Inscriptible: %1"
 
-#: packages/filebrowser/src/listing.ts:2608
+#: packages/filebrowser/src/listing.ts:2608 packages/filebrowser/src/listing.ts:2625
 msgid "Deselect directory \"%1\""
 msgstr "Désélectionner le dossier \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2609
+#: packages/filebrowser/src/listing.ts:2609 packages/filebrowser/src/listing.ts:2626
 msgid "Select directory \"%1\""
 msgstr "Sélectionnez le dossier \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2612
+#: packages/filebrowser/src/listing.ts:2612 packages/filebrowser/src/listing.ts:2629
 msgid "Deselect file \"%1\""
 msgstr "Désélectionner le fichier \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2613
+#: packages/filebrowser/src/listing.ts:2613 packages/filebrowser/src/listing.ts:2630
 msgid "Select file \"%1\""
 msgstr "Sélectionner le fichier \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2687
+#: packages/filebrowser/src/listing.ts:2687 packages/filebrowser/src/listing.ts:2704
 msgid "%1 Item"
 msgid_plural "%1 Items"
 msgstr[0] "%1 élément"
 msgstr[1] "%1 éléments"
 
-#: packages/filebrowser/src/listing.ts:396
+#: packages/filebrowser/src/listing.ts:396 packages/filebrowser/src/listing.ts:400
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr "Impossible de coller"
 
-#: packages/filebrowser/src/listing.ts:416
+#: packages/filebrowser/src/listing.ts:416 packages/filebrowser/src/listing.ts:420
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr "Êtes-vous sûr(e) de vouloir supprimer définitivement %1 ?"
 
-#: packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420 packages/filebrowser/src/listing.ts:424
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] "Êtes-vous sûr de vouloir supprimer définitivement l'élément sélectionné %1?"
 msgstr[1] "Êtes-vous sûr de vouloir supprimer définitivement les éléments sélectionnés %1?"
 
-#: packages/filebrowser/src/listing.ts:472
+#: packages/filebrowser/src/listing.ts:472 packages/filebrowser/src/listing.ts:476
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr "Dupliquer le fichier"
 
-#: packages/filebrowser/src/listing.ts:512
+#: packages/filebrowser/src/listing.ts:512 packages/filebrowser/src/listing.ts:516
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr "Arrêter le noyau"
 
-#: packages/filebrowser/src/listing.ts:852
+#: packages/filebrowser/src/listing.ts:852 packages/filebrowser/src/listing.ts:856
 msgid "Deselect all files and directories"
 msgstr "Désélectionner tous les fichiers et dossiers"
 
-#: packages/filebrowser/src/listing.ts:853
+#: packages/filebrowser/src/listing.ts:853 packages/filebrowser/src/listing.ts:857
 msgid "Select all files and directories"
 msgstr "Sélectionner tous les fichiers et dossiers"
 
-#: packages/filebrowser/src/listing.ts:906
+#: packages/filebrowser/src/listing.ts:906 packages/filebrowser/src/listing.ts:910
 msgid "unknown"
 msgstr "inconnu"
 
-#: packages/filebrowser/src/listing.ts:908
+#: packages/filebrowser/src/listing.ts:908 packages/filebrowser/src/listing.ts:912
 msgid "%1\n"
 "Kernel: %2"
 msgstr "%1\n"
 "Noyau: %2"
 
 #: packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
@@ -5390,18 +5458,14 @@
 
 #: packages/hub-extension/src/index.ts:167
 msgid "Your server at %1 is not running.\n"
 "Would you like to restart it?"
 msgstr "Votre serveur à %1 n'est pas en cours d'exécution.\n"
 "Voulez-vous le redémarrer ?"
 
-#: packages/hub-extension/src/index.ts:172
-msgid "Restart"
-msgstr "Redémarrer"
-
 #: packages/hub-extension/src/index.ts:67
 msgid "Restart Server"
 msgstr "Redémarrer le serveur"
 
 #: packages/hub-extension/src/index.ts:68
 msgid "Request that the Hub restart this server"
 msgstr "Demander au Hub de redémarrer ce serveur"
@@ -6251,31 +6315,35 @@
 msgid "Notebook is already trusted"
 msgstr "Le notebook est déjà de confiance"
 
 #: packages/notebook/src/actions.tsx:2061
 msgid "Trust this notebook?"
 msgstr "Faire confiance au notebook?"
 
-#: packages/notebook/src/actions.tsx:2064
+#: packages/notebook/src/actions.tsx:2064 packages/notebook/src/actions.tsx:2065
 msgid "Trust"
 msgstr "Approuver"
 
-#: packages/notebook/src/actions.tsx:2279
+#: packages/notebook/src/actions.tsx:2066
+msgid "Confirm Trusting this notebook"
+msgstr "Confirmer ce notebook est de confiance"
+
+#: packages/notebook/src/actions.tsx:2279 packages/notebook/src/actions.tsx:2282
 msgid "Kernel Terminating"
 msgstr "Fermeture du noyau"
 
-#: packages/notebook/src/actions.tsx:2280
+#: packages/notebook/src/actions.tsx:2280 packages/notebook/src/actions.tsx:2283
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr "Le noyau pour %1 semble être en train de se fermer. Vous ne pouvez pas exécuter de cellule pour le moment."
 
-#: packages/notebook/src/actions.tsx:2290
+#: packages/notebook/src/actions.tsx:2290 packages/notebook/src/actions.tsx:2293
 msgid "Cell not executed due to pending input"
 msgstr "La cellule n'a pas été exécutée en raison d'une entrée en attente"
 
-#: packages/notebook/src/actions.tsx:2291
+#: packages/notebook/src/actions.tsx:2291 packages/notebook/src/actions.tsx:2294
 msgid "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again."
 msgstr "La cellule n'a pas été exécutée pour éviter de bloquer le noyau car une autre entrée est en attente ! Soumettez une entrée et réessayez."
 
 #: packages/notebook/src/default-toolbar.tsx:141
 msgid "Cut the selected cells"
 msgstr "Couper les cellules sélectionnées"
 
@@ -6455,15 +6523,15 @@
 msgid "Handle Local Link"
 msgstr "Gérer le lien local"
 
 #: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "Cette sortie HTML contient des scripts en ligne. Êtes-vous sûr de vouloir exécuter du code arbitraire JavaScript au cours de votre session JupyterLab?"
 
-#: packages/rendermime/src/widgets.ts:428
+#: packages/rendermime/src/widgets.ts:428 packages/rendermime/src/widgets.ts:446
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr "La sortie JavaScript est désactivée dans JupyterLab"
 
 #: packages/running-extension/src/index.ts:66
 msgid "Running Terminals and Kernels"
 msgstr "Terminaux et noyaux en cours d'exécution"
 
@@ -6744,23 +6812,23 @@
 msgstr "Terminal"
 
 #: packages/terminal-extension/src/index.ts:191
 msgctxt "menu"
 msgid "Terminal Theme"
 msgstr "Thème du terminal"
 
-#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534
+#: packages/terminal-extension/src/index.ts:196 packages/terminal-extension/src/index.ts:251 packages/terminal-extension/src/index.ts:534 packages/terminal-extension/src/index.ts:540
 msgid "Inherit"
 msgstr "Hériter"
 
-#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535
+#: packages/terminal-extension/src/index.ts:204 packages/terminal-extension/src/index.ts:258 packages/terminal-extension/src/index.ts:535 packages/terminal-extension/src/index.ts:541
 msgid "Light"
 msgstr "Clair"
 
-#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536
+#: packages/terminal-extension/src/index.ts:210 packages/terminal-extension/src/index.ts:263 packages/terminal-extension/src/index.ts:536 packages/terminal-extension/src/index.ts:542
 msgid "Dark"
 msgstr "Sombre"
 
 #: packages/terminal-extension/src/index.ts:316
 msgid "Terminals"
 msgstr "Terminaux"
 
@@ -6772,47 +6840,47 @@
 msgid "New Terminal"
 msgstr "Nouveau Terminal"
 
 #: packages/terminal-extension/src/index.ts:351
 msgid "Start a new terminal session"
 msgstr "Démarrer une nouvelle session de terminal"
 
-#: packages/terminal-extension/src/index.ts:389
+#: packages/terminal-extension/src/index.ts:389 packages/terminal-extension/src/index.ts:395
 msgid "Open a terminal by its `name`."
 msgstr "Ouvrir un terminal par son nom (`name`)."
 
-#: packages/terminal-extension/src/index.ts:407
+#: packages/terminal-extension/src/index.ts:407 packages/terminal-extension/src/index.ts:413
 msgid "Refresh Terminal"
 msgstr "Actualiser le terminal"
 
-#: packages/terminal-extension/src/index.ts:408
+#: packages/terminal-extension/src/index.ts:408 packages/terminal-extension/src/index.ts:414
 msgid "Refresh the current terminal session"
 msgstr "Rafraîchir la session du terminal actuel"
 
-#: packages/terminal-extension/src/index.ts:492
+#: packages/terminal-extension/src/index.ts:492 packages/terminal-extension/src/index.ts:498
 msgid "Shutdown Terminal"
 msgstr "Arrêter le terminal"
 
-#: packages/terminal-extension/src/index.ts:506
+#: packages/terminal-extension/src/index.ts:506 packages/terminal-extension/src/index.ts:512
 msgid "Increase Terminal Font Size"
 msgstr "Augmenter la taille de police du terminal"
 
-#: packages/terminal-extension/src/index.ts:520
+#: packages/terminal-extension/src/index.ts:520 packages/terminal-extension/src/index.ts:526
 msgid "Decrease Terminal Font Size"
 msgstr "Diminuer la taille de police du terminal"
 
-#: packages/terminal-extension/src/index.ts:542
+#: packages/terminal-extension/src/index.ts:542 packages/terminal-extension/src/index.ts:548
 msgid "Set terminal theme to the provided `theme`."
 msgstr "Définir le thème du terminal par le thème (`theme`) fourni."
 
-#: packages/terminal-extension/src/index.ts:550
+#: packages/terminal-extension/src/index.ts:550 packages/terminal-extension/src/index.ts:556
 msgid "Use Terminal Theme: %1"
 msgstr "Utiliser le thème du terminal : %1"
 
-#: packages/terminal-extension/src/index.ts:553
+#: packages/terminal-extension/src/index.ts:553 packages/terminal-extension/src/index.ts:559
 msgid "Set the terminal theme"
 msgstr "Définissez le thème du terminal"
 
 #: packages/terminal/src/widget.ts:345
 msgid "Terminal %1"
 msgstr "Terminal %1"
```

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: fr\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_lsp/locale/jupyterlab_lsp.pot\n"
 "X-Crowdin-File-ID: 199\n"
 "Language-Team: French\n"
 "Language: fr_FR\n"
-"PO-Revision-Date: 2023-04-27 12:40\n"
+"PO-Revision-Date: 2023-05-29 08:42\n"
 
 #: /packages/jupyterlab-lsp/schema/completion.json:/description
 msgctxt "schema"
 msgid "LSP Completion settings."
 msgstr "Paramètres de complétion par LSP."
 
 #: /packages/jupyterlab-lsp/schema/completion.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/diagnostics.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/highlights.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/hover.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/jump_to.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/rename.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/signature.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/syntax_highlighting.json:/jupyter.lab.setting-icon-label
@@ -220,14 +220,24 @@
 msgstr "Codes de diagnostics qui ne devraient pas être affichés dans le panneau ni mis en évidence dans l'éditeur."
 
 #: /packages/jupyterlab-lsp/schema/diagnostics.json:/properties/ignoreMessagesPatterns/title
 msgctxt "settings"
 msgid "Diagnostic messages to ignore"
 msgstr "Messages de diagnostic à ignorer"
 
+#: /packages/jupyterlab-lsp/schema/diagnostics.json:/properties/ignoreSeverities/description
+msgctxt "settings"
+msgid "Severities of diagnostics which should not be shown in the panel nor highlighted in the editor."
+msgstr "Niveaux de diagnostics qui ne devraient pas être affichés dans le panneau ni mis en évidence dans l'éditeur."
+
+#: /packages/jupyterlab-lsp/schema/diagnostics.json:/properties/ignoreSeverities/title
+msgctxt "settings"
+msgid "Diagnostic severity levels to ignore"
+msgstr "Niveaux de diagnostic à ignorer"
+
 #: /packages/jupyterlab-lsp/schema/diagnostics.json:/title
 msgctxt "schema"
 msgid "Code Diagnostics"
 msgstr "Diagnostics de Code"
 
 #: /packages/jupyterlab-lsp/schema/highlights.json:/description
 msgctxt "schema"
@@ -405,14 +415,69 @@
 "  serverSettings: {\n"
 "    \"pyls. lugins.pydocstyle.enabled\": true,\n"
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
+msgstr "Configuration spécifique du serveur de language, trie par l'implémentation, par exemple: \n\n"
+"pyls: {\n"
+"  serverSettings: {\n"
+"    pyls: {\n"
+"      plugins: {\n"
+"        pydocstyle: {\n"
+"          enabled: true\n"
+"        },\n"
+"        flocons : {\n"
+"          enabled: false\n"
+"        },\n"
+"        flake8 : {\n"
+"          enabled: true\n"
+"        }\n"
+"      }\n"
+"    }\n"
+"  }\n"
+"}\n\n"
+"Alternativement, en utilisant les noms séparés par des points :\n\n"
+"pyls: {\n"
+"  serverSettings: {\n"
+"    \"pyls.plugins.pydocstyle.enabled\": true,\n"
+"    \"pyls.plugins.pyflakes.enabled\": false,\n"
+"    \"pyls.plugins.flake8.enabled\": true\n"
+"  }\n"
+"}"
+
 #: /packages/jupyterlab-lsp/schema/plugin.json:/properties/language_servers/title
 msgctxt "settings"
 msgid "Language Server"
 msgstr "Serveur de langage"
 
 #: /packages/jupyterlab-lsp/schema/plugin.json:/properties/logAllCommunication/description
 msgctxt "settings"
```

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/notebook.po`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: fr\n"
 "X-Crowdin-File: /main/extensions/notebook/locale/notebook.pot\n"
 "X-Crowdin-File-ID: 231\n"
 "Language-Team: French\n"
 "Language: fr_FR\n"
-"PO-Revision-Date: 2023-05-21 14:17\n"
+"PO-Revision-Date: 2023-07-04 11:34\n"
 
 #: /packages/application-extension/schema/menus.json:/description /packages/application-extension/schema/menus.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Menu Entries"
 msgstr "Entrées du menu de Jupyter Notebook"
 
 #: /packages/application-extension/schema/menus.json:/jupyter.lab.menus/main[2]/items[1]/submenu/label
@@ -25,14 +25,34 @@
 msgstr "Type de cellule"
 
 #: /packages/application-extension/schema/pages.json:/description /packages/application-extension/schema/pages.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Pages"
 msgstr "Pages du Jupyter Notebook"
 
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
 msgstr "Widget de titre"
 
 #: /packages/application-extension/schema/top.json:/description
 msgctxt "schema"
@@ -60,19 +80,14 @@
 msgstr "Zone supérieure de Jupyter Notebook"
 
 #: /packages/application-extension/schema/zen.json:/description /packages/application-extension/schema/zen.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Zen Mode"
 msgstr "Mode Zen de Jupyter Notebook"
 
-#: /packages/documentsearch-extension/schema/notebookShellWidgetListener.json:/description /packages/documentsearch-extension/schema/notebookShellWidgetListener.json:/title
-msgctxt "schema"
-msgid "Jupyter Notebook DocumentSearch Settings"
-msgstr "Paramètres de la recherche de documents de Jupyter Notebook"
-
 #: /packages/help-extension/schema/open.json:/description /packages/help-extension/schema/open.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Help Menu Entries"
 msgstr "Entrées du menu aide de Jupyter Notebook"
 
 #: /packages/lab-extension/schema/interface-switcher.json:/description
 msgctxt "schema"
@@ -130,14 +145,24 @@
 msgstr "Défilement automatique des sorties de cellules"
 
 #: /packages/notebook-extension/schema/scroll-output.json:/title
 msgctxt "schema"
 msgid "Jupyter Notebook Notebook"
 msgstr "Notebooks de Jupyter Notebook"
 
+#: /packages/tree-extension/schema/file-actions.json:/description
+msgctxt "schema"
+msgid "File Browser widget - File Actions settings."
+msgstr "Navigateur de fichiers - Paramètres des actions de fichiers."
+
+#: /packages/tree-extension/schema/file-actions.json:/title
+msgctxt "schema"
+msgid "File Browser Widget - File Actions"
+msgstr "Navigateur de fichiers - Actions de fichiers"
+
 #: /packages/tree-extension/schema/widget.json:/definitions/toolbarItem/properties/args/title
 msgctxt "settings"
 msgid "Command arguments"
 msgstr "Arguments de la commande"
 
 #: /packages/tree-extension/schema/widget.json:/definitions/toolbarItem/properties/command/title
 msgctxt "settings"
@@ -222,61 +247,65 @@
 msgstr "Éléments de la barre d'outils du navigateur de fichiers"
 
 #: /packages/tree-extension/schema/widget.json:/title
 msgctxt "schema"
 msgid "File Browser Widget"
 msgstr "Navigateur de fichiers"
 
-#: packages/application-extension/src/index.ts:119
+#: packages/application-extension/src/index.ts:1058
+msgid "Toggle Zen Mode"
+msgstr "Activer/désactiver le mode Zen"
+
+#: packages/application-extension/src/index.ts:141
 msgid "Are you sure you want to exit Jupyter Notebook?\n\n"
 "Any unsaved changes will be lost."
 msgstr "Êtes-vous sûr de vouloir quitter Jupyter Notebook ?\n\n"
 "Toutes les modifications non enregistrées seront perdues."
 
-#: packages/application-extension/src/index.ts:258
+#: packages/application-extension/src/index.ts:310
 msgid "Open JupyterLab"
 msgstr "Ouvrir JupyterLab"
 
-#: packages/application-extension/src/index.ts:266
+#: packages/application-extension/src/index.ts:318
 msgid "File Browser"
 msgstr "Navigateur de fichiers"
 
-#: packages/application-extension/src/index.ts:415
+#: packages/application-extension/src/index.ts:376
+msgid "Handle Local Link"
+msgstr "Gérer le lien local"
+
+#: packages/application-extension/src/index.ts:586
 msgid "Rename…"
 msgstr "Renommer…"
 
-#: packages/application-extension/src/index.ts:481
+#: packages/application-extension/src/index.ts:652
 msgid "Show Header"
 msgstr "Afficher l'en-tête"
 
-#: packages/application-extension/src/index.ts:571
+#: packages/application-extension/src/index.ts:742
 msgid "Show %1 in the left sidebar"
 msgstr "Afficher %1 dans la barre latérale de gauche"
 
-#: packages/application-extension/src/index.ts:576
+#: packages/application-extension/src/index.ts:747
 msgid "Show %1 in the right sidebar"
 msgstr "Afficher %1 dans la barre latérale de droite"
 
-#: packages/application-extension/src/index.ts:581
+#: packages/application-extension/src/index.ts:752
 msgid "Show %1 in the sidebar"
 msgstr "Afficher %1 dans la barre latérale"
 
-#: packages/application-extension/src/index.ts:696
+#: packages/application-extension/src/index.ts:867
 msgid "Left Sidebar"
 msgstr "Barre latérale gauche"
 
-#: packages/application-extension/src/index.ts:698
+#: packages/application-extension/src/index.ts:869
 msgid "Right Sidebar"
 msgstr "Barre latérale droite"
 
-#: packages/application-extension/src/index.ts:887
-msgid "Toggle Zen Mode"
-msgstr "Activer/désactiver le mode Zen"
-
-#: packages/application/src/shell.ts:203 packages/application/src/shell.ts:207
+#: packages/application/src/shell.ts:238 packages/application/src/shell.ts:242
 msgid "Collapse %1 side panel"
 msgstr "Réduire le panneau latéral %1"
 
 #: packages/help-extension/src/index.tsx:114
 msgid "Version: %1"
 msgstr "Version : %1"
 
@@ -284,15 +313,15 @@
 msgid "© 2021-2023 Jupyter Notebook Contributors"
 msgstr "©️ 2021-2023 Jupyter Notebook Contributeurs"
 
 #: packages/help-extension/src/index.tsx:131
 msgid "Dismiss"
 msgstr "Ignorer"
 
-#: packages/help-extension/src/index.tsx:77 packages/lab-extension/src/index.ts:178
+#: packages/help-extension/src/index.tsx:77 packages/lab-extension/src/index.ts:221
 msgid "Help"
 msgstr "Aide"
 
 #: packages/help-extension/src/index.tsx:80
 msgid "About %1"
 msgstr "À propos de %1"
 
@@ -300,38 +329,46 @@
 msgid "JUPYTER NOTEBOOK ON GITHUB"
 msgstr "JUPYTER NOTEBOOK SUR GITHUB"
 
 #: packages/help-extension/src/index.tsx:93
 msgid "CONTRIBUTOR LIST"
 msgstr "LISTE DES CONTRIBUTEURS"
 
-#: packages/lab-extension/src/index.ts:131
-msgid "Notebook"
-msgstr "Notebook"
+#: packages/lab-extension/src/index.ts:104
+msgid "JupyterLab"
+msgstr "JupyterLab"
 
-#: packages/lab-extension/src/index.ts:132 packages/lab-extension/src/index.ts:142
+#: packages/lab-extension/src/index.ts:105 packages/lab-extension/src/index.ts:115 packages/lab-extension/src/index.ts:95
 msgid "Open in %1"
 msgstr "Ouvrir dans %1"
 
-#: packages/lab-extension/src/index.ts:141
-msgid "JupyterLab"
-msgstr "JupyterLab"
+#: packages/lab-extension/src/index.ts:114
+msgid "NbClassic"
+msgstr "NbClassic"
 
-#: packages/lab-extension/src/index.ts:181
+#: packages/lab-extension/src/index.ts:184
+msgid "Open in..."
+msgstr "Ouvrir dans..."
+
+#: packages/lab-extension/src/index.ts:224
 msgid "Launch Jupyter Notebook File Browser"
 msgstr "Ouvrir le navigateur de fichiers Jupyter Notebook"
 
-#: packages/lab-extension/src/index.ts:82
-msgid "Open in..."
-msgstr "Ouvrir dans..."
+#: packages/lab-extension/src/index.ts:94
+msgid "Notebook"
+msgstr "Notebook"
 
-#: packages/notebook-extension/src/index.ts:107
+#: packages/notebook-extension/src/index.ts:109
 msgid "Last Checkpoint: %1"
 msgstr "Dernier point de contrôle : %1"
 
+#: packages/notebook-extension/src/index.ts:150
+msgid "Close and Shut Down Notebook"
+msgstr ""
+
 #: packages/notebook-extension/src/trusted.tsx:75
 msgid "JavaScript enabled for notebook display"
 msgstr "JavaScript activé pour l'affichage des notebooks"
 
 #: packages/notebook-extension/src/trusted.tsx:76
 msgid "JavaScript disabled for notebook display"
 msgstr "JavaScript désactivé pour l'affichage des notebooks"
@@ -340,31 +377,35 @@
 msgid "Not Trusted"
 msgstr "Non fiable"
 
 #: packages/notebook-extension/src/trusted.tsx:79
 msgid "Trusted"
 msgstr "Fiable"
 
-#: packages/tree-extension/src/index.ts:232
+#: packages/tree-extension/src/fileactions.tsx:39
+msgid "Select items to perform actions on them."
+msgstr "Sélectionnez les éléments sur lesquels effectuer des actions."
+
+#: packages/tree-extension/src/index.ts:284
 msgid "Files"
 msgstr "Fichiers"
 
-#: packages/tree-extension/src/index.ts:234
+#: packages/tree-extension/src/index.ts:286
 msgid "File Browser Section"
 msgstr "Section du navigateur de fichiers"
 
-#: packages/tree-extension/src/index.ts:249
+#: packages/tree-extension/src/index.ts:300
 msgid "Upload"
 msgstr "Importer"
 
-#: packages/tree-extension/src/index.ts:267
+#: packages/tree-extension/src/index.ts:318
 msgid "Filter files by name"
 msgstr "Filtrer les fichiers par nom"
 
-#: packages/tree-extension/src/index.ts:289
+#: packages/tree-extension/src/index.ts:340
 msgid "Running"
 msgstr "En cours"
 
-#: packages/tree-extension/src/index.ts:91
+#: packages/tree-extension/src/index.ts:95
 msgid "New"
 msgstr "Nouveau"
```

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_fr_fr-4.0.post1/jupyterlab_language_pack_fr_FR/locale/fr_FR/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/.gitignore` & `jupyterlab_language_pack_fr_fr-4.0.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/LICENSE.txt` & `jupyterlab_language_pack_fr_fr-4.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/pyproject.toml` & `jupyterlab_language_pack_fr_fr-4.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_fr_fr-4.0.post0/PKG-INFO` & `jupyterlab_language_pack_fr_fr-4.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-fr-FR
-Version: 4.0.post0
+Version: 4.0.post1
 Summary: JupyterLab French (France) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

