# Comparing `tmp/biodatatypes-0.1.1.tar.gz` & `tmp/biodatatypes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biodatatypes-0.1.1.tar", last modified: Mon Jul  3 07:05:15 2023, max compression
+gzip compressed data, was "biodatatypes-0.2.1.tar", last modified: Tue Jul  4 08:36:50 2023, max compression
```

## Comparing `biodatatypes-0.1.1.tar` & `biodatatypes-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 kent       (501) wheel        (0)        0 2023-07-03 07:05:15.938846 biodatatypes-0.1.1/
--rw-r--r--   0 kent       (501) wheel        (0)     1071 2023-06-28 08:48:43.000000 biodatatypes-0.1.1/LICENSE
--rw-r--r--   0 kent       (501) wheel        (0)     1982 2023-07-03 07:05:15.938177 biodatatypes-0.1.1/PKG-INFO
--rw-r--r--   0 kent       (501) wheel        (0)     1474 2023-07-03 07:01:21.000000 biodatatypes-0.1.1/README.md
-drwxr-xr-x   0 kent       (501) wheel        (0)        0 2023-07-03 07:05:15.932295 biodatatypes-0.1.1/biodatatypes/
--rw-r--r--   0 kent       (501) wheel        (0)      156 2023-06-30 08:31:09.000000 biodatatypes-0.1.1/biodatatypes/__init__.py
-drwxr-xr-x   0 kent       (501) wheel        (0)        0 2023-07-03 07:05:15.936592 biodatatypes-0.1.1/biodatatypes/constants/
--rw-r--r--   0 kent       (501) wheel        (0)        0 2023-06-30 07:42:44.000000 biodatatypes-0.1.1/biodatatypes/constants/__init__.py
--rw-r--r--   0 kent       (501) wheel        (0)     2957 2023-07-03 05:58:55.000000 biodatatypes-0.1.1/biodatatypes/constants/aminoacid.py
--rw-r--r--   0 kent       (501) wheel        (0)     5725 2023-07-03 05:58:55.000000 biodatatypes-0.1.1/biodatatypes/constants/codon.py
--rw-r--r--   0 kent       (501) wheel        (0)     1026 2023-07-03 05:58:55.000000 biodatatypes-0.1.1/biodatatypes/constants/nucleotide.py
-drwxr-xr-x   0 kent       (501) wheel        (0)        0 2023-07-03 07:05:15.937301 biodatatypes-0.1.1/biodatatypes/sequence/
--rw-r--r--   0 kent       (501) wheel        (0)        0 2023-06-30 08:30:53.000000 biodatatypes-0.1.1/biodatatypes/sequence/__init__.py
--rw-r--r--   0 kent       (501) wheel        (0)    46107 2023-07-03 07:03:01.000000 biodatatypes-0.1.1/biodatatypes/sequence/sequence.py
--rw-r--r--   0 kent       (501) wheel        (0)    52277 2023-07-03 05:58:55.000000 biodatatypes-0.1.1/biodatatypes/units.py
-drwxr-xr-x   0 kent       (501) wheel        (0)        0 2023-07-03 07:05:15.935114 biodatatypes-0.1.1/biodatatypes.egg-info/
--rw-r--r--   0 kent       (501) wheel        (0)     1982 2023-07-03 07:05:15.000000 biodatatypes-0.1.1/biodatatypes.egg-info/PKG-INFO
--rw-r--r--   0 kent       (501) wheel        (0)      440 2023-07-03 07:05:15.000000 biodatatypes-0.1.1/biodatatypes.egg-info/SOURCES.txt
--rw-r--r--   0 kent       (501) wheel        (0)        1 2023-07-03 07:05:15.000000 biodatatypes-0.1.1/biodatatypes.egg-info/dependency_links.txt
--rw-r--r--   0 kent       (501) wheel        (0)       13 2023-07-03 07:05:15.000000 biodatatypes-0.1.1/biodatatypes.egg-info/top_level.txt
--rw-r--r--   0 kent       (501) wheel        (0)      104 2023-07-03 07:01:21.000000 biodatatypes-0.1.1/pyproject.toml
--rw-r--r--   0 kent       (501) wheel        (0)       38 2023-07-03 07:05:15.939250 biodatatypes-0.1.1/setup.cfg
--rw-r--r--   0 kent       (501) wheel        (0)      784 2023-07-03 07:04:04.000000 biodatatypes-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:50.668506 biodatatypes-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-04 08:36:50.668506 biodatatypes-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:50.664506 biodatatypes-0.2.1/biodatatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:50.668506 biodatatypes-0.2.1/biodatatypes/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/constants/aminoacid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/constants/codon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/constants/nucleotide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:50.668506 biodatatypes-0.2.1/biodatatypes/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48757 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/sequence/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:50.668506 biodatatypes-0.2.1/biodatatypes/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/unit/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/unit/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46240 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/biodatatypes/unit/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:36:50.664506 biodatatypes-0.2.1/biodatatypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-04 08:36:50.000000 biodatatypes-0.2.1/biodatatypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 08:36:50.000000 biodatatypes-0.2.1/biodatatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:36:50.000000 biodatatypes-0.2.1/biodatatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 08:36:50.000000 biodatatypes-0.2.1/biodatatypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:36:50.668506 biodatatypes-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 08:36:37.000000 biodatatypes-0.2.1/setup.py
```

### Comparing `biodatatypes-0.1.1/LICENSE` & `biodatatypes-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biodatatypes-0.1.1/biodatatypes/constants/aminoacid.py` & `biodatatypes-0.2.1/biodatatypes/constants/aminoacid.py`

 * *Files identical despite different names*

### Comparing `biodatatypes-0.1.1/biodatatypes/constants/codon.py` & `biodatatypes-0.2.1/biodatatypes/constants/codon.py`

 * *Files identical despite different names*

### Comparing `biodatatypes-0.1.1/biodatatypes/constants/nucleotide.py` & `biodatatypes-0.2.1/biodatatypes/constants/nucleotide.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+STANDARD_NUCLEOTIDES = ['A', 'C', 'G', 'T']
 FROM_NUCLEOTIDE_ONE_LETTER_TOKEN = {
     'A': 'A',
     'C': 'C',
     'G': 'G',
     'T': 'T',
     'U': 'T',
     '-': 'Gap',
@@ -36,15 +37,15 @@
     'M': 'M',
     'B': 'B',
     'D': 'D',
     'H': 'H',
     'V': 'V',
     'N': 'N',
 }
