# Comparing `tmp/qfunk-0.1.2.tar.gz` & `tmp/qfunk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qfunk-0.1.2.tar", last modified: Tue Jul 26 11:31:09 2022, max compression
+gzip compressed data, was "qfunk-0.1.3.tar", last modified: Fri Jul  7 13:31:18 2023, max compression
```

## Comparing `qfunk-0.1.2.tar` & `qfunk-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-07-26 11:31:09.000000 qfunk-0.1.2/
--rw-rw-rw-   0        0        0     1086 2021-09-12 18:34:10.000000 qfunk-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      533 2022-07-26 11:31:09.000000 qfunk-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5267 2021-10-12 10:57:54.000000 qfunk-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-07-26 11:31:09.000000 qfunk-0.1.2/qfunk/
--rw-rw-rw-   0        0        0        0 2020-12-21 12:08:47.000000 qfunk-0.1.2/qfunk/__init__.py
--rw-rw-rw-   0        0        0     6383 2022-01-14 23:52:32.000000 qfunk-0.1.2/qfunk/generator.py
--rw-rw-rw-   0        0        0    27590 2022-01-14 22:51:51.000000 qfunk-0.1.2/qfunk/opensys.py
--rw-rw-rw-   0        0        0    15464 2022-05-28 12:00:33.000000 qfunk-0.1.2/qfunk/qoptic.py
--rw-rw-rw-   0        0        0     2291 2022-01-21 18:56:08.000000 qfunk-0.1.2/qfunk/testbench.py
--rw-rw-rw-   0        0        0    10130 2022-05-28 08:50:30.000000 qfunk-0.1.2/qfunk/utility.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:31:09.000000 qfunk-0.1.2/qfunk.egg-info/
--rw-rw-rw-   0        0        0      533 2022-07-26 11:31:08.000000 qfunk-0.1.2/qfunk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2022-07-26 11:31:08.000000 qfunk-0.1.2/qfunk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-26 11:31:08.000000 qfunk-0.1.2/qfunk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-07-26 11:31:08.000000 qfunk-0.1.2/qfunk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-26 11:31:09.000000 qfunk-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      663 2020-12-29 13:55:05.000000 qfunk-0.1.2/setup.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-07 13:31:18.585781 qfunk-0.1.3/
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     1086 2021-09-12 18:34:10.000000 qfunk-0.1.3/LICENSE.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      556 2023-07-07 13:31:18.585781 qfunk-0.1.3/PKG-INFO
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     5267 2021-10-12 10:57:54.000000 qfunk-0.1.3/README.md
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-07 13:31:18.585781 qfunk-0.1.3/qfunk/
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2020-12-21 12:08:47.000000 qfunk-0.1.3/qfunk/__init__.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    14942 2022-09-19 12:31:27.000000 qfunk-0.1.3/qfunk/decompose.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     6401 2023-07-06 14:45:16.000000 qfunk-0.1.3/qfunk/generator.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)    27590 2022-01-14 22:51:51.000000 qfunk-0.1.3/qfunk/opensys.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)    16393 2023-07-07 13:08:44.000000 qfunk-0.1.3/qfunk/qoptic.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     2291 2022-01-21 18:56:08.000000 qfunk-0.1.3/qfunk/testbench.py
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)    10134 2022-11-07 10:07:09.000000 qfunk-0.1.3/qfunk/utility.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-07 13:31:18.585781 qfunk-0.1.3/qfunk.egg-info/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      556 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      281 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        6 2023-07-07 13:31:18.000000 qfunk-0.1.3/qfunk.egg-info/top_level.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       79 2023-07-07 13:31:18.585781 qfunk-0.1.3/setup.cfg
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)      760 2023-07-07 13:31:16.000000 qfunk-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qfunk-0.1.2/LICENSE.txt` & `qfunk-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.2/PKG-INFO` & `qfunk-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-Metadata-Version: 2.1
-Name: qfunk
-Version: 0.1.2
-Summary: quantum information library
-Home-page: https://github.com/simonsupercool/qfunk
-Author: Simon Milz, Joshua Morris
-Author-email: Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: qfunk
+Version: 0.1.3
+Summary: quantum information library
+Home-page: https://github.com/simonsupercool/qfunk
+Download-URL: https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.3.tar.gz
+Author: Simon Milz, Joshua Morris
+Author-email: Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
```

### Comparing `qfunk-0.1.2/README.md` & `qfunk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.2/qfunk/generator.py` & `qfunk-0.1.3/qfunk/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,23 @@
     
     Returns
     -------
     randomly (according to Haar measure) generated unitary matrix of dimension n x n
     
     """
     z = (np.random.rand(n,n) + 1j*np.random.rand(n,n))/np.sqrt(2.0)
+
     q,r = np.linalg.qr(z)
+    
     d = np.diagonal(r)
+    
     ph = d/np.absolute(d)
+    
     q = np.multiply(q,ph,q)
+    
     return q
 
 
 def rand_rho(n, pure=False):
     """
     
     Parameters
