# Comparing `tmp/irff-1.5.3.tar.gz` & `tmp/irff-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irff-1.5.3.tar", last modified: Mon Jul  3 14:53:55 2023, max compression
+gzip compressed data, was "irff-1.5.4.tar", last modified: Fri Jul  7 00:38:23 2023, max compression
```

## Comparing `irff-1.5.3.tar` & `irff-1.5.4.tar`

### file list

```diff
@@ -1,178 +1,180 @@
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/
--rwxrwxrwx   0 feng      (1000) feng      (1000)    35181 2023-06-24 01:41:43.000000 irff-1.5.3/LICENSE
--rwxrwxrwx   0 feng      (1000) feng      (1000)      288 2023-07-03 14:53:55.000000 irff-1.5.3/PKG-INFO
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1482 2023-06-24 01:41:43.000000 irff-1.5.3/README.md
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/
--rwxrwxrwx   0 feng      (1000) feng      (1000)    48550 2023-06-24 01:41:43.000000 irff-1.5.3/irff/AtomDance.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    34873 2023-06-24 01:41:43.000000 irff-1.5.3/irff/LearningMachine.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2861 2023-06-24 01:41:43.000000 irff-1.5.3/irff/RadiusCutOff.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)        4 2023-06-24 01:41:43.000000 irff-1.5.3/irff/__init__.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/data/
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2268 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/ColData.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      439 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/dpdata.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    20949 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/mdtodata.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3005 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/prep_data.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      726 2023-06-24 01:41:43.000000 irff-1.5.3/irff/data/qeout_to_traj.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/deb/
--rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     7652 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/compare_energies.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    28016 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/deb_bde.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3746 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/hbdeb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2338 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/ird.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3542 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/irdeb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    27553 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/irffdeb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      696 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/irnan.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4126 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/mpdeb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    30455 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/reax_debug.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    28582 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/reax_gulp.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2712 2023-06-24 01:41:43.000000 irff-1.5.3/irff/deb/theta.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/dft/
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1764 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/CheckEmol.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4168 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/SinglePointEnergy.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    16923 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/cpmd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    16974 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/dftb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     9604 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/nwchem.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    32584 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/qe.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    34877 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/siesta.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    22010 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/siesta_zmatix_constrain.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4145 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dft/smd_server.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1712 2023-06-24 01:41:43.000000 irff-1.5.3/irff/dingtalk.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    32101 2023-06-24 01:41:43.000000 irff-1.5.3/irff/emdk.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    44033 2023-06-24 01:41:43.000000 irff-1.5.3/irff/fitbo.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)   230745 2023-07-03 14:53:54.000000 irff-1.5.3/irff/getNeighbor.c
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1822 2023-06-24 01:41:43.000000 irff-1.5.3/irff/getNeighbors.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6453 2023-06-24 01:41:43.000000 irff-1.5.3/irff/intCheck.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    56628 2023-06-24 01:41:43.000000 irff-1.5.3/irff/irff.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    58276 2023-06-24 01:41:43.000000 irff-1.5.3/irff/irff_np.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    16472 2023-06-24 01:41:43.000000 irff-1.5.3/irff/link.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/md/
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4042 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/ReactionCapture.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3104 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2360 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/gofr.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    16896 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/gulp.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4704 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/hugoniot.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    18130 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/irmd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    19211 2023-06-24 01:41:43.000000 irff-1.5.3/irff/md/lammps.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff/ml/
--rwxrwxrwx   0 feng      (1000) feng      (1000)        3 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6999 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/data.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     7349 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/evaluate_data.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     7764 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/evolution.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6427 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/ffield.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    10950 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/fit.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4110 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/fluctuation.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6011 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/gaqeq.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     9327 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/genetic.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    11038 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/gpfit_tfv2.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6406 2023-06-24 01:41:43.000000 irff-1.5.3/irff/ml/harmonic.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    10769 2023-06-24 14:27:05.000000 irff-1.5.3/irff/ml/train.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    20150 2023-06-24 01:41:43.000000 irff-1.5.3/irff/mlqeq.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    14721 2023-06-24 01:41:43.000000 irff-1.5.3/irff/molecule.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    67947 2023-06-24 01:41:43.000000 irff-1.5.3/irff/mpnn.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)   908572 2023-07-03 14:53:54.000000 irff-1.5.3/irff/neighbor.c
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2987 2023-06-24 01:41:43.000000 irff-1.5.3/irff/neighbors.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/plot/
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1557 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/BondEnergy.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2152 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/CheckAng.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1608 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/LearningResults.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3477 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/LearningResultsAng.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     5896 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/MessagePassing.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      185 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1782 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/abc.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2811 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/angel_to_bond.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4040 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/bde.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     7652 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/compare_energies.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1766 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/fingerprint.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2360 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/gofr.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    18668 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/irnn_plot.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3899 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/label_md.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3813 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/labels.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     5155 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/morse.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     8837 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/morse_taper.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     8460 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/mpbd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3813 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/mpnn_plbd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3165 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/nx.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1853 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pdf.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1120 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plbd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     7085 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plbo.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1831 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/ple.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3406 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plea.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1522 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pleb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2451 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pleo.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1697 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plev.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1401 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plevdw.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4559 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plf.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3707 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_atoms.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2110 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_atoms_matplot.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2391 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_atoms_momenta.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1701 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_bond_energy.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1632 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_charge.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2454 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_energy.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2183 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_eover.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4129 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_eover_atom.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2696 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_functions.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1358 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_morse.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2543 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_pes.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3304 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_pressure.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2752 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plot_zmat_pes.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1917 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plotenergy.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1900 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/plotenergy_bond.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2240 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/pltp.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4694 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_plbd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1821 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_pldd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    18380 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_plot.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     4402 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/reax_plov.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    24951 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/rffbd.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1199 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/sigmoid.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     8207 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/vdw_taper.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3108 2023-06-24 01:41:43.000000 irff-1.5.3/irff/plot/view.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/prop/
--rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/prop/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2362 2023-06-24 01:41:43.000000 irff-1.5.3/irff/prop/gofr.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6059 2023-06-24 01:41:43.000000 irff-1.5.3/irff/qeq.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)   103280 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reax.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    34168 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reax_data.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    87075 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reax_nn.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    27071 2023-06-24 01:41:43.000000 irff-1.5.3/irff/reaxfflib.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)    11293 2023-06-24 01:41:43.000000 irff-1.5.3/irff/spectra.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/structures/
--rwxrwxrwx   0 feng      (1000) feng      (1000)      607 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/Al.gen
--rwxrwxrwx   0 feng      (1000) feng      (1000)      767 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/C2C4.gen
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2495 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/HMX_MOL.gen
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2495 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/NM.gen
--rwxrwxrwx   0 feng      (1000) feng      (1000)      434 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2469 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/ball.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2776 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/ball_bulk.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      844 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/diamond.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     2749 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/fox7.gen
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1949 2023-06-24 01:41:43.000000 irff-1.5.3/irff/structures/nm3.gen
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:55.000000 irff-1.5.3/irff/tools/
--rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/__init__.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1189 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/eos_opt.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      203 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/epstopdf.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1518 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/ffield_to_json.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1422 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/ffieldtolib.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1470 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/fingerprint.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6093 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/fit_hugoniot_state.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     9738 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/fitnn.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1259 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/json_to_ffield.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     8741 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/morse_taper.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1626 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/pre_opt.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     6657 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/prepare_ffield.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1351 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/pressure.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3953 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/pseudo_gen.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3567 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/rsetff.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3328 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/setwb.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)      728 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/vdw.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     1241 2023-06-24 01:41:43.000000 irff-1.5.3/irff/tools/zmat_to_atoms.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     9800 2023-06-24 01:41:43.000000 irff-1.5.3/irff/trainer.py
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3798 2023-06-24 01:41:43.000000 irff-1.5.3/irff/zmatrix.py
-drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/
--rwxrwxrwx   0 feng      (1000) feng      (1000)      288 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/PKG-INFO
--rwxrwxrwx   0 feng      (1000) feng      (1000)     3493 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/SOURCES.txt
--rwxrwxrwx   0 feng      (1000) feng      (1000)        1 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/dependency_links.txt
--rwxrwxrwx   0 feng      (1000) feng      (1000)        5 2023-07-03 14:53:54.000000 irff-1.5.3/irff.egg-info/top_level.txt
--rwxrwxrwx   0 feng      (1000) feng      (1000)       38 2023-07-03 14:53:55.000000 irff-1.5.3/setup.cfg
--rwxrwxrwx   0 feng      (1000) feng      (1000)      857 2023-06-24 01:41:43.000000 irff-1.5.3/setup.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    35181 2023-06-24 01:41:43.000000 irff-1.5.4/LICENSE
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      288 2023-07-07 00:38:23.000000 irff-1.5.4/PKG-INFO
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1482 2023-06-24 01:41:43.000000 irff-1.5.4/README.md
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:22.000000 irff-1.5.4/irff/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    48550 2023-06-24 01:41:43.000000 irff-1.5.4/irff/AtomDance.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    34873 2023-06-24 01:41:43.000000 irff-1.5.4/irff/LearningMachine.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2861 2023-06-24 01:41:43.000000 irff-1.5.4/irff/RadiusCutOff.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        4 2023-06-24 01:41:43.000000 irff-1.5.4/irff/__init__.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:22.000000 irff-1.5.4/irff/data/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2268 2023-06-24 01:41:43.000000 irff-1.5.4/irff/data/ColData.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.4/irff/data/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      439 2023-06-24 01:41:43.000000 irff-1.5.4/irff/data/dpdata.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    20949 2023-06-24 01:41:43.000000 irff-1.5.4/irff/data/mdtodata.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3005 2023-06-24 01:41:43.000000 irff-1.5.4/irff/data/prep_data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      726 2023-06-24 01:41:43.000000 irff-1.5.4/irff/data/qeout_to_traj.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/deb/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7652 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/compare_energies.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    28016 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/deb_bde.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3746 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/hbdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2338 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/ird.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3542 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/irdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    27553 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/irffdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      696 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/irnan.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4126 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/mpdeb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    30455 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/reax_debug.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    28582 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/reax_gulp.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2712 2023-06-24 01:41:43.000000 irff-1.5.4/irff/deb/theta.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/dft/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1764 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/CheckEmol.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4168 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/SinglePointEnergy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16923 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/cpmd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16974 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/dftb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9604 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/nwchem.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    32584 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/qe.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    34877 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/siesta.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    22010 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/siesta_zmatix_constrain.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4145 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dft/smd_server.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1712 2023-06-24 01:41:43.000000 irff-1.5.4/irff/dingtalk.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    32101 2023-06-24 01:41:43.000000 irff-1.5.4/irff/emdk.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    44033 2023-06-24 01:41:43.000000 irff-1.5.4/irff/fitbo.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)   230745 2023-07-03 14:53:54.000000 irff-1.5.4/irff/getNeighbor.c
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1848 2023-06-24 01:41:43.000000 irff-1.5.4/irff/getNeighbor.pyx
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1822 2023-06-24 01:41:43.000000 irff-1.5.4/irff/getNeighbors.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6453 2023-06-24 01:41:43.000000 irff-1.5.4/irff/intCheck.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    56628 2023-06-24 01:41:43.000000 irff-1.5.4/irff/irff.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    58276 2023-06-24 01:41:43.000000 irff-1.5.4/irff/irff_np.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16472 2023-06-24 01:41:43.000000 irff-1.5.4/irff/link.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/md/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4042 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/ReactionCapture.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3104 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2360 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/gofr.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    16896 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/gulp.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4704 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/hugoniot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    18130 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/irmd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    19211 2023-06-24 01:41:43.000000 irff-1.5.4/irff/md/lammps.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/ml/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        3 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6999 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7349 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/evaluate_data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7764 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/evolution.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6427 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/ffield.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    10950 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/fit.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4110 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/fluctuation.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6011 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/gaqeq.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9327 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/genetic.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    11038 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/gpfit_tfv2.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6406 2023-06-24 01:41:43.000000 irff-1.5.4/irff/ml/harmonic.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    10769 2023-06-24 14:27:05.000000 irff-1.5.4/irff/ml/train.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    20150 2023-06-24 01:41:43.000000 irff-1.5.4/irff/mlqeq.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    14721 2023-06-24 01:41:43.000000 irff-1.5.4/irff/molecule.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    67947 2023-06-24 01:41:43.000000 irff-1.5.4/irff/mpnn.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)   908572 2023-07-03 14:53:54.000000 irff-1.5.4/irff/neighbor.c
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3561 2023-06-24 01:41:43.000000 irff-1.5.4/irff/neighbor.pyx
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2987 2023-06-24 01:41:43.000000 irff-1.5.4/irff/neighbors.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/plot/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1557 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/BondEnergy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2152 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/CheckAng.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1608 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/LearningResults.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3477 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/LearningResultsAng.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     5896 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/MessagePassing.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      185 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1782 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/abc.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2811 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/angel_to_bond.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4040 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/bde.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7652 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/compare_energies.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1766 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/fingerprint.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2360 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/gofr.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    18668 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/irnn_plot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3899 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/label_md.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3813 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/labels.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     5155 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/morse.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8837 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/morse_taper.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8460 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/mpbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3813 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/mpnn_plbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3165 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/nx.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1853 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/pdf.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1120 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     7085 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plbo.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1831 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/ple.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3406 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plea.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1522 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/pleb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2451 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/pleo.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1697 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plev.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1401 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plevdw.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4559 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plf.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3707 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_atoms.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2110 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_atoms_matplot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2391 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_atoms_momenta.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1701 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_bond_energy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1632 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_charge.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2454 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_energy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2183 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_eover.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4129 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_eover_atom.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2696 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_functions.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1358 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_morse.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2543 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_pes.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3304 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_pressure.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2752 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plot_zmat_pes.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1917 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plotenergy.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1900 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/plotenergy_bond.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2240 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/pltp.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4694 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/reax_plbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1821 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/reax_pldd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    18380 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/reax_plot.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     4402 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/reax_plov.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    24951 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/rffbd.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1199 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/sigmoid.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8207 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/vdw_taper.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3108 2023-06-24 01:41:43.000000 irff-1.5.4/irff/plot/view.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/prop/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.4/irff/prop/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2362 2023-06-24 01:41:43.000000 irff-1.5.4/irff/prop/gofr.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6059 2023-06-24 01:41:43.000000 irff-1.5.4/irff/qeq.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)   103280 2023-06-24 01:41:43.000000 irff-1.5.4/irff/reax.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    34168 2023-06-24 01:41:43.000000 irff-1.5.4/irff/reax_data.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    87075 2023-06-24 01:41:43.000000 irff-1.5.4/irff/reax_nn.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    27071 2023-06-24 01:41:43.000000 irff-1.5.4/irff/reaxfflib.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)    11293 2023-06-24 01:41:43.000000 irff-1.5.4/irff/spectra.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/structures/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      607 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/Al.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      767 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/C2C4.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2495 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/HMX_MOL.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2495 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/NM.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      434 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2469 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/ball.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2776 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/ball_bulk.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      844 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/diamond.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     2749 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/fox7.gen
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1949 2023-06-24 01:41:43.000000 irff-1.5.4/irff/structures/nm3.gen
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:23.000000 irff-1.5.4/irff/tools/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      523 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/__init__.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1189 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/eos_opt.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      203 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/epstopdf.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1518 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/ffield_to_json.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1422 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/ffieldtolib.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1470 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/fingerprint.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6093 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/fit_hugoniot_state.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9738 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/fitnn.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1259 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/json_to_ffield.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     8741 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/morse_taper.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1626 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/pre_opt.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     6657 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/prepare_ffield.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1351 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/pressure.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3953 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/pseudo_gen.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3567 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/rsetff.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3328 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/setwb.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      728 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/vdw.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     1241 2023-06-24 01:41:43.000000 irff-1.5.4/irff/tools/zmat_to_atoms.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     9800 2023-06-24 01:41:43.000000 irff-1.5.4/irff/trainer.py
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3798 2023-06-24 01:41:43.000000 irff-1.5.4/irff/zmatrix.py
+drwxrwxrwx   0 feng      (1000) feng      (1000)        0 2023-07-07 00:38:22.000000 irff-1.5.4/irff.egg-info/
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      288 2023-07-07 00:38:22.000000 irff-1.5.4/irff.egg-info/PKG-INFO
+-rwxrwxrwx   0 feng      (1000) feng      (1000)     3532 2023-07-07 00:38:22.000000 irff-1.5.4/irff.egg-info/SOURCES.txt
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        1 2023-07-07 00:38:22.000000 irff-1.5.4/irff.egg-info/dependency_links.txt
+-rwxrwxrwx   0 feng      (1000) feng      (1000)        5 2023-07-07 00:38:22.000000 irff-1.5.4/irff.egg-info/top_level.txt
+-rwxrwxrwx   0 feng      (1000) feng      (1000)       38 2023-07-07 00:38:23.000000 irff-1.5.4/setup.cfg
+-rwxrwxrwx   0 feng      (1000) feng      (1000)      865 2023-07-07 00:36:36.000000 irff-1.5.4/setup.py
```

### Comparing `irff-1.5.3/LICENSE` & `irff-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/README.md` & `irff-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/AtomDance.py` & `irff-1.5.4/irff/AtomDance.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/LearningMachine.py` & `irff-1.5.4/irff/LearningMachine.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/RadiusCutOff.py` & `irff-1.5.4/irff/RadiusCutOff.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/data/ColData.py` & `irff-1.5.4/irff/data/ColData.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/data/__init__.py` & `irff-1.5.4/irff/data/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/data/mdtodata.py` & `irff-1.5.4/irff/data/mdtodata.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/data/prep_data.py` & `irff-1.5.4/irff/data/prep_data.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/data/qeout_to_traj.py` & `irff-1.5.4/irff/data/qeout_to_traj.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/__init__.py` & `irff-1.5.4/irff/deb/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/compare_energies.py` & `irff-1.5.4/irff/deb/compare_energies.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/deb_bde.py` & `irff-1.5.4/irff/deb/deb_bde.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/hbdeb.py` & `irff-1.5.4/irff/deb/hbdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/ird.py` & `irff-1.5.4/irff/deb/ird.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/irdeb.py` & `irff-1.5.4/irff/deb/irdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/irffdeb.py` & `irff-1.5.4/irff/deb/irffdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/irnan.py` & `irff-1.5.4/irff/deb/irnan.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/mpdeb.py` & `irff-1.5.4/irff/deb/mpdeb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/reax_debug.py` & `irff-1.5.4/irff/deb/reax_debug.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/reax_gulp.py` & `irff-1.5.4/irff/deb/reax_gulp.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/deb/theta.py` & `irff-1.5.4/irff/deb/theta.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/CheckEmol.py` & `irff-1.5.4/irff/dft/CheckEmol.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/SinglePointEnergy.py` & `irff-1.5.4/irff/dft/SinglePointEnergy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/__init__.py` & `irff-1.5.4/irff/dft/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/cpmd.py` & `irff-1.5.4/irff/dft/cpmd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/dftb.py` & `irff-1.5.4/irff/dft/dftb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/nwchem.py` & `irff-1.5.4/irff/dft/nwchem.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/qe.py` & `irff-1.5.4/irff/dft/qe.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/siesta.py` & `irff-1.5.4/irff/dft/siesta.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/siesta_zmatix_constrain.py` & `irff-1.5.4/irff/dft/siesta_zmatix_constrain.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dft/smd_server.py` & `irff-1.5.4/irff/dft/smd_server.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/dingtalk.py` & `irff-1.5.4/irff/dingtalk.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/emdk.py` & `irff-1.5.4/irff/emdk.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/fitbo.py` & `irff-1.5.4/irff/fitbo.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/getNeighbor.c` & `irff-1.5.4/irff/getNeighbor.c`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/getNeighbors.py` & `irff-1.5.4/irff/getNeighbors.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/intCheck.py` & `irff-1.5.4/irff/intCheck.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/irff.py` & `irff-1.5.4/irff/irff.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/irff_np.py` & `irff-1.5.4/irff/irff_np.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/link.py` & `irff-1.5.4/irff/link.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/ReactionCapture.py` & `irff-1.5.4/irff/md/ReactionCapture.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/__init__.py` & `irff-1.5.4/irff/md/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/gofr.py` & `irff-1.5.4/irff/md/gofr.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/gulp.py` & `irff-1.5.4/irff/md/gulp.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/hugoniot.py` & `irff-1.5.4/irff/md/hugoniot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/irmd.py` & `irff-1.5.4/irff/md/irmd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/md/lammps.py` & `irff-1.5.4/irff/md/lammps.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/data.py` & `irff-1.5.4/irff/ml/data.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/evaluate_data.py` & `irff-1.5.4/irff/ml/evaluate_data.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/evolution.py` & `irff-1.5.4/irff/ml/evolution.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/ffield.py` & `irff-1.5.4/irff/ml/ffield.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/fit.py` & `irff-1.5.4/irff/ml/fit.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/fluctuation.py` & `irff-1.5.4/irff/ml/fluctuation.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/gaqeq.py` & `irff-1.5.4/irff/ml/gaqeq.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/genetic.py` & `irff-1.5.4/irff/ml/genetic.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/gpfit_tfv2.py` & `irff-1.5.4/irff/ml/gpfit_tfv2.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/harmonic.py` & `irff-1.5.4/irff/ml/harmonic.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/ml/train.py` & `irff-1.5.4/irff/ml/train.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/mlqeq.py` & `irff-1.5.4/irff/mlqeq.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/molecule.py` & `irff-1.5.4/irff/molecule.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/mpnn.py` & `irff-1.5.4/irff/mpnn.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/neighbor.c` & `irff-1.5.4/irff/neighbor.c`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/neighbors.py` & `irff-1.5.4/irff/neighbors.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/BondEnergy.py` & `irff-1.5.4/irff/plot/BondEnergy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/CheckAng.py` & `irff-1.5.4/irff/plot/CheckAng.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/LearningResults.py` & `irff-1.5.4/irff/plot/LearningResults.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/LearningResultsAng.py` & `irff-1.5.4/irff/plot/LearningResultsAng.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/MessagePassing.py` & `irff-1.5.4/irff/plot/MessagePassing.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/abc.py` & `irff-1.5.4/irff/plot/abc.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/angel_to_bond.py` & `irff-1.5.4/irff/plot/angel_to_bond.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/bde.py` & `irff-1.5.4/irff/plot/bde.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/compare_energies.py` & `irff-1.5.4/irff/plot/compare_energies.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/fingerprint.py` & `irff-1.5.4/irff/plot/fingerprint.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/gofr.py` & `irff-1.5.4/irff/plot/gofr.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/irnn_plot.py` & `irff-1.5.4/irff/plot/irnn_plot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/label_md.py` & `irff-1.5.4/irff/plot/label_md.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/labels.py` & `irff-1.5.4/irff/plot/labels.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/morse.py` & `irff-1.5.4/irff/plot/morse.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/morse_taper.py` & `irff-1.5.4/irff/plot/morse_taper.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/mpbd.py` & `irff-1.5.4/irff/plot/mpbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/mpnn_plbd.py` & `irff-1.5.4/irff/plot/mpnn_plbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/nx.py` & `irff-1.5.4/irff/plot/nx.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/pdf.py` & `irff-1.5.4/irff/plot/pdf.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plbd.py` & `irff-1.5.4/irff/plot/plbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plbo.py` & `irff-1.5.4/irff/plot/plbo.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/ple.py` & `irff-1.5.4/irff/plot/ple.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plea.py` & `irff-1.5.4/irff/plot/plea.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/pleb.py` & `irff-1.5.4/irff/plot/pleb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/pleo.py` & `irff-1.5.4/irff/plot/pleo.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plev.py` & `irff-1.5.4/irff/plot/plev.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plevdw.py` & `irff-1.5.4/irff/plot/plevdw.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plf.py` & `irff-1.5.4/irff/plot/plf.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_atoms.py` & `irff-1.5.4/irff/plot/plot_atoms.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_atoms_matplot.py` & `irff-1.5.4/irff/plot/plot_atoms_matplot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_atoms_momenta.py` & `irff-1.5.4/irff/plot/plot_atoms_momenta.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_bond_energy.py` & `irff-1.5.4/irff/plot/plot_bond_energy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_charge.py` & `irff-1.5.4/irff/plot/plot_charge.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_energy.py` & `irff-1.5.4/irff/plot/plot_energy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_eover.py` & `irff-1.5.4/irff/plot/plot_eover.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_eover_atom.py` & `irff-1.5.4/irff/plot/plot_eover_atom.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_functions.py` & `irff-1.5.4/irff/plot/plot_functions.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_morse.py` & `irff-1.5.4/irff/plot/plot_morse.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_pes.py` & `irff-1.5.4/irff/plot/plot_pes.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_pressure.py` & `irff-1.5.4/irff/plot/plot_pressure.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plot_zmat_pes.py` & `irff-1.5.4/irff/plot/plot_zmat_pes.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plotenergy.py` & `irff-1.5.4/irff/plot/plotenergy.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/plotenergy_bond.py` & `irff-1.5.4/irff/plot/plotenergy_bond.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/pltp.py` & `irff-1.5.4/irff/plot/pltp.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/reax_plbd.py` & `irff-1.5.4/irff/plot/reax_plbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/reax_pldd.py` & `irff-1.5.4/irff/plot/reax_pldd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/reax_plot.py` & `irff-1.5.4/irff/plot/reax_plot.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/reax_plov.py` & `irff-1.5.4/irff/plot/reax_plov.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/rffbd.py` & `irff-1.5.4/irff/plot/rffbd.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/sigmoid.py` & `irff-1.5.4/irff/plot/sigmoid.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/vdw_taper.py` & `irff-1.5.4/irff/plot/vdw_taper.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/plot/view.py` & `irff-1.5.4/irff/plot/view.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/prop/__init__.py` & `irff-1.5.4/irff/prop/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/prop/gofr.py` & `irff-1.5.4/irff/prop/gofr.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/qeq.py` & `irff-1.5.4/irff/qeq.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/reax.py` & `irff-1.5.4/irff/reax.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/reax_data.py` & `irff-1.5.4/irff/reax_data.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/reax_nn.py` & `irff-1.5.4/irff/reax_nn.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/reaxfflib.py` & `irff-1.5.4/irff/reaxfflib.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/spectra.py` & `irff-1.5.4/irff/spectra.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/Al.gen` & `irff-1.5.4/irff/structures/Al.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/C2C4.gen` & `irff-1.5.4/irff/structures/C2C4.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/HMX_MOL.gen` & `irff-1.5.4/irff/structures/HMX_MOL.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/NM.gen` & `irff-1.5.4/irff/structures/NM.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/ball.py` & `irff-1.5.4/irff/structures/ball.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/ball_bulk.py` & `irff-1.5.4/irff/structures/ball_bulk.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/diamond.py` & `irff-1.5.4/irff/structures/diamond.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/fox7.gen` & `irff-1.5.4/irff/structures/fox7.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/structures/nm3.gen` & `irff-1.5.4/irff/structures/nm3.gen`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/__init__.py` & `irff-1.5.4/irff/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/eos_opt.py` & `irff-1.5.4/irff/tools/eos_opt.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/ffield_to_json.py` & `irff-1.5.4/irff/tools/ffield_to_json.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/ffieldtolib.py` & `irff-1.5.4/irff/tools/ffieldtolib.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/fingerprint.py` & `irff-1.5.4/irff/tools/fingerprint.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/fit_hugoniot_state.py` & `irff-1.5.4/irff/tools/fit_hugoniot_state.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/fitnn.py` & `irff-1.5.4/irff/tools/fitnn.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/json_to_ffield.py` & `irff-1.5.4/irff/tools/json_to_ffield.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/morse_taper.py` & `irff-1.5.4/irff/tools/morse_taper.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/pre_opt.py` & `irff-1.5.4/irff/tools/pre_opt.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/prepare_ffield.py` & `irff-1.5.4/irff/tools/prepare_ffield.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/pressure.py` & `irff-1.5.4/irff/tools/pressure.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/pseudo_gen.py` & `irff-1.5.4/irff/tools/pseudo_gen.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/rsetff.py` & `irff-1.5.4/irff/tools/rsetff.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/setwb.py` & `irff-1.5.4/irff/tools/setwb.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/vdw.py` & `irff-1.5.4/irff/tools/vdw.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/tools/zmat_to_atoms.py` & `irff-1.5.4/irff/tools/zmat_to_atoms.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/trainer.py` & `irff-1.5.4/irff/trainer.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff/zmatrix.py` & `irff-1.5.4/irff/zmatrix.py`

 * *Files identical despite different names*

