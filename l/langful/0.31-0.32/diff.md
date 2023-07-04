# Comparing `tmp/langful-0.31-py3-none-any.whl.zip` & `tmp/langful-0.32-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5431 bytes, number of entries: 7
+Zip file size: 5419 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      224 b- defN 23-Jun-20 12:20 langful/__init__.py
--rw-rw-rw-  2.0 fat     9748 b- defN 23-Jul-03 10:08 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3130 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      527 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/RECORD
-7 files, 14795 bytes uncompressed, 4501 bytes compressed:  69.6%
+-rw-rw-rw-  2.0 fat     9963 b- defN 23-Jul-04 11:45 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      527 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/RECORD
+7 files, 15269 bytes uncompressed, 4489 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.31.dist-info/LICENSE
+Filename: langful-0.32.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.31.dist-info/METADATA
+Filename: langful-0.32.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.31.dist-info/WHEEL
+Filename: langful-0.32.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.31.dist-info/top_level.txt
+Filename: langful-0.32.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.31.dist-info/RECORD
+Filename: langful-0.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -1,133 +1,155 @@
 """
 # lang
 """
 from locale import getdefaultlocale
 import json
 import os
 
-def lang_to_json( lang_file : str ) -> dict :
+def to_json( lang_file : str ) -> dict :
     """
     .lang -> .json
     """
     ret = {}
     for i in lang_file.split( "\n" ) :
-        text = i.split("#")[0]
+        text = i.split( "#" )[ 0 ]
         line = "".join( text.split( maxsplit = 2 ) )
         if line :
-            key_value = i.split( "=" , 1 )
+            key_value = line.split( "=" , 1 )
             if len( key_value ) == 2 :
-                key , value = i.split( "=" , 1 )
+                key , value = key_value
             else :
                 raise SyntaxError( "can't to read .lang file" )
             ret[ key ] = value
     return ret
 
-def json_to_lang( dict_file : dict ) -> str :
+def to_lang( dict_file : dict ) -> str :
     """
     .json -> .lang
     """
     ret = ""
     for key , value in dict_file.items() :
-        if not ( isinstance( value , int ) or isinstance( value , str ) ) :
-            raise TypeError( f"can't use type '{ type( value ) }'" )
         ret += f"{ key } = { value }\n"
     return ret
 
 class lang :
     """
     # lang
     """
 
     def __setitem__( self , key , value ) -> None :
+        """
+        set
+        """
         self.set( key , value )
 
     def __delitem__( self , key ) -> None :
+        """
+        remove
+        """
         self.remove( key )
 
     def __getitem__( self , key ) -> str :
+        """
+        get
+        """
         return self.get( key )
 
     def __call__( self ) -> None :
+        """
+        init
+        """
         self.init()
 
     def __len__( self ) -> int :
         return len( self.languages )
 
