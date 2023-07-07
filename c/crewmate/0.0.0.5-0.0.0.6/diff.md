# Comparing `tmp/crewmate-0.0.0.5.tar.gz` & `tmp/crewmate-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewmate-0.0.0.5.tar", last modified: Fri Jun 30 04:33:15 2023, max compression
+gzip compressed data, was "crewmate-0.0.0.6.tar", last modified: Fri Jul  7 05:50:47 2023, max compression
```

## Comparing `crewmate-0.0.0.5.tar` & `crewmate-0.0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.817556 crewmate-0.0.0.5/
--rw-rw-rw-   0        0        0      178 2023-06-30 04:33:15.816540 crewmate-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-26 09:14:10.000000 crewmate-0.0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 04:33:15.817556 crewmate-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      554 2023-06-30 04:33:07.000000 crewmate-0.0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.803276 crewmate-0.0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.810526 crewmate-0.0.0.5/src/crewmate/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:10:04.000000 crewmate-0.0.0.5/src/crewmate/__init__.py
--rw-rw-rw-   0        0        0     1269 2023-05-26 07:31:14.000000 crewmate-0.0.0.5/src/crewmate/cost_functions.py
--rw-rw-rw-   0        0        0        0 2023-05-26 04:55:14.000000 crewmate-0.0.0.5/src/crewmate/fit.py
--rw-rw-rw-   0        0        0     9933 2023-06-30 03:53:53.000000 crewmate-0.0.0.5/src/crewmate/qctrl.py
--rw-rw-rw-   0        0        0     6134 2023-06-30 04:31:27.000000 crewmate-0.0.0.5/src/crewmate/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.815032 crewmate-0.0.0.5/src/crewmate.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 05:50:47.973019 crewmate-0.0.0.6/
+-rw-rw-rw-   0        0        0      178 2023-07-07 05:50:47.973019 crewmate-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-05-26 09:14:10.000000 crewmate-0.0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 05:50:47.974025 crewmate-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-07-07 05:50:42.000000 crewmate-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:50:47.955503 crewmate-0.0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 05:50:47.963333 crewmate-0.0.0.6/src/crewmate/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:10:04.000000 crewmate-0.0.0.6/src/crewmate/__init__.py
+-rw-rw-rw-   0        0        0     1269 2023-05-26 07:31:14.000000 crewmate-0.0.0.6/src/crewmate/cost_functions.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 04:55:14.000000 crewmate-0.0.0.6/src/crewmate/fit.py
+-rw-rw-rw-   0        0        0     8969 2023-07-03 08:45:02.000000 crewmate-0.0.0.6/src/crewmate/qctrl.py
+-rw-rw-rw-   0        0        0     7967 2023-07-07 05:49:31.000000 crewmate-0.0.0.6/src/crewmate/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:50:47.971026 crewmate-0.0.0.6/src/crewmate.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-07 05:50:47.000000 crewmate-0.0.0.6/src/crewmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-07-07 05:50:47.000000 crewmate-0.0.0.6/src/crewmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 05:50:47.000000 crewmate-0.0.0.6/src/crewmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-07 05:50:47.000000 crewmate-0.0.0.6/src/crewmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 05:50:47.000000 crewmate-0.0.0.6/src/crewmate.egg-info/top_level.txt
```

### Comparing `crewmate-0.0.0.5/README.md` & `crewmate-0.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `crewmate-0.0.0.5/setup.py` & `crewmate-0.0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='crewmate',
-    version='0.0.0.5',
+    version='0.0.0.6',
     url="https://github.com/Qcrew/crewmate",
     author="Qcrew",
     author_email="general.qcrew@gmail.com",
     description='',
     py_modules=['crewmate.utils', 'crewmate.qctrl',
                 'crewmate.fit', 'crewmate.cost_functions'],
     package_dir={
```

### Comparing `crewmate-0.0.0.5/src/crewmate/cost_functions.py` & `crewmate-0.0.0.6/src/crewmate/cost_functions.py`

 * *Files identical despite different names*

### Comparing `crewmate-0.0.0.5/src/crewmate/qctrl.py` & `crewmate-0.0.0.6/src/crewmate/qctrl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 import numpy as np
 from types import SimpleNamespace
 import matplotlib.pyplot as plt
 
 import qctrl
 import qctrlvisualizer
 import qctrlcommons
@@ -64,66 +66,14 @@
         ])
         ladder_operators['q'] = q
         ladder_operators['qd'] = qd
 
     return SimpleNamespace(**ladder_operators)
 
 
