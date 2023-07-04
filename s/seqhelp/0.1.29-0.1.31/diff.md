# Comparing `tmp/seqhelp-0.1.29.tar.gz` & `tmp/seqhelp-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqhelp-0.1.29.tar", max compression
+gzip compressed data, was "seqhelp-0.1.31.tar", max compression
```

## Comparing `seqhelp-0.1.29.tar` & `seqhelp-0.1.31.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      505 2023-03-03 08:11:56.829659 seqhelp-0.1.29/pyproject.toml
--rw-r--r--   0        0        0      941 2022-11-17 07:31:40.113608 seqhelp-0.1.29/seqhelp/__init__.py
--rw-r--r--   0        0        0    14069 2022-11-28 12:55:37.230627 seqhelp-0.1.29/seqhelp/codon.py
--rw-r--r--   0        0        0    13205 2022-11-28 12:56:18.688681 seqhelp-0.1.29/seqhelp/codon_pair.py
--rw-r--r--   0        0        0     9007 2023-03-03 08:05:52.356302 seqhelp-0.1.29/seqhelp/common.py
--rw-r--r--   0        0        0     4849 2023-03-03 08:09:16.564495 seqhelp-0.1.29/seqhelp/dinucleotides.py
--rw-r--r--   0        0        0     2249 2023-03-03 08:09:46.704217 seqhelp-0.1.29/seqhelp/gc_content.py
--rw-r--r--   0        0        0     3661 2022-04-03 22:01:38.729989 seqhelp-0.1.29/seqhelp/relations.py
--rw-r--r--   0        0        0    35338 2023-02-03 15:28:31.257874 seqhelp-0.1.29/seqhelp/sequences.py
--rw-r--r--   0        0        0     4892 2022-10-25 07:13:45.647882 seqhelp-0.1.29/seqhelp/taxonomy.py
--rw-r--r--   0        0        0     3098 2022-05-05 07:41:51.791780 seqhelp-0.1.29/seqhelp/virus_hosts.py
--rw-r--r--   0        0        0  6926585 2022-04-03 22:01:40.179989 seqhelp-0.1.29/seqhelp/virushostdb.tsv.bak
--rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 seqhelp-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-07-04 08:45:50.783764 seqhelp-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0      941 2022-11-17 07:31:40.113608 seqhelp-0.1.31/seqhelp/__init__.py
+-rw-r--r--   0        0        0    14069 2022-11-28 12:55:37.230627 seqhelp-0.1.31/seqhelp/codon.py
+-rw-r--r--   0        0        0    13205 2022-11-28 12:56:18.688681 seqhelp-0.1.31/seqhelp/codon_pair.py
+-rw-r--r--   0        0        0     9007 2023-03-03 08:05:52.356302 seqhelp-0.1.31/seqhelp/common.py
+-rw-r--r--   0        0        0     4849 2023-03-03 08:09:16.564495 seqhelp-0.1.31/seqhelp/dinucleotides.py
+-rw-r--r--   0        0        0     2249 2023-03-03 08:09:46.704217 seqhelp-0.1.31/seqhelp/gc_content.py
+-rw-r--r--   0        0        0     3661 2022-04-03 22:01:38.729989 seqhelp-0.1.31/seqhelp/relations.py
+-rw-r--r--   0        0        0    36103 2023-07-04 07:23:48.370849 seqhelp-0.1.31/seqhelp/sequences.py
+-rw-r--r--   0        0        0     4892 2022-10-25 07:13:45.647882 seqhelp-0.1.31/seqhelp/taxonomy.py
+-rw-r--r--   0        0        0     3098 2022-05-05 07:41:51.791780 seqhelp-0.1.31/seqhelp/virus_hosts.py
+-rw-r--r--   0        0        0  6926585 2022-04-03 22:01:40.179989 seqhelp-0.1.31/seqhelp/virushostdb.tsv.bak
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 seqhelp-0.1.31/PKG-INFO
```

### Comparing `seqhelp-0.1.29/seqhelp/__init__.py` & `seqhelp-0.1.31/seqhelp/__init__.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/codon.py` & `seqhelp-0.1.31/seqhelp/codon.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/codon_pair.py` & `seqhelp-0.1.31/seqhelp/codon_pair.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/common.py` & `seqhelp-0.1.31/seqhelp/common.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/dinucleotides.py` & `seqhelp-0.1.31/seqhelp/dinucleotides.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/gc_content.py` & `seqhelp-0.1.31/seqhelp/gc_content.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/relations.py` & `seqhelp-0.1.31/seqhelp/relations.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/sequences.py` & `seqhelp-0.1.31/seqhelp/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,18 @@
                     f.write(fasta.format("fasta"))
 
     if return_path:
         return path
     else:
         if path.suffix == ".gz":
             with gzip.open(path, "rt") as f:
-                return next(SeqIO.parse(f, "fasta"))
+                return next(SeqIO.parse(f, "fasta"), None)
         else:
