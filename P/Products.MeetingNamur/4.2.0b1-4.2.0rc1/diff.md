# Comparing `tmp/Products.MeetingNamur-4.2.0b1.tar.gz` & `tmp/Products.MeetingNamur-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingNamur-4.2.0b1.tar", last modified: Tue Jul  4 09:15:54 2023, max compression
+gzip compressed data, was "Products.MeetingNamur-4.2.0rc1.tar", last modified: Tue Jul  4 14:20:07 2023, max compression
```

## Comparing `Products.MeetingNamur-4.2.0b1.tar` & `Products.MeetingNamur-4.2.0rc1.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4697 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/CHANGES.rst
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      679 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/MANIFEST.in
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5348 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/PKG-INFO
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      148 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/README.rst
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/docs/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    18092 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/docs/LICENSE.GPL
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/docs/LICENSE.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       38 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/setup.cfg
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1464 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/setup.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       76 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/EXTERNALS.txt
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/Extensions/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       26 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/Extensions/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      964 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/README.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1751 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    31219 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/adapters.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       22 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      562 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/configure.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6528 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      120 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/overrides.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/templates/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       75 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/templates/display_certified_signatures.pt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3222 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/config.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3773 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/configure.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1438 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      674 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4083 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/interfaces.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5058 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/PloneMeeting.pot
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5541 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1666 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3371 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5498 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1661 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1893 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3234 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5772 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1890 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3663 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8355 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2299 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2397 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4133 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1400 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.actionspanel.pot
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1721 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.history.pot
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5412 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1575 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3287 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2850 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/plone.pot
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      307 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/sync_pos.sh
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5060 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4200.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      976 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       23 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/__init__.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      305 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/generate.sh
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4238 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/pm_updates.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      405 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/overrides.zcml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      709 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/cssregistry.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1421 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/import_steps.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      423 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/jsregistry.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      104 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/metadata.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      984 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/rolemap.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      890 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/skins.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/toolset.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    58818 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10860 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.573683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/MeetingNamur_examples_fr_marker.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/budgetAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1032 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/decisionAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/itemAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      761 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      305 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/nil.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/remarks.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1663 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      898 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)   104980 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    37100 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    34356 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/toolset.xml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/MeetingNamur_tests_marker.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/attach.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/budget.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/budgetAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/cahier.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/decisionAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/itemAnnex.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/legalAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      411 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/negative.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/positive.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/remarks.png
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1585 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/import_data.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      327 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/import_steps.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      171 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/metadata.xml
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/toolset.xml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1269 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles.zcml
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/refresh.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4488 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/setuphandlers.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.571683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_images/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      657 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      787 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      348 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/readme.txt
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.574683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    11157 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    42515 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1102 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      597 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.zcml
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.575683 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     1610 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1292 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/__init__.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1243 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/helpers.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10872 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAdvices.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3710 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAnnexes.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1326 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1217 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testColumns.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1342 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testContacts.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     3127 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeeting.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5502 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1250 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testFaceted.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4244 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeeting.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1303 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingCategory.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1445 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingConfig.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     8524 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingItem.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1263 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testPortlets.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2204 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSearches.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1254 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSetup.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1307 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1207 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testUtils.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1266 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testValidators.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4289 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testViews.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3399 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWFAdaptations.py
--rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     6685 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWorkflows.py
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        8 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/version.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)       56 2023-07-04 09:15:53.000000 Products.MeetingNamur-4.2.0b1/src/Products/__init__.py
-drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 09:15:54.572683 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5348 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/PKG-INFO
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8265 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/SOURCES.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/dependency_links.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/namespace_packages.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/not-zip-safe
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)      271 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/requires.txt
--rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-07-04 09:15:54.000000 Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/top_level.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.649685 Products.MeetingNamur-4.2.0rc1/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4852 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/CHANGES.rst
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      679 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/MANIFEST.in
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5504 2023-07-04 14:20:07.649685 Products.MeetingNamur-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      148 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/README.rst
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/docs/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    18092 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/docs/LICENSE.GPL
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/docs/LICENSE.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       38 2023-07-04 14:20:07.649685 Products.MeetingNamur-4.2.0rc1/setup.cfg
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1465 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/setup.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       76 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/EXTERNALS.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/Extensions/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       26 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/Extensions/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      964 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/README.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1751 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    31435 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/adapters.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       22 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      562 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/configure.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6239 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      120 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/overrides.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/templates/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       73 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/templates/display_certified_signatures.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3116 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/config.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3773 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/configure.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1438 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/events.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      674 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/events.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4083 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/interfaces.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5058 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/PloneMeeting.pot
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5541 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1666 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3371 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5498 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1661 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1893 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3234 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5772 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1890 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3663 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8599 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2299 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2397 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4133 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1400 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/imio.actionspanel.pot
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1721 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/imio.history.pot
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5412 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1575 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3287 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2850 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/plone.pot
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      307 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/sync_pos.sh
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/migrations/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/migrations/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5060 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/migrations/migrate_to_4200.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      976 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/model/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       23 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/model/__init__.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      305 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/model/generate.sh
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4280 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/model/pm_updates.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      405 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/overrides.zcml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      709 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/cssregistry.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1421 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/import_steps.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      423 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/jsregistry.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      104 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/metadata.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      600 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/rolemap.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      890 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/skins.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/toolset.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    58818 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10860 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.647685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/MeetingNamur_examples_fr_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/budgetAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1032 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/decisionAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/itemAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      761 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      305 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/nil.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/remarks.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1663 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      898 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)   104980 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    37100 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    34356 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/toolset.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/MeetingNamur_tests_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/attach.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/budget.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/budgetAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/cahier.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/decisionAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/itemAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/legalAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      411 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/negative.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/positive.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/remarks.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1585 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/import_data.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      327 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/import_steps.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      171 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/metadata.xml
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/toolset.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1269 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/refresh.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4488 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/setuphandlers.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.645685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      657 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_styles/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      787 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      348 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_styles/readme.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.648685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_templates/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    11157 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    42856 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1102 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/testing.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      597 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/testing.zcml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.649685 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     1610 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1292 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1243 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/helpers.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10872 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testAdvices.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3710 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testAnnexes.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1326 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1217 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testColumns.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1342 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testContacts.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     3088 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testCustomMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5114 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1250 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testFaceted.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4325 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1303 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeetingCategory.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1445 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeetingConfig.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     8524 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeetingItem.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1263 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testPortlets.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2204 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testSearches.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1254 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testSetup.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1307 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1207 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testUtils.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1266 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testValidators.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4289 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testViews.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3458 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testWFAdaptations.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     6685 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testWorkflows.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        8 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/version.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       56 2023-07-04 14:20:06.000000 Products.MeetingNamur-4.2.0rc1/src/Products/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2023-07-04 14:20:07.646685 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5504 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8265 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/SOURCES.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/dependency_links.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/namespace_packages.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/not-zip-safe
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      271 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/requires.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2023-07-04 14:20:07.000000 Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/top_level.txt
```

### Comparing `Products.MeetingNamur-4.2.0b1/CHANGES.rst` & `Products.MeetingNamur-4.2.0rc1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.0rc1 (2023-07-04)
+---------------------
+
+- Fixed broken tests.
+  [aduchene]
+- Don't use a custom permission for ItemCertifiedSignatures
+  [aduchene]
+
+
 4.2.0b1 (2023-07-04)
 --------------------
 
 - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
   [gbastien]
 - Fixed issue with WF, roles, permissions and fields
   [aduchene]
