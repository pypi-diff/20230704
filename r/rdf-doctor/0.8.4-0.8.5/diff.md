# Comparing `tmp/rdf_doctor-0.8.4-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.8.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18542 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-21 08:19 doctor/__init__.py
+Zip file size: 18942 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-04 08:21 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jun-19 02:18 doctor/consts.py
--rw-r--r--  2.0 unx    31152 b- defN 23-Jun-21 08:15 doctor/doctor.py
+-rw-r--r--  2.0 unx    32735 b- defN 23-Jul-04 07:45 doctor/doctor.py
 -rw-r--r--  2.0 unx    20305 b- defN 23-Jun-19 02:18 doctor/reference/correct-prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 23-Jun-19 02:18 doctor/reference/refine-classes.tsv
 -rw-r--r--  2.0 unx      679 b- defN 23-Jun-19 02:18 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8844 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      994 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/RECORD
-12 files, 63929 bytes uncompressed, 16858 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9140 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/RECORD
+12 files, 65808 bytes uncompressed, 17258 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-classes.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefixes.tsv
 Comment: 
 
-Filename: rdf_doctor-0.8.4.dist-info/LICENSE
+Filename: rdf_doctor-0.8.5.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.8.4.dist-info/METADATA
+Filename: rdf_doctor-0.8.5.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.8.4.dist-info/WHEEL
+Filename: rdf_doctor-0.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.8.4.dist-info/entry_points.txt
+Filename: rdf_doctor-0.8.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.4.dist-info/top_level.txt
+Filename: rdf_doctor-0.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.4.dist-info/RECORD
+Filename: rdf_doctor-0.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.8.4"
+__version__ = "0.8.5"
```

## doctor/doctor.py

```diff
@@ -26,15 +26,19 @@
 
     validation_result, error_msg = validate_command_line_args(args)
     if validation_result == False:
         print(error_msg)
         return
 
     compression_mode = get_compression_mode(args.input[0])
-    input_format = get_input_format(args.input[0], compression_mode)
+    if args.force_format:
+        input_format = args.force_format
+    else:
+        input_format = get_input_format(args.input[0], compression_mode)
+
     result_queue = queue.Queue()
 
     try:
         # Processing branch by report format
         if args.report == REPORT_FORMAT_SHEX:
             # shex
             thread_calc = threading.Thread(target=get_shex_result, args=(args, input_format, compression_mode, result_queue,))
@@ -133,15 +137,15 @@
                         help="input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.",
                         metavar="RDF-FILE")
 
     # Report format (-r、--report [FORMAT]、default: shex)
     parser.add_argument("-r","--report", type=str,
                         default=REPORT_FORMAT_SHEX,
                         help="set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)",
-                        metavar="FORMAT")
+                        metavar="REPORT-FORMAT")
 
     # Output report file (-o、--output [FILE]、default: Standard output)
     parser.add_argument("-o","--output", type=str,
                         help="write to file instead of stdout",
                         metavar="FILE")
 
     # Target class(-c、--classes [URL1, URL2,...]、default: all、Multiple can be specified.)
@@ -159,14 +163,19 @@
 
     # Class errata file path(-l, --class-dict [FILE]、default: reference/refine-classes.tsv)
     parser.add_argument("-l","--class-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(CLASS_ERRATA_FILE_PATH)),
                         help="path to a tab delimited file listing incorrect and correct URI pairs for the class (default: predefined file in rdf-doctor)",
                         metavar="FILE")
 
+    # input format (-f、--format [INPUT_FORMAT]、default: Standard output)
+    parser.add_argument("-f","--force-format", type=str,
+                        help='This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle" or "nt" can be specified.',
+                        metavar="INPUT-FORMAT")
+
     return parser.parse_args(args)
 
 
 # Determine if the input file is compressed and get the compression mode ("gz" or None)
 def get_compression_mode(input_file):
     extension = os.path.splitext(input_file)[1]
     if extension == EXTENSION_GZ:
@@ -209,14 +218,19 @@
             error_msg = "Input file error: No input file specified. (-i [RDF_FILE], --input [RDF_FILE])"
             return False, error_msg
 
         if os.path.isfile(input_file) == False:
             error_msg = "Input file error: " + input_file + " does not exist."
             return False, error_msg
 