-DEGENERATE_NUCLEOTIDES = ['R', 'Y', 'S', 'W', 'K', 'M', 'B', 'D', 'H', 'V', 'N']
+AMBIGUOUS_NUCLEOTIDES = ['R', 'Y', 'S', 'W', 'K', 'M', 'B', 'D', 'H', 'V', 'N']
 COMPLEMENTARY_NUCLEOTIDES = {
     'A': 'T',
     'C': 'G',
     'G': 'C',
     'T': 'A',
     'U': 'A',
     'R': 'Y',
```

### Comparing `biodatatypes-0.1.1/biodatatypes/sequence/sequence.py` & `biodatatypes-0.2.1/biodatatypes/sequence/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Union, Optional, List, Any, Iterator, Iterable, cast
+from typing import Union, Optional, List, Any, Iterator, Iterable, cast, Type
 from collections.abc import Sequence
 
-from biodatatypes.units import BioToken, Nucleotide, AminoAcid, Codon
+from biodatatypes.unit.types import Nucleotide, AminoAcid, Codon
+from biodatatypes.unit.base import BioToken, NucleotideEnum, AminoAcidEnum, CodonEnum
 from biodatatypes.constants.nucleotide import COMPLEMENTARY_NUCLEOTIDES
 
 
 class BioSequence(Sequence):
     """
     A BioSequence is a generic sequence composed objects inheriting from the BioToken class
     such as Nucleotide, AminoAcid, or Codon. It is a wrapper around a list of BioTokens
@@ -23,23 +24,22 @@
     is_degenerate : bool
         Whether or not the sequence contains any ambiguous tokens.
     is_gapped : bool
         Whether or not the sequence contains any gap tokens.
     is_masked : bool
         Whether or not the sequence contains any mask tokens.
     
-    """
-    unit = BioToken
-    
+    """    
     def __init__(self, 
             sequence: Sequence[BioToken], 
             is_standard: Optional[bool] = None,
             is_ambiguous: Optional[bool] = None, 
             is_gapped: Optional[bool] = None, 
             is_masked: Optional[bool] = None):
+        self.unit = type(sequence[0])
         self._sequence = list(sequence)
         self._is_standard = is_standard
         self._is_degenerate = is_ambiguous
         self._is_gapped = is_gapped
         self._is_masked = is_masked
     
     def __getitem__(self, index: int) -> Any:
@@ -49,14 +49,22 @@
         return len(self.sequence)
     
     def __str__(self) -> str:
         return ''.join(list(map(str, self.sequence)))
     
     def __repr__(self) -> str:
         return self.__str__()
+    
+    # def __eq__(self, other: Union['BioSequence', str]) -> bool:
+    #     if isinstance(other, str):
+    #         return str(self) == other
+    #     elif isinstance(other, BioSequence):
+    #         return str(self) == str(other)
+    #     else:
+    #         return False
 
     @property
     def is_standard(self) -> bool:
         if self._is_standard is None:
             self._is_standard = all([s.is_standard() for s in self.sequence])
         return self._is_standard
     
@@ -65,58 +73,62 @@
         if self._is_degenerate is None:
             self._is_degenerate = any([s.is_ambiguous() for s in self.sequence])
         return self._is_degenerate
     
     @property
     def is_gapped(self) -> bool:
         if self._is_gapped is None:
-            self._is_gapped = any([s.is_gap() for s in self.sequence])
+            self._is_gapped = any([s.is_gap() for s in self.sequence])  # type: ignore
         return self._is_gapped
     
     @property
     def is_masked(self) -> bool:
         if self._is_masked is None:
-            self._is_masked = any([s.is_mask() for s in self.sequence])
+            self._is_masked = any([s.is_mask() for s in self.sequence])  # type: ignore
         return self._is_masked
     
     @property
     def sequence(self) -> Sequence[BioToken]:
         return self._sequence
     
     @classmethod
-    def from_str(cls, sequence: Iterable[str]) -> 'BioSequence':
+    def from_str(cls, 
+            sequence: Iterable[str],
+            unit: Type[BioToken] = BioToken) -> 'BioSequence':
         """Create an BioSequence from a string of tokens.
         
         Parameters
         ----------
         sequence : Iterable[str]
             A string or iterable of tokens.
             
         Returns
         -------
         NucleotideSequence
             An BioSequence object.
         """
-        return cls([cls.unit.from_str(s) for s in sequence])
+        return cls([unit.from_str(s) for s in sequence])
     
     @classmethod
-    def from_onehot(cls, sequence: Sequence[Sequence[int]]) -> 'BioSequence':
+    def from_onehot(cls, 
+            sequence: Sequence[Sequence[int]], 
+            unit: Type[BioToken] = BioToken) -> 'BioSequence':
         """Create an NucleotideSequence from a one-hot encoded sequence.
         
         Parameters
         ----------
         sequence : Sequence[Sequence[int]]
             A sequence of one-hot encoded tokens.
         
         Returns
         -------
         BioSequence
             A BioSequence object.
         """        
-        return cls([cls.unit.from_onehot(s) for s in sequence])
+        return cls([unit.from_onehot(s) for s in sequence])
     
     def to_str(self) -> str:
         """Return a string of amino acid tokens in one-letter code.
         
         Returns
         -------
         str
@@ -251,24 +263,14 @@
     def count_masked(self) -> int:
         """Return the number of masked positions.
         
         Returns
         -------
         int
             The number of masked positions.
-            
-        Examples
-        --------
-        >>> seq = AminoAcidSequence.from_str('ARNDCEQGHILKMFPSTWYV')
-        >>> seq.count_masked()
-        0
-        >>> seq.mask(0).count_masked()
-        1
-        >>> seq.mask([0, 1, -1]).count_masked()
-        3
         """
         return len(self.masked_positions())
 
     def gapped_positions(self) -> List[int]:
         """Return the positions that are gapped.
         
         Returns
@@ -295,37 +297,35 @@
 
 class NucleotideSequence(BioSequence):
     """
     A sequence of nucleotides.
     
     Parameters
     ----------
-    sequence : Sequence[Nucleotide]
+    sequence : Sequence[NucleotideEnum]
         A sequence of nucleotides as Nucleotide objects.
     is_standard : bool, optional
         Whether the sequence is standard (i.e. only contains standard nucleotides).
     is_ambiguous : bool, optional
         True if the sequence contains ambiguous nucleotides
     is_gapped : bool, optional
         True if the sequence is gapped (i.e. contains at least one gap).
     is_masked : bool, optional
         True if the sequence is masked (i.e. contains at least one the masked position).
-    """
-    unit = Nucleotide
-    
+    """    
     def __init__(self, 
-            sequence: Sequence[Nucleotide], 
+            sequence: Sequence[NucleotideEnum], 
             is_standard: Optional[bool] = None,
             is_ambiguous: Optional[bool] = None, 
             is_gapped: Optional[bool] = None, 
             is_masked: Optional[bool] = None):
         super().__init__(sequence, is_standard, is_ambiguous, is_gapped, is_masked)
         
     @classmethod
-    def from_str(cls, sequence: str) -> 'NucleotideSequence':
+    def from_str(cls, sequence: str, unit: Type = Nucleotide) -> 'NucleotideSequence':
         """Create an NucleotideSequence from a string of nucleotide tokens.
         
         Parameters
         ----------
         sequence : str
             A string of nucleotide tokens in one-letter code.
             
@@ -337,31 +337,31 @@
         Examples
         --------
         >>> NucleotideSequence.from_str('ATGCCGTATGAATGA')
         ATGCCGTATGAATGA
         >>> NucleotideSequence.from_str('ATG-A-CCGTATGAA---TGA')
         ATG-A-CCGTATGAA---TGA
         """
-        return cast(NucleotideSequence, super().from_str(sequence))
+        return cast(NucleotideSequence, super().from_str(sequence, unit))
     
     @classmethod
-    def from_onehot(cls, sequence: Sequence[Sequence[int]]) -> 'NucleotideSequence':
+    def from_onehot(cls, sequence: Sequence[Sequence[int]], unit: Type = Nucleotide) -> 'NucleotideSequence':
         """Create an NucleotideSequence from a one-hot encoded sequence.
         
         Parameters
         ----------
         sequence : Sequence[Sequence[int]]
             A sequence of one-hot encoded nucleotide tokens.
         
         Returns
         -------
         NucleotideSequence
             An NucleotideSequence object.
         """        
-        return cast(NucleotideSequence, super().from_onehot(sequence))
+        return cast(NucleotideSequence, super().from_onehot(sequence, unit))
     
     def to_str(self) -> str:
         """Return a string of nucleotide tokens in one-letter code.
         
         Returns
         -------
         str
@@ -377,78 +377,94 @@
         'ATG-A-CCGTATGAA---TGA'
         """
         return super().to_str()
         
     def to_onehot(self) -> Sequence[Sequence[int]]:
         return super().to_onehot()
     
-    def startswith(self, seq: Union[str, Sequence[Nucleotide], 'NucleotideSequence']) -> bool:
+    def startswith(self, seq: Union[str, Sequence[NucleotideEnum], 'NucleotideSequence']) -> bool:
         """Return True if the sequence starts with the given nucleotide or sequence.
         
         Parameters
         ----------
-        seq : Union[str, Sequence[Nucleotide]]
+        seq : Union[str, Sequence[NucleotideEnum]]
             A nucleotide or sequence of nucleotides.
         
         Returns
         -------
         bool
             True if the sequence starts with the given nucleotide or sequence, False otherwise.
             
         Examples
         --------
         >>> seq = NucleotideSequence.from_str('ATGCCGTATGAATGA')
         >>> seq.startswith('A')
         True
+        >>> seq.startswith([Nucleotide.A])
+        True
+        >>> other_seq = NucleotideSequence.from_str('A')
+        >>> seq.startswith(other_seq)
+        True
         >>> seq.startswith('ATG')
         True
+        >>> seq.startswith([Nucleotide.A, Nucleotide.T, Nucleotide.G])
+        True
         >>> seq.startswith('-')
         False
         >>> seq.startswith('A--')
         False
         """
         if isinstance(seq, str):
-            seq = NucleotideSequence.from_str(seq)
+            seq = cast(Sequence[NucleotideEnum], self.from_str(seq, self.unit).sequence)
+        elif isinstance(seq, self.__class__):
+            seq = cast(Sequence[NucleotideEnum], seq.sequence)
         return super().startswith(seq)
 
-    def endswith(self, seq: Union[str, Sequence[Nucleotide], 'NucleotideSequence']) -> bool:
+    def endswith(self, seq: Union[str, Sequence[NucleotideEnum], 'NucleotideSequence']) -> bool:
         """Return True if the sequence ends with the given nucleotide or sequence.
         
         Parameters
         ----------
-        seq : Union[str, Sequence[Nucleotide]]
+        seq : Union[str, Sequence[NucleotideEnum]]
             A nucleotide or sequence of nucleotides.
         
         Returns
         -------
         bool
             True if the sequence ends with the given nucleotide or sequence, False otherwise.
             
         Examples
         --------
         >>> seq = NucleotideSequence.from_str('ATGCCGTATGAATGA')
         >>> seq.endswith('A')
         True
+        >>> seq.endswith([Nucleotide.A])
+        True
+        >>> other_seq = NucleotideSequence.from_str('A')
+        >>> seq.endswith(other_seq)
+        True
         >>> seq.endswith('TGA')
         True
         >>> seq.endswith('-')
         False
         >>> seq.endswith('A--')
         False
         """
         if isinstance(seq, str):
-            seq = NucleotideSequence.from_str(seq)
+            seq = cast(Sequence[NucleotideEnum], self.from_str(seq, self.unit).sequence)
+        elif isinstance(seq, self.__class__):
+            seq = cast(Sequence[NucleotideEnum], seq.sequence)
         return super().endswith(seq)
 
-    def find(self, seq: Union[str, Sequence[Nucleotide], 'NucleotideSequence']) -> int:
+    def find(self, seq: Union[str, Sequence[NucleotideEnum], 'NucleotideSequence']) -> int:
         """Return the index of the first occurrence of the given nucleotide or sequence.
         
         Parameters
         ----------
-        seq : Union[str, Sequence[Nucleotide]]
+        seq : Union[str, Sequence[NucleotideEnum]]
             A nucleotide or sequence of nucleotides.
         
         Returns
         -------
         int
             The index of the first occurrence of the given nucleotide or sequence.
             
@@ -466,24 +482,24 @@
         >>> seq.find('A--')
         -1
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, NucleotideSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], Nucleotide):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], NucleotideEnum):
             seq = ''.join([str(n) for n in seq])
         return super().find(cast(str, seq))
 
-    def rfind(self, seq: Union[str, Sequence[Nucleotide], 'NucleotideSequence']) -> int:
+    def rfind(self, seq: Union[str, Sequence[NucleotideEnum], 'NucleotideSequence']) -> int:
         """Return the index of the last occurrence of the given nucleotide or sequence.
         
         Parameters
         ----------
-        seq : Union[str, Sequence[Nucleotide]]
+        seq : Union[str, Sequence[NucleotideEnum]]
             A nucleotide or sequence of nucleotides.
         
         Returns
         -------
         int
             The index of the last occurrence of the given nucleotide or sequence.
             
@@ -501,24 +517,24 @@
         >>> seq.rfind('A--')
         -1
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, NucleotideSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], Nucleotide):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], NucleotideEnum):
             seq = ''.join([str(n) for n in seq])
         return super().rfind(cast(str, seq))
 
-    def count(self, seq: Union[str, Sequence[Nucleotide], 'NucleotideSequence']) -> int:
+    def count(self, seq: Union[str, Sequence[NucleotideEnum], 'NucleotideSequence']) -> int:
         """Return the number of occurrences of the given nucleotide or sequence.
         
         Parameters
         ----------
-        nucl : Union[str, Sequence[Nucleotide]]
+        nucl : Union[str, Sequence[NucleotideEnum]]
             A nucleotide or sequence of nucleotides.
         
         Returns
         -------
         int
             The number of occurrences of the given nucleotide or sequence.
             
@@ -536,15 +552,15 @@
         >>> seq.count('A--')
         0
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, NucleotideSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], Nucleotide):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], NucleotideEnum):
             seq = ''.join([str(n) for n in seq])
         return super().count(cast(str, seq))
 
     def mask(self, positions: Union[int, Sequence[int]]) -> 'NucleotideSequence':
         """Return a copy of the sequence with the given positions masked.
         
         Parameters
@@ -633,37 +649,37 @@
         >>> gapped_seq.count_gaps()
         5
         """
         return super().count_gaps()
 
     # NucleotideSequence-specific methods
     
-    def to_reverse_complement(self) -> 'NucleotideSequence':
+    def to_reverse_complement(self, unit: Type = Nucleotide) -> 'NucleotideSequence':
         """Return the reverse complement of the sequence.
         
         Returns
         -------
         NucleotideSequence
             The reverse complement of the sequence.
             
         Examples
         --------
         >>> seq = NucleotideSequence.from_str('ATGCCGTATGAATGA')
         >>> seq.to_reverse_complement()
         TCATTCATACGGCAT
         """
-        rc_list = [cast(Nucleotide, s).to_complement() for s in self._sequence[::-1]]
-        return NucleotideSequence(
+        rc_list = [cast(unit, s).to_complement() for s in self._sequence[::-1]]
+        return self.__class__(
             rc_list, 
             self._is_standard, 
             self._is_degenerate, 
             self._is_gapped, 
             self._is_masked)
 
-    def to_codon_sequence(self) -> 'CodonSequence':
+    def to_codon_sequence(self, unit: Type = Codon) -> 'CodonSequence':
         """Return the sequence as a CodonSequence.
         
         Returns
         -------
         CodonSequence
             The sequence as a CodonSequence.
             
@@ -678,20 +694,19 @@
         ValueError: Cannot convert to CodonSequence. Sequence length must be a multiple of 3: 14
         >>> gapped_seq = NucleotideSequence.from_str('ATG---TATGAATGA')
         >>> gapped_seq.to_codon_sequence()
         ATG --- TAT GAA TGA
         >>> invalid_gapped_seq = NucleotideSequence.from_str('AT---CTATGAATGA')
         >>> invalid_gapped_seq.to_codon_sequence()
         Traceback (most recent call last):
-        ValueError: Invalid codon string: AT-
+        ValueError: Invalid nucleotide sequence triplet: [A, T, -]
         """
         if len(self) % 3 != 0:
             raise ValueError(f'Cannot convert to CodonSequence. Sequence length must be a multiple of 3: {len(self)}')
-        return CodonSequence.from_nucleotides(self)
-
+        return CodonSequence.from_nucleotides(self, unit)
 
 
 class AminoAcidSequence(BioSequence):
     """
     A sequence of amino acids.
     
     Parameters
@@ -702,27 +717,25 @@
         Whether the sequence is standard (i.e. only contains standard amino acids).
     is_ambiguous : bool, optional
         True if the sequence contains ambiguous nucleotides
     is_gapped : bool, optional
         True if the sequence is gapped (i.e. contains at least one gap).
     is_masked : bool, optional
         True if the sequence is masked (i.e. contains at least one the masked position).
-    """
-    unit = AminoAcid
-    
+    """    
     def __init__(self, 
-            sequence: Sequence[AminoAcid],
+            sequence: Sequence[AminoAcidEnum],
             is_standard: Optional[bool] = None,
             is_ambiguous: Optional[bool] = None, 
             is_gapped: Optional[bool] = None, 
             is_masked: Optional[bool] = None):
         super().__init__(sequence, is_standard, is_ambiguous, is_gapped, is_masked)
             
     @classmethod
-    def from_str(cls, sequence: str) -> 'AminoAcidSequence':
+    def from_str(cls, sequence: str, unit: Type = AminoAcid) -> 'AminoAcidSequence':
         """Create an AminoAcidSequence from a string of amino acid tokens.
         
         Parameters
         ----------
         sequence : str
             A string of amino acid tokens in one-letter code.
             
@@ -732,31 +745,31 @@
             An AminoAcidSequence object.
             
         Examples
         --------
         >>> AminoAcidSequence.from_str('ARNDCEQGHILKMFPSTWYV')
         ARNDCEQGHILKMFPSTWYV
         """
-        return cast(AminoAcidSequence, super().from_str(sequence))
+        return cast(AminoAcidSequence, super().from_str(sequence, unit))
     
     @classmethod
-    def from_onehot(cls, sequence: Sequence[Sequence[int]]) -> 'AminoAcidSequence':
+    def from_onehot(cls, sequence: Sequence[Sequence[int]], unit: Type = AminoAcid) -> 'AminoAcidSequence':
         """Create an AminoAcidSequence from a one-hot encoded sequence.
         
         Parameters
         ----------
         sequence : Sequence[Sequence[int]]
             A sequence of one-hot encoded amino acid tokens.
         
         Returns
         -------
         AminoAcidSequence
             An AminoAcidSequence object.
         """        