```

### Comparing `Products.MeetingNamur-4.2.0b1/MANIFEST.in` & `Products.MeetingNamur-4.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/PKG-INFO` & `Products.MeetingNamur-4.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingNamur
-Version: 4.2.0b1
+Version: 4.2.0rc1
 Summary: PloneMeeting profile for city of Namur
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -21,14 +21,23 @@
 'Products.MeetingNamur' is a custom profile for 'Products.MeetingCommunes'.
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.0rc1 (2023-07-04)
+---------------------
+
+- Fixed broken tests.
+  [aduchene]
+- Don't use a custom permission for ItemCertifiedSignatures
+  [aduchene]
+
+
 4.2.0b1 (2023-07-04)
 --------------------
 
 - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
   [gbastien]
 - Fixed issue with WF, roles, permissions and fields
   [aduchene]
```

### Comparing `Products.MeetingNamur-4.2.0b1/docs/LICENSE.GPL` & `Products.MeetingNamur-4.2.0rc1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/docs/LICENSE.txt` & `Products.MeetingNamur-4.2.0rc1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/setup.py` & `Products.MeetingNamur-4.2.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 
-version = '4.2.0b1'
+version = '4.2.0rc1'
 
 setup(name='Products.MeetingNamur',
       version=version,
       description="PloneMeeting profile for city of Namur",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       classifiers=[
         "Environment :: Web Environment",
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/README.txt` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/__init__.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/adapters.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from AccessControl import ClassSecurityInfo
 from AccessControl.class_init import InitializeClass
-from Products.MeetingNamur.config import WriteDecisionProject, WriteCertified
-from Products.PloneMeeting.model.adaptations import WF_APPLIED, grantPermission
+from Products.MeetingNamur.config import WriteDecisionProject
+from Products.PloneMeeting.model.adaptations import WF_APPLIED
 from collective.contact.plonegroup.utils import get_organizations
+from collective.contact.plonegroup.utils import get_plone_group_id
+from imio.helpers.cache import get_plone_groups_for_user
 from imio.helpers.xhtml import xhtmlContentIsEmpty
 from plone import api
 from Products.Archetypes.atapi import DisplayList
 from Products.CMFCore.utils import getToolByName
 from Products.MeetingCommunes.adapters import CustomMeeting, CustomMeetingConfig
 from Products.MeetingCommunes.adapters import CustomMeetingItem
 from Products.MeetingCommunes.adapters import CustomToolPloneMeeting
@@ -28,28 +30,29 @@
 from Products.MeetingNamur.interfaces import IMeetingNamurCouncilWorkflowConditions
 from Products.MeetingNamur.interfaces import IMeetingNamurWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingNamurWorkflowConditions
 from Products.PloneMeeting.adapters import ItemPrettyLinkAdapter
 from Products.PloneMeeting.interfaces import IMeetingCustom, IMeetingConfigCustom
 from Products.PloneMeeting.interfaces import IMeetingItemCustom
 from Products.PloneMeeting.interfaces import IToolPloneMeetingCustom
-from Products.PloneMeeting.Meeting import MeetingWorkflowActions
 from Products.PloneMeeting.MeetingConfig import MeetingConfig
 from Products.PloneMeeting.MeetingItem import MeetingItem
 from Products.PloneMeeting.MeetingItem import MeetingItemWorkflowActions
 from Products.PloneMeeting.utils import sendMail, org_id_to_uid
 from zope.i18n import translate
 from zope.interface import implements
 
 
 
 customWfAdaptations = (
     'item_validation_shortcuts',
     'item_validation_no_validate_shortcuts',
     'only_creator_may_delete',
+    'meeting_remove_global_access',
+    'meetingmanager_correct_closed_meeting',
     # first define meeting workflow state removal
     'no_freeze',
     'no_publication',
     'no_decide',
     # then define added item decided states
     'accepted_but_modified',
     'postpone_next_meeting',
@@ -67,15 +70,14 @@
     'return_to_proposing_group_with_all_validations',
     'accepted_out_of_meeting',
     'accepted_out_of_meeting_and_duplicated',
     'accepted_out_of_meeting_emergency',
     'accepted_out_of_meeting_emergency_and_duplicated',
     'transfered',
     'transfered_and_duplicated',
-    'meetingmanager_correct_closed_meeting',
     'namur_meetingmanager_may_not_edit_decision_project',
 )
 MeetingConfig.wfAdaptations = customWfAdaptations
 
 
 class CustomNamurMeetingConfig(CustomMeetingConfig):
     implements(IMeetingConfigCustom)
@@ -278,25 +280,35 @@
             res = []
             for item in items:
                 res.append((i, item))
                 i = i + 1
             items = res
         return res
 
-
-
 class CustomNamurMeetingItem(CustomMeetingItem):
     """Adapter that adapts a meeting item implementing IMeetingItem to the
        interface IMeetingItemCustom."""
     implements(IMeetingItemCustom)
     security = ClassSecurityInfo()
 
     def __init__(self, item):
         self.context = item
 
+    security.declarePublic('mayEditCertifiedSignatures')
+
+    def mayEditCertifiedSignatures(self):
+        """Check whether the current user may edit the certified signatures.
+           Manager may always do it but only the creators may edit them in accepted states"""
+        tool = api.portal.get_tool('portal_plonemeeting')
+        item = self.getSelf()
+        cfg = tool.getMeetingConfig(self.context)
+        if tool.isManager(cfg):
+            return True
+        is_creator = get_plone_group_id(item.getProposingGroup(), "creators") in get_plone_groups_for_user()
+        return is_creator and item.query_state() in cfg.getItemPositiveDecidedStates()
 
     security.declarePublic('print_scan_id_barcode')
 
     def print_scan_id_barcode(self, **kwargs):
         """Helper that will call scan_id_barcode from imio.zamqp.core
            and that will make sure that it is not called several times."""
         from imio.zamqp.core.utils import scan_id_barcode
@@ -614,30 +626,19 @@
             self, meetingConfig, wfAdaptation, logger, itemWorkflow, meetingWorkflow
     ):
         """This function applies workflow changes as specified by the
         p_meetingConfig."""
 
         if wfAdaptation == "namur_meetingmanager_may_not_edit_decision_project":
             itemStates = itemWorkflow.states
-
-            itemWorkflow.permissions = itemWorkflow.permissions + (WriteCertified, )
-            creators_certified_sign_states = ["delayed", "accepted_but_modified", "accepted"]
-            for state_id in itemStates:
-                if state_id in creators_certified_sign_states:
-                    itemStates[state_id].setPermission(WriteCertified, False, ["Manager", "Contributor"])
-                else:
-                    itemStates[state_id].setPermission(WriteCertified, False, ["Manager"])
-
-
             # First, we make sure that WriteDecisionProject perm is not acquired
             for state_id in itemStates:
                 itemStates[state_id].setPermission(WriteDecisionProject, False, [])
             # Then, we set appropriate roles for the validationWF
             itemWorkflow.permissions = itemWorkflow.permissions + (WriteDecisionProject, )
-
             if "itemcreated" in itemStates:
                 itemStates.itemcreated.setPermission(WriteDecisionProject, False, ["Manager", "Editor"])
             if "returned_to_proposing_group" in itemStates:
                 itemStates["returned_to_proposing_group"].setPermission(WriteDecisionProject, False, ["Manager", "Editor"])
 
             for validation_level in meetingConfig.getItemWFValidationLevels():
                 state_id = validation_level['state']
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/configure.zcml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,16 @@
     @button.buttonAndHandler(_('Cancel'), name='cancel')
     def handleCancel(self, action):
         self._finishedSent = True
 
     def update(self):
         """ """
         # raise Unauthorized if current user can not manage itemAssembly
-        if not api.user.get_current().has_permission('MeetingNamur: Write certified signatures',
-                                                                         self.context):
+        if not self.context.adapted().mayEditCertifiedSignatures():
             raise Unauthorized
-
         super(ManageItemCertifiedSignaturesForm, self).update()
         # after calling parent's update, self.actions are available
         self.actions.get('cancel').addClass('standalone')
 
     def updateWidgets(self):
         # XXX manipulate self.fields BEFORE doing form.Form.updateWidgets
         form.Form.updateWidgets(self)
@@ -139,18 +137,15 @@
         return super(ManageItemCertifiedSignaturesForm, self).render()
 
     def _doApplyItemCertifiedSignatures(self):
         """
           The method actually do the job, set the itemSignatures on self.context
           and following items if defined
         """
-        user = self.context.portal_membership.getAuthenticatedMember()
-        if not user.has_permission('MeetingNamur: Write certified signatures',
-                                                                         self.context):
-
+        if not self.context.adapted().mayEditCertifiedSignatures():
             raise Unauthorized
 
         self.context.setItemCertifiedSignatures(self.item_certified_signatures)
 
         plone_utils = getToolByName(self.context, 'plone_utils')
         plone_utils.addPortalMessage(_("Item certified signatures have been updated."))
         self._finishedSent = True
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/config.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 
 PROJECTNAME = "MeetingNamur"
 
 # Permissions
 WriteDecisionProject = 'MeetingNamur: Write decisionProject'
 setDefaultRoles(WriteDecisionProject, ('Manager', 'Member'))
-WriteCertified = 'MeetingNamur: Write certified signatures'
-setDefaultRoles(WriteCertified, ('Manager',))
 
 product_globals = globals()
 
 STYLESHEETS = [{'id': 'meetingnamur.css',
                 'title': 'MeetingNamur CSS styles'}]
 
 PMconfig.EXTRA_GROUP_SUFFIXES = [
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/configure.zcml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/events.zcml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/interfaces.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/PloneMeeting.pot` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files 2% similar despite different names*

```diff
@@ -194,7 +194,11 @@
 #. Default: "validated items"
 msgid "searchvalidateditems"
 msgstr "les points validés"
 
 #. Default: "TaxController"
 msgid "taxControllerGroupTitle"
 msgstr "Receveur"
+
+#. Default: "wa_namur_meetingmanager_may_not_edit_decision_project"
+msgid "wa_namur_meetingmanager_may_not_edit_decision_project"
+msgstr "Les gestionnaires de séances ne peuvent pas éditer les projets de décision sauf en correction (Namur)"
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 #. Default: "backToFrozen_done_descr"
 msgid "backToFrozen_done_descr"
 msgstr "Vous ne pouvez plus rédiger le Procès-verbal pour l'instant."
 
 #. Default: "close"
 msgid "close"
-msgstr "clôturer"
+msgstr "Clôturer"
 
 #. Default: "close_done_descr"
 msgid "close_done_descr"
 msgstr "Le procès-verbal est maintenant clôturé, tous les points pour lesquels aucune décision n'avait été prise ont été automatiquement acceptés."
 
 #. Default: "closed"
 msgid "closed"
@@ -117,15 +117,15 @@
 #. Default: "Create an item council from an item college"
 msgid "create_to_meeting-config-council_from_meeting-config-college"
 msgstr "Envoyer vers Conseil Communal"
 
 # College meeting workflow transitions specific vocabulary
 #. Default: ""
 msgid "decide"
-msgstr "rédiger le PV"
+msgstr "Rédiger le PV"
 
 #. Default: "decide_done_descr"
 msgid "decide_done_descr"
 msgstr "Vous pouvez maintenant rédiger le Procès-verbal de cette séance."
 
 # College meeting workflow states specific vocabulary
 #. Default: "decided"
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.actionspanel.pot` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/imio.history.pot` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/locales/plone.pot` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4200.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/model/pm_updates.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/model/pm_updates.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
         StringField(
             name='grpBudgetInfos',
             widget=MultiSelectionWidget(
                 description="GrpBudgetInfos",
                 description_msgid="MeetingNamur_descr_grpBudgetInfos",
                 size=10,
+                format="checkbox",
                 label='GrpBudgetInfos',
                 label_msgid='MeetingNamur_label_grpBudgetInfos',
                 i18n_domain='PloneMeeting',
             ),
             vocabulary='listGrpBudgetInfosAdviser',
             multiValued=1,
             enforceVocabulary=False,
@@ -79,15 +80,15 @@
                 label='decisionProject',
                 label_msgid='projectOfDecision_label',
                 i18n_domain='PloneMeeting',
             ),
             optional=True,
             searchable=True,
             read_permission="PloneMeeting: Read decision",
-            write_permission='PloneMeeting: Write decision',
+            write_permission="MeetingNamur: Write decisionProject",
             default_content_type="text/html",
             allowable_content_types=('text/html',),
             default_output_type="text/x-html-safe",
         ),
     ), )
 
     baseSchema['decision'].write_permission = "PloneMeeting: Write item MeetingManager reserved fields"
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/cssregistry.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/import_steps.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/skins.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/default/workflows.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/attach.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/budget.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/cahier.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/images/positive.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles/testing/import_data.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/profiles.zcml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/setuphandlers.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt`

 * *Files 1% similar despite different names*

```diff
@@ -227,35 +227,14 @@
                    tal:define="edit_css_classes python: context.mayQuickEdit('listType') and 'tooltipster-item-listtype-change item_listType Editable pmAction' or ''"
                    tal:attributes="data-base_url string:${context_url};
                                    class string:${edit_css_classes} item_attribute_label item_listType_${context/getListType}">
                     <span metal:use-macro="python: here.widget('listType', mode='view')" />
                 </span>
             </div>
 
