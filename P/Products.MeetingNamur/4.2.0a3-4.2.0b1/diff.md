# Comparing `tmp/Products.MeetingNamur-4.2.0a3.tar.gz` & `tmp/Products.MeetingNamur-4.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingNamur-4.2.0a3.tar", last modified: Thu Apr  6 13:52:25 2023, max compression
+gzip compressed data, was "Products.MeetingNamur-4.2.0b1.tar", last modified: Tue Jul  4 09:15:54 2023, max compression
```

## Comparing `Products.MeetingNamur-4.2.0a3.tar` & `Products.MeetingNamur-4.2.0b1.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.898542 Products.MeetingNamur-4.2.0a3/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4489 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/CHANGES.rst
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      679 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/MANIFEST.in
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5140 2023-04-06 13:52:25.898542 Products.MeetingNamur-4.2.0a3/PKG-INFO
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      148 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/README.rst
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/docs/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    18092 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/docs/LICENSE.GPL
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/docs/LICENSE.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       38 2023-04-06 13:52:25.898542 Products.MeetingNamur-4.2.0a3/setup.cfg
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1464 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/setup.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       76 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/EXTERNALS.txt
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/Extensions/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       26 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/Extensions/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      964 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/README.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1751 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    20146 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/adapters.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       22 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      562 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/configure.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6528 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      120 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/overrides.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/templates/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       75 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/templates/display_certified_signatures.pt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3222 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/config.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3773 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/configure.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1360 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/events.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      674 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/events.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4083 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/interfaces.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5058 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/PloneMeeting.pot
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5541 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1666 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3371 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5498 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1661 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1893 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3234 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5772 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1890 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3663 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8355 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2299 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2397 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4133 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1400 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/imio.actionspanel.pot
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1721 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/imio.history.pot
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5412 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1575 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3287 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2850 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/plone.pot
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      307 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/sync_pos.sh
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/migrations/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/migrations/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5060 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/migrations/migrate_to_4200.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      976 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/migrations/migrate_to_4_1.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/model/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       23 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/model/__init__.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      305 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/model/generate.sh
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4154 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/model/pm_updates.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      405 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/overrides.zcml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      709 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/cssregistry.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1421 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/import_steps.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      423 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/jsregistry.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      104 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/metadata.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      984 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/rolemap.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      890 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/skins.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      167 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/toolset.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    58818 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10860 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/MeetingNamur_examples_fr_marker.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.896541 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/budgetAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1032 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/decisionAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/itemAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      761 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/legalAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      305 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/nil.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/remarks.png
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     1663 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/import_data.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      898 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.897542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)   104980 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    37100 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    34356 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/toolset.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.897542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/MeetingNamur_tests_marker.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.897542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/attach.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/budget.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/budgetAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/cahier.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/decisionAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/itemAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/legalAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      411 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/negative.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/positive.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/remarks.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1585 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/import_data.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      327 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/import_steps.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      171 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/metadata.xml
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/toolset.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1269 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/refresh.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4488 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/setuphandlers.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.894542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.897542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_images/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      657 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.897542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_styles/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      787 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      348 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_styles/readme.txt
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.897542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_templates/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    11157 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    42515 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1102 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/testing.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      597 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/testing.zcml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.898542 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     1610 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1292 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1243 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/helpers.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10872 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testAdvices.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3710 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testAnnexes.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1326 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testChangeItemOrderView.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1217 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testColumns.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1342 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testContacts.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     3127 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testCustomMeeting.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5502 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testCustomMeetingItem.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1250 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testFaceted.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4244 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeeting.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1303 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeetingCategory.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1445 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeetingConfig.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     8524 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeetingItem.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1263 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testPortlets.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2204 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testSearches.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1254 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testSetup.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1307 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testToolPloneMeeting.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1207 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testUtils.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1266 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testValidators.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4289 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testViews.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3399 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testWFAdaptations.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     6685 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testWorkflows.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        8 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/version.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       56 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-04-06 13:52:25.895542 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5140 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/PKG-INFO
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8265 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/SOURCES.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/dependency_links.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/namespace_packages.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/not-zip-safe
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      271 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/requires.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-04-06 13:52:25.000000 Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/top_level.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4697 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/CHANGES.rst
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      679 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/MANIFEST.in
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5348 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      148 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/README.rst
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/docs/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    18092 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/docs/LICENSE.GPL
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/docs/LICENSE.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       38 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/setup.cfg
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1464 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/setup.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       76 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/EXTERNALS.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/Extensions/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       26 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/Extensions/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      964 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/README.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1751 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    31219 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/adapters.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       22 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      562 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/configure.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6528 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      120 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/overrides.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/templates/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       75 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/templates/display_certified_signatures.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3222 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/config.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3773 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/configure.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1438 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      674 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4083 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/interfaces.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5058 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/PloneMeeting.pot
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5541 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1666 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3371 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5498 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1661 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1893 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3234 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5772 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1890 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3663 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8355 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2299 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2397 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4133 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1400 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.actionspanel.pot
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1721 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.history.pot
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5412 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1575 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3287 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2850 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/plone.pot
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      307 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/sync_pos.sh
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5060 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4200.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      976 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       23 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/__init__.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      305 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/generate.sh
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4238 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/pm_updates.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      405 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/overrides.zcml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      709 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/cssregistry.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1421 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/import_steps.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      423 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/jsregistry.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      104 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/metadata.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      984 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/rolemap.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      890 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/skins.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/toolset.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    58818 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/MeetingNamur_examples_fr_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/budgetAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1032 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/decisionAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/itemAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      761 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      305 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/nil.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/remarks.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1663 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      898 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)   104980 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    37100 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    34356 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/toolset.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/MeetingNamur_tests_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/attach.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/budget.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/budgetAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/cahier.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/decisionAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/itemAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/legalAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      411 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/negative.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/positive.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/remarks.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1585 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/import_data.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      327 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/import_steps.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      171 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/metadata.xml
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/toolset.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1269 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/refresh.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4488 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/setuphandlers.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      657 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      787 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      348 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/readme.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    11157 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    42515 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1102 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      597 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.zcml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     1610 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1292 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1243 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/helpers.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10872 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAdvices.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3710 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAnnexes.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1326 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1217 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testColumns.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1342 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testContacts.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     3127 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5502 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1250 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testFaceted.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4244 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1303 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingCategory.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1445 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingConfig.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     8524 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingItem.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1263 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testPortlets.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2204 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSearches.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1254 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSetup.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1307 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1207 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testUtils.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1266 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testValidators.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4289 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testViews.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3399 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWFAdaptations.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     6685 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWorkflows.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        8 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/version.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       56 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5348 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8265 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/SOURCES.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/dependency_links.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/namespace_packages.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/not-zip-safe
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      271 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/requires.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/top_level.txt
```

### Comparing `Products.MeetingNamur-4.2.0a3/CHANGES.rst` & `Products.MeetingNamur-4.2.0b1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.0b1 (2023-07-04)
+--------------------
+
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+- Fixed issue with WF, roles, permissions and fields
+  [aduchene]
+
 4.2.0a3 (2023-04-06)
 --------------------
 
 - New proper release.
   [aduchene]
 