-        return cast(AminoAcidSequence, super().from_onehot(sequence))
+        return cast(AminoAcidSequence, super().from_onehot(sequence, unit))
     
     def to_str(self) -> str:
         """Return a string of amino acid tokens in one-letter code.
         
         Returns
         -------
         str
@@ -772,15 +785,15 @@
         'ARNDC--EQGHILKMFPSTWYV'
         """
         return super().to_str()
         
     def to_onehot(self) -> Sequence[Sequence[int]]:
         return super().to_onehot()
 
-    def startswith(self, seq: Union[str, Sequence[AminoAcid], 'AminoAcidSequence']) -> bool:
+    def startswith(self, seq: Union[str, Sequence[AminoAcidEnum], 'AminoAcidSequence']) -> bool:
         """Return True if the sequence starts with the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[AminoAcid], AminoAcidSequence]
             The sequence to check.
             
@@ -788,28 +801,35 @@
         -------
         bool
             True if the sequence starts with the given sequence.
             
         Examples
         --------
         >>> seq = AminoAcidSequence.from_str('ARNDCEQGHILKMFPSTWYV')
+        >>> seq.startswith('A')
+        True
+        >>> seq.startswith([AminoAcid.Ala])
+        True
         >>> seq.startswith('ARN')
         True
-        >>> seq.startswith('A')
+        >>> other_seq = AminoAcidSequence.from_str('ARN')
+        >>> seq.startswith(other_seq)
         True
         >>> seq.startswith('ARNDCEQGHILKMFPSTWYVX')
         False
         >>> seq.startswith('-')
         False
         """
         if isinstance(seq, str):
-            seq = AminoAcidSequence.from_str(seq)
+            seq = cast(Sequence[AminoAcidEnum], self.from_str(seq, self.unit).sequence)
+        elif isinstance(seq, self.__class__):
+            seq = cast(Sequence[AminoAcidEnum], seq.sequence)
         return super().startswith(seq)
 
-    def endswith(self, seq: Union[str, Sequence[AminoAcid], 'AminoAcidSequence']) -> bool:
+    def endswith(self, seq: Union[str, Sequence[AminoAcidEnum], 'AminoAcidSequence']) -> bool:
         """Return True if the sequence ends with the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[AminoAcid], AminoAcidSequence]
             The sequence to check.
             
@@ -819,26 +839,33 @@
             True if the sequence ends with the given sequence.
             
         Examples
         --------
         >>> seq = AminoAcidSequence.from_str('ARNDCEQGHILKMFPSTWYV')
         >>> seq.endswith('V')
         True
+        >>> seq.endswith([AminoAcid.Val])
+        True
         >>> seq.endswith('WYV')
         True
+        >>> other_seq = AminoAcidSequence.from_str('WYV')
+        >>> seq.endswith(other_seq)
+        True
         >>> seq.endswith('ARNDC--EQGHILKMFPSTWYV')
         False
         >>> seq.endswith('-')
         False
         """
         if isinstance(seq, str):
-            seq = AminoAcidSequence.from_str(seq)
+            seq = cast(Sequence[AminoAcidEnum], self.from_str(seq, self.unit).sequence)
+        elif isinstance(seq, self.__class__):
+            seq = cast(Sequence[AminoAcidEnum], seq.sequence)
         return super().endswith(seq)
 
-    def find(self, seq: Union[str, Sequence[AminoAcid], 'AminoAcidSequence']) -> int:
+    def find(self, seq: Union[str, Sequence[AminoAcidEnum], 'AminoAcidSequence']) -> int:
         """Return the index of the first occurrence of the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[AminoAcid], AminoAcidSequence]
             The sequence to find.
             
@@ -861,19 +888,19 @@
         >>> seq.find('X')
         -1
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, AminoAcidSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], AminoAcid):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], AminoAcidEnum):
             seq = ''.join([str(s) for s in seq])
         return super().find(cast(str, seq))
 
-    def rfind(self, seq: Union[str, Sequence[AminoAcid], 'AminoAcidSequence']) -> int:
+    def rfind(self, seq: Union[str, Sequence[AminoAcidEnum], 'AminoAcidSequence']) -> int:
         """Return the index of the last occurrence of the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[AminoAcid], AminoAcidSequence]
             The sequence to find.
             
@@ -898,19 +925,19 @@
         >>> seq.rfind('X')
         -1
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, AminoAcidSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], AminoAcid):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], AminoAcidEnum):
             seq = ''.join([str(s) for s in seq])
         return super().rfind(cast(str, seq))
     
-    def count(self, seq: Union[str, Sequence[AminoAcid], 'AminoAcidSequence']) -> int:
+    def count(self, seq: Union[str, Sequence[AminoAcidEnum], 'AminoAcidSequence']) -> int:
         """Return the number of occurrences of the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[AminoAcid], AminoAcidSequence]
             The sequence to count.
             
@@ -933,15 +960,15 @@
         >>> seq.count('X')
         0
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, AminoAcidSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], AminoAcid):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], AminoAcidEnum):
             seq = ''.join([str(s) for s in seq])
         return super().count(cast(str, seq))
     
     def mask(self, positions: Union[int, Sequence[int]]) -> 'AminoAcidSequence':
         """Return a new sequence with the given positions masked.
         
         Parameters
@@ -1055,33 +1082,31 @@
     is_ambiguous : bool, optional
         True if the sequence contains ambiguous codons.
     is_gapped : bool, optional
         True if the sequence is gapped (i.e. contains at least one gap).
     is_masked : bool, optional
         True if the sequence is masked (i.e. contains at least one the masked position).
     """
-    unit = Codon
-
     def __init__(self, 
-            sequence: Sequence[Codon],
+            sequence: Sequence[CodonEnum],
             is_standard: Optional[bool] = None,
             is_ambiguous: Optional[bool] = None, 
             is_gapped: Optional[bool] = None, 
             is_masked: Optional[bool] = None):
         super().__init__(sequence, is_standard, is_ambiguous, is_gapped, is_masked)
 
     def __repr__(self) -> str:
         return ' '.join([str(c) for c in self._sequence])
     
     @staticmethod
     def unit_iterator(sequence) -> Iterator:
         return (sequence[i:i+3] for i in range(0, len(sequence), 3))
     
     @classmethod
-    def from_str(cls, sequence: str) -> 'CodonSequence':
+    def from_str(cls, sequence: str, unit: Type = Codon) -> 'CodonSequence':
         """Create a CodonSequence from a string of triplet nucleotides
         
         Parameters
         ----------
         sequence : str
             The string of triplet nucleotides.
             
@@ -1093,33 +1118,35 @@
         Examples
         --------
         >>> CodonSequence.from_str('ATGAAATAG')
         ATG AAA TAG
         """
         if len(sequence) % 3 != 0:
             raise ValueError('Sequence length must be a multiple of 3')
-        return cast(CodonSequence, super().from_str(cls.unit_iterator(sequence)))
+        return cast(CodonSequence, 
+                    super().from_str(cls.unit_iterator(sequence), unit))
 
     @classmethod
-    def from_onehot(cls, sequence: Sequence[Sequence[int]]) -> 'CodonSequence':
+    def from_onehot(cls, sequence: Sequence[Sequence[int]], unit: Type = Codon) -> 'CodonSequence':
         """Create a CodonSequence from a one-hot encoded sequence.
         
         Parameters
         ----------
         sequence : Sequence[Sequence[int]]
             The one-hot encoded sequence.
             
         Returns
         -------
         CodonSequence
             The CodonSequence.
         """
-        return cast(CodonSequence, super().from_onehot(sequence))
+        return cast(CodonSequence, 
+                    super().from_onehot(sequence, unit))
 
-    def startswith(self, seq: Union[str, Sequence[Codon], 'CodonSequence']) -> bool:
+    def startswith(self, seq: Union[str, Sequence[CodonEnum], 'CodonSequence']) -> bool:
         """Return True if the sequence starts with the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[Codon], CodonSequence]
             The sequence to check.
             
@@ -1129,24 +1156,32 @@
             True if the sequence starts with the given sequence.
             
         Examples
         --------
         >>> seq = CodonSequence.from_str('ATGAAATAG')
         >>> seq.startswith('ATG')
         True
+        >>> seq.startswith([Codon.ATG])
+        True
         >>> seq.startswith(CodonSequence([Codon.ATG]))
         True
         >>> seq.startswith('ATGAAA')
         True
+        >>> seq.startswith('ATGAAATAGTTT')
+        False
+        >>> seq.startswith('TGA')
+        False
         """
         if isinstance(seq, str):
-            seq = CodonSequence.from_str(seq)
+            seq = cast(Sequence[CodonEnum], self.from_str(seq, self.unit).sequence)
+        elif isinstance(seq, self.__class__):
+            seq = cast(Sequence[CodonEnum], seq.sequence)
         return super().startswith(seq)
 
-    def endswith(self, seq: Union[str, Sequence[Codon], 'CodonSequence']) -> bool:
+    def endswith(self, seq: Union[str, Sequence[CodonEnum], 'CodonSequence']) -> bool:
         """Return True if the sequence ends with the given sequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[Codon], CodonSequence]
             The sequence to check.
             
@@ -1156,24 +1191,32 @@
             True if the sequence ends with the given sequence.
             
         Examples
         --------
         >>> seq = CodonSequence.from_str('ATGAAATAG')
         >>> seq.endswith('TAG')
         True
+        >>> seq.endswith([Codon.TAG])
+        True
         >>> seq.endswith(CodonSequence([Codon.TAG]))
         True
         >>> seq.endswith('AAATAG')
         True
+        >>> seq.endswith('TTTATGAAATAG')
+        False
+        >>> seq.endswith('TGA')
+        False
         """
         if isinstance(seq, str):
-            seq = CodonSequence.from_str(seq)
+            seq = cast(Sequence[CodonEnum], self.from_str(seq, self.unit).sequence)
+        elif isinstance(seq, self.__class__):
+            seq = cast(Sequence[CodonEnum], seq.sequence)
         return super().endswith(seq)
     
-    def find(self, seq: Union[str, Sequence[Codon], 'CodonSequence']) -> int:
+    def find(self, seq: Union[str, Sequence[CodonEnum], 'CodonSequence']) -> int:
         """Return the lowest index in the sequence where the given subsequence is found.
         
         Parameters
         ----------
         seq : Union[str, Sequence[Codon], CodonSequence]
             The sequence to find.
             
@@ -1194,19 +1237,19 @@
         >>> seq.find('TAG')
         3
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, CodonSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], Codon):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], CodonEnum):
             seq = ''.join([str(s) for s in seq])
         return super().find(cast(str, seq)) // 3
         
-    def rfind(self, seq: Union[str, Sequence[Codon], 'CodonSequence']) -> int:
+    def rfind(self, seq: Union[str, Sequence[CodonEnum], 'CodonSequence']) -> int:
         """Return the highest index in the sequence where the given subsequence is found.
         
         Parameters
         ----------
         seq : Union[str, Sequence[Codon], CodonSequence]
             The sequence to find.
             
@@ -1227,19 +1270,19 @@
         >>> seq.find('TAG')
         3
         """
         if isinstance(seq, str):
             pass
         elif isinstance(seq, CodonSequence):
             seq = str(seq)
-        elif isinstance(seq, Sequence) and isinstance(seq[0], Codon):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], CodonEnum):
             seq = ''.join([str(s) for s in seq])
         return super().rfind(cast(str, seq)) // 3
 
-    def count(self, seq: Union[str, Sequence[Codon], 'CodonSequence']) -> int:
+    def count(self, seq: Union[str, Sequence[CodonEnum], 'CodonSequence']) -> int:
         """Return the number of non-overlapping occurrences of the given subsequence.
         
         Parameters
         ----------
         seq : Union[str, Sequence[Codon], CodonSequence]
             The sequence to count.
             
@@ -1260,15 +1303,15 @@
         """
         if isinstance(seq, str):
             if len(seq) == 0:
                 return len(self) + 1
             seq = CodonSequence.from_str(seq)
         elif isinstance(seq, CodonSequence):
             pass
-        elif isinstance(seq, Sequence) and isinstance(seq[0], Codon):
+        elif isinstance(seq, Sequence) and isinstance(seq[0], CodonEnum):
             seq = CodonSequence(seq)
         seq = cast(CodonSequence, seq)
         return sum(self.sequence[i:i+len(seq)] == seq.sequence
                    for i in range(0, len(self)-len(seq)+1))
 
     def mask(self, positions: Union[int, Sequence[int]]) -> 'CodonSequence':
         """Return a new sequence with the given positions masked.
@@ -1371,20 +1414,22 @@
         2
         """
         return super().count_gaps()
 
     # CodonSequence-specific methods
 
     @classmethod