@@ -86,16 +91,15 @@
     
     Requires
     -------
     numpy as np
     
     Returns
     -------
-    A randomly generated bistochastic matrix - unclear what the sampling behaviour is however.
-    
+    A randomly generated bistochastic matrix - unclear what the sampling behaviour is however,  
     """
 
     # generate iid matrix
     B = np.random.rand(n,n)
     # normalise columns and rows until bistochastic
     biflag = False
     while not biflag:
@@ -130,15 +134,15 @@
 
     Requires
     -------
     numpy as np
 
     Returns
     -------
-    gellman : d^2 x d x d complex numpy array containing spanning set
+    mub : d^2 x d x d complex numpy array containing spanning set
 
     """
 
     # base constant
     w = np.exp(2*np.pi*1j/d)
     # MUB container
     mub = np.zeros((d+1,d,d,d),dtype=np.complex128)
```

### Comparing `qfunk-0.1.2/qfunk/opensys.py` & `qfunk-0.1.3/qfunk/opensys.py`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.2/qfunk/qoptic.py` & `qfunk-0.1.3/qfunk/qoptic.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     for i in combination[1:]:
         # append next operator
         U = block_diag(U, arrayset[i])
     return U
     
 
 
-def _str_base(num, base, length, numerals = '0123456789'):
+def _str_base(num, base, length, numerals=100):
     """
     Outputs a list of number states in each mode, useful when needing consistent dimension labels in a Fock space.
 
     Parameters
     -----------
     num: number to be converted to base string
     base: base to work in
@@ -52,100 +52,128 @@
     numpy as np
     
     Returns
     -----------
     Representation of input number given chosen base and word length in string format
     
     """
+    # generate the list of numeral basis elements 
+    numerals = [r for r in range(numerals)]
 
     if base < 2 or base > len(numerals):
         raise ValueError("str_base: base must be between 2 and %i" % len(numerals))
 
     if num == 0:
-        return '0'*length
+        return [0]*length
 
-    if num < 0:
-        sign = '-'
-        num = -num
-    else:
-        sign = ''
-
-    result = ''
+    result = []
     while num:
-        result = numerals[num % (base)] + result
+        result = [numerals[num % (base)]] + result
         num //= base
 
+    if len(result) < length:
+        result = [0]*(length - len(result)) + result
+
+    return result
+
+
+
+
 
-    out = sign + result
 
-    if len(out) < length:
-        out = '0'*(length - len(out)) + out
-    return out
+def fermi_to_boson(num, m, p):
+     """
+     Converts fermionic number states to bosonic number states. Map is surjective
+     """
+
+     # intialise list
+     boson_state = []
+     
+     # iterate over fermionic digits
+     for l in range(m):
+          boson_state.append(sum(np.equal(num,l)))
+
+     # return as immutable tuple
+     return tuple(boson_state)
 
 
 
 def symmetric_map(m_num, p_num):
-    """
-    Computes the permutation matrix to map the single Boson Hilbert space to that for p_num photons
-    and m_num modes, eliminating degenerate degrees of freedom. Exponentially faster than matrix permanent method
-    everyone else insists on using but at the cost of higher memory complexity. 
-    Useful for computing the action of single photon unitaries on multiphoton input states as U_{p_num} = S U^{\otimes p_num} S^T. 
-    
-    Parameters
-    -----------
-    m_num: number of bosonic modes in system
-    p_num: total number of bosons in system
-    
-    
-    Requires
-    -----------
-    numpy as np
-    
-    Returns
-    -----------
-    An isometric operator S that takes operators defined for F_{m_num,1} to F_{m_num, p_num}. 
-    
-    """
+     """
+     Computes the permutation matrix to map the single Boson Hilbert space to that for p_num photons
+     and m_num modes, eliminating degenerate degrees of freedom. Exponentially faster than matrix permanent method
+     everyone else insists on using but at the cost of higher memory complexity. 
+     Useful for computing the action of single photon unitaries on multiphoton input states as U_{p_num} = S U^{\otimes p_num} S^T. 
 
-    # compute size of output matrix
-    row_num = comb(m_num + p_num-1, p_num)
-    col_num = m_num**p_num
+     Parameters
+     -----------
+     m_num: number of bosonic modes in system
+     p_num: total number of bosons in system
 
-    # compute photon states as an m-ary number of p_num bits
-    photon_state = np.asarray([list(_str_base(n,m_num,p_num)) for n in range(m_num**p_num)]).astype(int)
 
-    # compute mode occupation number for each row
-    fock = np.zeros((col_num, m_num), dtype=np.int32)
-    # iterate over rows
-    for i in range(np.shape(photon_state)[0]):
-        # iterate over columns
-        for j in range(m_num):
-            fock[i,j] = np.sum(photon_state[i,:]==j)
+     Requires
+     -----------
+     numpy as np
 
-    # compute unique Fock states
-    uniques = np.fliplr(np.unique(fock, axis=0))
-    ldim = np.shape(uniques)[0]
+     Returns
+     -----------
+     An isometric operator S that takes operators defined on <p_num> subsystems each with <m_num> dof to the symmetric equivalent 
+
+     """
+
+     # compute size of output matrix
+     row_num = comb(m_num + p_num-1, p_num, exact=True)
+     col_num = m_num**p_num
 
-    # preallocate symmetric transform matrix
-    P = lil_matrix((ldim, col_num))
+     # initialise a dict to store index hits
+     photonic_states = {}
 
+     # preallocate symmetric transform matrix
+     P = lil_matrix((row_num, col_num))
 
-    # iterate over symmetric dimension
-    num = 0
-    for k in range(ldim):
-        num = 0
-        for m in range(col_num):
-            if (uniques[k,:] == fock[m,:]).all():
-                P[k,m] = 1
-                num += 1
+     # compute fermionic number states
+     fermionic_number_states = [tuple(_str_base(n,m_num,p_num)) for n in range(m_num**p_num)]
 
-        # ensure normalisation property holds
-        P[k,:] /= np.sqrt(np.sum(P[k,:]))
+     # iterate over ferminonic number states and compute corresponding bosonic state
+     index_counter = 0
+     for col_ind, fermi_state in enumerate(fermionic_number_states):
+          
+          # compute bosonic equivlaent
+          boson_state = fermi_to_boson(fermi_state, m_num, p_num)
+
+          # check if already had this number
+          if boson_state in photonic_states:
+               # get row index and update the symmetric map
+               row_ind = photonic_states[boson_state]
+               P[row_ind, col_ind] = 1
+
+               continue
+
+          # update our indexer and assign
+          else:
+               # update index dictionary
+               photonic_states[boson_state] = index_counter
+               
+               # update symmetric map
+               row_ind = photonic_states[boson_state]
+               P[row_ind, col_ind] = 1
+
+               # update counter
+               index_counter += 1
+
+     # reverse ordering to match fock state order
+     P = P[::-1,::-1]
+
+
+     # ensure normalisation property holds
+     for k in range(row_num):
+          P[k,:] /= np.sqrt(np.sum(P[k,:]))
+
+     return P
 
-    return P
 
 
 def number_states(m_num,p_num):
     """
     Outputs a list of number states in each mode, useful when needing consistent dimension labels in a Fock space.
 
     Parameters
@@ -209,15 +237,18 @@
         for p in range(1,p_num+1):
             # compute dimenion of each photon subspace
             dim += comb(m_num+p-1,p, exact=True)
         return dim
     else:
         return comb(m_num+p_num-1,p_num, exact=True)
 
-def lookup_gen(m_num, p_num):
+
+
+
+def lookup_gen(m_num, p_num, nstates=None):
     """
     Generate a lookup table for accessing indexes of number state basis - much more efficient that searching 
     the basis labels everytime.
 
     Parameters
     -----------
     m_num: number of bosonic modes in system 
@@ -230,15 +261,16 @@
     
     Returns
     -----------
     dim x m_num array giving the index of a particular number state
     """
 
     # generate number states
-    nstates = number_states(m_num, p_num)
+    if nstates is None:
+        nstates = number_states(m_num, p_num)
 
     # generate lookup table of correct dimension - TODO: turn this into a dictionary call - this is very memory inefficient
     dims = [p_num+1]*m_num
     lookup_table = {}
     # indexes of number state give corresponding index in table
     for i in range(len(nstates)):
         # assign index
@@ -348,26 +380,30 @@
     -----------
     m_num choose p_num x m_num numpy array of bosonic number states
 
 
     
     """
 
+    # catch trivial case
+    if p_num==0:
+        return np.asarray([[[1.0j]]])
+
     # compute dimension of isometric image
     dim = fock_dim(m_num, p_num, full=False)
     # generate number states for allocation 
     nstates = number_states(m_num=m_num, p_num=p_num)
     # generate lookup table for indexing
     lookup_table = lookup_gen(m_num=m_num, p_num=p_num)
     # preallocate single photon basis array
     basis = np.eye(dim)
     # initialise list to contain basis (allows for sparse representation)
     algebra_basis = np.zeros((m_num**2, dim, dim),dtype=np.complex128)
 
-    # compute the basis for the multiphoton algebra - is also the basis for the subalgebra so no need for exponential/logarithmic maps
+    # compute the basis for the multiphoton algebra
     cnt = 0
     for j in range(m_num): 
         for k in range(j+1):
             op_left = number_state_map(m_num=m_num, p_num=p_num, 
                              j=j,k=k, 
                              basis=basis, 
                              nstates=nstates, 
@@ -444,16 +480,15 @@
         return csc_matrix(rho)
     else:
         return rho
 
 
 def optical_projector(m_num, p_num, proj_modes, target, sparse=False):
     """
-    Computes operator that maps bosons in given modes to a target mode - acts like a partial trace operation while preserving dimension.
-    
+    Computes operator that maps bosons in given modes to a target mode - acts like a partial trace operation while preserving dimension,  
     Parameters
     -----------
     m_num: number of bosonic modes in system 
     p_num: total number of bosons in system
     nstate: list of integers of length m_num summing to p_num that define the desired number state
 
     Requires
```

