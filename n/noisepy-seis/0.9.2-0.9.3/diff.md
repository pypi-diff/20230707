# Comparing `tmp/noisepy_seis-0.9.2.tar.gz` & `tmp/noisepy_seis-0.9.3.tar.gz`

## Comparing `noisepy_seis-0.9.2.tar` & `noisepy_seis-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35007 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/pnwstore.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/LICENSE
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/README.md
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35007 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/LICENSE
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/README.md
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/PKG-INFO
```

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.3/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pandas as pd
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from noisepy.seis.datatypes import ConfigParameters
 from noisepy.seis.utils import TimeLogger
 from . import noise_module
 from obspy.clients.fdsn import Client
+from obspy.clients.fdsn.header import FDSNNoDataException
 
 logger = logging.getLogger(__name__)
 if not sys.warnoptions:
     import warnings
 
     warnings.simplefilter("ignore")
 
@@ -277,36 +278,42 @@
     endtime: obspy.UTCDateTime,
     index: int,
 ) -> Tuple[int, obspy.Stream]:
     logger.debug(f"Start download for {sta}.{chan}")
     client = Client(prepro_para.client_url_key, timeout=15)
     retries = 5
     while retries > 0:
+        retries -= 1
         try:
             tr = client.get_waveforms(
                 network=net,
                 station=sta,
                 channel=chan,
                 location=location,
                 starttime=starttime,
                 endtime=endtime,
             )
+        except FDSNNoDataException:
+            logger.warning(f"No data available for {starttime}-{endtime}/{sta}.{chan}")
+            return -1, None
         except Exception as e:
-            logger.warning(f"{e} for get_waveforms({sta}.{chan})")
+            logger.warning(f"{type(e)}/{e} for get_waveforms({sta}.{chan})")
+            continue
 
         logger.debug(f"Got waveforms for {sta}.{chan}")
 
         # preprocess to clean data
         tr = noise_module.preprocess_raw(
             tr,
             inv,
             prepro_para,
             starttime,
             endtime,
         )
         return index, tr
+    logger.warning(f"Could not download data for {starttime}-{endtime}/{sta}.{chan}")
     return -1, None
 
 
 # Point people to new entry point:
 if __name__ == "__main__":
     print("Please see:\n\npython noisepy.py download --help\n")
```

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.3/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.3/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Dict, Iterable, List, Tuple
 
 import numpy as np
 import obspy
 from datetimerange import DateTimeRange
 from scipy.fftpack.helper import next_fast_len
 
-from noisepy.seis.datatypes import Channel, ChannelData, ConfigParameters, NoiseFFT
-
 from . import noise_module
+from .datatypes import Channel, ChannelData, ConfigParameters, NoiseFFT
+from .scheduler import Scheduler, SingleNodeScheduler
 from .stores import CrossCorrelationDataStore, RawDataStore
 from .utils import TimeLogger, error_if
 
 logger = logging.getLogger(__name__)
 # ignore warnings
 if not sys.warnoptions:
     import warnings
@@ -31,57 +31,55 @@
     2) save all FFT data of the same time chunk in memory;
     3) performs cross-correlation for all station pairs in the same time chunk and
     output the sub-stacked (if selected) into ASDF format;
 Authors: Chengxin Jiang (chengxin_jiang@fas.harvard.edu)
          Marine Denolle (mdenolle@fas.harvard.edu)
 
 NOTE:
-    0. MOST occasions you just need to change parameters followed with detailed
-    explanations to run the script.
-    1. To read SAC/mseed files, we assume the users have sorted the data
-    by the time chunk they prefer (e.g., 1day)
-        and store them in folders named after the time chunk (e.g, 2010_10_1).
-        modify L135 to find your local data;
-    2. A script of S0B_to_ASDF.py is provided to help clean messy SAC/MSEED data and
+    1. A script of S0B_to_ASDF.py is provided to help clean messy SAC/MSEED data and
     convert them into ASDF format.
         the script takes minor time compared to that for cross-correlation.
         so we recommend to use S0B script for
         better NoisePy performance. the downside is that it duplicates the
         continuous noise data on your machine;
-    3. When "coherency" is preferred, please set "freq_norm" to "rma" and "time_norm" to "no"
+    2. When "coherency" is preferred, please set "freq_norm" to "rma" and "time_norm" to "no"
     for better performance.
 """
 
 
 def cross_correlate(
     raw_store: RawDataStore,
     fft_params: ConfigParameters,
     cc_store: CrossCorrelationDataStore,
+    scheduler: Scheduler = SingleNodeScheduler(),
 ):
     """
     Perform the cross-correlation analysis
 