-    def from_nucleotides(cls, sequence: Sequence[Nucleotide]) -> 'CodonSequence':
+    def from_nucleotides(cls, 
+            sequence: Sequence[NucleotideEnum], 
+            unit: Type = Codon) -> 'CodonSequence':
         """Create a CodonSequence from a NucleotideSequence.
         
         Parameters
         ----------
-        sequence : Sequence[Nucleotide]
+        sequence : Sequence[NucleotideEnum]
             Sequence of Nucleotide objects.
             
         Returns
         -------
         CodonSequence
             The CodonSequence.
             
@@ -1392,34 +1437,36 @@
         --------
         >>> seq = [Nucleotide.A, Nucleotide.T, Nucleotide.G, Nucleotide.A, Nucleotide.A, Nucleotide.A, Nucleotide.T, Nucleotide.A, Nucleotide.G]
         >>> CodonSequence.from_nucleotides(seq)
         ATG AAA TAG
         """
         if len(sequence) % 3 != 0:
             raise ValueError('Sequence length must be a multiple of 3')
-        return cls([Codon.from_nucleotides(s) for s in cls.unit_iterator(sequence)])
+        return cls([unit.from_nucleotides(s) for s in cls.unit_iterator(sequence)])
 
     @classmethod
-    def from_nucleotide_onehot(cls, sequence: Sequence[Sequence[int]]) -> 'CodonSequence':
+    def from_nucleotide_onehot(cls, 
+            sequence: Sequence[Sequence[int]], 
+            unit: Type = Codon) -> 'CodonSequence':
         """Create a CodonSequence from seqeunce of Nucleotide one-hot vectors.
         
         Parameters
         ----------
         sequence : Sequence[Sequence[int]]
             The one-hot encoded sequence.
             
         Returns
         -------
         CodonSequence
             The CodonSequence.
         """
         if len(sequence) % 3 != 0:
             raise ValueError('Sequence length must be a multiple of 3')
-        nucl_sequence = [Nucleotide.from_onehot(s) for s in sequence]
-        return cls([Codon.from_nucleotides(s) for s in cls.unit_iterator(nucl_sequence)])
+        nucl_sequence = [NucleotideEnum.from_onehot(s) for s in sequence]
+        return cls([unit.from_nucleotides(s) for s in cls.unit_iterator(nucl_sequence)])
 
     def translate(self) -> AminoAcidSequence:
         """Return the amino acid sequence translated from the codon sequence.
         
         Returns
         -------
         AminoAcidSequence
@@ -1433,15 +1480,15 @@
         >>> gapped_seq = CodonSequence.from_str('ATGAAA---AAATAG')
         >>> gapped_seq.translate()
         MK-K*
         >>> masked_seq = CodonSequence.from_str('ATGAAA###AAATAG')
         >>> masked_seq.translate()
         MK#K*
         """
-        return AminoAcidSequence([cast(Codon, c).translate() for c in self._sequence])
+        return AminoAcidSequence([c.translate() for c in self._sequence])  # type: ignore
 
     def to_reverse_complement(self) -> 'CodonSequence':
         """Return the reverse complement of the sequence.
         
         Returns
         -------
         NucleotideSequence
@@ -1458,18 +1505,18 @@
         >>> rc_rc
         ATG CCG TAT GAA TGA
         >>> str_seq == str(rc_rc)
         True
         """
         rc_nucl_str_list = [COMPLEMENTARY_NUCLEOTIDES[s] for s in str(self)[::-1]]
         rc_list = [
-            Codon.from_str(''.join(rc_nucl_str_list[i:i+3])) 
+            self.unit.from_str(''.join(rc_nucl_str_list[i:i+3])) 
             for i in range(0, len(rc_nucl_str_list), 3)]
         return CodonSequence(
-            rc_list, 
+            rc_list,  # type: ignore
             self._is_standard, 
             self._is_degenerate, 
             self._is_gapped, 
             self._is_masked)
     
     def to_amino_acid_sequence(self) -> 'AminoAcidSequence':
         """Translates the codon sequence to an amino acid sequence.
```

### Comparing `biodatatypes-0.1.1/biodatatypes/units.py` & `biodatatypes-0.2.1/biodatatypes/unit/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,58 @@
-from typing import Any
+from typing import cast, Type
 from collections.abc import Sequence
-from enum import Enum
 
 from biodatatypes.constants.nucleotide import *
 from biodatatypes.constants.aminoacid import *
 from biodatatypes.constants.codon import *
+from biodatatypes.unit.base import (
+    NucleotideEnum, 
+    AminoAcidEnum, 
+    CodonEnum,
+)
+from biodatatypes.unit.mixins import SpecialTokenMixin
 
 
-class BioToken(Enum):
-    """Base class for all biological sequence unit tokens as Enum members.
-
-    This subclasses the Enum datatype but does not define any members.
-    This class is intended to be subclassed for each type of unit token: 
-    Nucleotide, AminoAcid, Codon. 
-    Each subclass should define its own set of tokens as class attributes. 
-    
-    Attributes
-    ----------
-    name : str
-        The name of the token. This is used to identify the token and may be also be its string representations.
-        
-        Standard tokens should be named after their string representation.
-        Special tokens like those representing a gap, mask, or other are always named 'Gap', 'Mask', and 'Other' respectively.
-        
-    value : int
-        The integer value of the token. This is used for indexing into
-        onehot vectors.
-        
-        Gap tokens are always assigned the value 0.
-        Standard tokens are always assigned the values from 1 to n.
-        Special tokens are always assigned the the highest values, and the Mask token is always assigned the highest value.
-    """
-    def __repr__(self) -> str:
-        return self.__str__()
-    
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, BioToken):
-            return self.value == other.value
-        elif isinstance(other, str):
-            return str(self) == other
-        else:
-            return False
-    
-    def __hash__(self) -> int:
-        return hash(str(self))
-    
-    def __str__(self) -> str:
-        ...
-        
-    # Factory methods
-    
-    @classmethod
-    def from_str(cls, s: str) -> 'BioToken':
-        ...
-    
-    @classmethod
-    def from_int(cls, i: int) -> 'BioToken':
-        try:
-            return cls(i)
-        except ValueError:
-            raise ValueError(f'Invalid index value for {cls.__name__}: {i}')
-    
-    @classmethod
-    def from_onehot(cls, onehot:Sequence[int]) -> 'BioToken':
-        if (len(onehot) != len(cls)) or (sum(onehot) != 1):
-            raise ValueError(f'Invalid onehot vector for {cls.__name__}: {onehot}')
-        try:
-            return cls(onehot.index(1))
-        except ValueError:
-            raise ValueError(f'Invalid onehot vector for {cls.__name__}: {onehot}')
-        
-    # Conversion methods
-    
-    def to_onehot(self) -> Sequence[int]:
-        onehot = [0] * len(self.__class__)
-        onehot[self.value] = 1
-        return onehot
-        
-    def to_int(self) -> int:
-        return self.value
-        
-    # Token type methods
-    
-    def is_standard(self) -> bool:
-        ...
-        
-    def is_mask(self) -> bool:
-        return self == self.Mask
-        
-    def is_gap(self) -> bool:
-        return self == self.Gap
-    
-    def is_other(self) -> bool:
-        return self == self.Other
-        
-    def is_special(self) -> bool:
-        return self.is_mask() or self.is_gap() or self.is_other()
-        
-    def is_any(self) -> bool:
-        ...
-        
-    def is_ambiguous(self) -> bool:
-        ...
-
-
-class Nucleotide(BioToken):
+class Nucleotide(SpecialTokenMixin, NucleotideEnum):
     """A nucleotide token.
     
     Attributes
     ----------
     name : str
         The name of the token. This is used to identify the token and may be also be its string representations.
     value : int
         The integer value of the token. This is used for indexing into onehot vectors.
     """
+    #region Nucleotide tokens
     A = 1
     C = 2
     G = 3
     T = 4
-    # Non-standard symbols
     U = 5
-    # Degenerate symbols
     R = 6  # A or G, purine
     Y = 7 # C or T, pyrimidine
     S = 8  # G or C, strong
     W = 9  # A or T, weak
     K = 10  # G or T, keto
     M = 11  # A or C, amino
     B = 12  # C or G or T, not A
     D = 13  # A or G or T, not C
     H = 14  # A or C or T, not G
     V = 15  # A or C or G, not T
     N = 16  # A or C or G or T, any
-    # Special tokens
     Gap = 0  # Gap, -
     Other = 17  # Other unspecified but valid character, @
     Mask = 18  # Masked, #
+    #endregion
 
-    def __str__(self) -> str:
-        return TO_NUCLEOTIDE_ONE_LETTER_TOKEN[self.name]
-
-    # Factory methods
+    #region Override methods from NuclotideEnum
     
+    # Factory methods
     @classmethod
-    def from_str(cls, s: str) -> 'Nucleotide':
+    def from_str(cls, s: str) -> 'NucleotideEnum':
         """Convert a string to a Nucleotide.
         
         Parameters
         ----------
         s : str
             A string representing a nucleotide.
             
@@ -171,21 +76,18 @@
         -
         >>> Nucleotide.from_str('N')
         N
         >>> Nucleotide.from_str('X')
         Traceback (most recent call last):
         ValueError: Invalid nucleotide: X
         """
-        try:
-            return cls[FROM_NUCLEOTIDE_ONE_LETTER_TOKEN[s.upper()]]
-        except KeyError:
-            raise ValueError(f'Invalid nucleotide: {s}')
+        return super().from_str(s)
 
     @classmethod
-    def from_int(cls, i: int) -> 'Nucleotide':
+    def from_int(cls, i: int) -> 'NucleotideEnum':
         """Convert an integer to a Nucleotide.
         
         Parameters
         ----------
         i : int
             An integer representing a nucleotide.
             
@@ -210,15 +112,15 @@
         >>> Nucleotide.from_int(19)
         Traceback (most recent call last):
         ValueError: Invalid index value for Nucleotide: 19
         """
         return super().from_int(i)
 
     @classmethod
-    def from_onehot(cls, onehot:Sequence[int]) -> 'Nucleotide':
+    def from_onehot(cls, onehot:Sequence[int]) -> 'NucleotideEnum':
         """Convert a onehot encoding to a Nucleotide.
         
         Parameters
         ----------
         onehot : Sequence[int]
             A onehot encoding of a nucleotide.
             
@@ -242,17 +144,17 @@
         Traceback (most recent call last):
         ValueError: Invalid onehot vector for Nucleotide: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         >>> Nucleotide.from_onehot([1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1])
         Traceback (most recent call last):
         ValueError: Invalid onehot vector for Nucleotide: [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1]
         """
         return super().from_onehot(onehot)
-
-    # Conversion methods
     
+    # Conversion methods
+
     def to_onehot(self) -> Sequence[int]:
         """Convert a Nucleotide to a onehot encoding.
         
         Returns
         -------
         Sequence[int]
             A onehot encoding of the nucleotide.
@@ -282,38 +184,16 @@
         1
         >>> Nucleotide.Gap.to_int()
         0
         >>> Nucleotide.N.to_int()
         16
         """
         return super().to_int()
-    
-    # Nucleotide-only conversions
-    
-    def to_complement(self) -> 'Nucleotide':
-        """Convert a Nucleotide to its complement.
-        
-        Returns
-        -------
-        Nucleotide
-            The complement of the nucleotide.
-            
-        Examples
-        --------
-        >>> Nucleotide.A.to_complement()
-        T
-        >>> Nucleotide.Gap.to_complement()
-        -
-        >>> Nucleotide.N.to_complement()
-        N
-        """
-        complement_str = COMPLEMENTARY_NUCLEOTIDES[self.name]
-        return Nucleotide[complement_str]
-    
-    # Token type methods
+
+    # Propeties
 
     def is_standard(self):
         """Return True if the nucleotide is a standard nucleotide.
 
         Returns
         -------
         bool
