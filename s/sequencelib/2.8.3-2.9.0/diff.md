# Comparing `tmp/sequencelib-2.8.3.tar.gz` & `tmp/sequencelib-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequencelib-2.8.3.tar", last modified: Tue Jun  7 08:23:11 2022, max compression
+gzip compressed data, was "sequencelib-2.9.0.tar", last modified: Mon Nov 14 10:23:03 2022, max compression
```

## Comparing `sequencelib-2.8.3.tar` & `sequencelib-2.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 gorm       (501) staff       (20)        0 2022-06-07 08:23:11.904981 sequencelib-2.8.3/
--rw-r--r--   0 gorm       (501) staff       (20)    35149 2022-02-20 16:23:49.000000 sequencelib-2.8.3/LICENSE
--rw-r--r--   0 gorm       (501) staff       (20)     1010 2022-06-07 08:23:11.905088 sequencelib-2.8.3/PKG-INFO
--rw-r--r--   0 gorm       (501) staff       (20)      537 2021-11-24 15:09:35.000000 sequencelib-2.8.3/README.md
--rw-r--r--   0 gorm       (501) staff       (20)      104 2021-11-24 14:13:53.000000 sequencelib-2.8.3/pyproject.toml
-drwxr-xr-x   0 gorm       (501) staff       (20)        0 2022-06-07 08:23:11.904806 sequencelib-2.8.3/sequencelib.egg-info/
--rw-r--r--   0 gorm       (501) staff       (20)     1010 2022-06-07 08:23:11.000000 sequencelib-2.8.3/sequencelib.egg-info/PKG-INFO
--rw-r--r--   0 gorm       (501) staff       (20)      231 2022-06-07 08:23:11.000000 sequencelib-2.8.3/sequencelib.egg-info/SOURCES.txt
--rw-r--r--   0 gorm       (501) staff       (20)        1 2022-06-07 08:23:11.000000 sequencelib-2.8.3/sequencelib.egg-info/dependency_links.txt
--rw-r--r--   0 gorm       (501) staff       (20)       25 2022-06-07 08:23:11.000000 sequencelib-2.8.3/sequencelib.egg-info/requires.txt
--rw-r--r--   0 gorm       (501) staff       (20)       12 2022-06-07 08:23:11.000000 sequencelib-2.8.3/sequencelib.egg-info/top_level.txt
--rw-r--r--   0 gorm       (501) staff       (20)   172191 2022-06-07 08:18:12.000000 sequencelib-2.8.3/sequencelib.py
--rw-r--r--   0 gorm       (501) staff       (20)      588 2022-06-07 08:23:11.905499 sequencelib-2.8.3/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2022-11-14 10:23:03.506280 sequencelib-2.9.0/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:23:49.000000 sequencelib-2.9.0/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)     1273 2022-11-14 10:23:03.506326 sequencelib-2.9.0/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      800 2022-11-14 10:22:10.000000 sequencelib-2.9.0/README.md
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 14:13:53.000000 sequencelib-2.9.0/pyproject.toml
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2022-11-14 10:23:03.506161 sequencelib-2.9.0/sequencelib.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)     1273 2022-11-14 10:23:03.000000 sequencelib-2.9.0/sequencelib.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      231 2022-11-14 10:23:03.000000 sequencelib-2.9.0/sequencelib.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2022-11-14 10:23:03.000000 sequencelib-2.9.0/sequencelib.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       25 2022-11-14 10:23:03.000000 sequencelib-2.9.0/sequencelib.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       12 2022-11-14 10:23:03.000000 sequencelib-2.9.0/sequencelib.egg-info/top_level.txt
+-rw-r--r--   0 agpe       (502) staff       (20)   172654 2022-11-14 09:46:28.000000 sequencelib-2.9.0/sequencelib.py
+-rw-r--r--   0 agpe       (502) staff       (20)      588 2022-11-14 10:23:03.506541 sequencelib-2.9.0/setup.cfg
```

### Comparing `sequencelib-2.8.3/LICENSE` & `sequencelib-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequencelib-2.8.3/PKG-INFO` & `sequencelib-2.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-Metadata-Version: 2.1
-Name: sequencelib
-Version: 2.8.3
-Summary: Read, write, and analyze biological sequences
-Home-page: https://github.com/agormp/sequencelib
-Author: Anders Gorm Pedersen
-Author-email: agpe@dtu.dk
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sequencelib: python library for reading, writing, and analyzing biological sequences
 
