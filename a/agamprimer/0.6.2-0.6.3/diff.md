# Comparing `tmp/agamprimer-0.6.2.tar.gz` & `tmp/agamprimer-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agamprimer-0.6.2.tar", max compression
+gzip compressed data, was "agamprimer-0.6.3.tar", max compression
```

## Comparing `agamprimer-0.6.2.tar` & `agamprimer-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35766 2023-07-02 20:25:19.636906 agamprimer-0.6.2/AgamPrimer/AgamPrimer.py
--rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.2/AgamPrimer/__init__.py
--rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/top_level.txt
--rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.2/LICENSE
--rw-r--r--   0        0        0      730 2023-07-02 20:22:33.331225 agamprimer-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    41366 2023-07-03 22:12:06.896656 agamprimer-0.6.3/AgamPrimer/AgamPrimer.py
+-rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.3/AgamPrimer/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.3/AgamPrimer/agamPrimer.egg-info/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.3/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.3/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.3/AgamPrimer/agamPrimer.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.3/LICENSE
+-rw-r--r--   0        0        0      730 2023-07-03 22:13:45.928186 agamprimer-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.3/PKG-INFO
```

### Comparing `agamprimer-0.6.2/AgamPrimer/AgamPrimer.py` & `agamprimer-0.6.3/AgamPrimer/AgamPrimer.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,28 @@
     genome_seq,
     assay_name,
     assay_type,
     probe_exclude_region_size=20,
 ):
     """
     Extracts sequence of interest from genome sequence
+
+    PARAMETERS
+    ----------
+    target_loc : int
+        The target location of the SNP in the genome sequence
+    amplicon_size_range : list
+        The minimum and maximum size of the amplicon to design primers for
+    genome_seq : dask.array.core.Array
+        The genome sequence from ag3.genome_sequence()
+    assay_name : str
+        The name of the assay
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
     """
     target = int(target_loc)
     # Set up range for the input sequence, we'll take the max range
     # of the amplicon size and add that either side of the target SNP
     amp_size_range = int(np.max(amplicon_size_range))
     start = target - amp_size_range
     end = target + amp_size_range
@@ -60,15 +74,27 @@
 
     return (target_sequence, gdna_pos, seq_parameters)
 
 
 def prepare_cDNA_sequence(transcript, genome_seq, assay_name, cDNA_exon_junction):
     """
     Extract exonic sequence for our transcript and record exon-exon junctions
+
+    PARAMETERS
+    ----------
+    transcript : str
+        The AGAP identifier of the transcript to design primers for
+    genome_seq : dask.array.core.Array
+        The genome sequence from ag3.genome_sequence()
+    assay_name : str
+        The name of the assay
+    cDNA_exon_junction : bool
+        If True, cDNA primers will be designed to span an exon-exon junction. We strongly recommend for qPCR purposes.
     """
+
     # subset gff to your gene
     gff = ag3.geneset()
     gff = gff.query("type == 'exon' & Parent == @transcript")
     # Get fasta sequence for each of our exons, and remember gDNA position
     seq = dict()
     gdna_pos = dict()
     for i, exon in enumerate(zip(gff.start, gff.end)):
@@ -103,14 +129,31 @@
     assay_name,
     genome_seq,
     amplicon_size_range,
     cDNA_exon_junction=True,
 ):
     """
     Prepare the sequence for primer3, depending on cDNA or gDNA input type
+
+    PARAMETERS
+    ----------
+    target : str
+        The target to design primers for. For gDNA primers, this should be a contig:position string,
+        for example '2L:28545767'. For cDNA primers, this should be an AGAP identifier.
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
+    assay_name : str
+        The name of the assay
+    genome_seq : dask.array.core.Array
+        The genome sequence from ag3.genome_sequence()
+    amplicon_size_range : list
+        The minimum and maximum size of the amplicon to design primers for
+    cDNA_exon_junction : bool
+        If True, cDNA primers will be designed to span an exon-exon junction. We strongly recommend for qPCR purposes.
     """
 
     if any(item in assay_type for item in ["gDNA", "probe"]):
         # genomic DNA
         target_sequence, gdna_pos, seq_parameters = prepare_gDNA_sequence(
             target_loc=target,
             amplicon_size_range=amplicon_size_range,
@@ -136,14 +179,29 @@
     n_primer_pairs=None,
     amplicon_size_range=None,
     generate_defaults=False,
 ):
     """
     adds necessary parameters depending on assay_type, or can
     generate the default parameters
+
+    PARAMETERS
+    ----------
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
+    primer_parameters : dict
+        A dictionary of primer3 parameters to use for primer design. If 'default' is specified, default
+        primer3 parameters will be generated.
+    n_primer_pairs : int
+        The number of primer pairs to design.
+    amplicon_size_range : list
+        The minimum and maximum size of the amplicon to design primers for
+    generate_defaults : bool
+        If True, default primer3 parameters will be generated.
     """
 
     if generate_defaults:
         primer_parameters = {
             "PRIMER_OPT_SIZE": 20,
             "PRIMER_TASK": "generic",
             "PRIMER_MIN_SIZE": 17,
@@ -180,15 +238,23 @@
         primer_parameters["PRIMER_PICK_RIGHT_PRIMER"] = 0
         primer_parameters["PRIMER_PICK_LEFT_PRIMER"] = 0
     return primer_parameters
 
 
 def primer3_run_statistics(primer_dict, assay_type):
     """
-    Prints out primer3 run statistics from the primer3 results dictionary
+    Prints out primer3 run statistics from the primer3 results dictionary.
+
+    PARAMETERS
+    ----------
+    primer_dict : dict
+        The primer3 results dictionary returned by primer3.designPrimers()
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
     """
     _, row_start = _return_oligo_list(assay_type)
     primer_dict = _convert_results_dict_naming(primer_dict)
     # Convert the dict into a pandas dataframe
     primer_df = pd.DataFrame.from_dict(primer_dict.items())
     # Rename the columns
     primer_df = primer_df.rename(columns={0: "parameter", 1: "value"})
@@ -202,14 +268,27 @@
     ) in explanations_df.iterrows():
         print(row["parameter"], " : ", row["value"], "\n")
 
 
 def primer3_to_pandas(primer_dict, assay_type):
     """
     Convert primer3 results to pandas dataframe
+
+    PARAMETERS
+    ----------
+    primer_dict : dict
+        The primer3 results dictionary returned by primer3.designPrimers()
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
+
+    RETURNS
+    -------
+    primer_df : pandas.DataFrame
+        A pandas DataFrame containing the primer sequences and their information.
     """
     oligos, row_start = _return_oligo_list(assay_type)
     # Convert the dict into a pandas dataframe
     primer_dict = _convert_results_dict_naming(primer_dict)
     primer_df = pd.DataFrame.from_dict(primer_dict.items())
     # Rename the columns
     primer_df = primer_df.rename(columns={0: "parameter", 1: "value"})