@@ -326,133 +206,27 @@
         Examples
         --------
         >>> Nucleotide.A.is_standard()
         True
         >>> Nucleotide.Gap.is_standard()
         False
         """
-        return self.name in ['A', 'C', 'G', 'T']
+        return super().is_standard()
 
-    def is_mask(self):
-        """Return True if the nucleotide is masked.
-        
-        Returns
-        -------
-        bool
-            True if the nucleotide is masked, False otherwise.
-        
-        See Also
-        --------
-        is_special : Checks if it is a special token
-        
-        Examples
-        --------
-        >>> Nucleotide.Mask.is_mask()
-        True
-        >>> Nucleotide.A.is_mask()
-        False
-        >>> Nucleotide.Gap.is_mask()
-        False
-        """
-        return super().is_mask()
-    
-    def is_gap(self):
-        """Return True if the nucleotide is a gap.
-        
-        Returns
-        -------
-        bool
-            True if the nucleotide is a gap, False otherwise.
-        
-        See Also
-        --------
-        is_special : Checks if it is a special token
-        
-        Examples
-        --------
-        >>> Nucleotide.Gap.is_gap()
-        True
-        >>> Nucleotide.A.is_gap()
-        False
-        >>> Nucleotide.Mask.is_gap()
-        False
-        """
-        return super().is_gap()
-    
-    def is_other(self):
-        """Return True if the nucleotide is a valid character but is not specified
-        in the enumeration.
-        
-        Returns
-        -------
-        bool
-            True if the nucleotide is an unspecified but valid character, False otherwise.
-            
-        See Also
-        --------
-        is_special : Checks if it is a special token
-        
-        Examples
-        --------
-        >>> Nucleotide.Other.is_other()
-        True
-        >>> Nucleotide.A.is_other()
-        False
-        >>> Nucleotide.N.is_other()
-        False
-        >>> Nucleotide.Gap.is_other()
-        False
-        """
-        return super().is_other()
-
-    def is_special(self):
-        """Return True if it represents a special sequence.
-        
-        Returns
-        -------
-        bool
-            True if the nucleotide token represents a gap, mask or special character.
-        
-        See Also
-        --------
-        is_masked : Checks if it is a masked token
-        is_gap : Checks if it is a gap token
-        
-        Examples
-        --------
-        >>> gap = Nucleotide.Gap
-        >>> gap.is_special()
-        True
-        >>> mask = Nucleotide.Mask
-        >>> mask.is_special()
-        True
-        >>> other = Nucleotide.Other
-        >>> other.is_special()
-        True
-        >>> a = Nucleotide.A
-        >>> a.is_special()
-        False
-        >>> n = Nucleotide.N
-        >>> n.is_special()
-        False
-        """
-        return super().is_special()
-    
     def is_any(self):
         """Return True if it represents any nucleotide.
         
         Returns
         -------
         bool
             True if the nucleotide token represents any nucleotide.
         
         See Also
         --------
         is_ambiguous : Checks if it is an ambiguous token
-        is_degenerate : Checks if it is a degenerate token
         
         Examples
         --------
         >>> n = Nucleotide['N']
         >>> n.is_any()
         True
         >>> gap = Nucleotide['Gap']
@@ -461,46 +235,47 @@
         >>> mask = Nucleotide['Mask']
         >>> mask.is_any()
         False
         >>> a = Nucleotide['A']
         >>> a.is_any()
         False
         """
-        return self.name == 'N'
-   
+        return super().is_any()
+    
     def is_ambiguous(self):
         """Return True if it represents an ambiguous nucleotide.
         
+        Subclasses should override this method to check if the token represents
+        an ambiguous nucleotide.
+        
         Returns
         -------
         bool
             True if the nucleotide token represents an ambiguous nucleotide.
         
         See Also
         --------
-        is_degenerate : Checks if it is a degenerate token
+        is_any : Checks if the token represents any nucleotide
         
         Examples
         --------
         >>> Nucleotide['N'].is_ambiguous()
         True
         >>> Nucleotide['R'].is_ambiguous()
         True
         >>> Nucleotide['Gap'].is_ambiguous()
         False
         >>> Nucleotide['Mask'].is_ambiguous()
         False
         >>> Nucleotide['A'].is_ambiguous()
         False
         """
-        return self.name in DEGENERATE_NUCLEOTIDES
+        return super().is_ambiguous()
  
-    # Properties
-    
-    def is_purine(self):
+    def is_purine(self) -> bool:
         """Return True if the nucleotide is a purine.
         
         Returns
         -------
         bool
             True if the nucleotide is a purine, False otherwise.
             
@@ -515,17 +290,17 @@
         >>> Nucleotide['C'].is_purine()
         False
         >>> Nucleotide['N'].is_purine()
         False
         >>> Nucleotide['Gap'].is_purine()
         False
         """
-        return self == Nucleotide.A or self == Nucleotide.G or self == Nucleotide.R
+        return super().is_purine() or self.name == 'R'
 
-    def is_pyrimidine(self):
+    def is_pyrimidine(self) -> bool:
         """Return True if the nucleotide is a pyrimidine.
         
         Returns
         -------
         bool
             True if the nucleotide is a pyrimidine, False otherwise.
             
@@ -540,17 +315,17 @@
         >>> Nucleotide['A'].is_pyrimidine()
         False
         >>> Nucleotide['N'].is_pyrimidine()
         False
         >>> Nucleotide['Gap'].is_pyrimidine()
         False
         """
-        return self == Nucleotide.C or self == Nucleotide.T or self == Nucleotide.Y
+        return super().is_pyrimidine() or self.name == 'U' or self.name == 'Y'
 
-    def is_strong(self):
+    def is_strong(self) -> bool:
         """Return True if the nucleotide is a nucleotide involved in strong triple H-bond interaction.
         
         Returns
         -------
         bool
             True if the nucleotide is C or G, False otherwise.
             
@@ -565,17 +340,17 @@
         >>> Nucleotide['A'].is_strong()
         False
         >>> Nucleotide['N'].is_strong()
         False
         >>> Nucleotide['Gap'].is_strong()
         False
         """
-        return self == Nucleotide.G or self == Nucleotide.C or self == Nucleotide.S
+        return super().is_strong() or self.name == 'S'
 
-    def is_weak(self):
+    def is_weak(self) -> bool:
         """Return True if the nucleotide is a nucleotide involved in weak double H-bond interaction.
         
         Returns
         -------
         bool
             True if the nucleotide is A or T, False otherwise.
         
@@ -590,24 +365,113 @@
         >>> Nucleotide['C'].is_weak()
         False
         >>> Nucleotide['N'].is_weak()
         False
         >>> Nucleotide['Gap'].is_weak()
         False
         """
-        return self == Nucleotide.A or self == Nucleotide.T or self == Nucleotide.W
+        return super().is_weak() or self.name == 'W'
+
+    def is_amino(self) -> bool:
+        return super().is_amino() or self.name == 'M'
 
-    def is_amino(self):
-        return self == Nucleotide.A or self == Nucleotide.C or self == Nucleotide.M
+    def is_keto(self) -> bool:
+        return super().is_keto() or self.name == 'K'
+    
+ 
+    #endregion
+    
+    #region Override methods from SpecialTokenMixin
+    
+    def is_mask(self) -> bool:
+        """Return True if the token is a mask token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a mask token, False otherwise.
+        
+        Examples
+        --------
+        >>> Nucleotide.Mask.is_mask()
+        True
+        >>> Nucleotide.A.is_mask()
+        False
+        >>> Nucleotide.Gap.is_mask()
+        False
+        """
+        return super().is_mask()
 
-    def is_keto(self):
-        return self == Nucleotide.G or self == Nucleotide.T or self == Nucleotide.K
+    def is_gap(self) -> bool:
+        """Return True if the token is a gap token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a gap token, False otherwise.
+            
+        Examples
+        --------
+        >>> Nucleotide.Gap.is_gap()
+        True
+        >>> Nucleotide.A.is_gap()
+        False
+        >>> Nucleotide.Mask.is_gap()
+        False
+        """
+        return super().is_gap()
+    
+    def is_other(self) -> bool:
+        """Return True if the token is a valid but unspecified amino acid token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a valid but unspecified amino acid token, False otherwise.
+            
+        Examples
+        --------
+        >>> Nucleotide.Other.is_other()
+        True
+        >>> Nucleotide.A.is_other()
+        False
+        >>> Nucleotide.Mask.is_other()
+        False
+        >>> Nucleotide.Gap.is_other()
+        False
+        """
+        return super().is_other()
+    
+    def is_special(self) -> bool:
+        """Return True if the token is a mask, gap, or other token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a mask, gap, or other token, False otherwise.
+         
+        Examples
+        --------
+        >>> Nucleotide.Mask.is_special()
+        True
+        >>> Nucleotide.Gap.is_special()
+        True
+        >>> Nucleotide.Other.is_special()
+        True
+        >>> Nucleotide.A.is_special()
+        False
+        """
+        return super().is_special()
+    
+        # Factory methods unique to Codon
+    
+    #endregion
 
 
-class AminoAcid(BioToken):
+class AminoAcid(SpecialTokenMixin, AminoAcidEnum):
     """Amino acid tokens.
     
     Attributes
     ----------
     name : str
         The name of the amino acid in three-letter code.
         
@@ -619,14 +483,15 @@
         The integer value of the amino acid.
         
         Standard amino acids are assigned values from 1 to 20.
         Sec and Pyl are assigned values 21 and 22, respectively.
         Ambiguous amino acids are assigned values 23 to 26.
         Special non-amino acid tokens are assigned values 0, and 27 to 29 inclusive.
     """
+    #region Token enum
     Ala = 1
     Arg = 2
     Asn = 3
     Asp = 4
     Cys = 5
     Glu = 6
     Gln = 7
@@ -639,45 +504,43 @@
     Phe = 14
     Pro = 15
     Ser = 16
     Thr = 17
     Trp = 18
     Tyr = 19
     Val = 20
-    # Non-standard amino acids
-    Sec = 21  # Selenocysteine, U
-    Pyl = 22  # Pyrrolysine, O
-    # Ambiguous amino acids
+    Sec = 21
+    Pyl = 22
     Asx = 23  # Asn or Asp, B
     Glx = 24  # Gln or Glu, Z
     Xle = 25  # Leu or Ile, J
     Xaa = 26  # Unknown or Ambiguous, X
-    # Special tokens
     Gap = 0  # Gap, -
     Stop = 27 # Terminator, *
     Other = 28  # Other unspecified but valid character, @
     Mask = 29  # Masked, ?
+    #endregion
     
-    def __str__(self) -> str:
-        return NAME_TO_AMINO_ACID_ONE_LETTER_TOKEN[self.value]
+    #region Override methods from AminoAcidEnum
     
+    # Factory methods
     @classmethod
-    def from_str(cls, s: str) -> 'AminoAcid':
-        """Convert a string to an AminoAcid object.
+    def from_str(cls, s: str) -> 'AminoAcidEnum':
+        """Convert a string to an AminoAcidEnum object.
         
         Parameters
         ----------
         s : str
             A string representing an amino acid. It can be a one-letter code or
             a three-letter code.
 
         Returns
         -------
-        AminoAcid
-            An AminoAcid object.
+        AminoAcidEnum
+            An AminoAcidEnum object.
             
         Raises
         ------
         ValueError
             If the string is not a valid amino acid.
             
         Examples
@@ -688,34 +551,29 @@
         A
         >>> AminoAcid.from_str('gap')
         -
         >>> AminoAcid.from_str('!')
         Traceback (most recent call last):
         ValueError: Invalid one-letter code: !
         """
-        if len(s) == 1:
-            return cls.from_one_letter(s)
-        elif len(s) == 3:
-            return cls.from_three_letter(s)
-        else:
-            raise ValueError(f'Invalid amino acid string: {s}')
+        return super().from_str(s)
     
     @classmethod
-    def from_int(cls, i: int) -> 'AminoAcid':
+    def from_int(cls, i: int) -> 'AminoAcidEnum':
         """Convert an integer to an AminoAcid object.
         
         Parameters
         ----------
         i : int
             An integer representing an amino acid.
             
         Returns
         -------
-        AminoAcid
-            An AminoAcid object.
+        AminoAcidEnum
+            An AminoAcidEnum object.
             
         Raises
         ------
         ValueError
             If the integer is not a valid amino acid.
             
         Examples
@@ -731,26 +589,26 @@
         >>> AminoAcid.from_int(30)
         Traceback (most recent call last):
         ValueError: Invalid index value for AminoAcid: 30
         """
         return super().from_int(i)
     
     @classmethod
-    def from_onehot(cls, onehot: Sequence[int]) -> 'AminoAcid':
+    def from_onehot(cls, onehot: Sequence[int]) -> 'AminoAcidEnum':
         """Convert a onehot vector to an AminoAcid object.
         
         Parameters
         ----------
         onehot : Sequence[int]
             A onehot vector representing an amino acid.
             
         Returns
         -------
-        AminoAcid
-            An AminoAcid object.
+        AminoAcidEnum
+            An AminoAcidEnum object.
             
         Raises
         ------
         ValueError
             If the onehot vector is not a valid amino acid.
             
         Examples
@@ -762,30 +620,28 @@
         >>> AminoAcid.from_onehot([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1])
         #
         >>> AminoAcid.from_onehot([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
         Traceback (most recent call last):
         ValueError: Invalid onehot vector for AminoAcid: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         """
         return super().from_onehot(onehot)
-    
-    # Factory methods unique to AminoAcid
-    
+
     @classmethod