-def quick_wigner_qctrl(qctrl: qctrl.Qctrl, psi: np.array, c_dim: int, q_dim: int, title="Wigner"):
-    """Plot the Wigner function of the state in the cavity starting from the full state (qubit x cavity).
-
-    Parameters
-    ----------
-    qctrl : qctrl.Qctrl
-        qctrl session reference
-    psi : np.array
-        state in the form qubit x cavity
-    c_dim : int
-        dimension of the cavity Hilbert space
-    q_dim : int
-        dimension of the qubit Hilbert space
-    title : str, optional
-        plot title, by default "Wigner"
-
-    Examples
-    --------
-    Consider psi = |cavity> x |qubit> = [1,0,0,0,0,0]
-    >>> quick_wigner_qctrl(qctrl, [1,0,0,0,0,0], 3, 2)
-    """
-
-    graph = qctrl.create_graph()
-
-    # Cavity state
-    final_cavity_state = graph.partial_trace(
-        graph.outer_product(psi, psi),
-        [c_dim, q_dim],
-        1,
-    )
-    # Wigner
-    wigner_range = 3
-    wigner_density = 128
-    # Axes for wigner plot
-    position = np.linspace(-wigner_range, wigner_range, wigner_density)
-    momentum = np.linspace(-wigner_range, wigner_range, wigner_density)
-    # Wigner transform
-    graph.wigner_transform(
-        final_cavity_state, position, momentum, name="wigner")
-
-    # Simulate system
-    simulation = qctrl.functions.calculate_graph(
-        graph=graph,
-        output_node_names=["wigner"]
-    )
-
-    qctrlvisualizer.plot_wigner_function(
-        simulation.output["wigner"]["value"], position, momentum)
-    plt.suptitle(title)
-    plt.show()
-
-
 # FIXME: super inefficient implementation forced by qctrl. Should find a workaround.
 def displacement(graph: qctrlcommons.data_types.Graph, alpha: float, c_dim: int) -> qctrlcommons.node.node_data.Tensor:
     """Generate the matrix associated with the displacement operator D(alpha)
 
     Parameters
     ----------
     graph : qctrlcommons.data_types.Graph
@@ -145,15 +95,22 @@
     for i in range(1, 30):
         term = -graph.sum(graph.outer_product(1/i *
                           (alpha * ad - graph.conjugate(alpha) * a), term), 0)
         D = graph.add(D, term)
     return D
 
 
-def build_snap_sequence_params(graph: qctrlcommons.data_types.Graph, c_dim: int, seq_length: int, D_var: qctrlcommons.node.node_data.Tensor, S_var: qctrlcommons.node.node_data.Tensor, verbose: bool = False) -> list:
+def build_snap_sequence_params(
+    graph: qctrlcommons.data_types.Graph,
+    c_dim: int,
+    seq_length: int,
+    D_var: qctrlcommons.node.node_data.Tensor,
+    S_var: qctrlcommons.node.node_data.Tensor,
+    verbose: bool = False
+) -> list:
     """Bundle the displacement and SNAP parameters in the format used by the apply_D_SNAP_D_sequence function.
 
     Parameters
     ----------
     graph : qctrlcommons.data_types.Graph
         QCTRL graph
     c_dim : int
@@ -194,15 +151,20 @@
             params.append(graph.concatenate([S_var[idx:idx+S_dim], S_fill], 0))
             if verbose:
                 print(f"{i}\tS-{s}  {S_var[idx:idx+S_dim].shape}")
             s += 1
     return params
 
 
-def apply_D_SNAP_sequence(graph: qctrlcommons.data_types.Graph, params: np.array or list, c_dim: int, psi_init: qctrlcommons.node.node_data.Tensor or np.array) -> qctrlcommons.node.node_data.Tensor:
+def apply_D_SNAP_sequence(
+    graph: qctrlcommons.data_types.Graph,
+    params: Union[np.array, list],
+    c_dim: int,
+    psi_init: Union[qctrlcommons.node.node_data.Tensor, np.array]
+) -> qctrlcommons.node.node_data.Tensor:
     """Apply an interleaved sequence of displacement and SNAP gates (D-SNAP-D...) to psi_init.
 
     Parameters
     ----------
     graph : qctrlcommons.data_types.Graph
         QCTRL graph
     params : np.array | list
@@ -230,42 +192,52 @@
             gate = I * graph.exp(1j*params[i])
         state = gate @ state
     return state[:, 0]
 
 
 def define_bandwidth_drive(
     graph: qctrlcommons.data_types.Graph,
-    segment_count: int,
-    duration: int,
+    variable_count: int,
+    duration: float,
     maximum: float,
-    cutoff_frequency: float
+    cutoff_frequency: float,
+    segment_count: int = -1
 ) -> qctrlcommons.node.node_data.Pwc:
-    """Define an optimizable complex pwc signal limited by the cutoff_frequency.
+    """Define an optimizable complex pwc signal limited by the `cutoff_frequency`.
+    The pulse is optimized using a number of variables `variable_count`.
+    Then the pulse is resampled in `segment_count` points and convoluted with a sinc kernel,
+    before the cost function is calculated.
 
     Parameters
     ----------
     graph : qctrlcommons.data_types.Graph
         QCTRL graph
-    segment_count : int
-        number of segments per pulse
+    variable_count : int
+        Number of optimizable variables
     duration : int
-        pulse duration [s]
+        Pulse duration [s]
     maximum : float
-        drive maximum
+        Drive maximum
     cutoff_frequency : float
-        maximum frequency allowed by the drive
+        Maximum frequency allowed by the drive
+    segment_count : int, optioinal
+        Number of pwc segments after sampling.
+        By default = -1, meaning the pulse will be sampled every nanosecond (duration * 1e9).
 
     Returns
     -------
     qctrlcommons.node.node_data.Pwc
         QCTRL complex optimizable pwc signal
     """
