# Comparing `tmp/redturtle.volto-5.0.0rc1.tar.gz` & `tmp/redturtle.volto-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.volto-5.0.0rc1.tar", last modified: Mon Mar 20 21:43:32 2023, max compression
+gzip compressed data, was "redturtle.volto-5.0.1.tar", last modified: Tue Jul  4 13:11:41 2023, max compression
```

## Comparing `redturtle.volto-5.0.0rc1.tar` & `redturtle.volto-5.0.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10303 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       73 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      666 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       94 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    21603 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9963 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/constraints.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/constraints_plone52.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       62 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/constraints_plone60.txt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.406878 redturtle.volto-5.0.0rc1/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       68 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       52 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      439 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2815 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.402878 redturtle.volto-5.0.0rc1/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.406878 redturtle.volto-5.0.0rc1/src/redturtle/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle/volto/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1977 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle/volto/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      495 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1408 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1710 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      543 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/controlpanel.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3708 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/find_blocks.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4458 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/find_blocks.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6192 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/fix_links.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5735 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/fix_links.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       39 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/noindex.pt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2953 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/Products.CMFPlone.browser.syndication.templates.RSS.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      829 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.document.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      813 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       34 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/plone.volto.browser.voltobackendwarning.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4288 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/sitemap.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1357 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/dependencies.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2651 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/indexers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      853 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/indexers.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      881 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.406878 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2559 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/it/LC_MESSAGES/redturtle.volto.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2239 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/redturtle.volto.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1746 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      482 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6877 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/monkey.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1467 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/monkey.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.406878 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      171 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/controlpanel.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      390 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2346 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/caching.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      193 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/controlpanel.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      858 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/criteria.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      213 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/rss.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      335 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      445 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/types/Event.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      262 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/types/Folder.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      451 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/types/News_Item.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      125 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      347 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/uninstall/controlpanel.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/uninstall/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      206 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/uninstall/registry/controlpanel.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       93 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/uninstall/registry/rss.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      304 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4109 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/blocks.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1149 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4550 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/dxfields.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/search/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/search/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/search/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      823 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/search/query.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4763 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/blocks.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      969 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2517 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/dxfields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4807 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/summary.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      530 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/controlpanel.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/navigation/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/navigation/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      510 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/navigation/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2247 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/navigation/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/querystringsearch/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/querystringsearch/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      829 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/querystringsearch/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5612 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/querystringsearch/post.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.414878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/search/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/search/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      497 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/search/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4955 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/search/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/site_search/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/site_search/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      440 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/site_search/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1339 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/site_search/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/sitemap/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/sitemap/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      778 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/sitemap/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      497 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/sitemap/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    19795 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3012 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4593 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/logo.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7170 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_advancedsearch.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4248 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_blocks_searchable_text.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3368 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_blocks_serializer.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3924 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_content_types.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1345 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_controlpanel_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4532 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_ct_link.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1500 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_monkeypatches.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2361 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_publication_fields_fixes.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4981 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_service_context_navigation.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1551 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_service_sitemap.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3185 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2129 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_site_search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3713 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_summary_customization.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4659 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_vocabulary_endpoint.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.418878 redturtle.volto-5.0.0rc1/src/redturtle/volto/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/types/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1234 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/types/adapters.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      220 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/types/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16314 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4812 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle/volto/upgrades.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-03-20 21:43:32.410878 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    21603 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5687 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      120 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      316 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-03-20 21:43:32.000000 redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10482 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       73 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      666 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       94 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    21779 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9963 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/constraints.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/constraints_plone52.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       62 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/constraints_plone60.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.429225 redturtle.volto-5.0.1/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       68 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       33 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      439 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2813 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.429225 redturtle.volto-5.0.1/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.429225 redturtle.volto-5.0.1/src/redturtle/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1977 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      495 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1518 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1710 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      543 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/controlpanel.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3708 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/find_blocks.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4458 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/find_blocks.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6804 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/fix_links.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5778 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/fix_links.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       39 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/noindex.pt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2953 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/Products.CMFPlone.browser.syndication.templates.RSS.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      829 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.document.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      813 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       34 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/plone.volto.browser.voltobackendwarning.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4288 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/browser/sitemap.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1357 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/dependencies.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2651 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/indexers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      853 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/indexers.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      881 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/locales/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.429225 redturtle.volto-5.0.1/src/redturtle/volto/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2559 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/locales/it/LC_MESSAGES/redturtle.volto.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2239 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/locales/redturtle.volto.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1746 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      482 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6877 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/monkey.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1467 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/monkey.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/permissions.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.429225 redturtle.volto-5.0.1/src/redturtle/volto/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      171 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/controlpanel.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      390 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2346 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/caching.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      193 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/controlpanel.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      858 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/criteria.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      213 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/rss.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      335 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      445 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/types/Event.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      262 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/types/Folder.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      451 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/types/News_Item.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      125 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      347 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/uninstall/controlpanel.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/profiles/uninstall/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      206 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/uninstall/registry/controlpanel.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       93 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/profiles/uninstall/registry/rss.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      304 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4109 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/blocks.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1149 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4550 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/dxfields.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/search/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/search/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/search/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      823 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/search/query.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4763 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/blocks.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      969 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2517 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/dxfields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4807 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/summary.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      530 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/controlpanel.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/navigation/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/navigation/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      510 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/navigation/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2247 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/navigation/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/querystringsearch/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/querystringsearch/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      829 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/querystringsearch/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5612 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/querystringsearch/post.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/search/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/search/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      497 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/search/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4955 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/search/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/site_search/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/site_search/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      440 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/site_search/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1339 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/site_search/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/sitemap/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/sitemap/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      778 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/sitemap/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      497 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/sitemap/get.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      525 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3012 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4593 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/logo.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7170 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_advancedsearch.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4248 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_blocks_searchable_text.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3368 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_blocks_serializer.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3924 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_content_types.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1345 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_controlpanel_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4532 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_ct_link.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1500 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_monkeypatches.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2361 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_publication_fields_fixes.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4981 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_service_context_navigation.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1551 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_service_sitemap.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3185 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2129 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_site_search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3713 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_summary_customization.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4659 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/tests/test_vocabulary_endpoint.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.433225 redturtle.volto-5.0.1/src/redturtle/volto/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/types/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1234 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/types/adapters.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      220 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/types/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16314 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4812 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle/volto/upgrades.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-04 13:11:41.429225 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    21779 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5687 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      120 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      316 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-07-04 13:11:41.000000 redturtle.volto-5.0.1/src/redturtle.volto.egg-info/top_level.txt
```

### Comparing `redturtle.volto-5.0.0rc1/CHANGES.rst` & `redturtle.volto-5.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+5.0.1 (2023-07-04)
+------------------
+
+- Custom portal url in @@fix-links
+  [mamico]
+
+
+5.0.0 (2023-04-04)
+------------------
+
+- Remove unused default text in homepage.
+  [cekk]
+
+
 5.0.0rc1 (2023-03-20)
 ---------------------
 
 - Plone 6.0 support
 
 - Handle custom search ranking with AdvancedQuery.
   [mamico]