+[![PyPI downloads](https://static.pepy.tech/personalized-badge/sequencelib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sequencelib)
+![](https://img.shields.io/badge/version-2.9.0-blue)
+
 Using classes and methods in sequencelib.py it is possible to read and write textfiles containing DNA or protein-sequences (possibly aligned) and to analyze and manipulate the sequence in various ways.
 
 ## Availability
 
 The sequencelib.py module is available on GitHub: https://github.com/agormp/sequencelib and on PyPI: https://pypi.org/project/sequencelib/
 
 ## Installation
 
 ```
 python3 -m pip install sequencelib
 ```
 
 ## Highlights
 
-To be written
+To be written
```

### Comparing `sequencelib-2.8.3/sequencelib.py` & `sequencelib-2.9.0/sequencelib.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,46 @@
 import copy
 import os
 import numpy as np
 import Levenshtein as lv
 
 ##############################################################################################################
 # Various functions used by methods, that do not fit neatly in any class
-# (These were previously in "utils.py", but were included here to avoid having to distribute extra library)
+##############################################################################################################
+
+def find_seqtype(seqsample):
+    letters = set(seqsample) - set("-")   # Accepts most input types (list, string, set)
+    non_DNAletters = letters - Const.DNA_maxambig
+    non_proteinletters = letters - Const.Protein_maxambig
+    non_ASCIIletters = letters - Const.ASCII
+    if non_ASCIIletters:
+        raise SeqError("Unknown sequence type. Unrecognized symbols: {}".format(list(non_ASCIIletters)))
+    elif non_proteinletters:
+        return "ASCII"
+    elif non_DNAletters:
+        return "protein"
+    else:
+        return "DNA"
+
+##############################################################################################################
+
+def seqtype_attributes(seqtype):
+    """Returns alphabet and ambigsymbols for given seqtype"""
+    
+    # Python note: hack. Should rethink logic around seqtypes and refactor
+    # They can be set too many places at both container and element level
+    if seqtype == "DNA":
+        return (Const.DNA_maxambig, Const.DNA_maxambig - Const.DNA)
+    elif seqtype == "protein":
+        return (Const.Protein_maxambig, Const.Protein_maxambig - Const.Protein)
+    elif seqtype == "ASCII":
+        return (Const.ASCII, set())
+    else:
+        raise SeqError("Unknown sequence type: {}".format(seqtype))
+
 ##############################################################################################################
 
 def indices(mystring, substring):
     """Helper function that finds indices of substring in string. Returns as set"""
     result = set()
     offset = -1
     while True:
@@ -108,15 +139,15 @@
                 raise Exception("Unmatched end-comment delimiter: {}".format(text[pos-5:pos+5]))
 
     # Add final block of text if relevant (i.e., if text does not stop with rightdelim), return processed text
     if prevpos < len(text):
         processed_text += text[prevpos:]
     return processed_text
 
-##############################################################################################################
+#############################################################################################################
 
 def make_sparseencoder(alphabet, padding="X"):
     """Returns function that can sparse-encode strings in specified alphabet"""
 
     # This function uses a "closure" to create and return a function that can later be used
     # for sparse-encoding strings in the specified alphabet.
     # The purpose is to avoid having to build the translation dictionary every time the
@@ -178,15 +209,15 @@
 
 #############################################################################################
 #############################################################################################
 
 class Sequence(object):
     """Baseclass for sequence classes"""
 
-    def __init__(self, name, seq, annotation="", comments="", check_alphabet=False, degap=False):
+    def __init__(self, name, seq, annotation="", comments="", check_alphabet=True, degap=False):
 
         # NOTE: additional fields can be added later (e.g., feature list, etc.)
         self.name = name
         self.seq = seq.upper()
         self.annotation = annotation
         self.comments = comments
         self.check_alphabet = check_alphabet
@@ -549,15 +580,15 @@
 class DNA_sequence(Sequence):
     """Class containing one DNA sequence, and corresponding methods"""
 
     # Implementation note: alphabet should really be set in a more principled manner
 
     def __init__(self, name, seq, annotation="", comments="", check_alphabet=False, degap=False):
         self.seqtype="DNA"
-        self.alphabet = Const.DNA_typicalambig
+        self.alphabet = Const.DNA_maxambig
         self.ambigsymbols = self.alphabet - Const.DNA
         Sequence.__init__(self, name, seq, annotation, comments, check_alphabet, degap)
 
 ##    #######################################################################################
 ##
 ## NOTE: Consider whether this is a productive idea for alignments, if so reimplement at some point
 ##
@@ -623,15 +654,15 @@
 #############################################################################################
 
 class Protein_sequence(Sequence):
     """Class containing one protein sequence, and corresponding methods"""
 
     def __init__(self, name, seq, annotation="", comments="", check_alphabet=False, degap=False):
         self.seqtype="protein"
-        self.alphabet = Const.Protein_minambig
+        self.alphabet = Const.Protein_maxambig
         self.ambigsymbols = self.alphabet - Const.Protein
         Sequence.__init__(self, name, seq, annotation, comments, check_alphabet, degap)
 
     #######################################################################################
 
     def shuffle(self):
         """Returns shuffled sequence as protein sequence object - original is unchanged"""
@@ -641,14 +672,16 @@
         return Protein_sequence(name, shufseq)
 
 #############################################################################################
 #############################################################################################
 
 class ASCII_sequence(Sequence):
     """Class containing one sequence containing ASCII letters, and corresponding methods"""
+    
+    # Python note: will this ever be used???
 
     def __init__(self, name, seq, annotation="", comments="", check_alphabet=False, degap=False):
         self.seqtype="ASCII"
         self.alphabet = Const.ASCII
         self.ambigsymbols = set()       # Empty set. Attribute used by some functions. Change?
         Sequence.__init__(self, name, seq, annotation, comments, check_alphabet, degap)
 
@@ -940,15 +973,22 @@
 
     #######################################################################################
 
     def __init__(self, name=None, seqtype=None):
         self.name = name            # Label for set of sequences
         self.seqdict = {}           # seqdict format: {seqname:seqobject, ...}
         self.seqnamelist = []       # seqnamelist format: [name1, name2, ...]
-        self.seqtype = seqtype
+        if seqtype is None:
+            self.seqtype = None
+        else:
+            # Python note: seqtype perhaps should be object with separate attributes for 
+            # seqtype, alphabet and ambigsymbols!
+            # Also: I am setting seqtype in too many different places (Sequence objects 
+            # for instance). Rethink and refactor!!
+            self.alphabet, self.ambigsymbols = seqtype_attributes(seqtype)
 
     #######################################################################################
 
     def __len__(self):
         """Implements the len() operator for sequence sets (=number of seqs)"""
         return len(self.seqnamelist)
 
@@ -1047,19 +1087,17 @@
 
         # If name already in set of sequences: silently omit, or raise exception depending on options
         name = seq.name
         if name in self.seqdict:
             if not silently_discard_dup_name:
                 raise SeqError("Duplicate sequence names: %s" % name)
         else:
-            # Set seqtype, alphabet, and ambiguitysymbols of Seq_set if this is the first sequence added.
-            # Check type consistency if not the first sequence added.
-            # Note: Strictly speaking mixed types should perhaps be allowed?
-            # BUT: Seq_alignment is a subclass and currently relies on this type check!!!
-            if len(self)==0:
+            # Set seqtype, alphabet, and ambiguitysymbols of Seq_set if not already set
+            # Check type consistency otherwise.
+            if not self.seqtype:
                 self.seqtype = seq.seqtype
                 self.alphabet = seq.alphabet
                 self.ambigsymbols = seq.ambigsymbols
 
             elif seq.seqtype != self.seqtype:
                 raise SeqError("Mismatch between sequence types: %s vs. %s" % (self.seqtype, seq.seqtype))
 
@@ -1462,16 +1500,54 @@
     #######################################################################################
 
     def __init__(self, name=None, seqtype=None):
         Sequences_base.__init__(self, name=name, seqtype=None)
         self.alignment = True
         self.seqpos2alignpos_cache = {}
         self.alignpos2seqpos_cache = {}
-        self.annotation = None              # Annotation of each position
-                                            # Potentially one char per column
+        self.annotation = None           
+
+    #######################################################################################
+
+    def addseq(self, seq, silently_discard_dup_name=False):
+        """Add Sequence object to alignment"""
+        # Overrides baseclass function. Sets partition info + ensures consistent sequencelengths
+        if len(self) == 0:
+            self.partitions = [(self.name, 0, len(seq))]  # List of (name, partition-start, partition-length) tuples
+        else:
+            if len(seq) != len(self[0]):
+                raise SeqError("Not an alignment: these sequences have different lengths: %s and %s" % (seq.name, self[0].name))
+
+        # If length was OK, add sequence by calling baseclass method
+        Sequences_base.addseq(self, seq, silently_discard_dup_name)
+
+    #######################################################################################
+
+    def appendalignment(self, other):
+        """Appends sequences in 'other' to the end of similarly named sequences in 'self'"""
+
+        # Update partition info in self
+        partitiontuple = (other.name, self.alignlen(), other.alignlen())    # (name, partition-start, partition-length)
+        if len(self) == 0:
+            self.partitions = [partitiontuple]  # List of (name, partition-start, partition-length) tuples
+        else:
+            self.partitions.append(partitiontuple)
+
+        # If alignment object is empty: Initialise with other
+        if len(self) == 0:
+            self.addseqset(other)
+        # Else: match sequences, appending end to end
+        else:
+            for seq in self:
+                try:
+                    matchingseq = other.getseq(seq.name)
+                except SeqError:
+                    # Re-throw exception with more precise description of problem (we know more than just that name was not found)
+                    raise SeqError("Sequences in files have different names. No match found for %s" % seq.name)
+                seq.appendseq(matchingseq)
 
     #######################################################################################
 
     def alignlen(self):
         """Returns length of alignment or zero if no sequences"""
         if len(self) == 0:
             return(0)
@@ -1792,53 +1868,14 @@
     #         newseq = seq.subseq(start, stop, slicesyntax, rename)
     #         subseqs.addseq(newseq)
     #
     #     return subseqs
     #
     #######################################################################################
 
-    def addseq(self, seq, silently_discard_dup_name=False):
-        """Add Sequence object to alignment"""
-        # Overrides baseclass function. Sets partition info + ensures consistent sequencelengths
-        if len(self) == 0:
-            self.partitions = [(self.name, 0, len(seq))]  # List of (name, partition-start, partition-length) tuples
-        else:
-            if len(seq) != len(self[0]):
-                raise SeqError("Not an alignment: these sequences have different lengths: %s and %s" % (seq.name, self[0].name))
-
-        # If length was OK, add sequence by calling baseclass method
-        Sequences_base.addseq(self, seq, silently_discard_dup_name)
-
-    #######################################################################################
-
-    def appendalignment(self, other):
-        """Appends sequences in 'other' to the end of similarly named sequences in 'self'"""
-
-        # Update partition info in self
-        partitiontuple = (other.name, self.alignlen(), other.alignlen())    # (name, partition-start, partition-length)
-        if len(self) == 0:
-            self.partitions = [partitiontuple]  # List of (name, partition-start, partition-length) tuples
-        else:
-            self.partitions.append(partitiontuple)
-
-        # If alignment object is empty: Initialise with other
-        if len(self) == 0:
-            self.addseqset(other)
-        # Else: match sequences, appending end to end
-        else:
-            for seq in self:
-                try:
-                    matchingseq = other.getseq(seq.name)
-                except SeqError:
-                    # Re-throw exception with more precise description of problem (we know more than just that name was not found)
-                    raise SeqError("Sequences in files have different names. No match found for %s" % seq.name)
-                seq.appendseq(matchingseq)
-
-    #######################################################################################
-
     def partitions_as_seqalignments(self):
         """Returns list containing all partitions as Seq_alignment objects"""
 
         plist = []
         for i in range(len(self.partitions)):
             name = self.partitions[i][0]
             if name == "Partition" or name is None:        # Name has not been set, use number instead
@@ -2707,41 +2744,30 @@
         # Note: this is an empty table, since I will only be using the "deletechars" functionality in .translate
         self.spacetrans = str.maketrans("", "", string.whitespace)
         self.alltrans = str.maketrans("", "", string.whitespace + "0123456789")
 
     #######################################################################################
 
     def makeseq(self, name, seq, annotation="", comments=""):
-        """Takes name, sequence, annotation, and comments, returns sequence object of correct type"""
-
-        # Called by subclass
+        """Takes name, sequence, annotation, and comments, returns sequence object of correct type.
+        Called by subclass"""
 
-        # Convert to upper case
         seq = seq.upper()
-
-        # Determine seqtype.
-
-        # If autodetection of seqtype is requested: compare letters in seq to possible alphabets.
-        # Only done for first sequence: after checking, the filehandle's seqtype is set to first detected type
         if self.seqtype == "autodetect":
-            seqletters = set(seq) - set("-") # automatically uniquefies chars
-            if seqletters <= Const.DNA_typicalambig:
-                self.seqtype = "DNA"
+            self.seqtype = find_seqtype(seq)
+            if self.seqtype == "DNA":
                 return DNA_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
-            elif seqletters <= Const.Protein_minambig:
-                self.seqtype = "protein"
+            elif self.seqtype ==  "protein":
                 return Protein_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
-            elif seqletters <= Const.ASCII:
-                self.seqtype = "ASCII"
+            elif self.seqtype == "ASCII":
                 return ASCII_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
             else:
-                raise SeqError("Unknown symbols encountered during seqtype autodetection: %s" %
-                               (list(seqletters - Const.ASCII)))
-
-        # If specific seqtype requested, use that
+                unknown_symbols = list(seqletters - Const.ASCII)
+                msg = "Unknown symbols encountered during seqtype autodetection: {}".format(unknown_symbols)
+                raise SeqError(msg)
         elif self.seqtype == "DNA":
             return DNA_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
         elif self.seqtype == "protein":
             return Protein_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
         elif self.seqtype == "ASCII":
             return ASCII_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
         else:
@@ -3196,45 +3222,35 @@
         self.alltrans = str.maketrans("", "", string.whitespace + "0123456789")
 
     #######################################################################################
 
     def makeseq(self, name, seq, annotation="", comments=""):
         """Takes name, sequence, annotation, and comments, returns sequence object of correct type"""
 
-        # Convert to upper case
         seq = seq.upper()
-
-        # Determine seqtype.
-
-        # If autodetection of seqtype is requested: compare letters in seq to possible alphabets.
-        # Only done for first sequence: after checking, the filehandles seqtype is set to first detected type
         if self.seqtype == "autodetect":
-            seqletters = set(seq) - set("-") # automatically uniquefies chars
-            if seqletters <= Const.DNA_typicalambig:
-                self.seqtype = "DNA"
+            self.seqtype = find_seqtype(seq)
+            if self.seqtype == "DNA":
                 return DNA_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
-            elif seqletters <= Const.Protein_minambig:
-                self.seqtype = "protein"
+            elif self.seqtype ==  "protein":
                 return Protein_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
-            elif seqletters <= Const.ASCII:
-                self.seqtype = "ASCII"
+            elif self.seqtype == "ASCII":
                 return ASCII_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
             else:
-                raise SeqError("Unknown symbols encountered during seqtype autodetection: %s" %
-                               (list(seqletters - Const.ASCII)))
-
-        # If specific seqtype requested, use that
+                unknown_symbols = list(seqletters - Const.ASCII)
+                msg = "Unknown symbols encountered during seqtype autodetection: {}".format(unknown_symbols)
+                raise SeqError(msg)
         elif self.seqtype == "DNA":
             return DNA_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
         elif self.seqtype == "protein":
             return Protein_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
         elif self.seqtype == "ASCII":
             return ASCII_sequence(name, seq, annotation, comments, self.check_alphabet, self.degap)
         else:
-            raise SeqError("Unknown sequence type: %s" % self.seqtype, self.degap)
+            raise SeqError("Unknown sequence type: %s" % self.seqtype)
 
     #######################################################################################
 
     def read_seqs(self, silently_discard_dup_name=False):
 
         aligned_seqs = self.read_alignment(silently_discard_dup_name)
         return aligned_seqs.seqset()
```

### Comparing `sequencelib-2.8.3/setup.cfg` & `sequencelib-2.9.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sequencelib
-version = 2.8.3
+version = 2.9.0
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Read, write, and analyze biological sequences
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/sequencelib
 classifiers =
```