-        Parameters:
-                raw_store: Store to load data from
-                fft_params: Parameters for the FFT calculations
-                cc_store: Store for saving cross correlations
-
+    Args:
+        raw_store: Store to load data from
+        fft_params: Parameters for the FFT calculations
+        cc_store: Store for saving cross correlations
     """
 
     executor = ThreadPoolExecutor()
     tlog = TimeLogger(logger, logging.INFO)
     t_s1_total = tlog.reset()
 
-    # set variables to broadcast
-    timespans = raw_store.get_timespans()
-    splits = len(timespans)
-    if splits == 0:
-        raise IOError("Abort! no available seismic files for FFT")
+    def init() -> List:
+        # set variables to broadcast
+        timespans = raw_store.get_timespans()
+        if len(timespans) == 0:
+            raise IOError("Abort! no available seismic files for FFT")
+        return [timespans]
+
+    [timespans] = scheduler.initialize(init, 1)
 
-    for ts in timespans:
+    for its in scheduler.get_indices(timespans):
+        ts = timespans[its]
         if cc_store.is_done(ts):
             continue
 
         """
         LOADING NOISE DATA AND DO FFT
         """
         nnfft = int(next_fast_len(int(fft_params.cc_len * fft_params.samp_freq)))  # samp_freq should be sampling_rate
```

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.3/src/noisepy/seis/S2_stacking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import sys
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 from datetimerange import DateTimeRange
-from mpi4py import MPI
 
 from noisepy.seis.datatypes import ConfigParameters, StackMethod
+from noisepy.seis.scheduler import Scheduler, SingleNodeScheduler
 from noisepy.seis.stores import CrossCorrelationDataStore, StackStore
 from noisepy.seis.utils import TimeLogger
 
 from . import noise_module
 
 logger = logging.getLogger(__name__)
 if not sys.warnoptions:
@@ -38,15 +38,20 @@
 """
 
 
 # maximum memory allowed per core in GB
 MAX_MEM = 4.0
 
 
-def stack(cc_store: CrossCorrelationDataStore, stack_store: StackStore, fft_params: ConfigParameters):
+def stack(
+    cc_store: CrossCorrelationDataStore,
+    stack_store: StackStore,
+    fft_params: ConfigParameters,
+    scheduler: Scheduler = SingleNodeScheduler(),
+):
     tlog = TimeLogger(logger=logger)
     t_tot = tlog.reset()
     if fft_params.rotation and fft_params.correction:
         if not fft_params.correction_csv:
             logger.warning("Missing correction_csv parameter but rotation=True and correction=True")
         else:
             locs = pd.read_csv(fft_params.correction_csv)
@@ -60,41 +65,31 @@
         enz_system = ["EE", "EN", "EZ", "NE", "NN", "NZ", "ZE", "ZN", "ZZ"]
 
     rtz_components = ["ZR", "ZT", "ZZ", "RR", "RT", "RZ", "TR", "TT", "TZ"]
 
     #######################################
     # #########PROCESSING SECTION##########
     #######################################
-
-    # --------MPI---------
-    comm = MPI.COMM_WORLD
-    rank = comm.Get_rank()
-    size = comm.Get_size()
-
-    if rank == 0:
+    def initializer():
         timespans = cc_store.get_timespans()
         pairs_all = list(set(pair for ts in timespans for pair in cc_store.get_station_pairs(ts)))
         logger.info(f"Station pairs: {pairs_all}")
 
-        splits = len(pairs_all)
-        if len(timespans) == 0 or splits == 0:
+        if len(timespans) == 0 or len(pairs_all) == 0:
             raise IOError("Abort! no available CCF data for stacking")
-    else:
-        splits, timespans, pairs_all = [None for _ in range(3)]
+        return timespans, pairs_all
+
+    timespans, pairs_all = scheduler.initialize(initializer, 2)
 
-    # broadcast the variables
-    splits = comm.bcast(splits, root=0)
-    timespans = comm.bcast(timespans, root=0)
-    pairs_all = comm.bcast(pairs_all, root=0)
     nccomp = fft_params.ncomp * fft_params.ncomp
     num_chunk = len(timespans) * nccomp
     num_segmts = 1
 
-    # MPI loop: loop through each user-defined time chunck
-    for ipair in range(rank, splits, size):
+    # loop through each pair assigned to this process by the scheduler
+    for ipair in scheduler.get_indices(pairs_all):
         tlog.reset()
 
         logger.debug("%dth path for station-pair %s" % (ipair, pairs_all[ipair]))
         sta_pair = pairs_all[ipair]
         src_sta = sta_pair[0]
         rec_sta = sta_pair[1]
 