```

### Comparing `redturtle.volto-5.0.0rc1/DEVELOP.rst` & `redturtle.volto-5.0.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/LICENSE.GPL` & `redturtle.volto-5.0.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/LICENSE.rst` & `redturtle.volto-5.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/PKG-INFO` & `redturtle.volto-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.volto
-Version: 5.0.0rc1
+Version: 5.0.1
 Summary: Helper package to setup a RedTurtle's Plone site ready to work with Volto.
 Home-page: https://github.com/collective/redturtle.volto
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.volto
 Project-URL: Source, https://github.com/RedTurtle/redturtle.volto
@@ -360,14 +360,28 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+5.0.1 (2023-07-04)
+------------------
+
+- Custom portal url in @@fix-links
+  [mamico]
+
+
+5.0.0 (2023-04-04)
+------------------
+
+- Remove unused default text in homepage.
+  [cekk]
+
+
 5.0.0rc1 (2023-03-20)
 ---------------------
 
 - Plone 6.0 support
 
 - Handle custom search ranking with AdvancedQuery.
   [mamico]
```

### Comparing `redturtle.volto-5.0.0rc1/README.rst` & `redturtle.volto-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/docs/conf.py` & `redturtle.volto-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/setup.py` & `redturtle.volto-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.volto",
-    version="5.0.0rc1",
+    version="5.0.1",
     description="Helper package to setup a RedTurtle's Plone site ready to work with Volto.",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -70,15 +70,15 @@
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
             "plone.testing>=5.0.0",
             "plone.app.contenttypes",
             "plone.app.robotframework[debug]",
             "collective.MockMailHost",