-            <tal:comment replace="nothing">XXX MeetingNamur</tal:comment>
-            <tal:comment replace="nothing">Item certified signatures</tal:comment>
-            <div class="discreet" tal:condition="python: meeting">
-                <tal:defines define="redefinedItemCertifiedSignatures python: context.getItemCertifiedSignatures();
-                       mayQuickEdit python: member.has_permission('MeetingNamur: Write certified signatures', context);
-                       class_if_highlighted python: redefinedItemCertifiedSignatures and 'highlightRedefinedValue' or '';
-                       class_to_use python: mayQuickEdit and (class_if_highlighted and class_if_highlighted + ' itemAssemblyEditable' or 'itemAssemblyEditable') or class_if_highlighted">
-                    <div tal:attributes="class class_to_use"><i>
-                        <a tal:condition="mayQuickEdit" href="manage_item_certified_signatures_form"
-                                                        class="link-overlay-pm">
-                            <span i18n:translate="item_certifiedSignatures"></span>
-                        </a>
-                        <span tal:condition="not: mayQuickEdit"
-                                 tal:attributes="class class_to_use"
-                                 i18n:translate="item_certified"></span>
-                    </i>:&nbsp;&nbsp;
-                    </div>
-                    <div tal:content="structure context/getItemCertifiedSignatures"/>
-                </tal:defines>
-            </div>
-
             <tal:comment replace="nothing">Send to authority?</tal:comment>
             <div class="discreet" tal:condition="python: 'sendToAuthority' in usedAttrs">
                 <span class="item_attribute_label"
                       i18n:translate="PloneMeeting_label_sendToAuthority"></span>:&nbsp;&nbsp;
                 <span metal:use-macro="python: here.widget('sendToAuthority', mode='view')" />
             </div>
 