@@ -255,15 +250,15 @@
                     ]
                     write_stacks(comp, tparameters, stacks)
         tlog.log(f"stack/rotate all station pairs {pairs_all[ipair]}", t_load)
 
         stack_store.mark_done(src_sta, rec_sta)
 
     tlog.log("step 2 in total", t_tot)
-    comm.barrier()
+    scheduler.synchronize()
 
 
 def validate_pairs(ncomp: int, sta_pair: str, fauto: int, ts: DateTimeRange, n_pairs: int) -> bool:
     if fauto == 1:
         if ncomp == 3 and n_pairs < 6:
             logger.warning("continue! not enough cross components for auto-correlation %s in %s" % (sta_pair, ts))
             return False
```

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.3/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.3/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.3/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.3/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/main.py` & `noisepy_seis-0.9.3/src/noisepy/seis/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .channelcatalog import CSVChannelCatalog, XMLStationChannelCatalog
 from .constants import CONFIG_FILE, STATION_FILE
 from .datatypes import Channel, ConfigParameters
 from .S0A_download_ASDF_MPI import download
 from .S1_fft_cc_MPI import cross_correlate
 from .S2_stacking import stack
 from .scedc_s3store import SCEDCS3DataStore
+from .scheduler import MPIScheduler, SingleNodeScheduler
 from .utils import fs_join, get_filesystem
 
 logger = logging.getLogger(__name__)
 # Utility running the different steps from the command line. Defines the arguments for each step
 
 default_data_path = "Documents/SCAL"
 
@@ -152,22 +153,24 @@
         params.save_yaml(fs_join(args.raw_data_path, CONFIG_FILE))
 
     def run_cross_correlation():
         ccf_dir = args.ccf_path
         cc_store = ASDFCCStore(ccf_dir)
         params = initialize_params(args, args.raw_data_path)
         raw_store = create_raw_store(args, params)
-        cross_correlate(raw_store, params, cc_store)
+        scheduler = MPIScheduler(0) if args.mpi else SingleNodeScheduler()
+        cross_correlate(raw_store, params, cc_store, scheduler)
         params.save_yaml(fs_join(ccf_dir, CONFIG_FILE))
 
     def run_stack():
         cc_store = ASDFCCStore(args.ccf_path, "r")
         stack_store = ASDFStackStore(args.stack_path)
         params = initialize_params(args, args.ccf_path)
-        stack(cc_store, stack_store, params)
+        scheduler = MPIScheduler(0) if args.mpi else SingleNodeScheduler()
+        stack(cc_store, stack_store, params, scheduler)
         params.save_yaml(fs_join(args.stack_path, CONFIG_FILE))
 
     if args.cmd == Command.DOWNLOAD:
         run_download()
     if args.cmd == Command.CROSS_CORRELATE:
         run_cross_correlation()
     if args.cmd == Command.STACK:
@@ -188,15 +191,15 @@
 
 
 def add_paths(parser, types: List[str]):
     for t in types:
         add_path(parser, t)
 
 
-def make_step_parser(subparsers: Any, cmd: Command, paths: List[str]):
+def make_step_parser(subparsers: Any, cmd: Command, paths: List[str]) -> Any:
     parser = subparsers.add_parser(
         cmd.name.lower(),
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     add_paths(parser, paths)
     parser.add_argument(
         "-log",
@@ -205,28 +208,33 @@
         default="info",
         choices=["notset", "debug", "info", "warning", "error", "critical"],
     )
     parser.add_argument(
         "-c", "--config", type=lambda f: _valid_config_file(parser, f), required=False, help="Configuration YAML file"
     )
     add_model(parser, ConfigParameters())
+    return parser
+
+
+def add_mpi(parser: Any):
+    parser.add_argument("-m", "--mpi", action="store_true")
 
 
 def main_cli():
     args = parse_args(sys.argv[1:])
     main(args)
 
 
 def parse_args(arguments: Iterable[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="cmd", required=True)
     make_step_parser(subparsers, Command.DOWNLOAD, ["raw_data"])
-    make_step_parser(subparsers, Command.CROSS_CORRELATE, ["raw_data", "ccf", "xml"])
-    make_step_parser(subparsers, Command.STACK, ["raw_data", "stack", "ccf"])
-    make_step_parser(subparsers, Command.ALL, ["raw_data", "ccf", "stack", "xml"])
+    add_mpi(make_step_parser(subparsers, Command.CROSS_CORRELATE, ["raw_data", "ccf", "xml"]))
+    add_mpi(make_step_parser(subparsers, Command.STACK, ["raw_data", "stack", "ccf"]))
+    add_mpi(make_step_parser(subparsers, Command.ALL, ["raw_data", "ccf", "stack", "xml"]))
 
     args = parser.parse_args(arguments)
 
     args.cmd = Command[args.cmd.upper()]
     return args
```

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.3/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.3/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/pnwstore.py` & `noisepy_seis-0.9.3/src/noisepy/seis/pnwstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.3/src/noisepy/seis/scedc_s3store.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/stores.py` & `noisepy_seis-0.9.3/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.3/src/noisepy/seis/utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/.gitignore` & `noisepy_seis-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/LICENSE` & `noisepy_seis-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.2/README.md` & `noisepy_seis-0.9.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,41 @@
 
 ### Note the order of the command lines below matters ###
 
 ## With Conda and pip:
 ```bash
 conda create -n noisepy python=3.8 pip
 conda activate noisepy
-conda install -c conda-forge openmpi
 pip install noisepy-seis
 ```
 