-    def from_one_letter(cls, one_letter_code: str) -> 'AminoAcid':
+    def from_one_letter(cls, one_letter_code: str) -> 'AminoAcidEnum':
         """Convert a one-letter code to an AminoAcid object.
         
         Parameters
         ----------
         one_letter_code : str
             A one-letter code representing an amino acid.
         
         Returns
         -------
-        AminoAcid
-            An AminoAcid object.
+        AminoAcidEnum
+            An AminoAcidEnum object.
             
         Raises
         ------
         ValueError
             If the one-letter code is not a valid amino acid.
             
         Examples
@@ -799,32 +655,29 @@
         >>> AminoAcid.from_one_letter('Asp')
         Traceback (most recent call last):
         ValueError: Invalid one-letter code: Asp
         >>> AminoAcid.from_one_letter('!')
         Traceback (most recent call last):
         ValueError: Invalid one-letter code: !
         """
-        try:
-            return cls[AMINO_ACID_ONE_LETTER_TOKEN_TO_NAME[one_letter_code.upper()]]
-        except KeyError:
-            raise ValueError(f'Invalid one-letter code: {one_letter_code}')
+        return super().from_one_letter(one_letter_code)
     
     @classmethod
-    def from_three_letter(cls, three_letter_code: str) -> 'AminoAcid':
-        f"""Convert a three-letter code to an AminoAcid object.
+    def from_three_letter(cls, three_letter_code: str) -> 'AminoAcidEnum':
+        """Convert a three-letter code to an AminoAcidEnum object.
         
         Parameters
         ----------
         three_letter_code : str
             A three-letter code representing an amino acid.
             
         Returns
         -------
-        AminoAcid
-            An AminoAcid object.
+        AminoAcidEnum
+            An AminoAcidEnum object.
             
         Raises
         ------
         ValueError
             If the three-letter code is not a valid amino acid.
             
         Examples
@@ -835,25 +688,21 @@
         A
         >>> AminoAcid.from_three_letter('ALA')
         A
         >>> AminoAcid.from_three_letter('Gap')
         -
         >>> AminoAcid.from_three_letter('XXX')
         Traceback (most recent call last):
-        ValueError: Invalid three-letter code for Amino Acid: XXX
+        ValueError: Invalid three-letter code for AminoAcid: XXX
         """
-        try:
-            return cls[AMINO_ACID_THREE_LETTER_TOKEN_TO_NAME[three_letter_code.capitalize()]]
-        except KeyError:
-            raise ValueError(f'Invalid three-letter code for {cls.__name__}: {three_letter_code}')
-    
+        return super().from_three_letter(three_letter_code)
+
     # Conversion methods
-    
     def to_onehot(self) -> Sequence[int]:
-        """Convert an AminoAcid object to a onehot vector.
+        """Convert an AminoAcidEnum object to a onehot vector.
         
         Returns
         -------
         Sequence[int]
             A onehot vector representing the amino acid.
             
         Examples
@@ -867,15 +716,15 @@
         >>> unknown_aa = AminoAcid.from_str('Xaa')
         >>> unknown_aa.to_onehot()
         [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0]
         """
         return super().to_onehot()
     
     def to_int(self) -> int:
-        """Convert an AminoAcid object to an integer representation.
+        """Convert an AminoAcidEnum object to an integer representation.
         
         Returns
         -------
         int
             An integer representing the amino acid.
             
         Examples
@@ -891,18 +740,16 @@
         26
         >>> masked_aa = AminoAcid.Mask
         >>> masked_aa.to_int()
         29
         """
         return super().to_int()
     
-    # Conversion methods unique to AminoAcid
-    
     def to_one_letter(self) -> str:
-        """Convert an AminoAcid object to a one-letter code.
+        """Convert an AminoAcidEnum object to a one-letter code.
         
         Returns
         -------
         str
             A one-letter code representing the amino acid.
         
         Examples
@@ -913,18 +760,18 @@
         >>> gap = AminoAcid.from_str('-')
         >>> gap.to_one_letter()
         '-'
         >>> unknown = AminoAcid.from_str('X')
         >>> unknown.to_one_letter()
         'X'
         """
-        return str(self)
+        return super().to_one_letter()
     
     def to_three_letter(self) -> str:
-        """Convert an AminoAcid object to a three-letter code.
+        """Convert an AminoAcidEnum object to a three-letter code.
         
         Returns
         -------
         str
             A three-letter code representing the amino acid.
             
         Examples
@@ -935,391 +782,390 @@
         >>> gap = AminoAcid.from_str('-')
         >>> gap.to_three_letter()
         'Gap'
         >>> unknown = AminoAcid.from_str('X')
         >>> unknown.to_three_letter()
         'Xaa'
         """
-        return NAME_TO_AMINO_ACID_THREE_LETTER_TOKEN[self.name]
-    
-    # Token type methods
+        return super().to_three_letter()
     
+    # Properties
     def is_standard(self) -> bool:
         """Return True if it is a standard amino acid.
             
         Returns
         -------
         bool
             True if the amino acid token represents a standard amino acid.
             
         Examples
         --------
-        >>> AminoAcid['Ala'].is_standard()
-        True
-        >>> AminoAcid['Sec'].is_standard()
-        False
-        >>> AminoAcid['Xaa'].is_standard()
-        False
-        """
-        return self.name in STANDARD_AA
-    
-    def is_mask(self) -> bool:
-        """Return True if masked.
-        
-        Returns
-        -------
-        bool
-            True if the amino acid object is masked.
-        
-        Examples
-        --------
-        >>> AminoAcid['Mask'].is_mask()
-        True
-        >>> AminoAcid['Ala'].is_mask()
-        False
-        >>> AminoAcid['Gap'].is_mask()
-        False
-        """
-        return super().is_mask()
-    
-    def is_gap(self) -> bool:
-        """Return True if it represents a gap.
-        
-        Returns
-        -------
-        bool
-            True if the amino acid token represents a gap.
-        
-        Examples
-        --------
-        >>> AminoAcid['Gap'].is_gap()
-        True
-        >>> AminoAcid['Ala'].is_gap()
-        False
-        >>> AminoAcid['Mask'].is_gap()
-        False
-        """
-        return super().is_gap()
-    
-    def is_special(self) -> bool:
-        """Return True if it represents a special sequence.
-        
-        Returns
-        -------
-        bool
-            True if the amino acid token represents a special sequence (Mask, Ter, Gap, Special).
-            
-        Examples
-        --------
-        >>> AminoAcid['Mask'].is_special()
-        True
-        >>> AminoAcid['Gap'].is_special()
-        True
-        >>> AminoAcid['Stop'].is_special()
+        >>> AminoAcid.Ala.is_standard()
         True
-        >>> AminoAcid['Other'].is_special()
-        True
-        >>> AminoAcid['Ala'].is_special()
-        False
-        >>> AminoAcid['Xaa'].is_special()
+        >>> AminoAcid.Sec.is_standard()
         False
-        >>> AminoAcid['Sec'].is_special()
+        >>> AminoAcid.Xaa.is_standard()
         False
         """
-        return super().is_special() or self.is_stop()
+        return super().is_standard()
     
     def is_any(self):
         """Return True if it represents any amino acid.
         
         Returns
         -------
         bool
             True if the amino acid token represents any amino acid.
         
         Examples
         --------
-        >>> AminoAcid['Xaa'].is_any()
+        >>> AminoAcid.Xaa.is_any()
         True
-        >>> AminoAcid['Ala'].is_any()
+        >>> AminoAcid.Ala.is_any()
         False
-        >>> AminoAcid['Gap'].is_any()
+        >>> AminoAcid.Gap.is_any()
         False
-        >>> AminoAcid['Mask'].is_any()
+        >>> AminoAcid.Mask.is_any()
         False
         """
-        return self == self.Xaa
+        return super().is_any()
     
     def is_ambiguous(self) -> bool:
         """Return True if it represents an ambiguous amino acid token.
         
         Returns
         -------
         bool
             True if the amino acid token represents an ambiguous amino acid token.
             
         Examples
         --------
-        >>> AminoAcid['Asx'].is_ambiguous()
+        >>> AminoAcid.Asx.is_ambiguous()
         True
-        >>> AminoAcid['Glx'].is_ambiguous()
+        >>> AminoAcid.Glx.is_ambiguous()
         True
-        >>> AminoAcid['Xle'].is_ambiguous()
+        >>> AminoAcid.Xle.is_ambiguous()
         True
-        >>> AminoAcid['Xaa'].is_ambiguous()
+        >>> AminoAcid.Xaa.is_ambiguous()
         True
-        >>> AminoAcid['Ala'].is_ambiguous()
+        >>> AminoAcid.Ala.is_ambiguous()
         False
-        >>> AminoAcid['Gap'].is_ambiguous()
+        >>> AminoAcid.Gap.is_ambiguous()
         False
         """
         return (
             self.is_any() or 
-            self == self.Asx or 
-            self == self.Glx or 
-            self == self.Xle)
-        
-    # Token type methods unique to AminoAcid
+            self.name == 'Asx' or 
+            self.name == 'Glx' or 
+            self.name == 'Xle')
     
-    def is_nonstandard(self) -> bool:
-        """Return True if the amino acid is a nonstandard amino acid.
-        
-        Returns
-        -------
-        bool
-            True if the amino acid is a nonstandard amino acid selenocysteine or pyrrolysine.
-            
-        Examples
-        --------
-        >>> AminoAcid['Ala'].is_nonstandard()
-        False
-        >>> AminoAcid['Sec'].is_nonstandard()
-        True
-        >>> AminoAcid['Xaa'].is_nonstandard()
-        False
-        """
-        return self.name == 'Sec' or self.name == 'Pyl'
-        
     def is_stop(self) -> bool:
         """Return True if it represents a terminator sequence.
         
         Returns
         -------
         bool
             True if the amino acid token is a terminator sequence.
             
         Examples
         --------
-        >>> AminoAcid['Stop'].is_stop()
+        >>> AminoAcid.Stop.is_stop()
         True
-        >>> AminoAcid['Ala'].is_stop()
+        >>> AminoAcid.Ala.is_stop()
         False
-        >>> AminoAcid['Gap'].is_stop()
+        >>> AminoAcid.Gap.is_stop()
         False
         """
-        return self == self.Stop
-
-    # Properties
+        return super().is_stop()
     
     def is_polar(self) -> bool:
         """Return True if the amino acid identity is known and is polar.
         
         Returns
         -------
         bool
             True if the amino acid token represents a polar amino acid.
             
         Examples
         --------
-        >>> AminoAcid['Arg'].is_polar()
+        >>> AminoAcid.Arg.is_polar()
         True
-        >>> AminoAcid['Ala'].is_polar()
+        >>> AminoAcid.Ala.is_polar()
         False
-        >>> AminoAcid['Xaa'].is_polar()
+        >>> AminoAcid.Xaa.is_polar()
         False
         """
-        return self.name in POLAR_AA
-
+        return super().is_polar()
+    
     def is_nonpolar(self) -> bool:
         """Return True if the amino acid identity is known and is nonpolar.
         
         Returns
         -------
         bool
             True if the amino acid token represents a nonpolar amino acid.
             
         Examples
         --------
-        >>> AminoAcid['Ala'].is_nonpolar()
+        >>> AminoAcid.Ala.is_nonpolar()
         True
-        >>> AminoAcid['Arg'].is_nonpolar()
+        >>> AminoAcid.Arg.is_nonpolar()
         False
-        >>> AminoAcid['Xaa'].is_nonpolar()
+        >>> AminoAcid.Xaa.is_nonpolar()
         False
         """
-        return self.name in NONPOLAR_AA
+        return super().is_nonpolar()
     
     def is_acidic(self) -> bool:
         """Return True if the amino acid identity is known and is acidic.
         
         Returns
         -------
         bool
             True if the amino acid token represents an acidic amino acid.
             
         Examples
         --------
-        >>> AminoAcid['Asp'].is_acidic()
+        >>> AminoAcid.Asp.is_acidic()
         True
-        >>> AminoAcid['Ala'].is_acidic()
+        >>> AminoAcid.Ala.is_acidic()
         False
-        >>> AminoAcid['Xaa'].is_acidic()
+        >>> AminoAcid.Xaa.is_acidic()
         False
         """
-        return self.name in ACIDIC_AA
+        return super().is_acidic()
     
     def is_basic(self) -> bool:
         """Return True if the amino acid identity is known and is basic.
         
         Returns
         -------
         bool
             True if the amino acid token represents a basic amino acid.
         
         Examples
         --------
-        >>> AminoAcid['Arg'].is_basic()
+        >>> AminoAcid.Arg.is_basic()
         True
-        >>> AminoAcid['Ala'].is_basic()
+        >>> AminoAcid.Ala.is_basic()
         False
-        >>> AminoAcid['Xaa'].is_basic()
+        >>> AminoAcid.Xaa.is_basic()
         False
         """
-        return self.name in BASIC_AA
+        return super().is_basic()
     
     def is_aromatic(self) -> bool:
         """Return True if the amino acid identity is known and is aromatic.
         
         Returns
         -------
         bool
             True if the amino acid token represents an aromatic amino acid.
             
         Examples
         --------