### Comparing `qfunk-0.1.2/qfunk/testbench.py` & `qfunk-0.1.3/qfunk/testbench.py`

 * *Files identical despite different names*

### Comparing `qfunk-0.1.2/qfunk/utility.py` & `qfunk-0.1.3/qfunk/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,8 +417,9 @@
 
     # assign new variable
     B = A
     # iterate through powers
     for i in range(n-1):
         B = np.kron(B,A)
         
-    return B
+    return B
+
```

### Comparing `qfunk-0.1.2/qfunk.egg-info/PKG-INFO` & `qfunk-0.1.3/qfunk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-Metadata-Version: 2.1
-Name: qfunk
-Version: 0.1.2
-Summary: quantum information library
-Home-page: https://github.com/simonsupercool/qfunk
-Author: Simon Milz, Joshua Morris
-Author-email: Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: qfunk
+Version: 0.1.3
+Summary: quantum information library
+Home-page: https://github.com/simonsupercool/qfunk
+Download-URL: https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.3.tar.gz
+Author: Simon Milz, Joshua Morris
+Author-email: Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
```

### Comparing `qfunk-0.1.2/setup.py` & `qfunk-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qfunk",
-    version="0.1.2",
+    version="0.1.3",
     author="Simon Milz, Joshua Morris",
     author_email="Simon.Milz@oeaw.ac.at, joshua.morris@univie.ac.at",
     description="quantum information library",
     long_description_content_type="text/markdown",
     url="https://github.com/simonsupercool/qfunk",
+    download_url = "https://github.com/simonsupercool/qfunk/archive/refs/tags/v0.1.3.tar.gz",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.5',
-)
+)
```