+            if path.stat().st_size == 0:
+                return None
             with path.open("r") as f:
                 return next(SeqIO.parse(f, "fasta"))
 
 
 class DownloadType(enum.Enum):
     Full = "Full"
     Coding = "Coding"
@@ -257,19 +259,24 @@
     Coding = "Coding"
     NonCoding = "NonCoding"
     DustMasked = "DustMasked"
     TandemRepeatsFinder = "TandemRepeatsFinder"
     Genes = "Genes"
 
 
-def _get_sequences(p: Path):
+def _get_sequences(p: Path) -> list[SeqRecord]:
     with gzip.open(p, "rt") as f:
         return list(SeqIO.parse(f, "fasta"))
 
 
+def _get_sequence(p: Path) -> SeqRecord:
+    with gzip.open(p, "rt") as f:
+        return SeqIO.read(f, "fasta")
+
+
 def get_sequence_batch(
     aids: list[str],
     download_folder: Path = Path.home() / "data" / "downloads",
     sequence_part: SequencePart = SequencePart.Full,
     return_path: bool = False,
     batch_size: int = 50,
 ) -> Iterable[SeqRecord | Path]:
@@ -314,15 +321,15 @@
         not_found_aids = [aid for aid, p in zip(aids, paths) if p is None]
 
         batch_download(not_found_aids, download_folder, batch_size, DownloadType.Full)
         all_paths = (get_path(aid, download_folder, [".fa", ".fasta"]) for aid in aids)
         if return_path:
             return all_paths
         else:
-            return (SeqIO.read(p, "fasta") for p in all_paths)
+            return (_get_sequence(p) for p in all_paths)
 
     elif sequence_part == SequencePart.Coding:
         paths = [Path(download_folder / f"{aid}_joined_cds.fa.gz") for aid in aids]
 
         not_found_aids = [aid for aid, p in zip(aids, paths) if not p.is_file()]
 
         batch_download(not_found_aids, download_folder, batch_size, DownloadType.Coding)
@@ -367,21 +374,35 @@
             get_path(
                 aid,
                 download_folder,
                 [".fa.dustmasked", ".fasta.dustmasked"],
             )
             for aid in aids
         ]
+        not_found_aids = [aid for aid, p in zip(aids, paths) if p is None]
+
+        batch_download(not_found_aids, download_folder, batch_size, DownloadType.Full)
+
         for path, aid in zip(paths, aids):
+            # If we had to download it, it also need dustmasking
             if path is None:
                 record = get_or_download_fasta(aid, download_folder, return_path=False)
+                if record is None:
+                    continue
                 dustmasked = dustmask_record(record)
                 path = download_folder / f"{aid}.fa.dustmasked"
                 SeqIO.write(dustmasked, path, "fasta")
 
+        working_paths = [p for p in paths if p is not None and p.is_file()]
+
+        if return_path:
+            return working_paths
+        else:
+            return (_get_sequence(p) for p in working_paths)
+
     elif sequence_part == SequencePart.TandemRepeatsFinder:
         paths = [
             get_path(
                 aid,
                 download_folder,
                 [".fa.2.7.7.80.10.50.500.mask", ".fasta.2.7.7.80.10.50.500.mask"],
             )
@@ -461,14 +482,16 @@
         path = get_path(
             aid,
             download_folder,
             [".fa.dustmasked", ".fasta.dustmasked"],
         )
         if path is None:
             record = get_or_download_fasta(aid, download_folder, return_path=False)
+            if record is None:
+                return None
             dustmasked = dustmask_record(record)
             path = download_folder / f"{aid}.fa.dustmasked.gz"
             with gzip.open(path, "wt") as f:
                 SeqIO.write(dustmasked, f, "fasta")
 
     elif sequence_part == SequencePart.TandemRepeatsFinder:
         path = get_path(
```

### Comparing `seqhelp-0.1.29/seqhelp/taxonomy.py` & `seqhelp-0.1.31/seqhelp/taxonomy.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/virus_hosts.py` & `seqhelp-0.1.31/seqhelp/virus_hosts.py`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/seqhelp/virushostdb.tsv.bak` & `seqhelp-0.1.31/seqhelp/virushostdb.tsv.bak`

 * *Files identical despite different names*

### Comparing `seqhelp-0.1.29/PKG-INFO` & `seqhelp-0.1.31/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: seqhelp
-Version: 0.1.29
+Version: 0.1.31
 Summary: Package with helper functions for the retrieval and analysis of sequences from ncbi
 Author: Joel Gustafsson
 Author-email: me@joelgustafsson.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: biopython (>=1.79,<2.0)
 Requires-Dist: ete3 (>=3.1,<4.0)
 Requires-Dist: numba (>=0.55)
 Requires-Dist: numpy (>=1.18)
-Requires-Dist: pandas (>=1.4,<2.0)
+Requires-Dist: pandas (>=1.4)
 Requires-Dist: tqdm (>=4.62,<5.0)
```

