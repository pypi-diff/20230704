# Comparing `tmp/copernicus_marine_client-0.8.0.tar.gz` & `tmp/copernicus_marine_client-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.8.0.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.1.tar", max compression
```

## Comparing `copernicus_marine_client-0.8.0.tar` & `copernicus_marine_client-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    16970 2023-07-03 09:04:50.547368 copernicus_marine_client-0.8.0/README.md
--rw-r--r--   0        0        0     3074 2023-07-03 07:22:16.275799 copernicus_marine_client-0.8.0/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544268 copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22216 2023-06-30 15:09:13.269129 copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6167 2023-07-03 09:04:50.547514 copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544602 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      858 2023-07-03 09:04:50.547623 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3707 2023-07-03 09:04:50.547754 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4424 2023-07-03 09:04:50.547827 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_login.py
--rw-r--r--   0        0        0     8886 2023-07-03 09:04:50.548072 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    18276 2023-07-03 09:04:50.548396 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     4798 2023-07-03 09:04:50.548576 copernicus_marine_client-0.8.0/copernicus_marine_client/configuration_files_creator.py
--rw-r--r--   0        0        0     7524 2023-07-03 09:04:50.548740 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     4542 2023-07-03 09:04:50.548845 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0    10512 2023-07-03 09:04:50.548971 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     6304 2023-07-03 09:04:50.549080 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     6453 2023-07-03 09:04:50.549222 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0      917 2023-06-29 09:51:23.593091 copernicus_marine_client-0.8.0/copernicus_marine_client/logging_conf.json
--rw-r--r--   0        0        0      870 2023-07-03 09:13:25.036758 copernicus_marine_client-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    18710 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.0/setup.py
--rw-r--r--   0        0        0    17909 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10980 2023-07-04 07:18:13.630269 copernicus_marine_client-0.8.1/README.md
+-rw-r--r--   0        0        0     3074 2023-07-03 07:22:16.275799 copernicus_marine_client-0.8.1/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544268 copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22216 2023-06-30 15:09:13.269129 copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6199 2023-07-03 12:56:17.483906 copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544602 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      924 2023-07-04 09:12:23.081236 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3773 2023-07-04 07:33:17.711168 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4424 2023-07-04 07:31:26.527623 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     9246 2023-07-04 07:31:41.140486 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    18511 2023-07-04 07:31:40.674207 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     4798 2023-07-03 12:00:07.546495 copernicus_marine_client-0.8.1/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7410 2023-07-03 12:56:17.484867 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4542 2023-07-03 12:00:07.546849 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0    10512 2023-07-03 12:00:07.547043 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     6561 2023-07-03 12:56:17.485055 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     6606 2023-07-04 07:18:13.631652 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0      917 2023-06-29 09:51:23.593091 copernicus_marine_client-0.8.1/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      888 2023-07-04 09:12:47.259688 copernicus_marine_client-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    12575 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.1/setup.py
+-rw-r--r--   0        0        0    11919 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.1/PKG-INFO
```

### Comparing `copernicus_marine_client-0.8.0/README.md` & `copernicus_marine_client-0.8.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 This package allows to recover products and datasets information from Command Line Interface or with Python code,
 as well as download subsets and native files.
 
 ## Command Line Interface (CLI)
 
 ### Command *describe*
-Retrieve information about products as JSON:
 