@@ -324,15 +303,39 @@
             <div class="discreet">
                 <i>
                     <div tal:condition="python: context.getIsConfidentialItem()">
                         <span i18n:translate="MeetingNamur_isConfidentialItem"></span>
                     </div>
                 </i>
             </div>
+            <tal:comment replace="nothing">XXX MeetingNamur</tal:comment>
+            <tal:comment replace="nothing">Item certified signatures</tal:comment>
+            <div class="discreet" tal:condition="python: meeting">
+                <tal:defines define="redefinedItemCertifiedSignatures python: context.getItemCertifiedSignatures();
+                      mayQuickEdit python: context.adapted().mayEditCertifiedSignatures();
+                      class_if_highlighted python: redefinedItemCertifiedSignatures and 'item_attribute_label highlightValue' or '';
+                      class_to_use python: mayQuickEdit and (class_if_highlighted and class_if_highlighted + ' item_attribute_label' or 'item_attribute_label') or class_if_highlighted">
+                    <div tal:attributes="class class_to_use">
+                        <a tal:condition="mayQuickEdit" href="manage_item_certified_signatures_form"
+                                                        class="link-overlay-pm">
+                            <span tal:attributes="class class_to_use" i18n:translate="item_certifiedSignatures"></span>:
+                            <img title="Edit this field"
+                                 style="cursor:pointer;border-bottom: 1px dotted #205c90;"
+                                 i18n:attributes="title fastedit_edit"
+                                 tal:attributes="src string:$portal_url/edit.png;
+                            "/>
+                        </a>
+                        <span tal:condition="not: mayQuickEdit"
+                                 tal:attributes="class class_to_use"
+                                 i18n:translate="item_certified"></span>
 