+    if segment_count == -1:
+        int(duration*1e9)
+
     # Define raw drive
     raw_drive = graph.utils.complex_optimizable_pwc_signal(
-        segment_count=segment_count,
+        segment_count=variable_count,
         duration=duration,
         maximum=maximum,
     )
     # Apply sinc cut to raw drives
     drive = graph.utils.filter_and_resample_pwc(
         pwc=raw_drive,
         cutoff_frequency=cutoff_frequency,
```

### Comparing `crewmate-0.0.0.5/src/crewmate/utils.py` & `crewmate-0.0.0.6/src/crewmate/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Union
+import pickle
+
 import numpy as np
 from scipy.linalg import block_diag
 
 import matplotlib.pyplot as plt
 from matplotlib import colors
 
 import qutip as qt
@@ -109,22 +112,22 @@
     beta = 2j * alpha * np.sin(chi * wait_time/2)
     D_gates = [qt.displace(c_dim, a) for a in [-beta, beta]]
     return np.flip(block_diag(*D_gates), 0)
 
 
 def quick_wigner(
     psi: np.array,
-    dims: np.array or list or int,
+    dims: Union[int, np.array, list],
     title: str = "Wigner",
     trace_idx: int = 1,
-    x_lim: np.array or list = [-3, 3],
-    y_lim: np.array or list = [-3, 3],
+    x_lim: Union[np.array, list] = [-3, 3],
+    y_lim: Union[np.array, list] = [-3, 3],
     pixel_count: int = 200,
     contour_levels: int = 100
-):
+) -> None:
     """Plot the Wigner function of psi. By default the system is assumed to be qubit-cavity.
 
     Parameters
     ----------
     psi : np.array
         State to plot.
     dims : np.arrayorlistorint
@@ -155,24 +158,93 @@
     psi = |g>|0>, considering qubit dimension = 2 and cavity dimension = 3.
     >>> quick_wigner([1,0,0,0,0,0], [2,3], trace_idx=0)
     """
     if len(x_lim) != 2:
         raise print(f"Length of x_lim must be 2, but got {len(x_lim)}.")
     if len(y_lim) != 2:
         raise print(f"Length of y_lim must be 2, but got {len(y_lim)}.")
-    if type(dims) == 'int':
+    if isinstance(dims, int):
         dims = [dims]
+        trace_idx = 0
 
     x = np.linspace(x_lim[0], x_lim[1], pixel_count)
     y = np.linspace(y_lim[0], y_lim[1], pixel_count)
     state = qt.Qobj(np.array(psi), dims=[dims, [1, 1]])
-    state_wigner = qt.wigner(state.ptrace(trace_idx), x, x)
+    state_wigner = qt.wigner(state.ptrace(trace_idx), x, y)
     # Plot
     fig = plt.figure(figsize=(5, 4), dpi=100)
     state_max = np.max(np.abs(np.array(state_wigner)))
     color_norm = colors.TwoSlopeNorm(
         vmin=-state_max, vcenter=0., vmax=state_max)
     contour = plt.contourf(
         x, y, state_wigner, contour_levels, cmap="bwr_r", norm=color_norm)
     fig.colorbar(contour)
     plt.title(title)
     plt.show()
+
+
+def save_drives_csv(drives: list[np.array], file_name: str) -> None:
+    """Save drives as complex numbers in a csv file.
+
+    Parameters
+    ----------
+    drives : list
+        A list containing the drives. Each drive must be a np.array.
+        IMPORTANT: if you want to save only one drive specify it as [drive]
+    file_name : str
+        File name.
+    """
+    if len(drives) > 5:
+        print("WARNING: you are trying to save more than 5 drives" +
+              "If you are trying to save just one drive you should specify it as [drive]")
+    if file_name.endswith('.csv'):
+        file_name = file_name[0:-4]
+    np.savetxt(f"{file_name}.csv", drives, delimiter=",")
+
+
+def read_drives_csv(file_name: str) -> list[np.array]:
+    """Read drives from csv file.
+
+    Parameters
+    ----------
+    file_name : str
+        File name.
+
+    Returns
+    -------
+    np.array
+        Drive list.
+    """
+    if file_name.endswith('.csv'):
+        file_name = file_name[0:-4]
+    return np.genfromtxt(f"{file_name}.csv", dtype="complex", delimiter=",")
+
+
+def save_object(obj, file_name: str):
+    """Save a python object to a file.
+
+    Parameters
+    ----------
+    obj : any
+        Object to save.
+    file_name : str
+        File name, including path if needed.
+    """
+    with open(f'{file_name}', 'wb') as outp:
+        pickle.dump(obj, outp, pickle.HIGHEST_PROTOCOL)
+
+
+def read_object(file_name: str):
+    """Read python object from a file
+
+    Parameters
+    ----------
+    file_name : str
+        File name, including path if needed.
+
+    Returns
+    -------
+    any
+        Object
+    """
+    with open(f'{file_name}', 'rb') as inp:
+        return pickle.load(inp)
```