@@ -252,14 +331,38 @@
     assay_type,
     seq_parameters,
     out_dir=None,
     sample_query=None,
 ):
     """
     Loop through n primer pairs, retrieving frequency data and plot allele frequencies
+
+    PARAMETERS
+    ----------
+    primer_df : pandas.DataFrame
+        A pandas DataFrame containing the primer sequences and their information, returned by primer3_to_pandas()
+    gdna_pos : numpy.ndarray
+        The genomic positions of the target sequence
+    contig : str
+        The contig of the target sequence, e.g. '2L'
+    sample_sets : str or list of str, optional
+        Can be a sample set identifier (e.g., "AG1000G-AO") or a list of
+        sample set identifiers (e.g., ["AG1000G-BF-A", "AG1000G-BF-B"]) or a
+        release identifier (e.g., "3.0") or a list of release identifiers.
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
+    seq_parameters : dict
+        A dictionary of parameters for primer3, returned by prepare_sequence()
+    out_dir : str, optional
+        The directory to write output files to. If not specified, outputs will not be written to file.
+    sample_query: str, optional
+        A pandas query string which will be evaluated against the sample
+        metadata e.g., "taxon == 'coluzzii' and country == 'Burkina Faso'" to subset
+        the genotypes to a specific set of samples.
     """
 
     if sample_query is not None:
         print(f"Subsetting allele frequencies to {sample_query}")
 
     name = seq_parameters["SEQUENCE_ID"]
     target = seq_parameters["GENOMIC_TARGET"]
@@ -292,14 +395,32 @@
     seq_parameters,
     assay_type,
     legend_loc="best",
     out_dir=None,
 ):
     """
     Plot the position of the primer sets in relation to any nearby exons
+
+    PARAMETERS
+    ----------
+    primer_res_dict : dict
+        A dictionary containing the primer3 results, returned by primer3.designPrimers()
+    primer_df : pandas.DataFrame
+        A pandas DataFrame containing the primer sequences and their information, returned by primer3_to_pandas()
+    contig : str
+        The contig of the target sequence, e.g. '2L'
+    seq_parameters : dict
+        A dictionary of parameters for primer3, returned by prepare_sequence()
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
+    legend_loc : str, optional
+        The location of the legend in the plot. Can be 'best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center' or 'center'.
+    out_dir : str, optional
+        The directory to write output files to. If not specified, outputs will not be written to file.
     """
     oligos, _ = _return_oligo_list(assay_type)
     assay_name = seq_parameters["SEQUENCE_ID"]
     # Load geneset (gff)
     gff = ag3.geneset()
     if any(item in assay_type for item in ["gDNA", "probe"]):
         start = seq_parameters["GENOMIC_TARGET"] - 500
@@ -445,14 +566,24 @@
     if out_dir:
         fig.savefig(f"{out_dir}/{assay_name}_primer_locs.png", dpi=300)
 
 
 def gget_blat_genome(primer_df, assay_type, assembly="anoGam3"):
     """
     Aligns primers to the AgamP3 genome with BLAT.
+
+    PARAMETERS
+    ----------
+    primer_df : pandas.DataFrame
+        A pandas DataFrame containing the primer sequences and their information, returned by primer3_to_pandas()
+    assay_type : str
+        The type of assay, either 'gDNA primers' or 'gDNA primers + probe', 'cDNA primers'
+        or 'probe'
+    assembly : str, optional
+        The genome assembly to use with Blat. 'anoGam3' is Anopheles gambiae. Please see the gget documentation for more information.
     """
     oligos, _ = _return_oligo_list(assay_type=assay_type)
 
     pair_dict = {}
     for primer_pair in primer_df:
         oligo_list = []
         for oligo in oligos:
```

### Comparing `agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/PKG-INFO` & `agamprimer-0.6.3/AgamPrimer/agamPrimer.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.2/LICENSE` & `agamprimer-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.2/pyproject.toml` & `agamprimer-0.6.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AgamPrimer"
-version = "0.6.2"
+version = "0.6.3"
 description = "A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "AgamPrimer" }
 ]
```

### Comparing `agamprimer-0.6.2/PKG-INFO` & `agamprimer-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agamprimer
-Version: 0.6.2
+Version: 0.6.3
 Summary: A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