+        # Check if the file has read permission
+        if os.access(input_file, os.R_OK) == False:
+            error_msg = "Input file error: you don't have permission to read the input file."
+            return False, error_msg
+
         if compression_mode == "":
             compression_mode = get_compression_mode(input_file)
         else:
             if compression_mode != get_compression_mode(input_file):
                 error_msg = "Input file error: If you enter multiple files, please use the same extension."
                 return False, error_msg
 
@@ -261,24 +275,38 @@
 
     # Make an error if another class name is specified with "all"
     if TARGET_CLASS_ALL in args.classes:
         if len(args.classes) != 1:
             error_msg = 'Target class error: If "all" is specified, other classes cannot be specified.'
             return False, error_msg
 
+    # Input Format only allows "turtle" or "nt"
+    if args.force_format is not None:
+        if args.force_format != TURTLE and \
+            args.force_format != NT:
+            error_msg = 'Input format error: "' + args.force_format + '" is an unsupported input format. "' + TURTLE + '" and "' + NT + '" are supported.'
+            return False, error_msg
 
     if os.path.isfile(args.prefix_dict) == False:
-        error_msg = "Prefix dictionary file error: Prefix dictionary does not exist."
+        error_msg = "Prefix dictionary file error: Prefix dictionary does not exist or you don't have read permission."
         return False, error_msg
 
+    # Check if the file has read permission
+    if os.access(args.prefix_dict, os.R_OK) == False:
+        error_msg = "Prefix dictionary file error: you don't have permission to read the input file."
+        return False, error_msg
 
     if os.path.isfile(args.class_dict) == False:
-        error_msg = "Class dictionary file error: Class dictionary does not exist."
+        error_msg = "Class dictionary file error: Class dictionary does not exist or you don't have read permission."
         return False, error_msg
 
+    # Check if the file has read permission
+    if os.access(args.class_dict, os.R_OK) == False:
+        error_msg = "Class dictionary file error: you don't have permission to read the input file."
+        return False, error_msg
 
     return True, None
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_format, compression_mode, result_queue):
 
@@ -467,15 +495,14 @@
 
     # Get instance of shexer's shaper class
     shaper = Shaper(graph_list_of_files_input=args.input,
                     target_classes=target_classes,
                     all_classes_mode=all_classes_mode,
                     input_format=input_format,
                     namespaces_dict=namespaces_dict,
-                    disable_exact_cardinality=True,
                     compression_mode=compression_mode,
                     instances_report_mode=MIXED_INSTANCES,
                     detect_minimal_iri=True)
 
     return shaper.shex_graph(string_output=True,
                             verbose=args.verbose,
                             acceptance_threshold=0.05)
```

## Comparing `rdf_doctor-0.8.4.dist-info/LICENSE` & `rdf_doctor-0.8.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.8.4.dist-info/METADATA` & `rdf_doctor-0.8.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.8.4
+Version: 0.8.5
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -53,24 +53,26 @@
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -e, --verbose         show progress while processing
   -i RDF-FILE [RDF-FILE ...], --input RDF-FILE [RDF-FILE ...]
                         input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.
-  -r FORMAT, --report FORMAT
+  -r REPORT-FORMAT, --report REPORT-FORMAT
                         set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)
   -o FILE, --output FILE
                         write to file instead of stdout
   -c URL [URL ...], --classes URL [URL ...]
                         set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...
   -p FILE, --prefix-dict FILE
                         path to a tab delimited file listing incorrect and correct URI pairs for the prefix (default: predefined file in rdf-doctor)
   -l FILE, --class-dict FILE
                         path to a tab delimited file listing incorrect and correct URI pairs for the class (default: predefined file in rdf-doctor)
+  -f INPUT-FORMAT, --force-format INPUT-FORMAT
+                        This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle" or "nt" can be specified.
 ```
 
 ## See Also
 - [1] https://github.com/DaniFdezAlvarez/shexer
 - [2] http://shex.io/shex-primer/#combined-constraints
 - [3] https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
```