-        >>> AminoAcid['Phe'].is_aromatic()
+        >>> AminoAcid.Phe.is_aromatic()
         True
-        >>> AminoAcid['Ala'].is_aromatic()
+        >>> AminoAcid.Ala.is_aromatic()
         False
-        >>> AminoAcid['Xaa'].is_aromatic()
+        >>> AminoAcid.Xaa.is_aromatic()
         False
         """
-        return self.name in AROMATIC_AA
+        return super().is_aromatic()
     
     def is_hydrophobic(self) -> bool:
         """Return True if the amino acid identity is known and is hydrophobic.
         
         Returns
         -------
         bool
             True if the amino acid token represents a hydrophobic amino acid.
             
         Examples
         --------
-        >>> AminoAcid['Ala'].is_hydrophobic()
+        >>> AminoAcid.Ala.is_hydrophobic()
         True
-        >>> AminoAcid['Gly'].is_hydrophobic()
+        >>> AminoAcid.Gly.is_hydrophobic()
         False
-        >>> AminoAcid['Xaa'].is_hydrophobic()
+        >>> AminoAcid.Xaa.is_hydrophobic()
         False
         """
-        return self.name in HYDROPHOBIC_AA
-
-    # Contains particular elements/functional groups
+        return super().is_hydrophobic()
     
     def has_sulfur(self) -> bool:
         """Return True if the amino acid identity is known and contains sulfur.
         
         Returns
         -------
         bool
             True if the amino acid token represents an amino acid with sulfur.
             
         Examples
         --------
-        >>> AminoAcid['Cys'].has_sulfur()
+        >>> AminoAcid.Cys.has_sulfur()
         True
-        >>> AminoAcid['Met'].has_sulfur()
+        >>> AminoAcid.Met.has_sulfur()
         True
-        >>> AminoAcid['Ala'].has_sulfur()
+        >>> AminoAcid.Ala.has_sulfur()
         False
-        >>> AminoAcid['Xaa'].has_sulfur()
+        >>> AminoAcid.Xaa.has_sulfur()
         False
         """
-        return self.name in SULFUR_AA
+        return super().has_sulfur()
     
     def has_amide(self) -> bool:
         """Return True if the amino acid identity is known and contains an amide.
         
         Returns
         -------
         bool
             True if the amino acid token represents an amino acid with an amide.
             
         Examples
         --------
-        >>> AminoAcid['Asn'].has_amide()
+        >>> AminoAcid.Asn.has_amide()
         True
-        >>> AminoAcid['Gln'].has_amide()
+        >>> AminoAcid.Gln.has_amide()
         True
-        >>> AminoAcid['Ala'].has_amide()
+        >>> AminoAcid.Ala.has_amide()
         False
-        >>> AminoAcid['Xaa'].has_amide()
+        >>> AminoAcid.Xaa.has_amide()
         False
         """
-        return self.name in AMIDE_AA
+        return super().has_amide()
     
     def has_hydroxyl(self) -> bool:
         """Return True if the amino acid identity is known and contains a hydroxyl.
         
         Returns
         -------
         bool
             True if the amino acid token represents an amino acid with a hydroxyl.
             
         Examples
         --------
-        >>> AminoAcid['Ser'].has_hydroxyl()
+        >>> AminoAcid.Ser.has_hydroxyl()
         True
-        >>> AminoAcid['Thr'].has_hydroxyl()
+        >>> AminoAcid.Thr.has_hydroxyl()
         True
-        >>> AminoAcid['Tyr'].has_hydroxyl()
+        >>> AminoAcid.Tyr.has_hydroxyl()
+        True
+        >>> AminoAcid.Ala.has_hydroxyl()
+        False
+        >>> AminoAcid.Xaa.has_hydroxyl()
+        False
+        """
+        return super().has_hydroxyl()
+    
+    #endregion
+    
+    #region Override methods from SpecialTokenMixin
+    def is_mask(self) -> bool:
+        """Return True if the token is a mask token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a mask token, False otherwise.
+        
+        Examples
+        --------
+        >>> AminoAcid.Mask.is_mask()
         True
-        >>> AminoAcid['Ala'].has_hydroxyl()
+        >>> AminoAcid.Ala.is_mask()
         False
-        >>> AminoAcid['Xaa'].has_hydroxyl()
+        >>> AminoAcid.Gap.is_mask()
         False
         """
-        return self.name in HYDROXYL_AA
+        return super().is_mask()
+
+    def is_gap(self) -> bool:
+        """Return True if the token is a gap token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a gap token, False otherwise.
+            
+        Examples
+        --------
+        >>> AminoAcid.Gap.is_gap()
+        True
+        >>> AminoAcid.Ala.is_gap()
+        False
+        >>> AminoAcid.Mask.is_gap()
+        False
+        """
+        return super().is_gap()
+    
+    def is_other(self) -> bool:
+        """Return True if the token is a valid but unspecified amino acid token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a valid but unspecified amino acid token, False otherwise.
+            
+        Examples
+        --------
+        >>> AminoAcid.Other.is_other()
+        True
+        >>> AminoAcid.Ala.is_other()
+        False
+        >>> AminoAcid.Mask.is_other()
+        False
+        >>> AminoAcid.Gap.is_other()
+        False
+        """
+        return super().is_other()
+    
+    def is_special(self) -> bool:
+        """Return True if the token is a mask, gap, or other token.
+        
+        Returns
+        -------
+        bool
+            True if the token is a mask, gap, or other token, False otherwise.
+         
+        Examples
+        --------
+        >>> AminoAcid.Mask.is_special()
+        True
+        >>> AminoAcid.Gap.is_special()
+        True
+        >>> AminoAcid.Other.is_special()
+        True
+        >>> AminoAcid.Ala.is_special()
+        False
+        >>> AminoAcid.Stop.is_special()
+        False
+        """
+        return super().is_special()
+    
+        # Factory methods unique to Codon
+    
+    #endregion
 
 
-class Codon(BioToken):
+class Codon(SpecialTokenMixin, CodonEnum):
     """A codon token.
     
     Attributes
     ----------
     name : str
         Three-letter sequence for the codon (e.g. 'AAA') or the designated name 
         of the special token.
     value : int
         The integer value of the codon.
         
         Standard codons are assigned values 1-64.
         Ambiguous codon NNN is assigned value 65.
         Special tokens 'Gap', 'Other', and 'Mask' are assigned values 0, 66, and 67, respectively.
     """
+    #region Token enum
     AAA = 1
     AAC = 2
     AAG = 3
     AAT = 4
     ACA = 5
     ACC = 6
     ACG = 7
@@ -1382,22 +1228,21 @@
     TTT = 64
     # Ambiguous codons
     NNN = 65
     # Special tokens
     Gap = 0
     Other = 66
     Mask = 67
-    
-    def __str__(self) -> str:
-        return NAME_TO_TRIPLET_TOKEN[self.name]
+    #endregion
+
+    #region Override methods from CodonEnum
     
     # Factory methods
-    
     @classmethod
-    def from_str(cls, s: str) -> 'Codon':
+    def from_str(cls, s: str) -> 'CodonEnum':
         """Convert a string to a Codon object.
         
         Parameters
         ----------
         s : str
             The string to convert.
         
@@ -1424,26 +1269,18 @@
         >>> Codon.from_str('AA')
         Traceback (most recent call last):
         ValueError: Invalid string length: 2 (AA)
         >>> Codon.from_str('A-A')
         Traceback (most recent call last):
         ValueError: Invalid codon string: A-A
         """
-        if len(s) != 3:
-            raise ValueError(f'Invalid string length: {len(s)} ({s})')
-        try:
-            return cls[TRIPLET_TOKEN_TO_NAME[s.upper()]]
-        except KeyError:
-            try:
-                return cls[TRIPLET_TOKEN_TO_NAME[s.capitalize()]]
-            except KeyError:
-                raise ValueError(f'Invalid codon string: {s}')
+        return super().from_str(s)
 
     @classmethod
-    def from_int(cls, i: int) -> 'Codon':
+    def from_int(cls, i: int) -> 'CodonEnum':
         """Convert an integer to a Codon object.
         
         Parameters
         ----------
         i : int
             The integer to convert.
             
@@ -1452,19 +1289,31 @@
         Codon
             The codon corresponding to the given integer.
             
         Raises
         ------
         ValueError
             If the integer is not a valid codon index.
+            
+        Examples
+        --------
+        >>> Codon.from_int(1)
+        AAA
+        >>> Codon.from_int(64)
+        TTT
+        >>> Codon.from_int(0)
+        ---
+        >>> Codon.from_int(68)
+        Traceback (most recent call last):
+        ValueError: Invalid index value for Codon: 68
         """
-        return super().from_int(i)
+        return cast('CodonEnum', super().from_int(i))
 
     @classmethod
-    def from_onehot(cls, onehot: Sequence[int]) -> 'Codon':
+    def from_onehot(cls, onehot: Sequence[int]) -> 'CodonEnum':
         """Convert a onehot vector to a Codon object.
         
         Parameters
         ----------
         onehot : Sequence[int]
             The one-hot vector.
             
@@ -1474,20 +1323,18 @@
             The codon corresponding to the given one-hot vector.
             
         Raises
         ------
         ValueError
             If the one-hot vector is invalid.
         """
-        return super().from_onehot(onehot)
+        return cast('CodonEnum', super().from_onehot(onehot))
 
-    # Factory methods unique to Codon
-        
     @classmethod
-    def from_nucleotides(cls, seq: Sequence[Nucleotide]) -> 'Codon':
+    def from_nucleotides(cls, seq: Sequence[NucleotideEnum]) -> 'CodonEnum':
         """Convert a sequence of nucleotides to a codon.
         
         Parameters
         ----------
         seq : Sequence[Nucleotide]
             The sequence of nucleotides.
             
@@ -1509,27 +1356,23 @@
         TAG
         >>> Codon.from_nucleotides([Nucleotide.Gap, Nucleotide.Gap, Nucleotide.Gap])
         ---
         >>> Codon.from_nucleotides([Nucleotide.Mask, Nucleotide.Mask, Nucleotide.Mask])
         ###
         >>> Codon.from_nucleotides([Nucleotide.A, Nucleotide.A])
         Traceback (most recent call last):
-        ValueError: Invalid nucleotide sequence: [A, A]
+        ValueError: Invalid nucleotide sequence triplet: [A, A]
         >>> Codon.from_nucleotides([Nucleotide.A, Nucleotide.Gap, Nucleotide.A])
         Traceback (most recent call last):
-        ValueError: Invalid nucleotide sequence: [A, -, A]
+        ValueError: Invalid nucleotide sequence triplet: [A, -, A]
         """
-        try:
-            str_triplet = ''.join([str(n) for n in seq])
-            return cls.from_str(str_triplet)
-        except ValueError:
-            raise ValueError(f'Invalid nucleotide sequence: {seq}')
-
+        return super().from_nucleotides(seq)
+    
     @classmethod
-    def from_nucleotide_onehot(cls, onehot: Sequence[Sequence[int]]) -> 'Codon':
+    def from_nucleotide_onehot(cls, onehot: Sequence[Sequence[int]]) -> 'CodonEnum':
         """Convert sequence of Nucleotide onehot vectors to a Codon object.
         
         Parameters
         ----------
         onehot : Sequence[Sequence[int]]
             The one-hot vector.
             
@@ -1539,62 +1382,42 @@
             The codon corresponding to the given one-hot vector.
             
         Raises
         ------
         ValueError
             If the one-hot vector is invalid.
         """
-        if len(onehot) != 3:
-            raise ValueError(f'Invalid number of onehot vectors: {onehot}')
-        try:
-            return cls.from_nucleotides([Nucleotide.from_onehot(onehot[i]) for i in range(3)])
-        except ValueError:
-            raise ValueError(f'Invalid one-hot value for {cls.__name__}: {onehot}')
+        return super().from_nucleotide_onehot(onehot)
 
     @classmethod
-    def start_codon(cls) -> 'Codon':
+    def start_codon(cls) -> 'CodonEnum':
         """Return the start codon.
         
         Returns
         -------
         Codon
             The start codon ATG.
             
         Examples
         --------
         >>> Codon.start_codon()
         ATG
         """
-        return cls.ATG
-
-    # Conversion methods
+        return super().start_codon()
     
-    def to_onehot(self) -> Sequence[int]:
-        """Convert the codon to a one-hot vector.
-        
-        Returns
-        -------
-        Sequence[int]
-            The one-hot vector.
-        """
-        return super().to_onehot()
-    
-    def to_int(self) -> int:
-        """Convert the codon to an integer representation.
-        
-        Returns
-        -------
-        int
-            The integer.
-        """
-        return super().to_int()
-    
-    # Conversion methods unique to Codon
+    # Conversion methods
+    @property
+    def nucleotide_class(self) -> Type['NucleotideEnum']:
+        return Nucleotide
+    
+    @property
+    def aminoacid_class(self) -> Type['AminoAcidEnum']:
+        return AminoAcid
     
-    def to_nucleotides(self) -> Sequence[Nucleotide]:
+    def to_nucleotides(self) -> Sequence[NucleotideEnum]:
         """Convert the codon to a sequence of nucleotides.
         
         Returns
         -------
         Sequence[Nucleotide]
             The sequence of nucleotides.
             