-        ]
+        ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = redturtle.volto.locales.update:update_locale
     """,
```

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/__init__.py` & `redturtle.volto-5.0.1/src/redturtle/volto/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/adapters/stringinterp.py` & `redturtle.volto-5.0.1/src/redturtle/volto/adapters/stringinterp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 from plone.stringinterp.adapters import BaseSubstitution
 from Products.CMFCore.interfaces import IContentish
 from zope.component import adapter
-from plone.stringinterp import _ as stringinterp_mf
 from redturtle.volto import _
 
+try:
+    from plone.stringinterp import _ as stringinterp_mf
+except ImportError:
+    # plone 6
+    from plone.base import PloneMessageFactory as stringinterp_mf
+
 
 @adapter(IContentish)
 class VoltoUrlSubstitution(BaseSubstitution):
     category = stringinterp_mf("All Content")
     description = _(
         "stringinterp_volto_url",
         default='Volto URL: Content url without "/api".',
```

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/controlpanel.py` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/find_blocks.pt` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/find_blocks.pt`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/find_blocks.py` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/find_blocks.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/fix_links.pt` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/fix_links.pt`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,31 @@
                             Insert a list of urls to replace. They can be localhost (http://localhost:8080/Plone) or staging urls (with /api at the end).
                             All links found with these patterns will be replaced with current portal url (${context/portal_url}) and then tried to converted into a safer way (like blocks deserializers works).
                         </span>
                     </label>
                     <textarea id="to_replace"
                               name="to_replace"
                               tal:define="to_replace request/form/to_replace|nothing"
+                              style="width:100%"
                               class="textarea-widget text-field">${to_replace}</textarea>
                 </div>
                 <div class="field">
                     <span class="option">
+                        <input id="portal_url"
+                            name="portal_url"
+                            style="width:100%"
+                            tal:attributes="value view/portal_url|nothing"
+                            type="text">
+                        <label for="portal_url" class="horizontal focus">
+                            current portal url
+                        </label>
+                    </span>
+                </div>
+                <div class="field">
+                    <span class="option">
                         <input id="dry_mode"
                             name="dry_mode"
                             class="single-checkbox-bool-widget bool-field"
                             checked
                             type="checkbox">
                         <label for="dry_mode" class="horizontal focus">
                             Dry mode
@@ -62,15 +75,15 @@
                     <div>
                         <div tal:repeat="res fixed" class="panel panel-default">
                             <div class="panel-heading">
                                 <a href="${res/url}">${res/url}</a>
                             </div>
                             <a href="#modal-fixed-${repeat/res/index}"
                             class="plone-btn plone-btn-large plone-btn-primary pat-plone-modal"
-                            data-pat-plone-modal="">See changes</a>
+                            data-pat-plone-modal="width: 2000px; margin: 0">See changes</a>
                                 <div id="modal-fixed-${repeat/res/index}" style="display: none">
                                     <div style="display:flex;gap: 10px;justify-content: center;">
                                         <div style="width:50%;">
                                             <h3>OLD</h3>
                                             <pre style="height:500px;">${res/old}</pre>
                                         </div>
                                         <div style="width:50%;">
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 
  Urls to replace  Insert a list of urls to replace. They can be localhost
 (http://localhost:8080/Plone) or staging urls (with /api at the end). All links
 found with these patterns will be replaced with current portal url (${context/
 portal_url}) and then tried to converted into a safer way (like blocks
 deserializers works).
 ${to_replace}
+ [portal_url          ]  current portal url
  *  Dry mode Do not save new data.
 [Confirm]
 ***** Results *****
  Fixed links (${tot})
 ${res/url}
 See_changes
 **** OLD ****
```

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/fix_links.py` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/fix_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class View(BrowserView):
     results = {}
 
     def __call__(self):
         submitted = self.request.form.get("confirm", None)
         dry_mode = self.request.form.get("dry_mode", False)
+        self.portal_url = self.request.form.get("portal_url", self.context.portal_url())
         to_replace = self.request.form.get("to_replace", "")
         if not submitted and not to_replace:
             return super().__call__()
         portal_catalog = api.portal.get_tool("portal_catalog")
         results = portal_catalog()
         tot = len(results)
         i = 0
@@ -114,19 +115,18 @@
         try:
             data = json.dumps(blocks)
         except Exception:
             return res
         if self.check_pattern(value=data):
             res["ok"] = False
             res["fixed"] = True
-            portal_url = self.context.portal_url()
             # convert broken links to current site ulr and then deserialize all
             # blocks to have the right values
             for url in self.request.form.get("to_replace", "").split():
-                data = data.replace(url, portal_url)
+                data = data.replace(url, self.portal_url)
             deserializer = queryMultiAdapter(
                 (field, context, self.request), IFieldDeserializer
             )
             new_value = deserializer(json.loads(data))
             new_value_json = json.dumps(new_value)
             for url in self.request.form.get("to_replace", "").split():
                 if url in new_value_json:
```

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/Products.CMFPlone.browser.syndication.templates.RSS.pt` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/Products.CMFPlone.browser.syndication.templates.RSS.pt`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.document.pt` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.document.pt`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/browser/sitemap.py` & `redturtle.volto-5.0.1/src/redturtle/volto/browser/sitemap.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/dependencies.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/dependencies.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/indexers.py` & `redturtle.volto-5.0.1/src/redturtle/volto/indexers.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/indexers.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/indexers.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/interfaces.py` & `redturtle.volto-5.0.1/src/redturtle/volto/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/README.rst` & `redturtle.volto-5.0.1/src/redturtle/volto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/it/LC_MESSAGES/redturtle.volto.po` & `redturtle.volto-5.0.1/src/redturtle/volto/locales/it/LC_MESSAGES/redturtle.volto.po`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/redturtle.volto.pot` & `redturtle.volto-5.0.1/src/redturtle/volto/locales/redturtle.volto.pot`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/locales/update.py` & `redturtle.volto-5.0.1/src/redturtle/volto/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/monkey.py` & `redturtle.volto-5.0.1/src/redturtle/volto/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/monkey.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/monkey.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/controlpanel.xml` & `redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/caching.xml` & `redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/profiles/default/registry/criteria.xml` & `redturtle.volto-5.0.1/src/redturtle/volto/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/blocks.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/blocks.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/deserializer/dxfields.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/search/query.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/search/query.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/blocks.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/blocks.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/dxfields.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/serializer/summary.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/serializer/summary.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/controlpanel.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/navigation/get.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/navigation/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/querystringsearch/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/querystringsearch/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/querystringsearch/post.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/querystringsearch/post.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/search/get.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/search/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/site_search/get.py` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/site_search/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/restapi/services/sitemap/configure.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/restapi/services/sitemap/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/testing.py` & `redturtle.volto-5.0.1/src/redturtle/volto/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/logo.png` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/logo.png`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_advancedsearch.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_advancedsearch.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_blocks_searchable_text.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_blocks_searchable_text.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_blocks_serializer.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_blocks_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_content_types.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_content_types.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_controlpanel_api.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_ct_link.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_ct_link.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_monkeypatches.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_monkeypatches.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_publication_fields_fixes.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_publication_fields_fixes.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_service_context_navigation.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_service_context_navigation.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_service_sitemap.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_service_sitemap.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_setup.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_site_search.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_site_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_summary_customization.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_summary_customization.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/tests/test_vocabulary_endpoint.py` & `redturtle.volto-5.0.1/src/redturtle/volto/tests/test_vocabulary_endpoint.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/types/adapters.py` & `redturtle.volto-5.0.1/src/redturtle/volto/types/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/upgrades.py` & `redturtle.volto-5.0.1/src/redturtle/volto/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle/volto/upgrades.zcml` & `redturtle.volto-5.0.1/src/redturtle/volto/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/PKG-INFO` & `redturtle.volto-5.0.1/src/redturtle.volto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.volto
-Version: 5.0.0rc1
+Version: 5.0.1
 Summary: Helper package to setup a RedTurtle's Plone site ready to work with Volto.
 Home-page: https://github.com/collective/redturtle.volto
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.volto
 Project-URL: Source, https://github.com/RedTurtle/redturtle.volto
@@ -360,14 +360,28 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+5.0.1 (2023-07-04)
+------------------
+
+- Custom portal url in @@fix-links
+  [mamico]
+
+
+5.0.0 (2023-04-04)
+------------------
+
+- Remove unused default text in homepage.
+  [cekk]
+
+
 5.0.0rc1 (2023-03-20)
 ---------------------
 
 - Plone 6.0 support
 
 - Handle custom search ranking with AdvancedQuery.
   [mamico]
```

### Comparing `redturtle.volto-5.0.0rc1/src/redturtle.volto.egg-info/SOURCES.txt` & `redturtle.volto-5.0.1/src/redturtle.volto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