-
 4.2.0a2 (2023-04-06)
 --------------------
 
 - Adapted code regarding removal of MeetingConfig.useGroupsAsCategories. 
   [gbastien]
 
 4.2.0a1 (2023-02-23)
```

### Comparing `Products.MeetingNamur-4.2.0a3/MANIFEST.in` & `Products.MeetingNamur-4.2.0b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/PKG-INFO` & `Products.MeetingNamur-4.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingNamur
-Version: 4.2.0a3
+Version: 4.2.0b1
 Summary: PloneMeeting profile for city of Namur
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -21,21 +21,28 @@
 'Products.MeetingNamur' is a custom profile for 'Products.MeetingCommunes'.
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.0b1 (2023-07-04)
+--------------------
+
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+- Fixed issue with WF, roles, permissions and fields
+  [aduchene]
+
 4.2.0a3 (2023-04-06)
 --------------------
 
 - New proper release.
   [aduchene]
 
-
 4.2.0a2 (2023-04-06)
 --------------------
 
 - Adapted code regarding removal of MeetingConfig.useGroupsAsCategories. 
   [gbastien]
 
 4.2.0a1 (2023-02-23)
```

### Comparing `Products.MeetingNamur-4.2.0a3/docs/LICENSE.GPL` & `Products.MeetingNamur-4.2.0b1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/docs/LICENSE.txt` & `Products.MeetingNamur-4.2.0b1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/setup.py` & `Products.MeetingNamur-4.2.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 
-version = '4.2.0a3'
+version = '4.2.0b1'
 
 setup(name='Products.MeetingNamur',
       version=version,
       description="PloneMeeting profile for city of Namur",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       classifiers=[
         "Environment :: Web Environment",
```

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/README.txt` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/__init__.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/configure.zcml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/config.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/configure.zcml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/events.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 __author__ = """Gauthier BASTIEN <gauthier.bastien@imio.be>"""
 __docformat__ = 'plaintext'
 
 from Products.PloneMeeting.utils import forceHTMLContentTypeForEmptyRichFields
 
 def onItemLocalRolesUpdated(item, event):
     """Called after localRoles have been updated on the item."""
+    item.adapted().updateMeetingBudgetImpactReviewerRole()
     item.adapted().updateMeetingCertifiedSignaturesWriterLocalRoles()
 
 def onItemDuplicated(original, event):
-    """After item's cloning, we copy in description field the decision field
+    """After item's cloning, we copy in decisionProject field the decision field
        and clear decision field.
     """
     newItem = event.newItem
     # copy decision from source items in destination's deliberation if item is accepted
     if original.query_state() in ['accepted', 'accepted_but_modified'] and newItem != original:
-        newItem.setDescription(original.getDecision())
+        newItem.setDecisionProject(original.getDecision())
     # clear decision for new item
     newItem.setDecision('<p>&nbsp;</p>')
     # when item send in other config, we must clean modification style
     if newItem.portal_plonemeeting.getMeetingConfig(newItem) != original.portal_plonemeeting.getMeetingConfig(original):
-        newItem.setDescription(newItem.Description().replace('class="mltcorrection"', ''))
+        newItem.setDecisionProject(newItem.getDecisionProject().replace('class="mltcorrection"', ''))
     # Make sure we have 'text/html' for every Rich fields
     forceHTMLContentTypeForEmptyRichFields(newItem)
```

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/events.zcml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/interfaces.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/PloneMeeting.pot` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 #. Default: "close_done_descr"
 msgid "close_done_descr"
 msgstr "Le procès-verbal est maintenant clôturé, tous les points pour lesquels aucune décision n'avait été prise ont été automatiquement acceptés."
 
 #. Default: "closed"
 msgid "closed"
-msgstr "clôturé"
+msgstr "Clôturé"
 
 #. Default: "Create an item college from an item council"
 msgid "create_to_meeting-config-college_from_meeting-config-council"
 msgstr "Envoyer vers Collège Communal"
 
 #. Default: "Create an item council from an item college"
 msgid "create_to_meeting-config-council_from_meeting-config-college"
@@ -126,26 +126,26 @@
 #. Default: "decide_done_descr"
 msgid "decide_done_descr"
 msgstr "Vous pouvez maintenant rédiger le Procès-verbal de cette séance."
 
 # College meeting workflow states specific vocabulary
 #. Default: "decided"
 msgid "decided"
-msgstr "rédaction du PV"
+msgstr "Rédaction du PV"
 
 # transitions descriptions
 #. Default: "freeze_done_descr"
 msgid "freeze_done_descr"
 msgstr "L'ordre du jour vient d'être gelé."
 
 #. Default: "frozen"
 msgid "frozen"
-msgstr "gelé"
+msgstr "Gelé"
 
 #. Default: "itemfrozen"
 msgid "itemfrozen"
-msgstr "gelé"
+msgstr "Gelé"
 
 # College item workflow states specific vocabulary
 #. Default: "validated"
 msgid "validated"
-msgstr "validé"
+msgstr "Validé"
```

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/imio.actionspanel.pot` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/imio.history.pot` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/locales/plone.pot` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/migrations/migrate_to_4200.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/migrations/migrate_to_4_1.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/model/pm_updates.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/pm_updates.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 i18n_domain='PloneMeeting',
             ),
             optional=True,
         ),
         TextField(
             name='vote',
             widget=RichWidget(
-                condition="python: here.attributeIsUsed('vote')",
+                condition="python: here.attribute_is_used('vote')",
                 description="Vote",
                 description_msgid="item_vote_descr",
                 label='Vote',
                 label_msgid='MeetingNamur_vote',
                 i18n_domain='PloneMeeting',
             ),
             optional=True,
@@ -71,30 +71,33 @@
             default_content_type="text/html",
             allowable_content_types=('text/html',),
             default_output_type="text/x-html-safe",
         ),
         TextField(
             name='decisionProject',
             widget=RichWidget(
-                condition="python: here.attributeIsUsed('decisionProject')",
-                description="decisionProject",
-                description_msgid="item_decisionProject_descr",
+                condition="python: here.attribute_is_used('decisionProject')",
                 label='decisionProject',
                 label_msgid='projectOfDecision_label',
                 i18n_domain='PloneMeeting',
             ),
             optional=True,
-            write_permission="MeetingNamur: Write decisionProject",
+            searchable=True,
+            read_permission="PloneMeeting: Read decision",
+            write_permission='PloneMeeting: Write decision',
             default_content_type="text/html",
             allowable_content_types=('text/html',),
             default_output_type="text/x-html-safe",
         ),
     ), )
 
+    baseSchema['decision'].write_permission = "PloneMeeting: Write item MeetingManager reserved fields"
+
     completeSchema = baseSchema + specificSchema.copy()
+    
     return completeSchema
 
 
 MeetingItem.schema = update_item_schema(MeetingItem.schema)
 
 # Classes have already been registered, but we register them again here
 # because we have potentially applied some schema adaptations (see above).
```

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/cssregistry.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/import_steps.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/rolemap.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/skins.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/default/workflows.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/import_data.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/attach.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/budget.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/cahier.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/images/positive.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles/testing/import_data.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/profiles.zcml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/setuphandlers.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/testing.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/testing.zcml` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/__init__.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/helpers.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testAdvices.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testAnnexes.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testChangeItemOrderView.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testColumns.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testContacts.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testCustomMeeting.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testCustomMeetingItem.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testFaceted.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeeting.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeetingCategory.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeetingConfig.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testMeetingItem.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testPortlets.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testSearches.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testSetup.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testToolPloneMeeting.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testUtils.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testValidators.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testViews.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testWFAdaptations.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products/MeetingNamur/tests/testWorkflows.py` & `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/PKG-INFO` & `Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingNamur
-Version: 4.2.0a3
+Version: 4.2.0b1
 Summary: PloneMeeting profile for city of Namur
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -21,21 +21,28 @@
 'Products.MeetingNamur' is a custom profile for 'Products.MeetingCommunes'.
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.0b1 (2023-07-04)
+--------------------
+
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+- Fixed issue with WF, roles, permissions and fields
+  [aduchene]
+
 4.2.0a3 (2023-04-06)
 --------------------
 
 - New proper release.
   [aduchene]
 
-
 4.2.0a2 (2023-04-06)
 --------------------
 
 - Adapted code regarding removal of MeetingConfig.useGroupsAsCategories. 
   [gbastien]
 
 4.2.0a1 (2023-02-23)
```

### Comparing `Products.MeetingNamur-4.2.0a3/src/Products.MeetingNamur.egg-info/SOURCES.txt` & `Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