@@ -1605,17 +1428,17 @@
         >>> Codon.TAG.to_nucleotides()
         [T, A, G]
         >>> Codon.Gap.to_nucleotides()
         [-, -, -]
         >>> Codon.Mask.to_nucleotides()
         [#, #, #]
         """
-        return [Nucleotide.from_str(n) for n in str(self)]
+        return super().to_nucleotides()
     
-    def to_anticodon(self) -> 'Codon':
+    def to_anticodon(self) -> 'CodonEnum':
         """Return the anticodon of the codon.
         
         Returns
         -------
         Codon
             Complimentary sequence of the codon.
             
@@ -1626,138 +1449,67 @@
         >>> Codon.TAG.to_anticodon()  # stop codon
         ATC
         >>> Codon.Gap.to_anticodon()
         ---
         >>> Codon.Mask.to_anticodon()
         ###
         """
-        if self.is_special():
-            return self.__class__(self.value)
-        anticodn_str = ''.join([COMPLEMENTARY_NUCLEOTIDES[n] for n in str(self)])
-        return self.__class__[anticodn_str]
-        
-    # Token type methods
+        return super().to_anticodon()
     
-    def is_standard(self) -> bool:
-        """Return True if the codon is one of the 64 standard codon.
+    def translate(self) -> AminoAcidEnum:
+        """Translate the codon to an amino acid.
         
         Returns
         -------
-        bool
-            True if the codon is a standard codon.
+        AminoAcid
+            The amino acid corresponding to the codon.
             
-        Examples
-        --------
-        >>> Codon.AAA.is_standard()
-        True
-        >>> Codon.ATG.is_standard()  # start codon
-        True
-        >>> Codon.TAG.is_standard()  # Stop codon
-        True
-        >>> Codon.Gap.is_standard()
-        False
-        >>> Codon.Mask.is_standard()
-        False
-        """
-        return self.name in STANDARD_CODONS
-
-    def is_mask(self) -> bool:
-        """Return True if the codon is a mask codon.
-        
-        Returns
-        -------
-        bool
-            True if the codon is a mask codon, False otherwise.
-        
-        Examples
-        --------
-        >>> Codon.Mask.is_mask()
-        True
-        >>> Codon.AAA.is_mask()
-        False
-        >>> Codon.ATG.is_mask()
-        False
-        >>> Codon.TAG.is_mask()
-        False
-        >>> Codon.Gap.is_mask()
-        False
-        """
-        return super().is_mask()
-
-    def is_gap(self) -> bool:
-        """Return True if the codon is a gap codon.
-        
-        Returns
-        -------
-        bool
-            True if the codon is a gap codon, False otherwise.
+        Raises
+        ------
+        ValueError
+            If the codon is not a valid codon.
             
         Examples
         --------
-        >>> Codon.Gap.is_gap()
-        True
-        >>> Codon.AAA.is_gap()
-        False
-        >>> Codon.ATG.is_gap()
-        False
-        >>> Codon.TAG.is_gap()
-        False
-        >>> Codon.Mask.is_gap()
-        False
+        >>> Codon.ATG.translate()
+        M
+        >>> Codon.AAA.translate()
+        K
+        >>> Codon.TAG.translate()
+        *
+        >>> Codon.Gap.translate()
+        -
         """
-        return super().is_gap()
+        return super().translate()
     
-    def is_other(self) -> bool:
-        """Return True if the codon is a valid but unspecified codon.
+    # Properties
         
-        Returns
-        -------
-        bool
-            True if the codon is a valid but unspecified codon, False otherwise.
-            
-        Examples
-        --------
-        >>> Codon.Other.is_other()
-        True
-        >>> Codon.AAA.is_other()
-        False
-        >>> Codon.ATG.is_other()
-        False
-        >>> Codon.TAG.is_other()
-        False
-        >>> Codon.Gap.is_other()
-        False
-        """
-        return super().is_other()
-    
-    def is_special(self) -> bool:
-        """Return True if the codon is a mask, gap, or other codon.
+    def is_standard(self) -> bool:
+        """Return True if the codon is one of the 64 standard codon.
         
         Returns
         -------
         bool
-            True if the codon is a mask, gap, or other codon, False otherwise.
+            True if the codon is a standard codon.
             
         Examples
         --------
-        >>> Codon.Mask.is_special()
+        >>> Codon.AAA.is_standard()
         True
-        >>> Codon.Gap.is_special()
+        >>> Codon.ATG.is_standard()  # start codon
         True
-        >>> Codon.Other.is_special()
+        >>> Codon.TAG.is_standard()  # Stop codon
         True
-        >>> Codon.AAA.is_special()
-        False
-        >>> Codon.ATG.is_special()
+        >>> Codon.Gap.is_standard()
         False
-        >>> Codon.TAG.is_special()
+        >>> Codon.Mask.is_standard()
         False
         """
-        return super().is_special()
-    
+        return super().is_standard()
+
     def is_any(self) -> bool:
         """Return True if the codon is NNN.
         
         Returns
         -------
         bool
             True if the codon is NNN, False otherwise.
@@ -1769,15 +1521,15 @@
         >>> Codon.Gap.is_any()
         False
         >>> Codon.Mask.is_any()
         False
         >>> Codon.AAA.is_any()
         False
         """
-        return self.name == 'NNN'
+        return super().is_any()
     
     def is_ambiguous(self) -> bool:
         """Return True if the codon is ambiguous.
         
         Returns
         -------
         bool
@@ -1790,18 +1542,16 @@
         >>> Codon.Gap.is_ambiguous()
         False
         >>> Codon.Mask.is_ambiguous()
         False
         >>> Codon.AAA.is_ambiguous()
         False
         """
-        return self.is_any()
+        return super().is_ambiguous()
     
-    # Codon-specific token type methods
-        
     def is_start_codon(self) -> bool:
         """Return True if the codon is the start codon.
         
         Returns
         -------
         bool
             True if the codon is the start codon, False otherwise.
@@ -1811,15 +1561,15 @@
         >>> Codon.ATG.is_start_codon()
         True
         >>> Codon.AAA.is_start_codon()
         False
         >>> Codon.Mask.is_start_codon()
         False
         """
-        return self.name == 'ATG'
+        return super().is_start_codon()
     
     def is_stop_codon(self) -> bool:
         """Return True if the codon is a stop codon.
 
         Returns
         -------
         bool
@@ -1836,17 +1586,15 @@
         >>> Codon.ATG.is_stop_codon()
         False
         >>> Codon.AAA.is_stop_codon()
         False
         >>> Codon.Mask.is_stop_codon()
         False
         """
-        return self.name in STOP_CODONS
-
-    # Properties
+        return super().is_stop_codon()
     
     def is_twofold_degenerate(self) -> bool:
         """Return True if the codon is twofold degenerate.
         
         Returns
         -------
         bool
@@ -1857,16 +1605,16 @@
         >>> Codon.AAA.is_twofold_degenerate()  # other codon is AAG
         True
         >>> Codon.ATG.is_twofold_degenerate()  # Met is has no degenerate sites
         False
         >>> Codon.TAG.is_twofold_degenerate()
         False
         """
-        return self.name in TWOFOLD_DEGENERATE_CODONS
-    
+        return super().is_twofold_degenerate()
+
     def is_threefold_degenerate(self) -> bool:
         """Return True if the codon is threefold degenerate.
         
         Returns
         -------
         bool 
             True if the codon is threefold degenerate, False otherwise.
@@ -1876,16 +1624,16 @@
         >>> Codon.ATA.is_threefold_degenerate()  # Ile
         True
         >>> Codon.TAG.is_threefold_degenerate()  # Stop
         False
         >>> Codon.AAA.is_threefold_degenerate()
         False
         """
-        return self.name in THREEFOLD_DEGENERATE_CODONS
-    
+        return super().is_threefold_degenerate()
+
     def is_fourfold_degenerate(self) -> bool:
         """Return True if the codon is fourfold degenerate.
         
         Returns
         -------
         bool
             True if the codon is fourfold degenerate, False otherwise.
@@ -1893,16 +1641,16 @@
         Examples
         --------
         >>> Codon.GTA.is_fourfold_degenerate()  # Val
         True
         >>> Codon.TTT.is_fourfold_degenerate()  # Phe
         False
         """
-        return self.name in FOURFOLD_DEGENERATE_CODONS
-
+        return super().is_fourfold_degenerate()
+    
     def is_sixfold_degenerate(self) -> bool:
         """Return True if the codon is sixfold degenerate.
         
         Returns
         -------
         bool
             True if the codon is sixfold degenerate, False otherwise.
@@ -1910,39 +1658,109 @@
         Examples
         --------
         >>> Codon.CGA.is_sixfold_degenerate()  # Arg
         True
         >>> Codon.TTT.is_sixfold_degenerate()  # Phe
         False
         """
-        return self.name in SIXFOLD_DEGENERATE_CODONS
+        return super().is_sixfold_degenerate()
+    
+    #endregion
+    
+    #region Override methods from SpecialTokenMixin
+    def is_mask(self) -> bool:
+        """Return True if the codon is a mask codon.
+        
+        Returns
+        -------
+        bool
+            True if the codon is a mask codon, False otherwise.
+        
+        Examples
+        --------
+        >>> Codon.Mask.is_mask()
+        True
+        >>> Codon.AAA.is_mask()
+        False
+        >>> Codon.ATG.is_mask()
+        False
+        >>> Codon.TAG.is_mask()
+        False
+        >>> Codon.Gap.is_mask()
+        False
+        """
+        return super().is_mask()
 
-    def translate(self) -> AminoAcid:
-        """Translate the codon to an amino acid.
+    def is_gap(self) -> bool:
+        """Return True if the codon is a gap codon.
         
         Returns
         -------
-        AminoAcid
-            The amino acid corresponding to the codon.
+        bool
+            True if the codon is a gap codon, False otherwise.
             
-        Raises
-        ------
-        ValueError
-            If the codon is not a valid codon.
+        Examples
+        --------
+        >>> Codon.Gap.is_gap()
+        True
+        >>> Codon.AAA.is_gap()
+        False
+        >>> Codon.ATG.is_gap()
+        False
+        >>> Codon.TAG.is_gap()
+        False
+        >>> Codon.Mask.is_gap()
+        False
+        """
+        return super().is_gap()
+    
+    def is_other(self) -> bool:
+        """Return True if the codon is a valid but unspecified codon.
+        
+        Returns
+        -------
+        bool
+            True if the codon is a valid but unspecified codon, False otherwise.
             
         Examples
         --------
-        >>> Codon.ATG.translate()
-        M
-        >>> Codon.AAA.translate()
-        K
-        >>> Codon.TAG.translate()
-        *
-        >>> Codon.Gap.translate()
-        -
+        >>> Codon.Other.is_other()
+        True
+        >>> Codon.AAA.is_other()
+        False
+        >>> Codon.ATG.is_other()
+        False
+        >>> Codon.TAG.is_other()
+        False
+        >>> Codon.Gap.is_other()
+        False
         """
-        if self.is_stop_codon():
-            return AminoAcid.Stop
-        try:
-            return AminoAcid[TRANSLATION_TABLE[self.name]]
-        except KeyError:
-            raise ValueError(f'Cannot be translated: {self}')
+        return super().is_other()
+    
+    def is_special(self) -> bool:
+        """Return True if the codon is a mask, gap, or other codon.
+        
+        Returns
+        -------
+        bool
+            True if the codon is a mask, gap, or other codon, False otherwise.
+            
+        Examples
+        --------
+        >>> Codon.Mask.is_special()
+        True
+        >>> Codon.Gap.is_special()
+        True
+        >>> Codon.Other.is_special()
+        True
+        >>> Codon.AAA.is_special()
+        False
+        >>> Codon.ATG.is_special()
+        False
+        >>> Codon.TAG.is_special()
+        False
+        """
+        return super().is_special()
+    
+        # Factory methods unique to Codon
+
+    #endregion
```

### Comparing `biodatatypes-0.1.1/setup.py` & `biodatatypes-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
+
 long_desc = open('README.md').read()
 required = []
 
 setup(
     name='biodatatypes',
-    version='0.1.1',
+    version='0.2.1',
     author='Kent Kawashima',
     author_email='kentkawashima@gmail.com',
     license='MIT',
     description='Nucleotide, amino acid, and codon datatypes for Python',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://github.com/kentwait/biodatatypes',
```