-```
+Retrieve information about all products as JSON:
+
+```txt
 > copernicus-marine describe
 {
   "products": [
     {
       "title": "Antarctic Sea Ice Extent from Reanalysis",
       "product_id": "ANTARCTIC_OMI_SI_extent",
       "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
@@ -27,15 +28,15 @@
     ...
   ]
 }
 ```
 
 Retrieve all information about datasets as JSON:
 
-```
+```txt
 > copernicus-marine describe --include-datasets
 {
   "products": [
     {
       "title": "Antarctic Sea Ice Extent from Reanalysis",
       "product_id": "ANTARCTIC_OMI_SI_extent",
       "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
@@ -55,33 +56,14 @@
           "variables": []
         }
       ]
     },
     ...
   ]
 }
-
-```
-
-Check out the help:
-
-```
-> copernicus-marine describe --help
-Usage: copernicus-marine describe [OPTIONS]
-
-Options:
-  --one-line             Output JSON on one line
-  --include-description  Include product description in output
-  --include-datasets     Include product dataset details in output
-  --include-keywords     Include product keyword details in output
-  -c, --contains TEXT    Filter catalogue output. Returns products with
-                         attributes matching a string token
-  --overwrite-cache      Force to refresh the catalogue by overwriting the
-                         local cache
-  --help                 Show this message and exit.
 ```
 
 ### Command *login*
 
 Create the configuration files for access to the copernicus marine service:
 '.dodsrc', '.netrc', '.motuclient-python.ini'.
 The directory to store these configuration files can be modified by the user using the "config-file-directory" option
@@ -150,111 +132,31 @@
   --help                          Show this message and exit.
 '''
 
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
-```
+```txt
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 < Username:
 < Password:
 < Trying to download as one file...
 ```
 
-File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
-
-Check out the help:
-
-```
-> copernicus-marine subset --help
-
-Usage: copernicus-marine subset [OPTIONS]
-
-  Downloads subsets of datasets as NetCDF files or Zarr stores.     Either one
-  of 'dataset-id' or 'dataset-url' is required     (can be found via the
-  'copernicus-marine describe' command).     The arguments value passed
-  individually through the CLI take precedence     over the values from the
-  "motu-api-request" option, which takes precedence     over the ones from the
-  "request-file" option
-
-  Example:
-
-    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --variable analysed_sst --variable sea_ice_fraction --start-datetime
-    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
-    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
-
-    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
-    analysed_sst   -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02
-    13:00:00" -x 0.0 -X 0.1 -y 0.0 -Y 0.1
-
-Options:
-  -u, --dataset-url TEXT          The full dataset URL
-  -i, --dataset-id TEXT           The dataset id
-  --username TEXT
-  --password TEXT
-  -v, --variable TEXT             Specify dataset variables
-  -x, --minimal-longitude FLOAT RANGE
-                                  Minimal longitude for the subset. Requires a
-                                  float within this range:  [-180<=x<=180]
-  -X, --maximal-longitude FLOAT RANGE
-                                  Maximal longitude for the subset. Requires a
-                                  float within this range:  [-180<=x<=180]
-  -y, --minimal-latitude FLOAT RANGE
-                                  Minimal latitude for the subset. Requires a
-                                  float within this range:  [-90<=x<=90]
-  -Y, --maximal-latitude FLOAT RANGE
-                                  Maximal latitude for the subset. Requires a
-                                  float within this range:  [-90<=x<=90]
-  -z, --minimal-depth FLOAT RANGE
-                                  Minimal depth for the subset. Requires a
-                                  float within this range:  [x>=0]
-  -Z, --maximal-depth FLOAT RANGE
-                                  Maximal depth for the subset. Requires a
-                                  float within this range:  [x>=0]
-  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The start datetime of the temporal subset.
-                                  Caution: encapsulate date with " " to ensure
-                                  valid format for format "%Y-%m-%d %H:%M:%S"
-  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The end datetime of the temporal subset.
-                                  Caution: encapsulate date with " " to ensure
-                                  valid format for format "%Y-%m-%d %H:%M:%S"
-  -o, --output-directory PATH     The destination folder for the downloaded
-                                  files. Default is the current directory
-  -f, --output-filename PATH      Concatenate the downloaded data in the given
-                                  file name (under the output directory)
-  --assume-yes                    Flag to skip confirmation before download
-  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
-                                  Force download through one of the available
-                                  protocols
-  --dry-run                       Flag to specify NOT to send the request to
-                                  external server. Returns the request instead
-  --request-file PATH             Option to pass a filename corresponding to a
-                                  file containg CLI arguments. The file MUST
-                                  follow the structure of dataclass
-                                  'SubsetRequest'.
-  --motu-api-request TEXT         Option to pass a complete MOTU api request
-                                  as a string. Caution, user has to replace
-                                  double quotes " with single quotes ' in the
-                                  request
-  --log-level [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
-                                  Set the details printed to console by the
-                                  command (based on standard logging library).
-  --help                          Show this message and exit
-```
+File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with '.nc' suffix, the file will be downloaded as a netCDF file.
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
 
 Example:
-```
+
+```txt
 > copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/
 
 < Username:
 < Password:
 < You requested the download of the following files:
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
@@ -266,141 +168,127 @@
 Total size of the download: 19.62 MB
 
 
 Do you want to continue? [y/N]:
 ```
 
 File(s) downloaded to ./{path}/{filename} if not specified otherwise:
+
 - "--output-path" specifies a directory to dump the files in
 - "--no-directories" to not recreate the folder structure
 
 If not specified otherwise, after the header display with a summary of the request,
 the user is asked for confirmation:
+
 - "--no-confirmation" to turn down the confirmation prompt
 - "--show-outputnames" to display the full paths of the outputs files
 
-Check out the help:
+Option `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.
+**Be aware that the regular expression must match the full absolute path of the files to filter.**
 
+Example:
 ```
-> copernicus-marine native --help
+> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"
+Password:
+You requested the download of the following files:
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 
-Usage: copernicus-marine native [OPTIONS]
+Total size of the download: 9.82 MB
 
-  Downloads native data files based on     dataset_id or datafiles url path.
-  The function fetches the files recursively if a folder path is passed as
-  url.     When provided a dataset id,     all the files in the corresponding
-  folder will be downloaded.
 
-      By default for any download request, a summary of the request result is
-      displayed to the user and a confirmation is asked.     This can be
-      turned down. Example:
+Do you want to continue? [y/N]:
+```
 
-    copernicus-marine native -nd -o data_folder --dataset-id
-    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
+### The `--help` argument
 
-    copernicus-marine native -nd -o data_folder --dataset-url
-    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
-    pft_myint_7km-3D-diato_P1M-m
-
-Options:
-  -u, --dataset-url TEXT       Path to the data files
-  -i, --dataset-id TEXT        The dataset id
-  --username TEXT
-  --password TEXT
-  -nd, --no-directories        Option to not recreate folder hierarchy in
-                               ouput directory.
-  --show-outputnames           Option to display the names of the output files
-                               before download.
-  -o, --output-directory PATH  The destination directory for the downloaded
-                               files. Default is the current directory
-                               [required]
-  --assume-yes                 Whether to ask for confirmation before
-                               download, after header display. If 'True',
-                               skips confirmation.
-  --dry-run                    Flag to specify NOT to send the request to
-                               external server. Returns the request instead
-  --request-file PATH          Option to pass a file containg CLI arguments.
-                               The file MUST follow the structure of dataclass
-                               'SubsetRequest'. ANY PARAMETER SPECIFIED ASIDE
-                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION
-                               FOR THE REQUEST IF FILE IS SPECIFIED.
-  --help                       Show this message and exit.
-```
+In any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.
 
 ## Python functions
 
 The library also provide python functions to help with catalogue
 browsing and datasets download in scripts.
 
-### Basic example:
+### Basic example
 
 In this example 4 steps are performed:
   1- Fetch the catalogue to select a dataset
   2- Construct a SubsetRequest for this dataset
   3- Download the subset as a zarr store
   4- Open the subset as an xarray dataset
 
-```
+```python
 import copernicus_marine_client as cmc
 
 # Step 1: Fetch catalogue and parse information on dataset
 catalogue = cmc.fetch_catalogue()
-dataset_id = 'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m'
-assert(dataset_id in cmc.get_all_dataset_ids())
+dataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"
+assert dataset_id in cmc.get_all_dataset_ids()
 dataset = catalogue.filter([dataset_id]).products[0].datasets[0]
 # Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest
-variable = [variable for variable in dataset.variables if variable.short_name in ['zooc']][0]
-coordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}
+variable = [
+    variable for variable in dataset.variables if variable.short_name in ["zooc"]
+][0]
+coordinates = {
+    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)
+    for coordinate in variable.coordinates
+}
 
 # Step 2: Construct the request based on parsed information
 subset_request = cmc.SubsetRequest(
-  dataset_id='cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m',
-  start_datetime="2023-04-20",
-  end_datetime='2023-04-21',
-  minimal_latitude= 30.0,
-  maximal_latitude=30.1,
-  minimal_longitude=0.1,
-  maximal_longitude=0.2,
-  minimal_depth=100,
-  maximal_depth=1000,
-  variables = ['zooc'],
-  force_protocol = "zarr-map",
-  output_directory = 'data_folder',
-  output_filename = 'datastore.zarr',
-  assume_yes = True,
+    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",
+    start_datetime="2023-04-20",
+    end_datetime="2023-04-21",
+    minimal_latitude=30.0,
+    maximal_latitude=30.1,
+    minimal_longitude=0.1,
+    maximal_longitude=0.2,
+    minimal_depth=100,
+    maximal_depth=1000,
+    variables=["zooc"],
+    force_protocol="zarr-map",
+    output_directory="data_folder",
+    output_filename="datastore.zarr",
+    assume_yes=True,
 )
 
 # Step 3: Download the subset based on request content
-filename = cmc.download_subset(username='FAKE_USERNAME', password='FAKE_PASSWORD', subset_request=subset_request)
+filename = cmc.download_subset(
+    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request
+)
 
 # Step 4: Open the downloaded subset as an xarray dataset
-subset = cmc.open_dataset(filepath=filename, engine='zarr', out_type='xarray')
+subset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")
 ```
 
 ## Installation
 
 Using pip, for example:
-```
+
+```shell
 pip install copernicus-marine-client
 ```
+
 ## Technical details
 
 This module is organized around two capabilities:
+
 - a catalogue, parsed from web requests, that contains informations on the available datasets
 - a downloader, to simplify the download of dataset files or subsets
 
 The catalogue can be displayed by the user and is used by the downloader to link the user
 requests with files or subset of files to retrieve.
 The downloader will help the user download the needed datasets.
 
 A rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.
 
 For subset command, the format is:
 
-```
+```python
 @dataclass
 class SubsetRequest:
     dataset_url: Optional[str] = None
     dataset_id: Optional[str] = None
     variables: Optional[List[str]] = None
     minimal_longitude: Optional[float] = None
     maximal_longitude: Optional[float] = None
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     dataset_id: Optional[str] = None
     no_directories: bool = False
     show_outputnames: bool = False
     output_directory: str = "."
     assume_yes: bool = False
     dry_run: bool = False
     force_protocol: Optional[str] = None
+    regex: Optional[str] = None
 
     def update(self, new_dict: dict):
         """Method to update values in NativeRequest object.
         Skips "None" values
         """
         for key, value in new_dict.items():
             if value is None:
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,25 @@
     cli_group_subset,
 )
 
 log_config_dict = json.load(
     open(os.path.join(os.path.dirname(__file__), "..", "logging_conf.json"))
 )
 logging.config.dictConfig(log_config_dict)
-command_line_interface = click.CommandCollection(
+
+
+@click.command(
+    cls=click.CommandCollection,
     sources=[
         cli_group_describe,
         cli_group_login,
         cli_group_subset,
         cli_group_native,
-    ]
+    ],
 )
+@click.version_option()
+def command_line_interface():
+    pass
+
 
 if __name__ == "__main__":
     command_line_interface()
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,33 +15,34 @@
 @click.group()
 def cli_group_describe() -> None:
     pass
 
 
 @cli_group_describe.command(
     "describe",
+    short_help="Print Copernicus Marine catalog as JSON",
     help="""
-    Parse the Copernicus Marine catalogue, then display a
-    JSON-ified version of the corresponding python object.
+    Parse the Copernicus Marine catalog, then display a JSON-ified version of the corresponding python object.
 
     The default display contains information on the products, and more data
     can be displayed using the _include-<argument>_ flags (see Usage section).
 
     The _contains_ option allows the user to specify one or several strings to
     filter through the catalogue display. The search is performed recursively
     on all attributes of the catalogue, and the tokens only need to be
     contained in one of the attributes (i.e. not exact match).
 
     Example:
 
-    > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --include-datasets
+    \b
+    > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 --include-datasets
 
+    \b
     > copernicus-marine describe -c METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-        """,
+    """,  # noqa
 )
 @click.option(
     "--one-line",
     type=bool,
     is_flag=True,
     default=False,
     help="Output JSON on one line",
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_login.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import logging.config
 import os
+from typing import Optional
 
 import click
 
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     FTP_KEY,
     S3NATIVE_KEY,
     get_protocol_from_url,
@@ -37,31 +38,33 @@
 @click.group()
 def cli_group_native() -> None:
     pass
 
 
 @cli_group_native.command(
     "native",
-    help="""Downloads native data files based on
-    dataset_id or datafiles url path.
+    short_help="Download native data files",
+    help="""
+    Download native data files based on dataset_id or datafiles url path.
     The function fetches the files recursively if a folder path is passed as url.
     When provided a dataset id,
     all the files in the corresponding folder will be downloaded.
 
     By default for any download request, a summary of the request result is
     displayed to the user and a confirmation is asked.
     This can be turned down.
-Example:
 
-  copernicus-marine native -nd -o data_folder --dataset-id
-  cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
+    Example:
 
-  copernicus-marine native -nd -o data_folder --dataset-url
-  ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
-""",
+    \b
+    > copernicus-marine native -nd -o data_folder --dataset-id cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
+
+    \b
+    > copernicus-marine native -nd -o data_folder --dataset-url ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
+    """,  # noqa
 )
 @click.option(
     "--dataset-url",
     "-u",
     type=str,
     help="Path to the data files",
 )
@@ -139,28 +142,36 @@
     type=click.Choice(["DEBUG", "INFO", "WARN", "ERROR", "CRITICAL", "QUIET"]),
     default="INFO",
     help=(
         "Set the details printed to console by the command "
         "(based on standard logging library)."
     ),
 )
+@click.option(
+    "--regex",
+    type=str,
+    default=None,
+    help="The regular expression that must match the absolute paths of "
+    "the files to download. ",
+)
 def native(
     dataset_url: str,
     dataset_id: str,
     username: str,
     password: str,
     no_directories: bool,
     show_outputnames: bool,
     output_directory: str,
     config_file_directory: str,
     assume_yes: bool,
     request_file: str,
     force_protocol: str,
     dry_run: bool,
     log_level: str = "INFO",
+    regex: Optional[str] = None,
 ):
     if log_level == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
     else:
         logging.root.setLevel(level=log_level)
     native_request = NativeRequest()
@@ -182,14 +193,16 @@
         native_request.show_outputnames = show_outputnames
     if assume_yes:
         native_request.assume_yes = assume_yes
     if force_protocol:
         native_request.force_protocol = force_protocol
     if dry_run:
         native_request.dry_run = dry_run
+    if regex:
+        native_request.regex = regex
 
     native_function(
         username,
         password,
         native_request,
         config_file_directory,
     )
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,36 +56,34 @@
 @click.group()
 def cli_group_subset() -> None:
     pass
 
 
 @cli_group_subset.command(
     "subset",
-    help=(
-        """Downloads subsets of datasets as NetCDF files or Zarr stores.
-    Either one of 'dataset-id' or 'dataset-url' is required
-    (can be found via the 'copernicus-marine describe' command).
-    The arguments value passed individually through the CLI take precedence
-    over the values from the "motu-api-request" option, which takes precedence
-    over the ones from the "request-file" option
+    short_help="Downloads subsets of datasets as NetCDF files or Zarr stores",
+    help="""
+    Downloads subsets of datasets as NetCDF files or Zarr stores.
+    Either one of 'dataset-id' or 'dataset-url' is required (can be found via the 'copernicus-marine describe' command).
+    The arguments value passed individually through the CLI take precedence over the values from the "motu-api-request" option,
+    which takes precedence over the ones from the "request-file" option
 
-Example:
+    Example:
 
-  copernicus-marine subset
---dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
---variable analysed_sst --variable sea_ice_fraction
---start-datetime 2021-01-01 --end-datetime 2021-01-02
---minimal-longitude 0.0 --maximal-longitude 0.1
---minimal-latitude 0.0 --maximal-latitude 0.1
+    \b
+    > copernicus-marine subset
+    --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
+    --variable analysed_sst --variable sea_ice_fraction
+    --start-datetime 2021-01-01 --end-datetime 2021-01-02
+    --minimal-longitude 0.0 --maximal-longitude 0.1
+    --minimal-latitude 0.0 --maximal-latitude 0.1
 
-  copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst
-  -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02 13:00:00"
-  -x 0.0 -X 0.1 -y 0.0 -Y 0.1
-"""
-    ),
+    \b
+    > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
+    """,  # noqa
 )
 @click.option(
     "--dataset-url",
     "-u",
     type=str,
     help="The full dataset URL",
 )
@@ -182,16 +180,20 @@
     + ".copernicus_marine_client_credentials / .netrc or _netrc / "
     + ".motuclient-python.ini files",
 )
 @click.option(
     "--output-filename",
     "-f",
     type=click.Path(),
-    help="Concatenate the downloaded data in the given file name"
-    + " (under the output directory)",
+    help=(
+        "Concatenate the downloaded data in the given file name "
+        "(under the output directory). If "
+        "the output-filename argument ends with '.nc' suffix, the file will be "
+        "downloaded as a netCDF file."
+    ),
 )
 @click.option(
     "--assume-yes",
     is_flag=True,
     default=False,
     help="Flag to skip confirmation before download",
 )
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/configuration_files_creator.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/configuration_files_creator.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import os
+import re
 from ftplib import FTP
+from itertools import chain
 from multiprocessing.pool import ThreadPool
-from typing import Any, Tuple
+from typing import Any, Optional, Tuple
 
 import click
 from numpy import append, arange
 from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
@@ -19,15 +21,18 @@
 
 def download_ftp(
     username: str,
     password: str,
     native_request: NativeRequest,
 ) -> str:
     message, host, filenames_in = download_header(
-        [str(native_request.dataset_url)], username, password
+        str(native_request.dataset_url),
+        native_request.regex,
+        username,
+        password,
     )
     filenames_out = create_filenames_out(
         filenames_in,
         native_request.output_directory,
         native_request.no_directories,
     )
     logging.info(message)
@@ -62,51 +67,53 @@
         ),
     )
     download_summary = "".join(map(str, download_summary_list))
     return download_summary
 
 
 def download_header(
-    data_paths: list[str], username: str, password: str
+    data_path: str, regex: Optional[str], username: str, password: str
 ) -> Tuple[str, str, list[str]]:
 
-    path_dict = parse_ftp_dataset_url(data_paths)
+    (host, path) = parse_ftp_dataset_url(data_path)
     message = "You requested the download of the following files:\n"
     total_size = 0
-    for host, paths in path_dict.items():
-        with FTP(host) as ftp:
-            ftp.login(user=username, passwd=password)
-            for path in paths:
-                filenames = get_filenames_recursively(ftp, path)
-        pool = ThreadPool()
-        nfilenames_per_process, nfilenames = 100, len(filenames)
-        indexes = append(
-            arange(0, nfilenames, nfilenames_per_process, dtype=int),
-            nfilenames,
-        )
-        groups_filenames = [
-            filenames[indexes[i] : indexes[i + 1]]
-            for i in range(len(indexes) - 1)
-        ]
-        results = pool.map(
-            get_filename_size_tuple,
-            zip(
-                [host] * len(groups_filenames),
-                [username] * len(groups_filenames),
-                [password] * len(groups_filenames),
-                groups_filenames,
-            ),
-        )
-        flattened_results = [r for res in results for r in res]
-        total_size += sum([int(res[1]) for res in flattened_results])
-        for result in flattened_results[:20]:
-            message += str(result[0])
-            message += f" - {format_file_size(float(result[1]))}\n"
-        if len(flattened_results) > 20:
-            message += f"Printed 20 out of {len(flattened_results)} files\n"
+    with FTP(host) as ftp:
+        ftp.login(user=username, passwd=password)
+        raw_filenames = get_filenames_recursively(ftp, path)
+        if regex:
+            regex_compiled = re.compile(regex)
+            filenames = list(filter(regex_compiled.match, raw_filenames))
+        else:
+            filenames = raw_filenames
+    pool = ThreadPool()
+    nfilenames_per_process, nfilenames = 100, len(filenames)
+    indexes = append(
+        arange(0, nfilenames, nfilenames_per_process, dtype=int),
+        nfilenames,
+    )
+    groups_filenames = [
+        filenames[indexes[i] : indexes[i + 1]] for i in range(len(indexes) - 1)
+    ]
+    results = pool.map(
+        get_filename_size_tuple,
+        zip(
+            [host] * len(groups_filenames),
+            [username] * len(groups_filenames),
+            [password] * len(groups_filenames),
+            groups_filenames,
+        ),
+    )
+    flattened_results = list(chain(*results))
+    total_size += sum([int(res[1]) for res in flattened_results])
+    for result in flattened_results[:20]:
+        message += str(result[0])
+        message += f" - {format_file_size(float(result[1]))}\n"
+    if len(flattened_results) > 20:
+        message += f"Printed 20 out of {len(flattened_results)} files\n"
     message += (
         f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
     )
     return (message, host, filenames)
 
 
 def get_filenames_recursively(
@@ -182,24 +189,18 @@
 
 
 # /////////////////////////////
 # --- Tools
 # /////////////////////////////
 
 
-def parse_ftp_dataset_url(data_paths: list[str]) -> dict:
-    path_dict: dict[str, list[str]] = {}
-    for data_path in data_paths:
-        host = data_path[len("ftp://") :].split("/")[0]
-        path = data_path[len("ftp://" + host + "/") :]
-        if host in path_dict.keys():
-            path_dict[host].append(path)
-        else:
-            path_dict[host] = [path]
-    return path_dict
+def parse_ftp_dataset_url(data_path: str) -> tuple[str, str]:
+    host = data_path[len("ftp://") :].split("/")[0]
+    path = data_path[len("ftp://" + host + "/") :]
+    return (host, path)
 
 
 def create_filenames_out(
     filenames_in: list[str], output_directory: str = "", no_directories=False
 ) -> list[str]:
     filenames_out = []
     for filename_in in filenames_in:
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_motu.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
+import re
 from multiprocessing.pool import ThreadPool
-from typing import Tuple
+from typing import Optional, Tuple
 
 import click
 import s3fs
 from numpy import append, arange
 from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
@@ -14,15 +15,18 @@
 
 def download_s3native(
     username: str,
     password: str,
     native_request: NativeRequest,
 ) -> str:
     message, endpoint_url, filenames_in = download_header(
-        [str(native_request.dataset_url)], username, password
+        [str(native_request.dataset_url)],
+        native_request.regex,
+        username,
+        password,
     )
     filenames_out = create_filenames_out(
         filenames_in,
         native_request.output_directory,
         native_request.no_directories,
     )
     logging.info(message)
@@ -56,27 +60,31 @@
     )
     list(tqdm(download_summary_list, total=len(groups_in_files)))
     download_summary = "Download complete"
     return download_summary
 
 
 def download_header(
-    data_paths: list[str], username: str, password: str
+    data_paths: list[str], regex: Optional[str], username: str, password: str
 ) -> Tuple[str, str, list[str]]:
     path_dict = parse_s3native_dataset_url(data_paths)
     message = "You requested the download of the following files:\n"
     filenames, sizes, total_size = [], [], 0.0
     for endpoint_url, paths in path_dict.items():
         for path in paths:
-            files_name_size = get_filenames_recursively(endpoint_url, path)
-            for filename, size in files_name_size:
-                filenames += [filename]
-                sizes += [float(size)]
-                total_size += float(size)
-    for filename, size in files_name_size[:20]:
+            raw_filenames = get_filenames_recursively(endpoint_url, path)
+            filename_filtered = []
+            for filename, size in raw_filenames:
+                if not regex or re.match(regex, filename):
+                    filenames += [filename]
+                    sizes += [float(size)]
+                    total_size += float(size)
+                    filename_filtered.append((filename, size))
+
+    for filename, size in filename_filtered[:20]:
         message += str(filename)
         message += f" - {format_file_size(float(size))}\n"
     if len(filenames) > 20:
         message += f"Printed 20 out of {len(filenames)} files\n"
     message += (
         f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
     )
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,22 @@
     dataset = dataset.chunk(chunks="auto")
 
     if not assume_yes:
         logger = logging.getLogger("blank_logger")
         logger.warn(dataset)
         click.confirm("Do you want to continue?", abort=True, default=True)
 
-    store = zarr.DirectoryStore(path.join(output_directory, output_filename))
-    dataset.to_zarr(store)
+    if output_filename.endswith(".nc"):
+        dataset.to_netcdf(path.join(output_directory, output_filename))
+    else:
+        store = zarr.DirectoryStore(
+            path.join(output_directory, output_filename)
+        )
+        dataset.to_zarr(store)
+
     logging.info(
         f"Successfully downloaded to {path.join(output_directory, output_filename)}"
     )
 
 
 def download_zarr(
     username: str,
```

### Comparing `copernicus_marine_client-0.8.0/copernicus_marine_client/logging_conf.json` & `copernicus_marine_client-0.8.1/copernicus_marine_client/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.0/pyproject.toml` & `copernicus_marine_client-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.8.0"
+version = "0.8.1"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
@@ -24,14 +24,15 @@
 dask = ">=2022.1.1"
 netCDF4 = ">=1.6.3"
 s3fs = "^2023.6.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.20.0"
 types-requests = "2.27.11"
+ipython="^8.14.0"
 
 [tool.poetry.scripts]
 copernicus-marine = 'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `copernicus_marine_client-0.8.0/setup.py` & `copernicus_marine_client-0.8.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.8.0',
+    'version': '0.8.1',
     'description': '',
-    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n\nCheckout the help:\n\'\'\'\n> copernicus-marine login --help\nUsage: copernicus-marine login [OPTIONS]\n\n  This command creates the configurations files used by the various download\n  services and store them in a directory that can be specified by the user. If\n  the user specified a different \'config_file_directory\' from default one\n  ($HOME/.copernicus_marine_client), it needs to be passed also to the\n  download commands.\n\n  Examples:\n\n  Case 1 (Recommended):\n\n  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &\n  COPERNICUS_MARINE_CLIENT_PASSWORD specified:\n\n  > copernicus-marine login\n\n  Case 2:\n\n  > copernicus-marine login\n\n  < Username: [USER-INPUT]\n\n  < Password: [USER-INPUT]\n\n  Case 3:\n\n  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD\n\n  Case 4: Specific directory for config_files\n\n  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH\n\nOptions:\n  --username TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,\n                                  ask for user input\n  --password TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,\n                                  ask for user input\n  --config-file-directory TEXT    Path to the directory where the\n                                  configuration files are stored\n  --assume-yes                    Flag to skip confirmation before overwriting\n                                  configuration files\n  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]\n                                  Set the details printed to console by the\n                                  command (based on standard logging library).\n  --help                          Show this message and exit.\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files or Zarr stores.     Either one\n  of \'dataset-id\' or \'dataset-url\' is required     (can be found via the\n  \'copernicus-marine describe\' command).     The arguments value passed\n  individually through the CLI take precedence     over the values from the\n  "motu-api-request" option, which takes precedence     over the ones from the\n  "request-file" option\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02\n    13:00:00" -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --username TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset. Requires a\n                                  float within this range:  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset. Requires a\n                                  float within this range:  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset. Requires a\n                                  float within this range:  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset. Requires a\n                                  float within this range:  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset. Requires a\n                                  float within this range:  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset. Requires a\n                                  float within this range:  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset.\n                                  Caution: encapsulate date with " " to ensure\n                                  valid format for format "%Y-%m-%d %H:%M:%S"\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset.\n                                  Caution: encapsulate date with " " to ensure\n                                  valid format for format "%Y-%m-%d %H:%M:%S"\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output directory)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'.\n  --motu-api-request TEXT         Option to pass a complete MOTU api request\n                                  as a string. Caution, user has to replace\n                                  double quotes " with single quotes \' in the\n                                  request\n  --log-level [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]\n                                  Set the details printed to console by the\n                                  command (based on standard logging library).\n  --help                          Show this message and exit\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --username TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example:\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = \'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\'\nassert(dataset_id in cmc.get_all_dataset_ids())\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [variable for variable in dataset.variables if variable.short_name in [\'zooc\']][0]\ncoordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n  dataset_id=\'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\',\n  start_datetime="2023-04-20",\n  end_datetime=\'2023-04-21\',\n  minimal_latitude= 30.0,\n  maximal_latitude=30.1,\n  minimal_longitude=0.1,\n  maximal_longitude=0.2,\n  minimal_depth=100,\n  maximal_depth=1000,\n  variables = [\'zooc\'],\n  force_protocol = "zarr-map",\n  output_directory = \'data_folder\',\n  output_filename = \'datastore.zarr\',\n  assume_yes = True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(username=\'FAKE_USERNAME\', password=\'FAKE_PASSWORD\', subset_request=subset_request)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine=\'zarr\', out_type=\'xarray\')\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
+    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n\nCheckout the help:\n\'\'\'\n> copernicus-marine login --help\nUsage: copernicus-marine login [OPTIONS]\n\n  This command creates the configurations files used by the various download\n  services and store them in a directory that can be specified by the user. If\n  the user specified a different \'config_file_directory\' from default one\n  ($HOME/.copernicus_marine_client), it needs to be passed also to the\n  download commands.\n\n  Examples:\n\n  Case 1 (Recommended):\n\n  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &\n  COPERNICUS_MARINE_CLIENT_PASSWORD specified:\n\n  > copernicus-marine login\n\n  Case 2:\n\n  > copernicus-marine login\n\n  < Username: [USER-INPUT]\n\n  < Password: [USER-INPUT]\n\n  Case 3:\n\n  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD\n\n  Case 4: Specific directory for config_files\n\n  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH\n\nOptions:\n  --username TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,\n                                  ask for user input\n  --password TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,\n                                  ask for user input\n  --config-file-directory TEXT    Path to the directory where the\n                                  configuration files are stored\n  --assume-yes                    Flag to skip confirmation before overwriting\n                                  configuration files\n  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]\n                                  Set the details printed to console by the\n                                  command (based on standard logging library).\n  --help                          Show this message and exit.\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n**Be aware that the regular expression must match the full absolute path of the files to filter.**\n\nExample:\n```\n> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to continue? [y/N]:\n```\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    assume_yes=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `copernicus_marine_client-0.8.0/PKG-INFO` & `copernicus_marine_client-0.8.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -35,17 +35,18 @@
 
 This package allows to recover products and datasets information from Command Line Interface or with Python code,
 as well as download subsets and native files.
 
 ## Command Line Interface (CLI)
 
 ### Command *describe*
-Retrieve information about products as JSON:
 
-```
+Retrieve information about all products as JSON:
+
+```txt
 > copernicus-marine describe
 {
   "products": [
     {
       "title": "Antarctic Sea Ice Extent from Reanalysis",
       "product_id": "ANTARCTIC_OMI_SI_extent",
       "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
@@ -56,15 +57,15 @@
     ...
   ]
 }
 ```
 
 Retrieve all information about datasets as JSON:
 
-```
+```txt
 > copernicus-marine describe --include-datasets
 {
   "products": [
     {
       "title": "Antarctic Sea Ice Extent from Reanalysis",
       "product_id": "ANTARCTIC_OMI_SI_extent",
       "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
@@ -84,33 +85,14 @@
           "variables": []
         }
       ]
     },
     ...
   ]
 }
-
-```
-
-Check out the help:
-
-```
-> copernicus-marine describe --help
-Usage: copernicus-marine describe [OPTIONS]
-
-Options:
-  --one-line             Output JSON on one line
-  --include-description  Include product description in output
-  --include-datasets     Include product dataset details in output
-  --include-keywords     Include product keyword details in output
-  -c, --contains TEXT    Filter catalogue output. Returns products with
-                         attributes matching a string token
-  --overwrite-cache      Force to refresh the catalogue by overwriting the
-                         local cache
-  --help                 Show this message and exit.
 ```
 
 ### Command *login*
 
 Create the configuration files for access to the copernicus marine service:
 '.dodsrc', '.netrc', '.motuclient-python.ini'.
 The directory to store these configuration files can be modified by the user using the "config-file-directory" option
@@ -179,111 +161,31 @@
   --help                          Show this message and exit.
 '''
 
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
-```
+```txt
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 < Username:
 < Password:
 < Trying to download as one file...
 ```
 
-File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
-
-Check out the help:
-
-```
-> copernicus-marine subset --help
-
-Usage: copernicus-marine subset [OPTIONS]
-
-  Downloads subsets of datasets as NetCDF files or Zarr stores.     Either one
-  of 'dataset-id' or 'dataset-url' is required     (can be found via the
-  'copernicus-marine describe' command).     The arguments value passed
-  individually through the CLI take precedence     over the values from the
-  "motu-api-request" option, which takes precedence     over the ones from the
-  "request-file" option
-
-  Example:
-
-    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --variable analysed_sst --variable sea_ice_fraction --start-datetime
-    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
-    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
-
-    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
-    analysed_sst   -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02
-    13:00:00" -x 0.0 -X 0.1 -y 0.0 -Y 0.1
-
-Options:
-  -u, --dataset-url TEXT          The full dataset URL
-  -i, --dataset-id TEXT           The dataset id
-  --username TEXT
-  --password TEXT
-  -v, --variable TEXT             Specify dataset variables
-  -x, --minimal-longitude FLOAT RANGE
-                                  Minimal longitude for the subset. Requires a
-                                  float within this range:  [-180<=x<=180]
-  -X, --maximal-longitude FLOAT RANGE
-                                  Maximal longitude for the subset. Requires a
-                                  float within this range:  [-180<=x<=180]
-  -y, --minimal-latitude FLOAT RANGE
-                                  Minimal latitude for the subset. Requires a
-                                  float within this range:  [-90<=x<=90]
-  -Y, --maximal-latitude FLOAT RANGE
-                                  Maximal latitude for the subset. Requires a
-                                  float within this range:  [-90<=x<=90]
-  -z, --minimal-depth FLOAT RANGE
-                                  Minimal depth for the subset. Requires a
-                                  float within this range:  [x>=0]
-  -Z, --maximal-depth FLOAT RANGE
-                                  Maximal depth for the subset. Requires a
-                                  float within this range:  [x>=0]
-  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The start datetime of the temporal subset.
-                                  Caution: encapsulate date with " " to ensure
-                                  valid format for format "%Y-%m-%d %H:%M:%S"
-  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The end datetime of the temporal subset.
-                                  Caution: encapsulate date with " " to ensure
-                                  valid format for format "%Y-%m-%d %H:%M:%S"
-  -o, --output-directory PATH     The destination folder for the downloaded
-                                  files. Default is the current directory
-  -f, --output-filename PATH      Concatenate the downloaded data in the given
-                                  file name (under the output directory)
-  --assume-yes                    Flag to skip confirmation before download
-  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
-                                  Force download through one of the available
-                                  protocols
-  --dry-run                       Flag to specify NOT to send the request to
-                                  external server. Returns the request instead
-  --request-file PATH             Option to pass a filename corresponding to a
-                                  file containg CLI arguments. The file MUST
-                                  follow the structure of dataclass
-                                  'SubsetRequest'.
-  --motu-api-request TEXT         Option to pass a complete MOTU api request
-                                  as a string. Caution, user has to replace
-                                  double quotes " with single quotes ' in the
-                                  request
-  --log-level [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
-                                  Set the details printed to console by the
-                                  command (based on standard logging library).
-  --help                          Show this message and exit
-```
+File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with '.nc' suffix, the file will be downloaded as a netCDF file.
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
 
 Example:
-```
+
+```txt
 > copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/
 
 < Username:
 < Password:
 < You requested the download of the following files:
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
@@ -295,141 +197,127 @@
 Total size of the download: 19.62 MB
 
 
 Do you want to continue? [y/N]:
 ```
 
 File(s) downloaded to ./{path}/{filename} if not specified otherwise:
+
 - "--output-path" specifies a directory to dump the files in
 - "--no-directories" to not recreate the folder structure
 
 If not specified otherwise, after the header display with a summary of the request,
 the user is asked for confirmation:
+
 - "--no-confirmation" to turn down the confirmation prompt
 - "--show-outputnames" to display the full paths of the outputs files
 
-Check out the help:
+Option `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.
+**Be aware that the regular expression must match the full absolute path of the files to filter.**
 
+Example:
 ```
-> copernicus-marine native --help
+> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"
+Password:
+You requested the download of the following files:
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 
-Usage: copernicus-marine native [OPTIONS]
+Total size of the download: 9.82 MB
 
-  Downloads native data files based on     dataset_id or datafiles url path.
-  The function fetches the files recursively if a folder path is passed as
-  url.     When provided a dataset id,     all the files in the corresponding
-  folder will be downloaded.
 
-      By default for any download request, a summary of the request result is
-      displayed to the user and a confirmation is asked.     This can be
-      turned down. Example:
+Do you want to continue? [y/N]:
+```
 
-    copernicus-marine native -nd -o data_folder --dataset-id
-    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
+### The `--help` argument
 
-    copernicus-marine native -nd -o data_folder --dataset-url
-    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
-    pft_myint_7km-3D-diato_P1M-m
-
-Options:
-  -u, --dataset-url TEXT       Path to the data files
-  -i, --dataset-id TEXT        The dataset id
-  --username TEXT
-  --password TEXT
-  -nd, --no-directories        Option to not recreate folder hierarchy in
-                               ouput directory.
-  --show-outputnames           Option to display the names of the output files
-                               before download.
-  -o, --output-directory PATH  The destination directory for the downloaded
-                               files. Default is the current directory
-                               [required]
-  --assume-yes                 Whether to ask for confirmation before
-                               download, after header display. If 'True',
-                               skips confirmation.
-  --dry-run                    Flag to specify NOT to send the request to
-                               external server. Returns the request instead
-  --request-file PATH          Option to pass a file containg CLI arguments.
-                               The file MUST follow the structure of dataclass
-                               'SubsetRequest'. ANY PARAMETER SPECIFIED ASIDE
-                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION
-                               FOR THE REQUEST IF FILE IS SPECIFIED.
-  --help                       Show this message and exit.
-```
+In any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.
 
 ## Python functions
 
 The library also provide python functions to help with catalogue
 browsing and datasets download in scripts.
 
-### Basic example:
+### Basic example
 
 In this example 4 steps are performed:
   1- Fetch the catalogue to select a dataset
   2- Construct a SubsetRequest for this dataset
   3- Download the subset as a zarr store
   4- Open the subset as an xarray dataset
 
-```
+```python
 import copernicus_marine_client as cmc
 
 # Step 1: Fetch catalogue and parse information on dataset
 catalogue = cmc.fetch_catalogue()
-dataset_id = 'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m'
-assert(dataset_id in cmc.get_all_dataset_ids())
+dataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"
+assert dataset_id in cmc.get_all_dataset_ids()
 dataset = catalogue.filter([dataset_id]).products[0].datasets[0]
 # Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest
-variable = [variable for variable in dataset.variables if variable.short_name in ['zooc']][0]
-coordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}
+variable = [
+    variable for variable in dataset.variables if variable.short_name in ["zooc"]
+][0]
+coordinates = {
+    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)
+    for coordinate in variable.coordinates
+}
 
 # Step 2: Construct the request based on parsed information
 subset_request = cmc.SubsetRequest(
-  dataset_id='cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m',
-  start_datetime="2023-04-20",
-  end_datetime='2023-04-21',
-  minimal_latitude= 30.0,
-  maximal_latitude=30.1,
-  minimal_longitude=0.1,
-  maximal_longitude=0.2,
-  minimal_depth=100,
-  maximal_depth=1000,
-  variables = ['zooc'],
-  force_protocol = "zarr-map",
-  output_directory = 'data_folder',
-  output_filename = 'datastore.zarr',
-  assume_yes = True,
+    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",
+    start_datetime="2023-04-20",
+    end_datetime="2023-04-21",
+    minimal_latitude=30.0,
+    maximal_latitude=30.1,
+    minimal_longitude=0.1,
+    maximal_longitude=0.2,
+    minimal_depth=100,
+    maximal_depth=1000,
+    variables=["zooc"],
+    force_protocol="zarr-map",
+    output_directory="data_folder",
+    output_filename="datastore.zarr",
+    assume_yes=True,
 )
 
 # Step 3: Download the subset based on request content
-filename = cmc.download_subset(username='FAKE_USERNAME', password='FAKE_PASSWORD', subset_request=subset_request)
+filename = cmc.download_subset(
+    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request
+)
 
 # Step 4: Open the downloaded subset as an xarray dataset
-subset = cmc.open_dataset(filepath=filename, engine='zarr', out_type='xarray')
+subset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")
 ```
 
 ## Installation
 
 Using pip, for example:
-```
+
+```shell
 pip install copernicus-marine-client
 ```
+
 ## Technical details
 
 This module is organized around two capabilities:
+
 - a catalogue, parsed from web requests, that contains informations on the available datasets
 - a downloader, to simplify the download of dataset files or subsets
 
 The catalogue can be displayed by the user and is used by the downloader to link the user
 requests with files or subset of files to retrieve.
 The downloader will help the user download the needed datasets.
 
 A rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.
 
 For subset command, the format is:
 
-```
+```python
 @dataclass
 class SubsetRequest:
     dataset_url: Optional[str] = None
     dataset_id: Optional[str] = None
     variables: Optional[List[str]] = None
     minimal_longitude: Optional[float] = None
     maximal_longitude: Optional[float] = None
```