+## With Conda and pip and MPI support:
+```bash
+conda create -n noisepy python=3.8 pip
+conda activate noisepy
+conda install -c conda-forge openmpi
+pip install noisepy-seis[mpi]
+```
+
 ## With virtual environment:
+```bash
+python -m venv noisepy
+source noisepy/bin/activate
+pip install noisepy-seis
+```
+## With virtual environment and MPI support:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```bash
 brew install open-mpi
 ```
 
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
-pip install noisepy-seis
+pip install noisepy-seis[mpi]
 ```
 
 
 # Functionality
 Here is a list of features of the package:
 * download continous noise data based:
    + on webservices using obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
```

### Comparing `noisepy_seis-0.9.2/pyproject.toml` & `noisepy_seis-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
     "DateTimeRange==2.0.0",
     "h5py>=3.8.0",
-    "mpi4py>=3.1.4",
     "numba>=0.57.0",
     "numpy>=1.22.0",
     "pandas>=1.5.3",
     "pyasdf>=0.7.5",
     "pycwt>=0.3.0a22",
     "diskcache>=5.5",
     "fsspec>=2023.4.0",
@@ -75,14 +74,17 @@
     "pytest>=7.2.2",
     "memory-profiler>=0.61",
     "pre-commit>=3.2",
 ]
 sql = [
     "SQLite3-0611",
 ]
+mpi = [
+    "mpi4py>=3.1.4",
+]
 
 [project.scripts]
 noisepy = "noisepy.seis:main.main_cli"
 
 [tool.black]
 line-length = 120
```

### Comparing `noisepy_seis-0.9.2/PKG-INFO` & `noisepy_seis-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.2
+Version: 0.9.3
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -33,28 +33,29 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <3.11,>=3.8
 Requires-Dist: datetimerange==2.0.0
 Requires-Dist: diskcache>=5.5
 Requires-Dist: fsspec>=2023.4.0
 Requires-Dist: h5py>=3.8.0
-Requires-Dist: mpi4py>=3.1.4
 Requires-Dist: numba>=0.57.0
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: pyasdf>=0.7.5
 Requires-Dist: pycwt>=0.3.0a22
 Requires-Dist: pydantic-yaml>=0.11
 Requires-Dist: pydantic>=1.10.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: s3fs>=2023.4.0
 Provides-Extra: dev
 Requires-Dist: memory-profiler>=0.61; extra == 'dev'
 Requires-Dist: pre-commit>=3.2; extra == 'dev'
 Requires-Dist: pytest>=7.2.2; extra == 'dev'
+Provides-Extra: mpi
+Requires-Dist: mpi4py>=3.1.4; extra == 'mpi'
 Provides-Extra: sql
 Requires-Dist: sqlite3-0611; extra == 'sql'
 Description-Content-Type: text/markdown
 
 # About NoisePy
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions. It provides additional functionality for noise monitoring and surface wave dispersion analysis.
 
@@ -76,28 +77,41 @@
 
 ### Note the order of the command lines below matters ###
 
 ## With Conda and pip:
 ```bash
 conda create -n noisepy python=3.8 pip
 conda activate noisepy
-conda install -c conda-forge openmpi
 pip install noisepy-seis
 ```
 
+## With Conda and pip and MPI support:
+```bash
+conda create -n noisepy python=3.8 pip
+conda activate noisepy
+conda install -c conda-forge openmpi
+pip install noisepy-seis[mpi]
+```
+
 ## With virtual environment:
+```bash
+python -m venv noisepy
+source noisepy/bin/activate
+pip install noisepy-seis
+```
+## With virtual environment and MPI support:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```bash
 brew install open-mpi
 ```
 
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
-pip install noisepy-seis
+pip install noisepy-seis[mpi]
 ```
 
 
 # Functionality
 Here is a list of features of the package:
 * download continous noise data based:
    + on webservices using obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
```