-    def __init__( self , lang_dir : str | dict | bool = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
+    def __init__( self , lang_dir : str | dict = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
         """
         lang_dir: lang files dir, if use dict to set that to a dictionary or False
         default_locale: default locale
         json_first: is load json file first
         """
-        system_locale = self.system_locale_get()
+        self.system_locale = self.system_locale_get()
         self.default_locale = default_locale
-        self.system_locale = system_locale
         self.json_first = json_first
         self.replace_letter = "%"
         self.lang_dir = lang_dir
         self.is_file = False
         self.languages = {}
         self.types = {}
-        if isinstance( lang_dir , str ) :
-            self.init()
-        elif isinstance( lang_dir , dict ) :
-            self.init_dict( lang_dir )
+        self.init()
+
+    def init( self ) :
+        """
+        init
+        """
+        if isinstance( self.lang_dir , str ) :
+            self.init_file( self.lang_dir )
+        elif isinstance( self.lang_dir , dict ) :
+            self.init_dict( self.lang_dir )
 
-    def init( self ) -> None :
+    def init_file( self , path ) -> None :
         """
         init by a directory
         """
-        path = self.lang_dir
         self.is_file = True
-        if not isinstance( self.json_first , bool ) :
-            self.json_first = True
-        if self.json_first :
-            loads = [ ".json" , ".lang" ]
-        else :
-            loads = [ ".lang" , ".json" ]
-        if self.is_file :
-            if not os.path.exists( path ) :
-                raise FileNotFoundError( f"can't find '{ os.path.abspath( path ) }'" )
-            files = []
-            for i in os.listdir( path ) :
-                name , suffix = os.path.splitext( i )
-                if ( suffix in loads ) and ( ( suffix == loads[0] ) or ( name + loads[0] not in files ) ) :
-                    files.append( i )
-                    with open( os.path.join( path , i ) , encoding = "utf-8" ) as file :
-                        if suffix == ".json" :
-                            try :
-                                data = json.load( file )
-                            except json.decoder.JSONDecodeError :
-                                raise SyntaxError( "can't to load .json file" )
-                        elif suffix == ".lang" :
-                            data = lang_to_json( file.read() )
-                        else :
-                            continue
-                    self.languages[ name ] = data
-                    self.types[ name ] = suffix
+        if not os.path.exists( path ) :
+            raise FileNotFoundError( f"can't find '{ os.path.abspath( path ) }'" )
+        loads = [ [ ".lang" , ".json" ] , [ ".json" , ".lang" ] ][ self.json_first ]
+        files = []
+        for i in os.listdir( path ) :
+            name , suffix = os.path.splitext( i )
+            if ( suffix in loads ) and ( ( suffix == loads[ 0 ] ) or ( name + loads[ 0 ] not in files ) ) :
+                files.append( i )
+                with open( os.path.join( path , i ) , "r" , encoding = "utf-8" ) as file :
+                    if suffix == ".json" :
+                        try :
+                            data = json.load( file )
+                        except json.decoder.JSONDecodeError :
+                            raise SyntaxError( "can't to load .json file" )
+                    elif suffix == ".lang" :
+                        data = to_json( file.read() )
+                    else :
+                        continue
+                self.languages[ name ] = data
+                self.types[ name ] = suffix
 
-    def init_dict( self , language : dict ) -> None :
+    def init_dict( self , language : dict = None ) -> None :
         """
         init by a dictionary, so cant't to save it to the file
         """
-        if self.is_file :
-            raise TypeError( "can't init by a dictionary, because it's init by a dir" )
-        for value in language.values() :
-            if not isinstance( value , dict ) :
-                raise TypeError( f"can't use type '{ type( value ) }'" )
+        self.is_file = False
         for key in language.keys() :
             self.types[ key ] = ".json"
         self.languages = language
+        self.lang_dir = language
+
+    def to_dict( self ) :
+        """
+        set type to dict
+        """
+        self.types = { key : ".json" for key in self.types.keys() }
+        self.lang_dir = self.languages
+        self.is_file = False
+
+    def to_file( self , path ) :
+        """
+        set type to file
+        """
+        if not os.path.exists( path ) :
+            os.makedirs( path )
+        self.lang_dir = path
+        self.is_file = True
 
     def system_locale_get( self ) -> str :
         """
         get system locale
         """
-        return getdefaultlocale()[0].lower()
+        return getdefaultlocale()[ 0 ].lower()
 
     @property
     def locales( self ) -> list :
         """
         locales
         """
         return list( self.types.keys() )
@@ -145,15 +167,15 @@
             raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
 
     @property
     def language( self ) -> dict :
         """
         get now language
         """
-        return self.languages[ self.locale ]
+        return self.lang_get( self.locale )
 
     @property
     def lang( self ) -> dict :
         """
         same to language function
         """
         return self.language
@@ -195,14 +217,20 @@
         if give a locale then set that, else reset it
         """
         if locale != None :
             self.system_locale = locale
         else :
             self.system_locale = self.system_locale_get()
 
+    def lang_get( self , locale : str ) -> dict :
+        """
+        get a lang
+        """
+        return self.languages[ locale ]
+
     def lang_set( self , locale : str , value : dict = {} , suffix : str = ".json" ) -> None :
         """
         set a new lang
         """
         self.languages[ locale ] = value
         self.types[ locale ] = suffix
 
@@ -230,37 +258,37 @@
     def remove( self , key : str | int , locale : str = None ) -> None :
         """
         remove a value by a locale dictionary
         """
         locale = self.locale_get( locale )
         del self.languages[ locale ][ key ]
 
-    def save( self ) -> None :
+    def save( self , separators : list = [ " ," , ": " ] ) -> None :
         """
         save file when is_file variable is true, else raise the error
         """
-        if self.is_file :
+        if isinstance( self.lang_dir , str ) :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
-                with open( os.path.join( self.lang_dir , key , suffix ) , "w" , encoding = "utf-8" ) as file :
+                with open( os.path.join( self.lang_dir , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
-                        file.write( json.dumps( value , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
+                        file.write( json.dumps( value , indent = 4 , separators = separators , ensure_ascii = False ) )
                     elif suffix == ".lang" :
-                        file.write( json_to_lang( value ) )
-        else :
-            raise TypeError( "can't to save, because it's not a file" )
+                        file.write( to_lang( value ) )
+        return self.languages
 
-    def save_dict( self ) -> dict :
+    def merge( self , locale : str = None , args : list = [] ) -> dict :
         """
-        save dict. in fact, it just return the "languages" variable
+        merge
         """
-        if not self.is_file :
-            return self.languages
-        else :
-            raise TypeError( "can't to save, because it's not a dict" )
+        ret = self.lang_get( self.locale_get( locale ) )
+        for i in args :
+            for key , value in self.lang_get( i ).items() :
+                ret[ key ] = value
+        return ret
 
     def replace( self , key : str = None , args : list | str = None , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace
         """
         replace_letter = self.replace_letter_get( replace_letter )
         locale = self.locale_get( locale )
```

## Comparing `langful-0.31.dist-info/LICENSE` & `langful-0.32.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.31.dist-info/METADATA` & `langful-0.32.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.31
+Version: 0.32
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,19 +19,19 @@
     </a>
     <a href = "https://www.python.org" >
         <img alt = "Python version" src = "https://img.shields.io/badge/python-3.6+-blue" >
     </a>
     <a href = "https://opensource.org/license/mit" >
         <img alt = "license" src = "https://img.shields.io/badge/license-MIT-blue" >
     </a>
-    <a href = "https://github.com/cueavyqwp/langful" >
-        <img alt = "Github stars" src = "https://img.shields.io/github/stars/cueavyqwp/langful?color=blue" >
+    <a href = "https://github.com/cueavy/langful" >
+        <img alt = "Github stars" src = "https://img.shields.io/github/stars/cueavy/langful?color=blue" >
     </a>
-    <a href = "https://github.com/cueavyqwp/langful" >
-        <img alt = "Github issues" src = "https://img.shields.io/github/issues/cueavyqwp/langful?color=blue" >
+    <a href = "https://github.com/cueavy/langful" >
+        <img alt = "Github issues" src = "https://img.shields.io/github/issues/cueavy/langful?color=blue" >
     </a>
 
 ---
 
 [
 en_us
 |
@@ -111,15 +111,14 @@
 } )
 ```
 
 ## function
 
 ### replace
 
-
 ```python
 lang = langful.lang( False )
 lang.replace_letter = "&"
 lang.init_dict( {
     "en_us" : {
         "test" : "&.&%"
     }
@@ -141,14 +140,31 @@
         "hi" : "你好" ,
         "welcome" : "欢迎"
     }
 } )
 print(lang.replace_str( "%hi%, %welcome%!" ))
 ```
 
+### merge
+
+```python
+import langful
+lang = langful.lang( False )
+lang.init_dict( {
+    "en_us" : {
+        "hi" : "Hi" ,
+        "welcome" : "Welcome"
+    } ,
+    "zh_cn" : {
+        "hi" : "你好"
+    }
+} )
+print( lang.merge( "en_us" , [ "zh_cn" ] ) )
+```
+
 # about
 
 [
-[github](https://github.com/cueavyqwp/langful)
+[github](https://github.com/cueavy/langful)
 |
 [pypi](https://pypi.org/project/langful)
 ]
```