+                    </div>
+                    <div tal:content="structure python: context.getItemCertifiedSignatures().replace('\n', '<br>')"/>
+                </tal:defines>
+            </div>
             <tal:comment replace="nothing">Item initiator</tal:comment>
             <div class="discreet" tal:condition="python: 'itemInitiator' in usedAttrs">
                 <tal:defines define="itemInitiator python: context.getItemInitiator()">
                     <span class="item_attribute_label" i18n:translate="PloneMeeting_label_itemInitiator"></span>:&nbsp;&nbsp;
                     <tal:block condition="itemInitiator">
                         <span metal:use-macro="python: here.widget('itemInitiator', mode='view')" />
                     </tal:block>
```

#### html2text {}

```diff
@@ -2,37 +2,37 @@
 between items of the same meeting
 Proposing group (when                                                                      Preferred meeting
 proposingGroupWithGroupInCharge                                                                  :       -
 is not used)                                                            Meeting where this item is presented
 :       -                                                                    Presented in meeting:       -
 Groups in charge                                                                                   List type
 :      -
- Proposing group (when                                            XXX MeetingNamur Item certified signatures
-proposingGroupWithGroupInCharge
-is used)                                                                                                 :  
-:     ()   -                                                                           Send to authority?
-Associated groups                                                                                       :  
-:      -                                                                     Is acceptable out of meeting?
-Category                                                                                                :  
-:    -                                                                    Other MeetingConfigs Clonable To
- Classifier                                  :    Other mc clonable to (Emergency, privacy)  -  â Details
-:   - -                                                                                        To discuss?
-Committees                                                                                              :  
-:      -                                                                                         Poll type
-Advices                                                                                 :       â Details
-:    Advisers  - â Details                                                      Oral question or item
-Copy groups for this item            [#] This item is an oral question   This item is not an oral question
-  :    Copy groups  -                                                 XXX MeetingNamur Confidential item ?
- Item is signed?                                                                              Item initiator
-:                                                                                                :      -
-Taken over by                                                                                  Item keywords
-:                                                                                                     :  
-Item emergency                                                                                     Item tags
-:       â History                                                                                :  
-Item completeness                                                                                    Privacy
+ Proposing group (when                                                                    Send to authority?
+proposingGroupWithGroupInCharge                                                                         :  
+is used)                                                                       Is acceptable out of meeting?
+:     ()   -                                                                                         :  
+Associated groups                                                           Other MeetingConfigs Clonable To
+:      -                                   :    Other mc clonable to (Emergency, privacy)  -  â Details
+Category                                                                                         To discuss?
+:    -                                                                                                :  
+ Classifier                                                                                        Poll type
+:   - -                                                                               :       â Details
+Committees                                                                             Oral question or item
+:      -                           [#] This item is an oral question   This item is not an oral question
+Advices                                                                 XXX MeetingNamur Confidential item ?
+:    Advisers  - â Details                                 XXX MeetingNamur Item certified signatures
+Copy groups for this item                                                                         :_[Image]
+  :    Copy groups  -                                                                       Item initiator
+ Item is signed?                                                                                   :      -
+:                                                                                            Item keywords
+Taken over by                                                                                           :  
+:                                                                                                Item tags
+Item emergency                                                                                          :  
+:       â History                                                                             Privacy
+Item completeness
 :       â History
 Assembly and signatures
   Assembly Number of attendees  [Image]  and  signatures Number of attendees
 [Image]
 [Image]
 
   Assembly    signatures
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/testing.zcml` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/__init__.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/helpers.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAdvices.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testAnnexes.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testColumns.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testContacts.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeeting.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testCustomMeeting.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,37 @@
 class testCustomMeeting(MeetingNamurTestCase, mctcmi):
     """
         Tests the Meeting adapted methods
     """
 
     def test_InitializeDecisionField(self):
         """
-            In the doDecide method, we initialize the Decision field to a default value made of
-            Title+Description if the field is empty...
+            In the doDecide method, we initialize the Decision field with the decisionProject field
         """
         # check that it works
         # check that if the field contains something, it is not intialized again
         self.changeUser('admin')
         self._removeConfigObjectsFor(self.meetingConfig)
         self.changeUser('pmManager')
         m = self.create('Meeting', date=DateTime('2007/12/11 09:00:00').asdatetime())
         # create some items
         # empty decision
         i1 = self.create('MeetingItem', title='Item1')
         i1.setDecision("")
-        i1.setDescription("<p>Description Item1</p>")
+        i1.setDecisionProject("<p>Description Item1</p>")
         i1.setProposingGroup(self.developers_uid)
         # decision field is already filled
         i2 = self.create('MeetingItem', title='Item2')
         i2.setDecision("<p>Decision Item2</p>")
-        i2.setDescription("<p>Description Item2</p>")
+        i2.setDecisionProject("<p>Description Item2</p>")
         i2.setProposingGroup(self.developers_uid)
         # create an item with the default Kupu empty value
         i3 = self.create('MeetingItem', title='Item3')
         i3.setDecision("<p></p>")
-        i3.setDescription("<p>Description Item3</p>")
+        i3.setDecisionProject("<p>Description Item3</p>")
         i3.setProposingGroup(self.developers_uid)
         # present every items in the meeting
         items = (i1, i2, i3)
         # check the decision field of every item
         self.assertEquals(i1.getDecision(), "")
         self.assertEquals(i2.getDecision(), "<p>Decision Item2</p>")
         self.assertEquals(i3.getDecision(), "<p></p>")
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 from datetime import timedelta
 
 from AccessControl import Unauthorized
 from Products.MeetingCommunes.tests.testCustomMeetingItem import testCustomMeetingItem as mctcmi
 from Products.MeetingNamur.tests.MeetingNamurTestCase import MeetingNamurTestCase
+from Products.PloneMeeting.utils import org_id_to_uid
 
 
 class testCustomMeetingItem(MeetingNamurTestCase, mctcmi):
     """
         Tests the Meeting adapted methods
     """
 
@@ -17,33 +18,27 @@
         and state is, at least "itemFrozen". Retrieve role for other grp_budgetimpactreviewers
         """
         self.changeUser('pmManager')
         m = self._createMeetingWithItems()
         self.do(m, 'freeze')
         item = m.get_items()[0]
         # no MeetingBudgetImpactReviewer in rôle
-        self.assertEquals((u'developers_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
-        self.assertEquals((u'vendors_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
-        self.assertEquals((u'finances_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
-        self.assertEquals((u'taxes_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
-        item.setGrpBudgetInfos(('finances',))
-        item.adapted().onEdit(True)
+        developers_budgetimpactreviewers_uid = org_id_to_uid("developers_budgetimpactreviewers")
+        vendors_budgetimpactreviewers_uid = org_id_to_uid("vendors_budgetimpactreviewers")
+        self.assertFalse((developers_budgetimpactreviewers_uid, (
+            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
+        self.assertFalse((vendors_budgetimpactreviewers_uid, (
+            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
+        item.setGrpBudgetInfos(('developers',))
+        item.update_local_roles()
         # MeetingBudgetImpactReviewer role define for finance (only)
-        self.assertEquals((u'developers_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
-        self.assertEquals((u'vendors_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
-        self.assertEquals((u'finances_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), True)
-        self.assertEquals((u'taxes_budgetimpactreviewers', (
-            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles(), False)
+        self.assertTrue((developers_budgetimpactreviewers_uid, (
+            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
+        self.assertFalse((vendors_budgetimpactreviewers_uid, (
+            'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
 
     def test_manageItemCertifiedSignatures(self):
         """
           This tests the form that manage itemCertifiedSignatures and that can apply it on item.
         """
         self.changeUser('admin')
         # make items inserted in a meeting inserted in this order
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testFaceted.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeeting.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeeting.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,23 +44,24 @@
         """Test when inserting item in a meeting using
            'on_item_decision_first_words' insertion method."""
         cfg = self.meetingConfig
         cfg.setInsertingMethodsOnAddItem(({'insertingMethod': 'on_item_decision_first_words', 'reverse': '0'}, ))
         self.changeUser('pmManager')
         meeting = self.create('Meeting', date=DateTime('2019/09/20').asdatetime())
         # xxx Namur, creator place decision in description field and it's copied on decision field when the item is validate
-        data = ({'description': "<p>DÉCIDE d'engager Madame Untell Anne au poste proposé</p>"},
-                {'description': "<p>DÉCIDE de refuser</p>"},
-                {'description': "<p>REFUSE d'engager Madame Untell Anne au poste proposé</p>"},
-                {'description': "<p>A REFUSÉ d'engager Madame Untell Anne au poste proposé</p>"},
-                {'description': "<p>DECIDE aussi de ne pas décider</p>"},
-                {'description': "<p>ACCEPTE d'engager Madame Untell Anne au poste proposé</p>"},
-                {'description': "<p>ACCEPTENT d'engager Madame Untell Anne au poste proposé</p>"}, )
+        data = ({'decisionProject': "<p>DÉCIDE d'engager Madame Untell Anne au poste proposé</p>"},
+                {'decisionProject': "<p>DÉCIDE de refuser</p>"},
+                {'decisionProject': "<p>REFUSE d'engager Madame Untell Anne au poste proposé</p>"},
+                {'decisionProject': "<p>A REFUSÉ d'engager Madame Untell Anne au poste proposé</p>"},
+                {'decisionProject': "<p>DECIDE aussi de ne pas décider</p>"},
+                {'decisionProject': "<p>ACCEPTE d'engager Madame Untell Anne au poste proposé</p>"},
+                {'decisionProject': "<p>ACCEPTENT d'engager Madame Untell Anne au poste proposé</p>"}, )
         for itemData in data:
-            item = self.create('MeetingItem', **itemData)
+            item = self.create('MeetingItem')
+            item.setDecisionProject(itemData["decisionProject"])
             self.presentItem(item)
         self.assertEqual(
             [anItem.getDecision() for anItem in meeting.get_items(ordered=True)],
             ["<p>A REFUS\xc3\x89 d'engager Madame Untell Anne au poste propos\xc3\xa9</p>",
              "<p>ACCEPTE d'engager Madame Untell Anne au poste propos\xc3\xa9</p>",
              "<p>ACCEPTENT d'engager Madame Untell Anne au poste propos\xc3\xa9</p>",
              '<p>DECIDE aussi de ne pas d\xc3\xa9cider</p>',
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingCategory.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingConfig.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testMeetingItem.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testPortlets.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSearches.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testSetup.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testUtils.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testValidators.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testViews.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWFAdaptations.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testWFAdaptations.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     def test_pm_WFA_availableWFAdaptations(self):
         '''Most of wfAdaptations makes no sense, just make sure most are disabled.'''
         self.assertEquals(set(self.meetingConfig.listWorkflowAdaptations()),
                           {'item_validation_shortcuts',
                            'item_validation_no_validate_shortcuts',
                            'only_creator_may_delete',
+                           'meeting_remove_global_access',
+                           'meetingmanager_correct_closed_meeting',
                            'no_freeze',
                            'no_publication',
                            'no_decide',
                            'accepted_but_modified',
                            'postpone_next_meeting',
                            'mark_not_applicable',
                            'removed',
@@ -57,15 +59,14 @@
                            'return_to_proposing_group_with_all_validations',
                            'accepted_out_of_meeting',
                            'accepted_out_of_meeting_and_duplicated',
                            'accepted_out_of_meeting_emergency',
                            'accepted_out_of_meeting_emergency_and_duplicated',
                            'transfered',
                            'transfered_and_duplicated',
-                           'meetingmanager_correct_closed_meeting',
                            'namur_meetingmanager_may_not_edit_decision_project'
                            })
 
     def test_pm_Validate_workflowAdaptations_dependencies(self):
         '''Not all WFA are available yet...'''
         pass
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products/MeetingNamur/tests/testWorkflows.py` & `Products.MeetingNamur-4.2.0rc1/src/Products/MeetingNamur/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/PKG-INFO` & `Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingNamur
-Version: 4.2.0b1
+Version: 4.2.0rc1
 Summary: PloneMeeting profile for city of Namur
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -21,14 +21,23 @@
 'Products.MeetingNamur' is a custom profile for 'Products.MeetingCommunes'.
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.0rc1 (2023-07-04)
+---------------------
+
+- Fixed broken tests.
+  [aduchene]
+- Don't use a custom permission for ItemCertifiedSignatures
+  [aduchene]
+
+
 4.2.0b1 (2023-07-04)
 --------------------
 
 - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
   [gbastien]
 - Fixed issue with WF, roles, permissions and fields
   [aduchene]
```

### Comparing `Products.MeetingNamur-4.2.0b1/src/Products.MeetingNamur.egg-info/SOURCES.txt` & `Products.MeetingNamur-4.2.0rc1/src/Products.MeetingNamur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