### Comparing `irff-1.5.3/irff.egg-info/SOURCES.txt` & `irff-1.5.4/irff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 irff/LearningMachine.py
 irff/RadiusCutOff.py
 irff/__init__.py
 irff/dingtalk.py
 irff/emdk.py
 irff/fitbo.py
 irff/getNeighbor.c
+irff/getNeighbor.pyx
 irff/getNeighbors.py
 irff/intCheck.py
 irff/irff.py
 irff/irff_np.py
 irff/link.py
 irff/mlqeq.py
 irff/molecule.py
 irff/mpnn.py
 irff/neighbor.c
+irff/neighbor.pyx
 irff/neighbors.py
 irff/qeq.py
 irff/reax.py
 irff/reax_data.py
 irff/reax_nn.py
 irff/reaxfflib.py
 irff/spectra.py
```

### Comparing `irff-1.5.3/setup.py` & `irff-1.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 '''
 install with commond 
   "python setup.py build_ext --inplace"
   "python setup install --user"
 '''
 
 
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 install_requires = ['numpy','ase','tensorflow','matplotlib','paramiko']
 url = "https://gitee.com/fenggo/I-ReaxFF"
 
 
 setup(name="irff",
       version=__version__,
       description="Intelligent Reactive Force Field",
       author="FengGo",
       author_email='fengguo@lcu.edu.cn',
       url=url,
       download_url='{}/archive/{}.tar.gz'.format(url, __version__),
       license="LGPL",
       packages= find_packages(),
-      package_data={'': ['*.gen']},
+      package_data={'': ['*.gen','*.pyx']},
       ext_modules=cythonize(['irff/neighbor.pyx','irff/getNeighbor.pyx'],annotate=True))
```

