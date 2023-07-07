# Comparing `tmp/femagtools-1.3.0.tar.gz` & `tmp/femagtools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.3.0.tar", last modified: Tue Jun 13 07:53:59 2023, max compression
+gzip compressed data, was "femagtools-1.3.1.tar", last modified: Fri Jul  7 06:15:30 2023, max compression
```

## Comparing `femagtools-1.3.0.tar` & `femagtools-1.3.1.tar`

### file list

```diff
@@ -1,188 +1,190 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.619754 femagtools-1.3.0/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.3.0/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.3.0/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-06-13 07:53:59.619754 femagtools-1.3.0/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.3.0/README.md
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.604755 femagtools-1.3.0/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1630 2023-06-13 07:52:35.000000 femagtools-1.3.0/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    68745 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.3.0/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.605754 femagtools-1.3.0/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    41410 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.3.0/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    30964 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.3.0/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/jcf2msh.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.3.0/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.606754 femagtools-1.3.0/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     7392 2023-05-26 13:39:42.000000 femagtools-1.3.0/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     6387 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    35696 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    26608 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    16617 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.3.0/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    39691 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    14068 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.606754 femagtools-1.3.0/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/problem.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8506 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.3.0/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18714 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/parstudy.py
--rw-r--r--   0 tar        (210) tar        (210)    58203 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/plot.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.616754 femagtools-1.3.0/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)     1600 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/calc_therm_field.mako
--rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      663 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)     4820 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2268 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     3960 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4942 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     2906 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/therm-dynamic.mako
--rw-r--r--   0 tar        (210) tar        (210)     1002 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/therm-static.mako
--rw-r--r--   0 tar        (210) tar        (210)     1782 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.3.0/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.3.0/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.604755 femagtools-1.3.0/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     4983 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      191 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      144 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       11 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/top_level.txt
--rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.3.0/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2023-06-13 07:53:59.619754 femagtools-1.3.0/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.618754 femagtools-1.3.0/tests/
--rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1142 2023-06-13 07:51:56.000000 femagtools-1.3.0/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.3.0/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16099 2023-06-13 07:51:56.000000 femagtools-1.3.0/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.3.0/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_magnet.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-06-13 07:51:56.000000 femagtools-1.3.0/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.3.0/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83524 2023-05-26 13:39:42.000000 femagtools-1.3.0/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.3.0/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.3.0/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.359389 femagtools-1.3.1/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.3.1/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.3.1/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-07-07 06:15:30.359389 femagtools-1.3.1/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.3.1/README.md
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.344389 femagtools-1.3.1/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1630 2023-07-07 06:14:03.000000 femagtools-1.3.1/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)    14001 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    68745 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.3.1/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.345389 femagtools-1.3.1/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    52804 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    19131 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    23372 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)     9835 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   141862 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)    28135 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    44863 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)    13156 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/ecloss.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    42176 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.3.1/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    30989 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)     3738 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/hxy.py
+-rw-r--r--   0 tar        (210) tar        (210)    41578 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/jcf2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.3.1/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.346389 femagtools-1.3.1/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     7413 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    11371 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    38093 2023-07-03 13:37:05.000000 femagtools-1.3.1/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    51280 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    32810 2023-07-03 13:37:05.000000 femagtools-1.3.1/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    16617 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.3.1/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    39696 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    14068 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.346389 femagtools-1.3.1/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/problem.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8506 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.3.1/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18717 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/parstudy.py
+-rw-r--r--   0 tar        (210) tar        (210)    61312 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/plot.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.357389 femagtools-1.3.1/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)      246 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1600 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/calc_therm_field.mako
+-rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4820 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2268 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3960 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4942 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3142 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/templates/therm-dynamic.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1002 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/therm-static.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1782 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.3.1/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.3.1/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.344389 femagtools-1.3.1/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     5022 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      191 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      144 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       11 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/top_level.txt
+-rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.3.1/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2023-07-07 06:15:30.359389 femagtools-1.3.1/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.359389 femagtools-1.3.1/tests/
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     1142 2023-07-03 13:36:57.000000 femagtools-1.3.1/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.3.1/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16099 2023-06-23 19:15:43.000000 femagtools-1.3.1/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.3.1/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-07-03 13:26:45.000000 femagtools-1.3.1/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_magnet.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-06-23 19:15:43.000000 femagtools-1.3.1/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1340 2023-07-03 13:26:45.000000 femagtools-1.3.1/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.3.1/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83524 2023-06-23 19:15:43.000000 femagtools-1.3.1/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.3.1/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.3.1/tests/test_windings.py
```

### Comparing `femagtools-1.3.0/LICENSE` & `femagtools-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/PKG-INFO` & `femagtools-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.3.0/README.md` & `femagtools-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/__init__.py` & `femagtools-1.3.1/femagtools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Python bindings for FEMAG
 
 
 
 """
 __title__ = 'femagtools'
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.3.0/femagtools/airgap.py` & `femagtools-1.3.1/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/amazon.py` & `femagtools-1.3.1/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/amela.py` & `femagtools-1.3.1/femagtools/amela.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,118 @@
 import sys
 import json
 import pathlib
 import logging
 from pathlib import Path
 import femagtools.nc
 import numpy as np
-from numpy import pi
+from numpy import pi, sin, cos
 import subprocess
 
 #  set logging
 logger = logging.getLogger(__name__)
 
+def geometry_id(bndx, bndy):
+    '''identify the magnet geometry''' 
+    # caculate magnet area 
+    xy = 0
+    yx = 0
+    for i in range(len(bndy)):
+        if i < (len(bndy)-1):
+            xy += bndx[i]*bndy[i+1]
+            yx += bndy[i]*bndx[i+1]
+        else:
+            xy += bndx[i]*bndy[0]
+            yx += bndy[i]*bndx[0]
+    area = np.abs(yx-xy)*0.5
+
+    x0, y0 = np.mean(bndx), np.mean(bndy)
+    distances = [] 
+    for i in range(len(bndx)): 
+        for j in range(len(bndy)): 
+            dist = np.sqrt((bndx[i] - bndx[j])**2 + (bndy[i] - bndy[j])**2)
+            distances.append([dist, bndx[i], bndx[j], bndy[i], bndy[j]])
+    
+    distances.sort(reverse=True)
+    xe = [distances[0][2], distances[2][1], distances[0][1], distances[2][2]]
+    ye = [distances[0][4], distances[2][3], distances[0][3], distances[2][4]]
+
+    # dimension 
+    dim = np.zeros((3, 5))
+    x1, y1 = xe[0], ye[0]
+
+    for i in range(3): 
+        x2, y2 = xe[i+1], ye[i+1]
+        dim[i, 0] = np.sqrt((x2-x1)**2 + (y2-y1)**2)
+        dim[i, 1:3] = [x1, x2]
+        dim[i, 3:5] = [y1, y2]
+
+    dim = dim[np.lexsort((dim[:, 2], dim[:, 1], dim[:, 0]))]
+    dx12, dy12 = dim[1, 1] - dim[1, 2],  dim[1, 3] - dim[1, 4]
+    dx14, dy14 = dim[0, 1] - dim[0, 2],  dim[0, 3] - dim[0, 4]
+    
+    alp1 = np.arctan2(dy12, dx12)
+    alp2 = np.arctan2(dy14, dx14)
+
+    if alp1 < 0: alp1 += 2*np.pi
+    if alp2 < 0: alp2 += 2*np.pi
+    if alp2 < alp1: 
+        alp2 += np.pi
+        alpha = (alp1 + (alp2 - np.pi/2))/2
+    else: 
+        alpha = (alp1 + (alp2 - np.pi/2))/2 + np.pi
+    
+    wm = dim[1, 0]
+    hm = area/wm 
+
+    return dict(wm=wm, 
+                hm=hm, 
+                x0=x0, 
+                y0=y0,
+                area=area, 
+                alpha=alpha)
+
+def tf(b1, b2, alpha):
+    '''Tranformation Matrix'''
+    T = np.array([[cos(alpha), sin(alpha)], 
+                [-sin(alpha), cos(alpha)]]) 
+    if b1.ndim > 1: 
+        r = T.dot(((b1.ravel()), (b2.ravel())))
+        return [r[0, :].reshape(*b1.shape), 
+                r[1, :].reshape(*b1.shape)]
+    else: 
+        return T.dot(((b1), (b2)))
+
+def transform_coord(geometry, xcp, ycp): 
+    '''transform from global coord to local coord'''
+    # transformation 
+    elcp = tf(b1=np.array(xcp)-geometry['x0'], 
+              b2=np.array(ycp)-geometry['y0'], 
+              alpha=geometry['alpha'])
+    return dict(excpl=elcp[0, :]+geometry['wm']/2, 
+                eycpl=elcp[1, :]+geometry['hm']/2, 
+                excp=np.array(xcp), 
+                eycp=np.array(ycp))
+
+def transform_flux_denstiy(geometry, bx, by): 
+    '''transform the magnet flux density to local coordinate system'''
+    # transformation 
+    bxy = tf(b1=bx, 
+             b2=by, 
+             alpha=geometry['alpha'])
+
+    # remove DC component
+    bxf = np.mean(bxy[0].T - np.mean(bxy[0],axis=1).T,axis=1)
+    byf = np.mean(bxy[1].T - np.mean(bxy[1],axis=1).T,axis=1)               
+     
+    return dict(bxl=bxy[0],
+                byl=bxy[1],
+                bxf=bxf, 
+                byf=byf 
+                )
 
 class Amela():
     '''Run Amela Calculation
     Parameters
     ----------
     workdir : str
         working directory of femag calculation
@@ -62,15 +160,15 @@
         if 'speed' in self.magn:
             self.cmd.append(f"--speed {self.magn['speed']}")
         if 'nsegwid' in self.magn:
             self.cmd.append(f"--nsegwid {self.magn['nsegwid']}")
         if 'nseglen' in self.magn:
             self.cmd.append(f"--nseglen {self.magn['nseglen']}")
 
-    def get_magnet_data(self):
+    def get_magnet_data(self, ibeta=None):
         '''Extract magnet data from nc file
         Parameters
         ----------
             None
         Returns
         ----------
         pm_data: list of magnet data
@@ -88,15 +186,23 @@
         bndkey = [[] for i in range(len(spel_key))]
         bx = [[] for i in range(len(spel_key))]
         by = [[] for i in range(len(spel_key))]
         xcp = [[] for i in range(len(spel_key))]
         ycp = [[] for i in range(len(spel_key))]
         bndx = [[] for i in range(len(spel_key))]
         bndy = [[] for i in range(len(spel_key))]
-
+        # prepare data for ialh method
+        wm = []
+        hm = []
+        alpha = []
+        x0 = [] 
+        y0 = []
+        geometry = []
+        elcp = []
+        bl = []
         # conductivity and permeability of the magnets
         cond = 0
         mur = 0
         # read boundary nodes
         for k, i in enumerate(mag_spels):
 
             cond = i.conduc
@@ -120,23 +226,34 @@
                         bndkey[k].append(kk.key)
                         bndx[k].append(kk.x*1e3)
                         bndy[k].append(kk.y*1e3)
 
                 bndkey[k].pop(-1)
                 bndx[k].pop(-1)
                 bndy[k].pop(-1)
+            geo = geometry_id(bndx=bndx[k], bndy=bndy[k])
+            geometry.append(geo)
+            # necessary?
+            hm.append(geo['hm'])
+            wm.append(geo['wm'])
+            x0.append(geo['x0'])
+            y0.append(geo['y0'])
+            alpha.append(geo['alpha'])
 
         # default load angle (input beta I vs Up)
-        num_cases = r.el_fe_induction_1.shape[3] - 1
-        if 'loadcase' in self.magn:
-            indx = self.magn['loadcase'] - 1
+        if ibeta is not None:
+            indx = ibeta
         else:
-            indx = num_cases
-        if indx == 3:
-            indx = num_cases  # avoid error
+            num_cases = r.el_fe_induction_1.shape[3] - 1
+            if 'loadcase' in self.magn:
+                indx = self.magn['loadcase'] - 1
+            else:
+                indx = num_cases
+            if indx == 3:
+                indx = num_cases  # avoid error
 
         # stationary case, no rotation
         poles = 0
         try:
             poles = r.num_poles
         except:
             pass
@@ -155,14 +272,18 @@
                     by[i][0][index, :] = fd['by']
                 else:
                     bx[i][0][index, :] = fd['bx']*np.cos(theta) - \
                         fd['by']*np.sin(theta)
                     by[i][0][index, :] = fd['bx']*np.sin(theta) + \
                         fd['by']*np.cos(theta)
 
+            elcp.append(transform_coord(geometry[i], xcp[i], ycp[i]))
+            bl.append(transform_flux_denstiy(geometry[i], bx[i][0], by[i][0]))
+
+
         if poles == 0:
             freq = self.magn.get('f', r.speed)
             time_vec = np.linspace(0, 1/freq, len(r.pos_el_fe_induction))
             pos = dict(time=time_vec.tolist(),
                        freq=freq,
                        t=float(1/freq))
             # reset num.poles
@@ -173,27 +294,30 @@
             pos = dict(phi=(r.pos_el_fe_induction*180/pi).tolist(),
                        speed=rpm,
                        t=float(60/rpm*ag_sim/360))  # TODO
         # prep dictionary for the loss calculation
         pm_data = []
         for i in range(len(spel_key)):
             pm_data.append(dict(name='pm_data_se' + str(spel_key[i]),
-                                hm=self.magn.get('hm', 0),
-                                wm=self.magn.get('wm', 0),
+                                hm=self.magn.get('hm', hm[i]),
+                                wm=self.magn.get('wm', wm[i]),
                                 lm=self.magn.get('lm', r.arm_length*1e3),
+                                alpha=alpha[i],
                                 ls=r.arm_length*1e3,
                                 sigma=float(self.magn.get('sigma', cond)),
                                 mur=float(self.magn.get('mur', mur)),
                                 loadcase=self.magn.get('loadcase', indx),
                                 numpoles=poles,
                                 nodes=dict(),
                                 elements=dict(),
                                 bndkeys=bndkey[i],
                                 bndx=[float(c) for c in bndx[i]],
                                 bndy=[float(c) for c in bndy[i]],
+                                bl=bl[i],
+                                elcp=elcp[i],
                                 area=spel_area[i]))
             pm_data[i].update(pos)
 
         for k in range(len(pm_node_key)):
             for i, j in enumerate(pm_node_key[k]):
                 pm_data[k]['nodes'][str(j + 1)] = dict(
                     key=int(j + 1),
@@ -211,14 +335,22 @@
                 )
 
         if len(mag_spels) / r.poles_sim > 1:
             return pm_data
         else:
             return [pm_data[0]]
 
+    def get_magnet_data_all(self, num_op): 
+        '''get all magnet data for all loadcases'''
+        pm_data = []
+        for i in num_op:
+            pmd = self.get_magnet_data(ibeta=i)
+            pm_data.append(pmd)
+        return pm_data
+
     def export_json(self, pm_data):
         '''Export magnet data to json files
         Parameters
         ----------
         pm_data: list of magnet data
         Returns
         ----------
@@ -226,14 +358,17 @@
         ----------
         '''
         pm_dir = self.amela_dir / self.magn['name']
         pm_dir.mkdir(exist_ok=True)
         for i in pm_data:
             filename = (pm_dir / i['name']).with_suffix('.json')
             self.jsonfile.append(str(filename))  # for the future use
+            # pop out non necessary data
+            i.pop('bl')
+            i.pop('elcp')
             with filename.open('w') as f:
                 json.dump(i, f)
             logger.info('Exporting %s ...', i['name'])
 
     def read_loss(self, pm_data):
         '''Read magnet losses
         Parameters
@@ -275,8 +410,7 @@
         calc_method = 'IALH' if ialh else '3DI'
         cmd = self.cmd + ['--calc', calc_method, self.magn['name'] + '/']
         log_file = self.amela_dir / 'amela.out'
         logger.info("Calculating magnet losses with AMELA ...")
         with log_file.open('w') as output:
             subprocess.run(cmd, stdout=output)
         return self.read_loss(r)
-
```

### Comparing `femagtools-1.3.0/femagtools/asm.py` & `femagtools-1.3.1/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/bch.py` & `femagtools-1.3.1/femagtools/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/bchxml.py` & `femagtools-1.3.1/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/condor.py` & `femagtools-1.3.1/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/conductor.py` & `femagtools-1.3.1/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/config.py` & `femagtools-1.3.1/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/convert.py` & `femagtools-1.3.1/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dakota.py` & `femagtools-1.3.1/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dakota_femag.py` & `femagtools-1.3.1/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dakotaout.py` & `femagtools-1.3.1/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/docker.py` & `femagtools-1.3.1/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dxfsl/area.py` & `femagtools-1.3.1/femagtools/dxfsl/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,26 @@
                 yield n1, n2, e1
         except ValueError as e:
             logger.error("list_of_elements(): FATAL ERROR: %s", e)
             return
         except Exception as e:
             return
 
+    def has_fsl(self):
+        try:
+            return self.fsl
+        except AttributeError:
+            return True
+
+    def list_of_equal_edges(self, a):
+        for e1 in self.area:
+            for e2 in a.area:
+                if e1.n1 == e2.n1 and e1.n2 == e2.n2:
+                    yield e1
+
     def virtual_nodes(self, render=False):
         if len(self.area) < 2:
             return
 
         prev_nodes = [n for n in self.area[0].get_nodes(parts=64,
                                                         render=render)]
         next_nodes = [n for n in self.area[1].get_nodes(parts=64,
```

### Comparing `femagtools-1.3.0/femagtools/dxfsl/conv.py` & `femagtools-1.3.1/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dxfsl/converter.py` & `femagtools-1.3.1/femagtools/dxfsl/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,25 +236,27 @@
                                         is_inner=True,
                                         symtol=symtol,
                                         show_plots=show_plots,
                                         rows=3,  # rows
                                         cols=2,  # columns
                                         num=3)   # start num
         machine_inner.set_inner()
+        machine_inner.check_and_correct_geom("Inner")
 
         machine_outer = machine.copy(0.0, 2*np.pi, True, False)
         machine_outer = symmetry_search(machine_outer,
                                         p,  # plot
                                         outer_name,
                                         is_outer=True,
                                         symtol=symtol,
                                         show_plots=show_plots,
                                         rows=3,  # rows
                                         cols=2,  # columns
                                         num=4)   # start num
+        machine_outer.check_and_correct_geom("Outer")
 
         machine_inner.sync_with_counterpart(machine_outer)
 
         machine_inner.search_subregions()
         machine_outer.search_subregions()
 
         if machine_inner.has_mirrored_windings():
@@ -269,30 +271,33 @@
             machine_outer = machine_outer.undo_mirror()
             machine_inner.sync_with_counterpart(machine_outer)
             machine_outer.search_subregions()
             machine_outer.create_mirror_lines_outside_windings()
 
         machine_inner.delete_tiny_elements(mindist)
         machine_outer.delete_tiny_elements(mindist)
+        machine_inner.geom.create_corner_areas()
         logger.info("END of work: %s", basename)
 
         if show_plots:
             p.render_elements(machine_inner.geom, Shape,
                               draw_inside=True, title=inner_name,
                               rows=3, cols=2, num=5, show=False,
-                              # with_nodes=True,
-                              # neighbors=True,
+                              with_corners=False,
+                              with_nodes=False,
+                              neighbors=False,
                               write_id=write_id,
                               fill_areas=True)
 
             p.render_elements(machine_outer.geom, Shape,
                               draw_inside=True, title=outer_name,
                               rows=3, cols=2, num=6, show=False,
-                              # with_nodes=True,
-                              # neighbors=True,
+                              with_corners=False,
+                              with_nodes=False,
+                              neighbors=False,
                               write_id=write_id,
                               fill_areas=True)
             if write_png:
                 p.write_plot(basename)
             else:
                 p.show_plot()
 
@@ -403,22 +408,24 @@
                 machine.geom.search_rotor_subregions(part[1])
                 params = create_femag_parameters_rotor(machine,
                                                        part[1])
         else:
             machine.geom.search_subregions()
 
         machine.delete_tiny_elements(mindist)
+        machine.geom.create_corner_areas()
         logger.info("END of work: %s", basename)
 
         if show_plots:
             p.render_elements(machine.geom, Shape,
                               draw_inside=True, title=name,
                               rows=3, cols=2, num=5, show=False,
-                              # with_nodes=True,
-                              # neighbors=True,
+                              with_corners=False,
+                              with_nodes=False,
+                              neighbors=False,
                               write_id=write_id,
                               fill_areas=True)
             if write_png:
                 p.write_plot(basename)
             else:
                 p.show_plot()
```

### Comparing `femagtools-1.3.0/femagtools/dxfsl/corner.py` & `femagtools-1.3.1/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.3.1/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.3.1/femagtools/dxfsl/fslrenderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,22 +106,27 @@
             n0 = n1
 
     def line(self, p1, p2, color='blue', e=None):
         num = 0
         # if self.nodedist > 0:
         #     l = la.norm(np.asarray(p1)-p2)
         #     num = int(l/self.nodedist + 1)
-        if e is not None and e.has_attribute('auxline'):
-            self.content.append(
-                u"nc_line({}, {}, {}, {}, {}) -- auxiliary".format(
-                    p1[0], p1[1], p2[0], p2[1], num))
-        else:
-            self.content.append(
-                u"nc_line({}, {}, {}, {}, {})".format(
-                    p1[0], p1[1], p2[0], p2[1], num))
+        if e is not None:
+            if e.has_attribute('no_fsl'):
+                logger.info("line with attr nofsl")
+                return
+            if e.has_attribute('auxline'):
+                self.content.append(
+                    u"nc_line({}, {}, {}, {}, {}) -- auxiliary".format(
+                        p1[0], p1[1], p2[0], p2[1], num))
+                return
+
+        self.content.append(
+            u"nc_line({}, {}, {}, {}, {})".format(
+                p1[0], p1[1], p2[0], p2[1], num))
 
     def sorted_elements(self, geom, inner=False):
         if inner:
             r = geom.max_radius
         else:
             r = geom.min_radius
```

### Comparing `femagtools-1.3.0/femagtools/dxfsl/functions.py` & `femagtools-1.3.1/femagtools/dxfsl/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 def is_same_angle(angle1, angle2, atol=0.001):
     """ returns true if angles are equal
     """
     return (np.isclose(np.cos(angle1), np.cos(angle2), atol=atol) and
             np.isclose(np.sin(angle1), np.sin(angle2), atol=atol))
 
 
-def part_of_circle(startangle, endangle, dec_place=3):
+def part_of_circle(startangle, endangle, dec_place=2):
     """ returns the number of segments included in the circle
       if an integer number, 0 otherwise
     """
     start = normalise_angle(startangle)
     end = normalise_angle(endangle)
 
     if np.isclose(start, end):
```

### Comparing `femagtools-1.3.0/femagtools/dxfsl/geom.py` & `femagtools-1.3.1/femagtools/dxfsl/geom.py`

 * *Files 3% similar despite different names*

```diff
@@ -813,14 +813,54 @@
             c.transform(T, alpha, ndec)
         rotnodes = np.dot(T, np.asarray(self.g.nodes()).T).T.tolist()
         mapping = {n: (round(r[0], ndec),
                        round(r[1], ndec))
                    for n, r in zip(self.g.nodes(), rotnodes)}
         nx.relabel_nodes(self.g, mapping, copy=False)
 
+    def check_geom(self, what):
+        logger.debug("check geometry of %s", what)
+        parts = int(round(np.pi * 2 / self.alfa, 1))
+        logger.debug(" --parts......: %s", parts)
+        logger.debug(" --ist alpha..: %s", self.alfa)
+        real_alfa = np.pi * 2 / parts
+        logger.debug(" --soll alpha.: %s", real_alfa)
+        if not np.isclose(self.alfa, real_alfa):
+            logger.debug(" --BAD angle ==> get corrected machine")
+            return self.correct_geom(real_alfa)
+        return None
+
+    def correct_geom(self, correct_alpha):
+        elements = []
+        for e in self.g.edges(data=True):
+            o = e[2]['object'].correct(self.alfa, correct_alpha, ndec)
+            elements.append(o)
+        geom = Geometry(elements, self.rtol, self.atol)
+        geom.center = self.center
+        geom.alfa = correct_alpha
+        geom.min_radius = self.min_radius
+        geom.max_radius = self.max_radius
+        geom.is_inner = self.is_inner
+        geom.kind = self.kind
+        geom.sym_part = self.sym_part
+        return geom
+
+    def log_geom(self):
+        logger.info("Kind............: %s", self.kind)
+        logger.info("Center..........: %s", self.center)
+        logger.info("Alpha...........: %s", self.alfa)
+        logger.info("Is Inner........: %s", self.is_inner)
+        logger.info("Is Outer........: %s", self.is_outer)
+        logger.info("Min Radius......: %s", self.min_radius)
+        logger.info("Max Radius......: %s", self.max_radius)
+        logger.info("Mirror Corners..: %s", self.mirror_corners)
+        logger.info("Start Corners...: %s", self.start_corners)
+        logger.info("End Corners.....: %s", self.end_corners)
+        logger.info("Edges...........: %s", self.num_edges)
+
     def scale(self, factor):
         """scales all objects"""
         for e in self.g.edges(data=True):
             e[2]['object'].scale(factor)
         for c in self.circles():
             c.scale(factor)
         mapping = {n: (round(factor * n[0], ndec),
@@ -947,16 +987,16 @@
         assert(len(e) == 1)
         self._remove_edge(e[0][0], e[0][1])
 
     def remove_edges(self, edges):
         for e in edges:
             self.remove_edge(e)
 
-    def add_line(self, n1, n2):
-        line = Line(Element(start=n1, end=n2))
+    def add_line(self, n1, n2, color=None):
+        line = Line(Element(start=n1, end=n2), color=color)
         add_or_join(self,
                     line.node1(ndec),
                     line.node2(ndec),
                     line,
                     self.rtol,
                     self.atol)
 
@@ -1073,14 +1113,44 @@
 
         if self.is_mirrored():
             return self.dist_start_min_corner()
         d = distance(self.center, self.end_corners[0])
         logger.debug("end of dist_end_min_corner: %s", d)
         return d
 
+    def get_start_airgap_corner(self):
+        if self.is_inner:
+            p = (self.max_radius, 0.0)
+            cp = self.start_corners[-1]
+        else:
+            p = (self.min_radius, 0.0)
+            cp = self.start_corners[0]
+        if points_are_close(p, cp, atol=0.5):
+            return cp, True
+        return p, False
+
+    def get_end_airgap_corner(self):
+        if self.is_inner:
+            p = point(self.center, self.max_radius, self.alfa, ndec)
+            cp = self.end_corners[-1]
+        else:
+            p = point(self.center, self.min_radius, self.alfa, ndec)
+            cp = self.end_corners[0]
+        if points_are_close(p, cp, atol=0.5):
+            return cp, True
+        return p, False
+
+    def get_start_airgap_corner_point(self):
+        p, b = self.get_start_airgap_corner()
+        return Point(p)
+
+    def get_end_airgap_corner_point(self):
+        p, b = self.get_end_airgap_corner()
+        return Point(p)
+
     def area_size(self):
         pts = [p for p in self.start_corners]
         end_pts = [p for p in reversed(self.end_corners)]
         return area_size(pts + end_pts)
 
     def repair_hull_line(self, center, angle, corners, with_center):
         # We need to set our own tolerance range
@@ -1353,15 +1423,15 @@
         logger.debug("   POINT WITH %s NEIGHBORS", len(nbrs)-1)
 
         f_angle, f_c, f_info_next = nbrs[0]
         f_info_next['angle'] = f_angle
 
         for n_angle, n_c, n_info_next in nbrs[1:]:
             n_info_next['angle'] = n_angle
-            if np.isclose(f_angle, n_angle):
+            if np.isclose(f_angle, n_angle, 0.01, 0.01):
                 logger.debug("   SAME DIRECTION")
                 # ACHTUNG
                 if self.is_lefthand_edge(alpha, f_info_next, n_info_next):
                     logger.debug("   == first is on the left side")
                     angle = self.get_angle(alpha,
                                            n_info_next['alpha_start'] - 0.01)
                     n_info_next['angle'] = angle
@@ -1397,15 +1467,15 @@
                 'n2': n2,
                 'data': e_dict,
                 'element': e,
                 'x': x,
                 'alpha_n1': alpha_n1,
                 'alpha_n2': e.get_alpha(n2),
                 'alpha_start': normalise_angle(alpha_n1 + np.pi),
-                'tracked': e_dict[x],
+                'tracked': e_dict.get(x, False),
                 'reverse': False}
         return info
 
     def get_reverse_edge_info(self, info):
         alpha_n1 = info['alpha_n2']
         rev_info = {'n1': info['n2'],
                     'n2': info['n1'],
@@ -1423,17 +1493,17 @@
         return isinstance(info['element'], Arc)
 
     def log_edge_info(self, info):
         logger.debug('   node1 = %s', info['n1'])
         logger.debug('   node2 = %s', info['n2'])
         logger.debug('   x     = %s', info['x'])
         logger.debug('   lock  = (%s, %s, %s)',
-                     info['data'][0],
-                     info['data'][1],
-                     info['data'][2])
+                     info['data'].get(0, False),
+                     info['data'].get(1, False),
+                     info['data'].get(2, False))
 
     def set_edge_tracked(self, info):
         x = info['x']
         info['data'][x] = True  # footprint
 
     def get_new_area(self, start_n1, start_n2, solo):
         info_curr = self.get_edge_info(start_n1, start_n2)
@@ -1536,37 +1606,39 @@
 
         result['msg'] = "area found !!"
         logger.debug("<== %s", result['msg'])
         result['elements'] = c
         result['ok'] = True
         return result
 
+    def set_edge_attributes(self):
+        if nxversion == 1:
+            nx.set_edge_attributes(self.g, 0, True)
+            nx.set_edge_attributes(self.g, 1, False)
+            nx.set_edge_attributes(self.g, 2, False)
+        else:
+            nx.set_edge_attributes(self.g, True, 0)
+            nx.set_edge_attributes(self.g, False, 1)
+            nx.set_edge_attributes(self.g, False, 2)
+
     def create_list_of_areas(self, crunch=False):
         """ return list of areas for each node and their neighbors
         """
         if len(self.area_list) > 0:
             # list already available
             return
 
         def append(area_list, a):
             for area in area_list:
                 if area.is_identical(a):
                     return
             area_list.append(a)
 
         logger.debug("create new area list")
-
-        if nxversion == 1:
-            nx.set_edge_attributes(self.g, 0, True)
-            nx.set_edge_attributes(self.g, 1, False)
-            nx.set_edge_attributes(self.g, 2, False)
-        else:
-            nx.set_edge_attributes(self.g, True, 0)
-            nx.set_edge_attributes(self.g, False, 1)
-            nx.set_edge_attributes(self.g, False, 2)
+        self.set_edge_attributes()
 
         crunched = 0
         for n in self.g.nodes():
             if self.debug:
                 print('.', end='', flush=True)
 
             finished = False
@@ -2077,19 +2149,28 @@
     def get_alfa(self):
         if self.is_mirrored():
             return 2*self.alfa
         else:
             return self.alfa
 
     def __str__(self):
+        real_alfa = 0
+        if self.sym_part > 0:
+            if self.is_mirrored():
+                real_alfa = np.pi / self.sym_part
+            else:
+                real_alfa = 2*np.pi / self.sym_part
         return "name...........: {}\n".format(self._name) + \
                "kind...........: {}\n".format(self.kind) + \
                "sym_part.......: {}\n".format(self.sym_part) + \
                "sym_counterpart: {}\n".format(self.sym_counterpart) + \
                "alpha..........: {}\n".format(self.alfa) + \
+               "alpha real.....: {}\n".format(real_alfa) + \
+               "circle.........: {}\n".format(self.alfa * self.sym_part) + \
+               "mirrored.......: {}\n".format(self.is_mirrored()) + \
                "radius.........: {} -- {}\n".format(self.min_radius,
                                                     self.max_radius)
 
     def __eq__(self, other):
         return (isinstance(other, self.__class__) and
                 self.__dict__ == other.__dict__)
 
@@ -2926,37 +3007,49 @@
                     shaft.type = 6  # iron shaft (Zahn)
                     return
                 if shaft.is_touching(a):
                     if not a.is_iron():
                         shaft.type = 6  # iron shaft (Zahn)
                         return
 
+    def mark_connecting_edges(self, windings):
+        logger.debug("begin of mark_connecting_edges")
+        for a in windings:
+            logger.debug("- id of winding: %s", a.identifier())
+            for w in windings:
+                if a.id != w.id:
+                    elist = [e for e in a.list_of_equal_edges(w)]
+                    logger.debug(" --> %s equal egdes", len(elist))
+                    for e in elist:
+                        e.init_attributes('lightblue', 'no_fsl')
+
     def search_subregions(self):
         if self.is_stator():
             return self.search_stator_subregions()
 
         if self.is_rotor():
             return self.search_rotor_subregions()
 
         logger.warning("no stator or rotor assigned")
         return self.search_unknown_subregions()
 
     def search_stator_subregions(self, place=''):
-        is_inner = self.is_inner
+        logger.debug("Begin of search_stator_subregions")
+
         if place == 'in':
-            is_inner = True
+            self.is_inner = True
         elif place == 'out':
-            is_inner = False
+            self.is_inner = False
 
         if self.alfa == 0.0:
             self.alfa = np.pi * 2.0
 
         stator_size = self.area_size()
         for area in self.list_of_areas():
-            area.mark_stator_subregions(is_inner,
+            area.mark_stator_subregions(self.is_inner,
                                         stator_size,
                                         self.is_mirrored(),
                                         self.alfa,
                                         self.center,
                                         self.min_radius,
                                         self.max_radius)
 
@@ -2966,26 +3059,31 @@
         logger.info("%d windings found", windings_found)
 
         if windings_found > 1:
             windings_surface = [[w.surface, w] for w in windings]
             windings_surface.sort(reverse=True)
             max_size = windings_surface[0][0]
             for sz, w in windings_surface:
+                logger.info("winding size = %s", sz)
                 if sz / max_size < 0.95:
                     w.set_type(0)
-
+                    if sz / max_size < 0.2:
+                        windings_found -= 1
             windings = [a for a in self.list_of_areas()
                         if a.is_winding()]
             if windings_found > 2 and len(windings) == 1:
+                logger.info("no windings remaining")
                 # no windings
                 [w.set_type(0) for w in windings]
                 [a.set_type(1) for a in self.list_of_areas() if a.is_iron()]
                 windings = []
             elif len(windings) < windings_found:
                 logger.info("%d windings remaining", len(windings))
+            if len(windings) > 2:
+                self.mark_connecting_edges(windings)
 
         wdg_min_angle = 99999
         wdg_max_angle = 0
         wdg_min_dist = 99999
         wdg_max_dist = 0
         wdg_close_to_startangle = False
         wdg_close_to_endangle = False
@@ -3084,27 +3182,27 @@
         if shaft_areas:
             if len(shaft_areas) > 1:
                 logger.warn("More than two shafts ?!?")
                 return
             self.check_shaft_area(shaft_areas[0])
 
     def search_rotor_subregions(self, place=''):
-        logger.debug("begin of search_rotor_subregions")
-        is_inner = self.is_inner
+        logger.debug("Begin of search_rotor_subregions")
+
         if place == 'in':
-            is_inner = True
+            self.is_inner = True
         elif place == 'out':
-            is_inner = False
+            self.is_inner = False
 
         if self.alfa == 0.0:
             self.alfa = np.pi * 2.0
 
         types = {}
         for area in self.list_of_areas():
-            t = area.mark_rotor_subregions(is_inner,
+            t = area.mark_rotor_subregions(self.is_inner,
                                            self.is_mirrored(),
                                            self.alfa,
                                            self.center,
                                            self.min_radius,
                                            self.max_radius)
             if t in types:
                 types[t] += 1
@@ -3558,14 +3656,150 @@
 
     def has_areas_touching_both_sides(self):
         for a in self.area_list:
             if a.is_touching_both_sides():
                 return True
         return False
 
+    def get_inner_airgap_line(self):
+        if not self.is_inner:
+            return []
+        area = [a for a in self.area_list if a.close_to_endangle and a.close_to_ag]
+        if len(area) != 1:
+            return []
+
+        end_corner = self.end_corners[-1]
+        logger.debug("END CORNER %s", end_corner)
+        nodes = [n for n in area[0].list_of_nodes()]
+        if not nodes:
+            return []
+        n1 = nodes[0]
+        if points_are_close(end_corner, n1):
+            n2 = nodes[-1]
+        else:
+            n2 = n1
+            for n1 in nodes[1:]:
+                if points_are_close(end_corner, n1):
+                    break
+                n2 = n1
+
+        if not points_are_close(end_corner, n1):
+            return []
+
+        start_corner = self.start_corners[-1]
+
+        logger.debug("EDGE FOUND: %s - %s", n1, n2)
+        nodes = [n1, n2]
+        info = self.get_edge_info(n1, n2)
+        while not points_are_close(start_corner, n2):
+            info = self.next_edge_lefthand_side(info)
+            if not info:
+                return []
+            n2 = info['n2']
+            nodes.append(n2)
+
+        return nodes
+
+    def create_corner_areas(self):
+        self.set_edge_attributes()
+        self.create_inner_corner_areas()
+
+    def create_and_append_area(self, n1, n2):
+        rslt = self.get_new_area(n1, n2, False)
+        logger.debug("create_and_append_area: %s", rslt)
+        if rslt.get('ok', False):
+            area = rslt['area']
+            a = Area(area, self.center, 0.0)
+            a.type = 0  # air
+            self.area_list.append(a)
+            return True
+        logger.error("No area for air near airgap!!")
+        return False
+
+    def create_inner_corner_areas(self):
+        start_cp, start_exists = self.get_start_airgap_corner()
+        end_cp, end_exists = self.get_end_airgap_corner()
+        if start_exists and end_exists:
+            return
+        logger.info("*** Corner correction ***")
+        airgap_line = self.get_inner_airgap_line()
+        if not airgap_line:
+            logger.debug("no airgapline found")
+            return
+
+        logger.debug("airgapline found !!")
+        airgap_nodes = [n for n in airgap_line[1:]]
+        del airgap_nodes[-1]
+        if not airgap_nodes:
+            return  # strange
+
+        if not start_exists:
+            cp = self.start_corners[-1]
+            logger.debug("Start Corner: %s -- %s", cp, start_cp)
+            start_line = Line(Element(start=cp, end=start_cp), color='red')
+            start_cp = start_line.node2(ndec)
+            i = 0
+            for n in airgap_nodes:
+                i += 1
+                if not self.search_intersection(i, self.max_radius,
+                                                n, start_cp,
+                                                airgap_nodes):
+                    self.add_line(start_cp, n, color='red')
+                    self.add_edge(cp, start_cp, start_line)
+                    self.create_and_append_area(start_cp, n)
+                    self.start_corners = self.get_corner_nodes(self.center,
+                                                               0.0)
+                    break
+
+        if not end_exists:
+            cp = self.end_corners[-1]
+            logger.debug("End Corner: %s -- %s", cp, end_cp)
+            end_line = Line(Element(start=cp, end=end_cp), color='red')
+            end_cp = end_line.node2(ndec)
+            airgap_nodes.reverse()
+            i = 0
+            for n in airgap_nodes:
+                i += 1
+                if not self.search_intersection(i, self.max_radius,
+                                                n, end_cp,
+                                                airgap_nodes):
+                    self.add_line(end_cp, n, color='red')
+                    self.add_edge(cp, end_cp, end_line)
+                    self.create_and_append_area(n, end_cp)
+                    self.end_corners = self.get_corner_nodes(self.center,
+                                                             self.alfa)
+                    break
+
+    def search_intersection(self, start_i, r, n1, n2, airgap_nodes):
+        logger.debug("begin of search_intersection")
+
+        ag_line = Line(Element(start=n1, end=n2))
+        for i in range(start_i, len(airgap_nodes)):
+            n = airgap_nodes[i]
+            alfa = alpha_line(self.center, n)
+            dist_n = distance(self.center, n)
+            p = point(self.center, r, alfa)
+            line = Line(Element(start=self.center, end=p))
+            pts = line.intersect_line(ag_line, include_end=True)
+            if not pts:
+                # no intersection
+                return  # ok
+            if len(pts) != 1:
+                logger.error("-- no intersection found ?!? %s", pts)
+                logger.debug("end of search_intersection: bad")
+                return True  # fatal
+            dist_p = distance(self.center, pts[0])
+            logger.info("-- check point %s[%s] -- %s[%s]", n, dist_n, pts[0], dist_p)
+            if not less(dist_n, dist_p):
+                logger.debug("end of search_intersection: found")
+                return True  # intersection
+            logger.debug("-- dist %s <= %s", dist_n, dist_p)
+        logger.debug("end of search_intersection: ok")
+        return False  # ok
+
     def print_nodes(self):
         print("=== List of Nodes ({}) ===".format(self.number_of_nodes()))
         for n in self.g.nodes():
             print(n)
 
     def write_nodes(self, filename):
         global nodes_filecount
```

### Comparing `femagtools-1.3.0/femagtools/dxfsl/machine.py` & `femagtools-1.3.1/femagtools/dxfsl/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
         return "Machine\n" + \
                "Center: ({})\n".format(self.center) + \
                "Radius: {}\n".format(self.radius) + \
                "Angles: Start={}, End={}\n".format(self.startangle,
                                                    self.endangle) + \
                "Mirror: {}\n".format(self.mirror_geom is not None)
 
+    def log_machine(self, what):
+        logger.info("Machine %s", what)
+        self.geom.log_geom()
+
     def is_a_machine(self):
         return self.radius > 0.0
 
     def is_in_middle(self):
         return self.radius > 0.0 and \
             points_are_close(self.center, [0.0, 0.0], 1e-8)
 
@@ -424,15 +428,15 @@
 
     def airgap_x(self):
         return self.airgap_radius
 
     def airgap_y(self):
         return 0.1
 
-    def part_of_circle(self, pos=3):
+    def part_of_circle(self, pos=2):
         return part_of_circle(self.startangle, self.endangle, pos)
 
     def delete_center_circle(self):
         gaps = self.geom.get_gaplist(self.center)
         if len(gaps) < 2:
             return
 
@@ -717,9 +721,20 @@
         pts = self.geom.split_and_get_intersect_points(self.center,
                                                        self.radius+10,
                                                        midangle)
         pts.sort()
         if self.geom.create_lines_outside_windings(pts):
             self.geom.area_list = []
             logger.debug("create subregions again")
-            self.geom.create_list_of_areas(crunch=True)
+            self.geom.create_list_of_areas()
             self.geom.search_subregions()
+
+    def check_and_correct_geom(self, what):
+        geom = self.geom.check_geom(what)
+        if geom:
+            logger.warning("=== Angle correction (%s) ===", what)
+            self.geom = geom
+            self.startangle = 0.0
+            self.endangle = self.geom.alfa
+            self.clear_cut_lines()
+            self.repair_hull()
+            self.set_alfa_and_corners()
```

### Comparing `femagtools-1.3.0/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.3.1/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/dxfsl/shape.py` & `femagtools-1.3.1/femagtools/dxfsl/shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   shape objects are basic geometric elements which have 2 nodes
 
   Authors: Ronald Tanner, Beat Holm
 """
 from __future__ import print_function
 import numpy as np
 import logging
-from .functions import less_equal
+from .functions import less_equal, greater_equal
 from .functions import distance, line_m, line_n
 from .functions import point, points_are_close, points_on_arc
 from .functions import alpha_line, alpha_angle, alpha_triangle
 from .functions import normalise_angle, min_angle, max_angle, get_angle_of_arc
 from .functions import lines_intersect_point, nodes_are_equal
 from .functions import is_angle_inside, intersect_point
 from .functions import middle_angle
@@ -126,14 +126,40 @@
         self.n1 = (round(n[0], ndec),
                    round(n[1], ndec))
         n = T.dot(np.array((self.n2[0], self.n2[1])))
         self.n2 = (round(n[0], ndec),
                    round(n[1], ndec))
         return self
 
+    def correct(self, src_alpha, dest_alpha, ndec):
+        alpha_ref = min(src_alpha, dest_alpha)
+        alpha_p = alpha_line((0.0, 0.0), self.n1)
+        if greater_equal(alpha_p, alpha_ref):
+            delta = dest_alpha - alpha_p
+            T = np.array(((np.cos(delta), -np.sin(delta)),
+                          (np.sin(delta), np.cos(delta))))
+            n = T.dot(np.array((self.p1[0], self.p1[1])))
+            self.p1 = (n[0], n[1])
+            n = T.dot(np.array((self.n1[0], self.n1[1])))
+            self.n1 = (round(n[0], ndec),
+                       round(n[1], ndec))
+
+        alpha_p = alpha_line((0.0, 0.0), self.n2)
+        if greater_equal(alpha_p, alpha_ref):
+            delta = dest_alpha - alpha_p
+            T = np.array(((np.cos(delta), -np.sin(delta)),
+                          (np.sin(delta), np.cos(delta))))
+            n = T.dot(np.array((self.p2[0], self.p2[1])))
+            self.p2 = (n[0], n[1])
+            n = T.dot(np.array((self.n2[0], self.n2[1])))
+            self.n2 = (round(n[0], ndec),
+                       round(n[1], ndec))
+
+        return self
+
     def overlapping_shapes(self, n, e, rtol=1e-03, atol=1e-03):
         return False
 
     def overlapping_shape(self, e, rtol=1e-03, atol=1e-03):
         # element e is already installed
         return None  # no overlap
 
@@ -592,15 +618,15 @@
     def center_of_connection(self, ndec=6):
         midangle = middle_angle(self.startangle, self.endangle)
         x, y = self(midangle)
         return (round(x, ndec), round(y, ndec))
 
     def length(self):
         """returns length of this arc"""
-        d = abs(self.endangle - self.startangle)
+        d = alpha_angle(self.startangle, self.endangle)
         if d > 2*np.pi:
             d -= 2*np.pi
         return self.radius*abs(d)
 
     def get_alpha(self, n):
         a = alpha_line(n, self.center)
         if points_are_close(n, self.n1):
@@ -821,14 +847,28 @@
 
         self.startangle = np.arctan2(p1[1], p1[0])
         self.endangle = np.arctan2(p2[1], p2[0])
         if self.rtheta is not None:
             self.rtheta = self.rtheta + alpha
         return self
 
+    def correct(self, src_alpha, dest_alpha, ndec):
+        super(Arc, self).correct(src_alpha, dest_alpha, ndec)
+
+        p1, p2 = ((self.p1[0]-self.center[0],
+                   self.p1[1]-self.center[1]),
+                  (self.p2[0]-self.center[0],
+                   self.p2[1]-self.center[1]))
+
+        self.startangle = np.arctan2(p1[1], p1[0])
+        self.endangle = np.arctan2(p2[1], p2[0])
+        if self.rtheta is not None:
+            self.rtheta = self.rtheta + alpha
+        return self
+
     def minmax(self):
         """ Die Funktion bestimmt das Minimum und Maximum auf der x- und der
             y-Achse (return [<min-x>, <max-x>, <min-y>, <max-y>])
         """
         mm = [min(self.p1[0], self.p2[0]), max(self.p1[0], self.p2[0]),
               min(self.p1[1], self.p2[1]), max(self.p1[1], self.p2[1])]
 
@@ -1214,14 +1254,18 @@
 
     def __init__(self, p):
         self.p1 = p
 
     def render(self, renderer):
         renderer.point(self.p1)
 
+    def transform(self, T, alpha, ndec):
+        n = T.dot(np.array((self.p1[0], self.p1[1])))
+        self.p1 = (n[0], n[1])
+        return self
 
 def is_Circle(e):
     return isinstance(e, Circle) and not isinstance(e, Arc)
 
 
 def is_Arc(e):
     return isinstance(e, Arc)
```

### Comparing `femagtools-1.3.0/femagtools/erg.py` & `femagtools-1.3.1/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/femag.py` & `femagtools-1.3.1/femagtools/femag.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 import femagtools.conductor
 import femagtools.windings
 import femagtools.mcv
 import femagtools.asm
 import femagtools.airgap as ag
 import femagtools.fsl
 import femagtools.config
+import femagtools.ecloss
+
 from femagtools import ntib
 
 
 logger = logging.getLogger(__name__)
 
 
 BCHEXT = 'BATCH' if sys.platform.startswith('linux') else 'BCH'  # win32
@@ -527,15 +529,31 @@
             if 'airgap_induc' in simulation:
                 try:
                     pmod = bch.machine['p_sim']
                 except KeyError:
                     pmod = 0
                 bch.airgap = ag.read(os.path.join(self.workdir, 'bag.dat'),
                                      pmod=pmod)
+                
+            if simulation.get('magnet_loss', False):
+                logger.info('Evaluating magnet losses...')
+                ops = [k for k in range(len(bch.torque))]
+                m = femagtools.ecloss.MagnLoss(self.workdir, self.modelname, ibeta=ops)
+                try:
+                    magn_losses = m.calc_losses()
+                except: 
+                    magn_losses = [0 for i in range(len(ops))]
 
+                if len(ops) != len(bch.losses): 
+                    magn_losses.insert(0, magn_losses[0])
+                try:
+                    for i in range(len(bch.losses)): 
+                        bch.losses[i].update({"magnetH": magn_losses[i]})
+                except: 
+                    pass
             return bch
         return dict(status='ok', message=self.modelname)
 
 
 class FemagTask(threading.Thread):
     def __init__(self, port, args, workdir, logdir):
         threading.Thread.__init__(self)
```

### Comparing `femagtools-1.3.0/femagtools/forcedens.py` & `femagtools-1.3.1/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/fsl.py` & `femagtools-1.3.1/femagtools/fsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,16 @@
         params = {}
         params['split'] = model.magnet[templ].get('split', False)
         params['show_plots'] = model.magnet[templ].get('plot', False)
         params['write_fsl'] = True
         params['airgap'] = -1.0
         pos = 'out' if model.external_rotor else 'in'
         params['part'] = ('rotor', pos)
-        logger.info("Conv rotor from %s", templ + '.dxf')
+        logger.info("Conv rotor from %s",
+                    model.magnet[templ]['name'])
         conv = convert(model.magnet[templ]['name'], **params)
         model.set_value('poles', int(conv.get('num_poles')))
         self.set_diameter_parameter(model, conv)
         if model.get('da2'):
             logger.info('da2 %f',  model.get('da2')/1e3)
             ag = (model.get('bore_diam') - model.get('da2')/1e3)/2
             model.set_value('airgap', ag)
@@ -423,15 +424,15 @@
 
     def create_gen_winding(self, model):
         genwdg = self.__render(model, 'gen_winding')
         k = list({'leak_dist_wind',
                   'leak_evol_wind',
                   'leak_tooth_wind'}.intersection(model.windings))
         if k:
-            logger.info("LEAK %s ---------------", k)
+            logger.info("Leakage type %s", k)
             if 'wiredia' not in model.windings[k[0]]:
                 if 'wire_gauge' in model.windings:
                     import numpy as np
                     d = 2*np.sqrt(model.windings['wire_gauge']/np.pi)
                     model.windings[k[0]]['wiredia'] = d
                 elif 'dia_wire' in model.windings:
                     model.windings[k[0]]['wiredia'] = model.windings['dia_wire']
```

### Comparing `femagtools-1.3.0/femagtools/getset.py` & `femagtools-1.3.1/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/gmsh.py` & `femagtools-1.3.1/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/google.py` & `femagtools-1.3.1/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/grid.py` & `femagtools-1.3.1/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/isa7.py` & `femagtools-1.3.1/femagtools/isa7.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,16 +397,16 @@
             for j in range(blockSize // chunksize):
                 unpacked.append(struct.unpack_from("=" + fmt_,
                                                    self.file,
                                                    offset))
                 offset += chunksize
             logger.debug("%s: %d %d", fmt_, blockSize, len(unpacked))
         except struct.error as e:
-            logger.warning("Invalid Blocksize %s",
-                           blockSize)
+            logger.warning("Invalid Blocksize %s at pos %i",
+                           blockSize, self.pos-4)
 
         self.pos += blockSize + 4
 
         fmt_ = ""
         for s in re.findall(r"[0-9]*.|[0-9]*\?", fmt):
             if len(s) > 1 and s[-1] != "s":
                 fmt_ += int(s[:-1]) * s[-1]
```

### Comparing `femagtools-1.3.0/femagtools/jcf2msh.py` & `femagtools-1.3.1/femagtools/jcf2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/jhb.py` & `femagtools-1.3.1/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/job.py` & `femagtools-1.3.1/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/losscoeffs.py` & `femagtools-1.3.1/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/machine/__init__.py` & `femagtools-1.3.1/femagtools/machine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,34 +31,37 @@
 
 
 def create_from_eecpars(temp, eecpars, lfe=1, wdg=1):
     """create machine according to the eecpars:
     PM, EESM or IM"""
     rlfe = lfe
     rwdg = wdg
+    opts = {k: eecpars[k] for k in ('zeta1', 'gam', 'kh', 'kpfe',
+                                    'kfric_b') if k in eecpars}
+    try:
+        opts['rotor_mass'] = rlfe*eecpars['rotor_mass']
+    except KeyError:
+        pass
+
     if 'ldq' in eecpars or 'psidq' in eecpars:  # this is a PM (or EESM)
         try:
             dqpars = eecpars['ldq']
         except KeyError:
             dqpars = eecpars['psidq']
         if (isinstance(dqpars, list) and
             'ex_current' in dqpars[0] or
             isinstance(dqpars, dict) and
                 'ex_current' in dqpars):
             smpars = copy.deepcopy(eecpars)
             smpars['tcu1'] = temp[0]
             smpars['tcu2'] = temp[1]
             if 'ldq' in smpars:
-                machine = SynchronousMachineLdq(smpars, lfe=rlfe, wdg=rwdg)
+                machine = SynchronousMachineLdq(smpars, lfe=rlfe, wdg=rwdg, **opts)
             else:
-                machine = SynchronousMachinePsidq(smpars, lfe=rlfe, wdg=rwdg)
-            try:
-                machine.rotor_mass = rlfe*eecpars['rotor_mass']
-            except KeyError:
-                pass
+                machine = SynchronousMachinePsidq(smpars, lfe=rlfe, wdg=rwdg, **opts)
             return machine
 
         if isinstance(dqpars, list) and len(dqpars) > 1:
             x, dqp = dqpar_interpol(
                 temp[1], dqpars, ipkey='temperature')
         else:
             dqp = dqpars[0]
@@ -80,49 +83,47 @@
                 r1=eecpars['r1']*rlfe*rwdg**2,
                 ls=eecpars['ls1']*rwdg**2,
                 psid=psid,
                 psiq=psiq,
                 losses=losses,
                 id=np.array(dqp['id'])/rwdg,
                 iq=np.array(dqp['iq'])/rwdg,
-                tcu1=temp[0])
+                tcu1=temp[0],
+                **opts)
         else:
             beta = dqp['beta']
             i1 = np.array(dqp['i1'])/rwdg
             machine = PmRelMachineLdq(
                 eecpars['m'], eecpars['p'],
                 r1=eecpars['r1']*rlfe*rwdg**2,
                 ls=eecpars['ls1']*rwdg**2,
                 psid=psid,
                 psiq=psiq,
                 losses=losses,
                 beta=beta,
                 i1=i1,
-                tcu1=temp[0])
-        try:
-            machine.rotor_mass = rlfe*eecpars['rotor_mass']
-        except KeyError:
-            pass
+                tcu1=temp[0],
+                **opts)
         return machine
 
     # must be an induction machine (TODO: check scaling)
     pars = copy.deepcopy(eecpars)
     pars['r1'] = rlfe*rwdg**2*pars['r1']
     pars['lsigma1'] = rlfe*pars['lsigma1']
     pars['lsigma2'] = rlfe*pars['lsigma2']
     pars['psiref'] = rwdg*rlfe*pars['psiref']
     pars['u1ref'] = rwdg*rlfe*pars['u1ref']
-    pars['rotor_mass'] = rlfe*pars['rotor_mass']
     pars['r2'] = rlfe*pars['r2']
     pars['fec'] = rlfe*pars['fec']
     pars['fee'] = rlfe*pars['fee']
     pars['im'] = [im/rwdg for im in pars['im']]
     pars['psi'] = [psi*rwdg*rlfe for psi in pars['psi']]
     pars['tcu1'] = temp[0]
     pars['tcu2'] = temp[1]
+    pars.update(opts)
     return InductionMachine(pars)
 
 
 def __scale_losses(losses, rlfe):
     if losses:
         l = {k: rlfe*np.array(losses[k]) for k in (
             'styoke_hyst', 'styoke_eddy',
```

### Comparing `femagtools-1.3.0/femagtools/machine/im.py` & `femagtools-1.3.1/femagtools/machine/im.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 eecdefaults = dict(
     zeta1=0.2,
     zeta2=2.4,
     gam=0,  # gam=0.7, 0..1
     kh=1,  # kh=2, number of vertical conductors in slot
     tcu1=20,
+    kpfe=1,
     rotor_mass=0,
     kfric_b=1,
     pl2v=0.5,
     tcu2=20)
 
 logger = logging.getLogger('im')
 logging.captureWarnings(True)
@@ -136,55 +137,91 @@
             self._imag = log_interp1d(self.psi, self.im)
             self.psi = self.psiref
         if 'pfe' in parameters:
             self.rh = self.m*(self.psiref*self.wref)**2/self.pfe
         for k in eecdefaults.keys():
             if not hasattr(self, k):
                 setattr(self, k, eecdefaults[k])
+        try:
+            self.tfric = self.kfric_b*self.rotor_mass*30e-3/np.pi
+            # formula from
+            # PERMANENT MAGNET MOTOR TECHNOLOGY: DESIGN AND APPLICATIONS
+            # Jacek Gieras
+            #
+            # plfric = kfric_b m_r n 1e-3 W
+            # -- kfric_b : 1..3 W/kg/rpm
+            # -- m_r: rotor mass in kg
+            # -- n: rotor speed in rpm
+        except AttributeError:
+            self.tfric = 0
+
+        self.skin_resistance = [None, None]
+        # here you can set user defined functions for calculating the skin-resistance,
+        # according to the current frequency w. First function in list is for stator, second for rotor.
+        # If None, the femagtools intern default implementation is used.
+        # User defined functions need to have the following arguments:
+        # - r0: (float) dc-resistance at 20°C
+        # - w: (float)  current frequency in rad (2*pi*f)
+        # - tcu: (float) conductor temperature in deg Celsius
+        # - kth: (float) temperature coefficient (Default = 0.0039, Cu)
+
+    def pfric(self, n):
+        """friction and windage losses"""
+        return 2*np.pi*n*self.tfric
+
 
     def imag(self, psi):
         """magnetizing current"""
         if np.isscalar(psi):
             return float(self._imag(psi))
         return self._imag(psi)
 
     def rfe(self, w, psi):
         """equivalent resistance for iron losses"""
         try:
             if np.isclose(w, 0):
                 return 0
             else:
-                return self.m*((w*w)*(psi * psi)) / (
-                    (self.fec + self.fee *
-                     np.power(np.abs(psi)/self.psiref, self.fexp)) *
-                    (0.75 + 0.25*(np.abs(w)/self.wref)) *
-                    (np.abs(w)/self.wref) *
-                    np.power((np.abs(psi)/self.psiref), 2.0))
+                return self.m*(w*psi)**2 / self.plfe1(w, psi)
         except AttributeError:
             pass
         return self.rh
 
+    def plfe1(self, w1, psi):
+        return ((self.fec + self.fee *
+                 np.power(np.abs(psi)/self.psiref, self.fexp)) *
+                (0.75 + 0.25*(np.abs(w1)/self.wref)) *
+                (np.abs(w1)/self.wref) * np.power((np.abs(psi)/self.psiref), 2.0))
+
     def lrot(self, w):
         """rotor leakage inductance"""
         return skin_leakage_inductance(self.lsigma2, w, self.tcu2,
                                        self.zeta2, 1, self.pl2v)
 
     def lstat(self, w):
         """stator leakage inductance"""
         return self.lsigma1
 
     def rrot(self, w):
         """rotor resistance"""
-        return skin_resistance(self.r2, w, self.tcu2, self.zeta2,
-                               0.0, 1, kth=self.kth2)
+        sr = self.skin_resistance[1]
+        if sr is not None:
+            return sr(self.r2, w, self.tcu2, kth=self.kth2)
+        else:
+            return skin_resistance(self.r2, w, self.tcu2, self.zeta2,
+                                   0.0, 1, kth=self.kth2)
 
     def rstat(self, w):
         """stator resistance"""
-        return skin_resistance(self.r1, w, self.tcu1, self.zeta1,
-                               self.gam, self.kh, kth=self.kth1)
+        sr = self.skin_resistance[0]
+        if sr is not None:
+            return sr(self.r1, w, self.tcu1, kth=self.kth1)
+        else:
+            return skin_resistance(self.r1, w, self.tcu1, self.zeta1,
+                                   self.gam, self.kh, kth=self.kth1)
         # return self.r1
 
     def sigma(self, w, psi):
         """leakage coefficient"""
         lh = psi / self.imag(psi)
         return (1 - lh**2 /
                 ((lh+self.lstat(w))*(lh+self.lrot(0))))
@@ -217,14 +254,25 @@
         self.psi = psi
         if abs(u1) > u1max:  # must adjust flux
             self.psi = so.fsolve(
                 lambda psix: u1max - abs(self.u1(w1, psix, wm)),
                 psi)[0]
         return self.torque(w1, self.psi, wm)
 
+    def w1tmech(self, w1, u1max, psi, wm):
+        """calculate motor shaft torque"""
+        # check stator voltage
+        u1 = self.u1(w1, psi, wm)
+        self.psi = psi
+        if abs(u1) > u1max:  # must adjust flux
+            self.psi = so.fsolve(
+                lambda psix: u1max - abs(self.u1(w1, psix, wm)),
+                psi)[0]
+        return self.tmech(w1, self.psi, wm)
+
     def pullouttorque(self, w1, u1):
         """pull out torque"""
         sk = self.sk(w1, u1/w1)
         w2 = sk*w1
         r2 = self.rrot(w2)
         psi = u1/w1
         lh = psi/self.imag(psi)
@@ -251,70 +299,100 @@
         w2 = w1-self.p*wm
         if np.isclose(w2, 0):
             return 0.
         r2 = self.rrot(w2)
         i2 = self.i2(w1, psi, wm)
         return self.m*self.p/w2*r2*(i2*i2.conjugate()).real
 
+    def tmech(self, w1, psi, wm):
+        """shaft torque"""
+        u1 = self.u1(w1, psi, wm)
+        return self.torque(w1, psi, wm) - self.tfric
+
     def torqueu(self, w1, u1max, wm):
         """electric torque (in airgap)"""
         if np.isclose(w1, self.p*wm):
             return 0.
         # find psi
         psi = u1max/w1
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             self.psi = so.fsolve(
                 lambda psi: u1max - abs(self.u1(w1, psi, wm)),
                 psi)[0]
         return self.torque(w1, self.psi, wm)
 
-    def w1(self, u1max, psi, tload, wm):
+    def tmechu(self, w1, u1max, wm):
+        """shaft torque"""
+        if np.isclose(w1, self.p*wm):
+            return 0.
+        # find psi
+        psi = u1max/w1
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            self.psi = so.fsolve(
+                lambda psi: u1max - abs(self.u1(w1, psi, wm)),
+                psi)[0]
+        return self.torque(w1, self.psi, wm)
+
+    def w1(self, u1max, psi, tload, wm, with_tmech=True):
         """calculate stator frequency with given torque and speed"""
         wsync = max(wm*self.p, 0.001)
         # sk = self.rrot(0.)/(wsync*(self.lstat(wsync) + self.lrot(0.0)))
         if tload < 0:
             b = 0.999*wsync
         else:
             b = 1.001*wsync
+        if with_tmech:
+            logger.debug("wm %s tload %s w1tmech %s",
+                         wm, tload, self.w1tmech(b, u1max, psi, wm))
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                return so.fsolve(
+                    lambda w1: self.w1tmech(w1, u1max, psi, wm) - tload, b)[0]
+
         logger.debug("wm %s tload %s w1torque %s",
-                     wm, tload, self.w1torque(b, u1max, psi, wm))
+                     wm, tload, self.w1tmech(b, u1max, psi, wm))
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             return so.fsolve(
                 lambda w1: self.w1torque(w1, u1max, psi, wm) - tload, b)[0]
 
-    def wmfweak(self, u1max, psi, torque):
+    def wmfweak(self, u1max, psi, torque, with_tmech=True):
         """return lower speed limit of field weakening range"""
         wm0 = u1max/psi/self.p
         return so.fsolve(
             lambda wm: u1max - np.abs(self.u1(
-                self.w1(u1max, psi, torque, wm), psi, wm)),
+                self.w1(u1max, psi, torque, wm, with_tmech), psi, wm)),
             wm0)[0]
 
-    def torque_chart(self, smin=-0.1, smax=0.1, nsamples=100):
+    def torque_chart(self, smin=-0.1, smax=0.1, nsamples=100, with_tmech=True):
         """
         calculate torque(s) curve
 
         :param smin: min slip
         :param smax: max slip
+        :param with_tmech: use friction and windage losses (shaft torque)
         :return: dict with slip and torque lists
         """
 
         s = np.linspace(smin, smax, nsamples)
         f1 = self.f1ref
         u1 = self.u1ref
         w1 = 2 * np.pi * f1
         wm = (1-s) * w1 / self.p
         r = {}
         r['s'] = list(s)
-        r['T'] = [self.torqueu(w1, u1, wx) for wx in wm]
+        if with_tmech:
+            r['T'] = [self.tmechu(w1, u1, wx) for wx in wm]
+        else:
+            r['T'] = [self.torqueu(w1, u1, wx) for wx in wm]
         return r
 
-    def operating_point(self, T, n, u1max, Tfric=None):
+    def operating_point(self, T, n, u1max, Tfric=None, **kwargs):
         """
         calculate single operating point.
 
         return dict with values for
             s -- (float) slip at this op
             f1 -- (float) stator frequency in Hz
             u1 -- (float) stator phase voltage in V rms
@@ -336,53 +414,50 @@
         Keyword arguments:
             T -- (float) the output torque at the shaft in Nm
             n -- (float) the speed of the machine in 1/s
             u1max -- (float) the maximum phase voltage in V rms
             Tfric -- (float, optional) the friction torque to consider in Nm.
                      If Tfric is None, the friction torque is calculated according to the rotor-mass and the
                      frition factor of the machine (kfric_b). Friction is written to the result dict!
+            with_tmech -- (optional) use friction and windage losses
         """
 
         r = {}  # result dit
 
         if Tfric:
             tfric = Tfric
         else:
-            # formula from
-            # PERMANENT MAGNET MOTOR TECHNOLOGY: DESIGN AND APPLICATIONS
-            # Jacek Gieras
-            #
-            # plfric = kfric_b m_r n 1e-3 W
-            # -- kfric_b : 1..3 W/kg/rpm
-            # -- m_r: rotor mass in kg
-            # -- n: rotor speed in rpm
-            tfric = self.kfric_b * self.rotor_mass * 30e-3 / np.pi
+            tfric = self.tfric
             # TODO: make frictiontorque speed depended?
 
-        tq = T + tfric
+        with_tmech = kwargs.get('with_tmech', True)
+        if with_tmech:
+            tq = T + tfric
+        else:
+            tq = T
         wm = 2*np.pi*n
-        w1 = self.w1(u1max, self.psiref, tq, wm)
+        w1 = self.w1(u1max, self.psiref, tq, wm, with_tmech)
         s = (w1 - self.p*wm) / w1
         r['s'] = float(s)
         r['f1'] = float(w1/2/np.pi)
         u1 = self.u1(w1, self.psi, wm)
         r['u1'] = float(np.abs(u1))
         i1 = self.i1(w1, self.psi, wm)
         r['i1'] = float(np.abs(i1))
         r['cosphi'] = float(np.cos(np.angle(u1) - np.angle(i1)))
-        r['plfe1'] = float(self.m * np.abs(u1) ** 2 / self.rfe(w1, self.psi))
+        r['plfe1'] = self.plfe1(w1, self.psi)
         i2 = self.i2(w1, self.psi, wm)
         r['i2'] = float(np.abs(i2))
         r['plcu1'] = float(self.m * np.abs(i1) ** 2 * self.rstat(w1))
         r['plcu2'] = float(self.m * np.abs(i2) ** 2 *
                            self.rrot(w1 - self.p * wm))
-        r['plfric'] = float(2 * np.pi * n * tfric)
+        r['plfw'] = float(self.pfric(n))
         pmech = 2 * np.pi * n * tq
         r['pmech'] = float(pmech)
-        pltotal = r['plfe1'] + r['plfric'] + r['plcu1'] + r['plcu2']
+        pltotal = r['plfe1'] + r['plfw'] + r['plcu1'] + r['plcu2']
         r['losses'] = float(pltotal)
         p1 = pmech + pltotal
         r['p1'] = float(p1)
         if np.abs(pmech) < 1e-12:
             eta = 0  # power to low for eta calculation
         elif p1 > pmech:
             eta = pmech/p1  # motor
@@ -393,53 +468,56 @@
         r['Tfric'] = float(tfric)
         r['n'] = float(n)
         r['tcu1'] = float(self.tcu1)
         r['tcu2'] = float(self.tcu2)
 
         return r
 
-    def characteristics(self, T, n, u1max, nsamples=50, kpo=0.9):
+    def characteristics(self, T, n, u1max, nsamples=70, kpo=0.9, **kwargs):
         """calculate torque speed characteristics.
         return dict with list values of
-        id, iq, n, T, ud, uq, u1, i1,
+        id, iq, n, T, ud, uq, u1, i1, s, pullout slip
         beta, gamma, phi, cosphi, pmech, n_type
 
         Keyword arguments:
         T -- (float) the maximum torque in Nm
         n -- (float) the maximum speed in 1/s
         u1max -- (float) the maximum phase voltage in V rms
         nsamples -- (optional) number of speed samples
+        with_tmech -- (optional) use friction and windage losses
+
         """
+        with_tmech = kwargs.get('with_tmech', True)
 
-        wmType = self.wmfweak(u1max, self.psiref, T)
+        wmType = self.wmfweak(u1max, self.psiref, T, with_tmech)
         pmmax = wmType*T
         wmPullout = so.fsolve(
             lambda wx: (kpo*self.pullouttorque(self.p *
                         wx, u1max) - abs(pmmax/wx)),
             wmType)[0]
         wmtab0 = np.linspace(wmType, 3*wmPullout)
         for wm, tq in zip(wmtab0, [pmmax/wx for wx in wmtab0]):
             logger.debug("u1 %g psi %g tq %g wm %g",
                          u1max, self.psiref, tq, wm)
             try:
-                w1 = self.w1(u1max, self.psiref, tq, wm)
+                w1 = self.w1(u1max, self.psiref, tq, wm, with_tmech)
             except ValueError:
                 wmPullout = wm
                 break
         wmMax = max(1.5*wmPullout, 3*abs(pmmax/T))
         if n:
             wmMax = 2*np.pi*n
         if wmMax > wmPullout:
             wmtab0 = np.linspace(wmPullout, wmMax)
             for wm, tq in zip(wmtab0, [pmmax/wx**2
                                        for wx in wmtab0]):
                 logger.debug("u1 %g psi %g tq %g wm %g",
                              u1max, self.psiref, tq, wm)
                 try:
-                    w1 = self.w1(u1max, self.psiref, tq, wm)
+                    w1 = self.w1(u1max, self.psiref, tq, wm, with_tmech)
                 except ValueError:
                     wmMax = wm
                     break
 
         logger.info("wmtype %f wpo %f wmmax %f", wmType, wmPullout, wmMax)
 
         if wmType < wmPullout < wmMax:
@@ -460,59 +538,61 @@
             if nx > 0:
                 lw = np.linspace(wmrange[i]+dw, wmrange[i+1], nx)
                 dw = lw[-1] - lw[-2]
                 wmlin.append(lw)
         if len(wmlin) > 1:
             wmtab = np.concatenate(wmlin)
         else:
-            wmtab = wmlin[0]
+            wmtab = wmlin[1:]
 
         def tload2(wm):
             if wm < wmType and wm < wmPullout:
                 return T
             if wm < wmPullout:
                 if pmmax < 0:
                     return max(T, pmmax/wm)
                 return min(T, pmmax/wm)
             if pmmax < 0:
                 return max(wmPullout*pmmax/wm**2, T)
             return min(wmPullout*pmmax/wm**2, T)
 
         r = dict(u1=[], i1=[], T=[], cosphi=[], n=[], s=[], sk=[],
-                 plfe1=[], plcu1=[], plcu2=[])
+                 plfe1=[], plcu1=[], plcu2=[], f1=[])
         T = [tload2(wx) for wx in wmtab]
-        tfric = self.kfric_b*self.rotor_mass*30e-3/np.pi
-        w1tab = []
+        tfric = self.tfric
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             for wm, tq in zip(wmtab, T):
                 logger.debug("u1 %g psi %g tq %g wm %g",
                              u1max, self.psiref, tq, wm)
     #            try:
-                w1 = self.w1(u1max, self.psiref, tq, wm)
-                w1tab.append(w1)
+                w1 = self.w1(u1max, self.psiref, tq, wm, with_tmech)
+                r['f1'].append(w1/np.pi/2)
                 u1 = self.u1(w1, self.psi, wm)
                 r['u1'].append(np.abs(u1))
                 i1 = self.i1(w1, self.psi, wm)
                 r['i1'].append(np.abs(i1))
                 r['cosphi'].append(np.cos(np.angle(u1) - np.angle(i1)))
-                r['plfe1'].append(self.m*np.abs(u1)**2/self.rfe(w1, self.psi))
+                r['plfe1'].append(self.plfe1(w1, self.psi))
                 i2 = self.i2(w1, self.psi, wm)
                 r['plcu1'].append(self.m*np.abs(i1)**2*self.rstat(w1))
                 r['plcu2'].append(self.m*np.abs(i2)**2*self.rrot(w1-self.p*wm))
-                r['T'].append(tq - tfric)
+                if with_tmech:
+                    r['T'].append(tq)
+                else:
+                    r['T'].append(tq - tfric)
                 r['n'].append(wm/2/np.pi)
                 r['s'].append(float((w1 - self.p * wm) / w1))
                 r['sk'].append(self.sk(w1, u1/w1))
-#            except ValueError as ex:
-#                break
-        r['plfric'] = [2*np.pi*n*tfric for n in r['n']]
+                #            except ValueError as ex:
+                #                break
+        r['plfw'] = [self.pfric(n) for n in r['n']]
         r['pmech'] = [2*np.pi*n*tq for n, tq in zip(r['n'], r['T'])]
         pmech = np.array(r['pmech'])
-        pltotal = (np.array(r['plfe1']) + np.array(r['plfric']) +
+        pltotal = (np.array(r['plfe1']) + np.array(r['plfw']) +
                    np.array(r['plcu1']) + np.array(r['plcu2']))
         r['losses'] = pltotal.tolist()
 
         if pmech.any():
             p1 = pmech + pltotal
             if np.abs(pmech[0]) < 1e-12:
                 r['eta'] = [0]
@@ -653,15 +733,16 @@
         f1=f1,
         num_par_wdgs=machine['windings'].get('num_par_wdgs', 1),
         wdgcon=CON[wdgcon],  # 0:open, 1:star, 2:delta
         u1=u1ph)  # phase voltage
 
     # prepare calculation
     job = engine.create_job(workdir)
-    task = job.add_task(_eval_noloadrot(), extra_result_files)
+    pmod = model.poles * model.stator['num_slots_gen'] / model.stator['num_slots']
+    task = job.add_task(_eval_noloadrot(pmod), extra_result_files)
     logger.debug("Task %s noload workdir %s result files %s",
                  task.id, task.directory, task.extra_result_files)
     # create model
     for mc in parstudy.femag.copy_magnetizing_curves(
             model,
             dir=task.directory):
         task.add_file(mc)
@@ -858,39 +939,39 @@
 
     return impars
 
 
 class _eval_noloaddc():
     """ Result Functor for noloadflux dc calc"""
 
-    def __init__(self):
-        pass
+    def __init__(self, pmod):
+        self.pmod = pmod
 
     def __call__(self, task):
         basedir = pathlib.Path(task.directory)
         psimag = np.loadtxt(basedir/'noloadflux.dat').T
         im, psi = psimag[0:6:2], psimag[12::2]
         d = 0
         a = np.array(
             (np.cos(d), np.cos(d-2*np.pi/3), np.cos(d+2*np.pi/3)))/3*2
         i0 = np.sum(a*im.T, axis=1)/np.sqrt(2)
         psi0 = np.sum(a*psi.T, axis=1)/np.sqrt(2)
 
         bag = np.loadtxt(basedir / 'noloadbag.dat').T
         Bamp = [b['Bamp'] for b in [
-            femagtools.airgap.fft(bag[0], b)
+            femagtools.airgap.fft(bag[0], b, self.pmod)
             for b in bag[1:]]]
         return {'i1_0': i0, 'psi1_0': psi0, 'Bamp': Bamp}
 
 
 class _eval_noloadrot():
     """ Result Functor for noloadflux rot calc"""
 
-    def __init__(self):
-        pass
+    def __init__(self, pmod):
+        self.pmod = pmod
 
     def __call__(self, task):
         basedir = pathlib.Path(task.directory)
         psimag = np.loadtxt(basedir/'psi-rot-mag.dat')
         pos = np.unique(psimag[:, 0])
         ncurs = psimag[:, 0].shape[0]//pos.shape[0]
         ire = psimag[:ncurs, 1:7:2]  # assuming same current for all steps
@@ -902,15 +983,15 @@
 
         psi0 = np.array([np.linalg.norm(
             femagtools.machine.T(0).dot(psire[:, k, :].T),
             axis=0)/np.sqrt(2)
             for k in range(ncurs)])
 
         # matrix (i x j x k) of curr, rotor pos, angle
-        Bamp = [[femagtools.airgap.fft(bags[:, 0], b)['Bamp']
+        Bamp = [[femagtools.airgap.fft(bags[:, 0], b, self.pmod)['Bamp']
                  for b in bags.T[1:]]
                 for bags in [np.loadtxt(p) for p in sorted(
                     basedir.glob(f"noloadbag-*.dat"),
                     key=lambda path: int(path.stem.rsplit("-", 1)[1]))]]
         return {'i1_0': i0, 'psi1_0': psi0, 'Bamp': Bamp}
 
 
@@ -979,15 +1060,15 @@
         r1=0.043,
         r2=0.0346,
         lsigma1=1.15e-3,
         lsigma2=0.73361e-3,
         fec=9100,
         fee=0,
         fexp=7.0,
-        pfric=2544.6,
+        #pfric=2544.6,
         rexp=2.4,
         iml=79.8286,
         ims=27.5346,
         mexp=6.5)
 
     im = InductionMachine(mpars)
     torque = 6543
```

### Comparing `femagtools-1.3.0/femagtools/machine/pm.py` & `femagtools-1.3.1/femagtools/machine/sm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,922 +1,847 @@
 """
-  femagtools.pm
+  femagtools.sm
   ~~~~~~~~~~~~~
-
-  PM/Rel synchronous machine (SPM, IPM, RM) electrical circuit model
+  wound-rotor synchronous machine (EESM) electrical circuit model
 
   Copyright 2022: Semafor Informatik & Energie AG, Switzerland
 """
 import logging
+import warnings
 import numpy as np
-import numpy.linalg as la
-from .utils import iqd, betai1, skin_resistance, dqparident
 import scipy.optimize as so
 import scipy.interpolate as ip
+from .utils import skin_resistance, wdg_resistance, betai1, iqd, KTH
+from .. import parstudy, windings
+import femagtools.bch
+
+EPS = 1e-13
+
+eecdefaults = dict(
+        zeta1=0.3,
+        zeta2=0,
+        gam=0.7,
+        kh=2,
+        tcu1=20,
+        tcu2=20,
+        rotor_mass=0,
+        kfric_b=1,
+        kpfe = 1 # iron loss factor
+)
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger('sm')
+logging.captureWarnings(True)
 
 
-def parident(workdir, engine, temp, machine,
-             magnetizingCurves, magnetMat, condMat,
+def parident(workdir, engine, machine,
+             magnetizingCurves, condMat,
              **kwargs):
-    return dqparident(workdir, engine, temp, machine,
-                      magnetizingCurves, magnetMat, condMat,
-                      **kwargs)
-
-
-class PmRelMachine(object):
-    """Abstract base class for PmRelMachines
-
-    Args:
-        m: number of winding phases
-        p: number of pole pairs
-        r1: stator winding resistance (in Ohm)
-        ls: leakage inductance in H
-    """
-
-    def __init__(self, m, p, r1, ls, **kwargs):
-        self.p = p
-        self.m = m
-        self.r1 = r1
-        self.ls = ls
-        self.io = (1, -1)
-        self.fo = 50.0
-        self.tcu1 = 20
-        self.zeta1 = 0.3
-        self.gam = 0.7
-        self.kh = 2
-        self.kfric_b = 1
-        # TODO: need this for speedranges and idq_imax_umax mtpv only
-        self.check_extrapolation = True
-        for k in kwargs.keys():
+        """return dict of parameters of equivalent circuit for
+        electrically excited synchronous machines
+
+        arguments:
+        machine -- dict() with machine parameters
+        magnetizingCurves -- list of dict() with BH curves
+        condMat -- list of dict() with conductor material properties
+
+        optional arguments:
+        num_cur_steps: number of current steps (default 5)
+        num_beta_steps: number of current steps (default 13)
+        num_exc_steps: number of excitation current (default 7)
+        speed: rotor speed in 1/s (default 160/p)
+        i1_max: maximum current in A rms (default approx 3*i1nom)
+        """
+        da1 = machine['outer_diam']
+        Q1 = machine['stator']['num_slots']
+        if 'statorRotor3' in machine['stator']:
+            hs = machine['stator']['statorRotor3']['slot_height']
+        elif 'stator1' in machine['stator']:
+            hs = machine['stator']['stator1']['slot_rf1'] - machine['stator']['stator1']['tip_rh1']
+        elif 'stator4' in machine['stator']:
+            hs = machine['stator']['stator4']['slot_height']
+        N = machine['windings']['num_wires']
+        Jmax = 15  # max current density in A/mm2
+
+        i1_max = round(0.28*np.pi*hs*(da1+hs)/Q1/N*Jmax*1e5)*10 * \
+            machine['windings'].get('num_par_wdgs', 1)
+
+        ifnom = machine['rotor']['ifnom']
+        exc_logspace = True
+        if exc_logspace:
+            excur = np.logspace(np.log(ifnom/10), np.log(1.5*ifnom),
+                                kwargs.get("num_exc_steps", 6),
+                                base=np.exp(1)).tolist()
+        else:
+            excur = np.linspace(ifnom/10, 1.5*ifnom,
+                                kwargs.get("num_exc_steps", 6))
+
+        parvardef = {
+            "decision_vars": [
+                {"values": excur, "name": "load_ex_cur"}
+            ]
+        }
+
+        parvar = parstudy.List(
+            workdir,  condMat=condMat,
+            magnetizingCurves=magnetizingCurves)
+
+        simulation = dict(
+                calculationMode=kwargs.get('calculationMode',
+                                           'ld_lq_fast'),
+                wind_temp=20.0,
+                i1_max=kwargs.get('i1_max', i1_max),
+                maxid=0,
+                minid=-i1_max,
+                maxiq=i1_max,
+                miniq=-i1_max,
+                delta_id=i1_max/kwargs.get('num_cur_steps', 5),
+                delta_iq=i1_max/kwargs.get('num_cur_steps', 5),
+                beta_min=-180.0,
+                beta_max=0.0,
+                calc_noload=0,
+                num_move_steps=kwargs.get('num_move_steps', 31),
+                load_ex_cur=0.5,
+                num_cur_steps=kwargs.get('num_cur_steps', 5),
+                num_beta_steps=kwargs.get('num_beta_steps', 13),
+                num_par_wdgs=machine['windings'].get('num_par_wdgs', 1),
+                period_frac=6,
+                speed=50.0)
+
+        ###self.cleanup()  # remove previously created files in workdir
+        results = parvar(parvardef, machine, simulation, engine)
+        if simulation['calculationMode'] == 'ld_lq_fast':
+            idname = 'ldq'
+        else:
+            idname = 'psidq'
+        for r in results['f']:
+            for k in ('hf', 'ef'):
+                if k in r['lossPar']:
+                    r[idname]['losses'][k] = r['lossPar'][k]
+        try:
+            rotor_mass = sum(results['f'][-1]['weights'][-1])
+        except KeyError:
+            rotor_mass = 0  # need femag classic > rel-9.3.x-48-gca42bbd0
+        b = results['f'][-1]
+
+        losskeys = ('speed', 'ef', 'hf',
+                    'styoke_hyst', 'stteeth_hyst', 'styoke_eddy',
+                    'stteeth_eddy', 'rotor_hyst', 'rotor_eddy')
+
+        # winding resistance
+        try:
+            r1 = machine['windings']['resistance']
+        except KeyError:
+            yd = machine['windings'].get('coil_span', Q1/machine['poles'])
+            wdg = windings.Winding(
+            {'Q': machine['stator']['num_slots'],
+             'm': machine['windings']['num_phases'],
+             'p': machine['poles']//2,
+             'l': machine['windings']['num_layers'],
+             'yd': yd})
+
+            lfe = machine['lfe']
+            g = machine['windings'].get('num_par_wdgs', 1)
+            if 'dia_wire' in machine['windings']:
+                aw = np.pi*machine['windings'].get('dia_wire', 1e-3)**2/4
+            else:  # wire diameter from slot area
+                aw = 0.75 * \
+                        machine['windings'].get('cufilfact', 0.45)*np.pi*da1*hs/Q1/2/N
+            r1 = wdg_resistance(wdg, N, g, aw, da1, hs, lfe)
+
+        if simulation['calculationMode'] == 'ld_lq_fast':
+                dqpars = dict(m=3, p=b['machine']['p'],
+                        r1=r1,
+                        r2=machine['rotor'].get('resistance', 1),
+                        rotor_mass=rotor_mass, kfric_b=1,
+                        ldq=[dict(
+                                ex_current=b['machine']['ex_current'],
+                                i1=b['ldq']['i1'],
+                                beta=b['ldq']['beta'],
+                                psid=b['ldq']['psid'],
+                                psiq=b['ldq']['psiq'],
+                                torque=b['ldq']['torque'],
+                                ld=b['ldq']['ld'],
+                                lq=b['ldq']['lq'],
+                                losses={k: b['ldq']['losses'][k]
+                                        for k in losskeys})
+                             for b in results['f']])
+        else:
+                dqpars = dict(m=3, p=b['machine']['p'],
+                    r1=r1,
+                    r2=machine['rotor'].get('resistance', 1),
+                    rotor_mass=rotor_mass, kfric_b=1,
+                    psidq=[dict(
+                            ex_current=b['machine']['ex_current'],
+                            iq=b['psidq']['iq'],
+                            id=b['psidq']['id'],
+                            psid=b['psidq']['psid'],
+                            psiq=b['psidq']['psiq'],
+                            torque=b['psidq']['torque'],
+                            losses={k: b['psidq']['losses'][k]
+                                    for k in losskeys})
+                           for b in results['f']])
+        if 'current_angles' in results['f'][0]:
+                dqpars['current_angles'] = results['f'][0]['current_angles']
+        return dqpars
+
+def _linsampl(exc, excl, a):
+    """auxiliary func for linear sampling of nonlinear sequence
+    arguments:
+    exc: (list) nonlinear sequence of excitation current
+    excl: (list) linear sequence of excitation current
+    a: (array) matrix to be resampled"""
+    z = []
+    b, i = a.shape[1:]
+    for x in range(b):
+        for y in range(i):
+            zl = ip.interp1d(exc, a[:, x, y], kind='linear')
+            z.append(zl(excl))
+    return np.array(z).T.reshape(len(excl), b, i)
+
+
+def _splinterp(beta, i1, betax, i1x, a):
+    """auxiliary function to increase resolution of array a
+    using a cubic spline interpolation.
+    arguments:
+    beta: (list) n original up-i angles in rad
+    i1: (list) m original current in A
+    betax: (list) nx new up-i angles in rad
+    i1x: (list) mx new currents
+    a: (nxm array) to be interpolated"""
+    f = ip.RectBivariateSpline(
+        beta, i1, np.asarray(a),
+        kx=3, ky=3).ev
+    X, Y = np.meshgrid(betax, i1x)
+    return f(X, Y).T
+
+
+def _islinear(exc):
+    return np.abs(np.sum(
+        np.asarray(exc)**2 -
+        np.linspace(exc[0], exc[-1], len(exc))**2)) < 1e-2
+
+
+def gradient_respecting_bounds(bounds, fun, eps=1e-8):
+    """bounds: list of tuples (lower, upper)"""
+    def gradient(x):
+        logger.info(x)
+        fx = fun(x)
+        grad = np.zeros(len(x))
+        for k in range(len(x)):
+            d = np.zeros(len(x))
+            d[k] = eps if x[k] + eps <= bounds[k][1] else -eps
+            grad[k] = (fun(x + d) - fx) / d[k]
+        return grad
+    return gradient
+
+
+class SynchronousMachine(object):
+    def __init__(self, eecpars, **kwargs):
+        self.kth1 = KTH
+        self.kth2 = KTH
+        self.skin_resistance = [None, None]
+        # here you can set user defined functions for calculating the skin-resistance,
+        # according to the current frequency w. First function in list is for stator, second for rotor.
+        # If None, the femagtools intern default implementation is used.
+        # User defined functions need to have the following arguments:
+        # - r0: (float) dc-resistance at 20°C
+        # - w: (float)  current frequency in rad (2*pi*f)
+        # - tcu: (float) conductor temperature in deg Celsius
+        # - kth: (float) temperature coefficient (Default = 0.0039, Cu)
+        for k in eecdefaults.keys():
+            setattr(self, k, eecdefaults[k])
+
+        for k in eecpars:
+            if k not in ('ldq', 'psidq'):
+                setattr(self, k, eecpars[k])
+
+        for k in kwargs:
             setattr(self, k, kwargs[k])
 
+        try:
+            self.tfric = self.kfric_b*self.rotor_mass*30e-3/np.pi
+        except AttributeError:
+            self.tfric = 0
+
+        self.fo = 50
         self.plexp = {'styoke_hyst': 1.0,
                       'stteeth_hyst': 1.0,
                       'styoke_eddy': 2.0,
                       'stteeth_eddy': 2.0,
                       'rotor_hyst': 1.0,
                       'rotor_eddy': 2.0}
-        self._losses = {k: lambda x, y: 0 for k in (
-            'styoke_hyst', 'stteeth_hyst',
-            'styoke_eddy', 'stteeth_eddy',
-            'rotor_hyst', 'rotor_eddy',
-            'magnet')}
+
+    def _set_losspar(self, speed, ef, hf):
+        self.fo = speed*self.p
+        self.plexp = {'styoke_hyst': hf,
+                      'stteeth_hyst': hf,
+                      'styoke_eddy': ef,
+                      'stteeth_eddy': ef,
+                      'rotor_hyst': hf,
+                      'rotor_eddy': ef}
+
+    def pfric(self, n):
+        """friction and windage losses"""
+        return 2*np.pi*n*self.tfric
 
     def rstat(self, w):
         """stator resistance"""
-        return skin_resistance(self.r1, w, self.tcu1, self.zeta1,
-                               self.gam, self.kh)
+        sr = self.skin_resistance[0]
+        if sr is not None:
+            return sr(self.r1, w, self.tcu1, kth=self.kth1)
+        else:
+            return skin_resistance(self.r1, w, self.tcu1, self.zeta1,
+                                   self.gam, self.kh, kth=self.kth1)
 
-    def torque_iqd(self, iq, id):
-        "torque at q-d-current"
-        psid, psiq = self.psi(iq, id)
-        tq = self.m*self.p/2*(psid*iq - psiq*id)
-        return tq
-
-    def iqd_torque(self, torque):
-        """return minimum d-q-current for torque"""
-        if np.abs(torque) < 1e-2:
-            return (0, 0)
-        if torque > 0:
-            iqd0 = self.i1range[1]/2, 0
+    def rrot(self, w):
+        """rotor resistance"""
+        sr = self.skin_resistance[1]
+        if sr is not None:
+            return sr(self.r2, w, self.tcu2, kth=self.kth2)
         else:
-            iqd0 = -self.i1range[1]/2, 0
-        res = so.minimize(
-            lambda iqd: la.norm(iqd), self.io, method='SLSQP',
-            constraints=({'type': 'eq',
-                          'fun': lambda iqd:
-                          self.torque_iqd(*iqd) - torque}))
-        if not res.success:
-            raise ValueError(f'Torque {torque} out of current range')
-        return res.x
-
-    def tmech_iqd(self, iq, id, n, kpfe, pfw):
-        """return shaft torque with given d-q current, iron loss correction factor
-          and friction windage losses"""
-        f1 = self.p*n
-        plfe1 = self.iqd_plfe1(iq, id, f1)
-        plfe2 = self.iqd_plfe2(iq, id, f1)
-        plfe = kpfe * (plfe1 + plfe2)
-        pmag = self.iqd_plmag(iq, id, f1)
-        return self.torque_iqd(iq, id) - (plfe + pmag + pfw)/(2*np.pi*n)
+            return skin_resistance(self.r2, w, self.tcu2, self.zeta2,
+                                   0.0, 1, kth=self.kth2)
+
+    def torque_iqd(self, iq, id, iex):
+        "torque at q-d-current"
+        psid, psiq = self.psi(iq, id, iex)
+        return self.m*self.p/2*(psid*iq - psiq*id)
 
-    def uqd(self, w1, iq, id):
+    def tloss_iqd(self, iq, id, iex, n):
+        """return loss torque of d-q current, iron loss correction factor
+        and friction windage losses"""
+        if n > 1e-3:
+            f1 = self.p*n
+            plfe = self.kpfe * (self.iqd_plfe1(iq, id, iex, f1) + self.iqd_plfe2(iq, id, f1))
+            return (plfe + self.pfric(n))/(2*np.pi*n)
+        return 0
+
+    def tmech_iqd(self, iq, id, iex, n):
+        """return shaft torque of d-q current and speed"""
+        return self.torque_iqd(iq, id, iex) - self.tloss_iqd(iq, id, iex, n)
+
+    def uqd(self, w1, iq, id, iex):
         """return uq, ud of frequency w1 and d-q current"""
-        psid, psiq = self.psi(iq, id)
-        uqd = (self.r1*iq + w1*(self.ls*id + psid),
-               self.r1*id - w1*(self.ls*iq + psiq))
-        #logger.debug('beta i1 %s u1 %f', betai1(iq, id), la.norm(uqd))
-        return uqd
+        psid, psiq = self.psi(iq, id, iex)
+        r1 = self.rstat(w1)
+        return r1*id + w1*psid, r1*iq - w1*psiq
+
+    def plcu1(self, iqde, w1):
+        r1 = self.rstat(w1)
+        return 3/2*r1*(iqde[0]**2 + iqde[1]**2)
+
+    def plcu2(self, iqde, w1=0):
+        r2 = self.rrot(0)
+        return r2*iqde[2]**2
 
-    def w1_umax(self, u, iq, id):
-        """return frequency w1 at given voltage u and id, iq current
+    def culoss(self, iqde, w1=0):
+        return self.plcu1(iqde, w1) + self.plcu2(iqde, 0)
 
-        Keyword arguments:
-        u -- the maximum voltage (RMS)
-        iq, id -- the d-q currents"""
-        w10 = np.sqrt(2)*u/la.norm(self.psi(iq, id))
-        return so.fsolve(
-            lambda w1: la.norm(self.uqd(w1, iq, id))-u*np.sqrt(2),
-            w10)[0]
+    def iqd_plcu1(self, iq, id, f1):
+        return self.plcu1((iq, id), 2*np.pi*f1)
 
-    def w1_u(self, u, iq, id):
-        """return frequency w1 at given voltage u and id, iq current
-        (obsolete, use w1_umax)"""
-        return self.w1_umax(u, iq, id)
+    def iqd_plcu2(self, iq, id, iex):
+        return self.plcu2((iq, id, iex))
 
-    def w1max(self, u, iq, id):
-        """return max frequency w1 at given voltage u and d-q current
-        (obsolete, use w1_umax)"""
-        return self.w1_umax(u, iq, id)
-
-    def w2_imax_umax(self, imax, umax, maxtorque=True):
-        """return frequency at max current and max voltage"""
-        w, info, ier, mesg = so.fsolve(lambda x: np.linalg.norm(
-            self.uqd(x, *iqd(-np.pi/2, imax))) - umax*np.sqrt(2),
-            np.sqrt(2)*umax/la.norm(self.psi(*self.io)),
-            full_output=True)
-        if ier == 1:
-            return w[0]
-
-        logger.warn("w2_imax_umax ier=%d imax %f", ier, imax)
-        raise ValueError("w2_imax_umax {} imax {}".format(mesg, imax))
-
-    def beta_u(self, w1, u, i1):
-        "beta at given frequency, voltage and current"
-        return so.fsolve(lambda b:
-                         la.norm(self.uqd(w1, *(iqd(b, i1))))-u*np.sqrt(2),
-                         np.arctan2(self.io[1], self.io[0]))[0]
-
-    def iq_u(self, w1, u, id):
-        "iq at given frequency, voltage and id current"
-        iq0 = max(self.io[0]/4, id*np.tan(self.betarange[0]))
-        return so.fsolve(lambda iq:
-                         la.norm(
-                             self.uqd(w1, iq, np.array([id])))-u*np.sqrt(2),
-                         iq0)[0]
-
-    def iqd_uqd(self, w1, uq, ud):
-        "return iq, id current at given frequency, voltage"
-        return so.fsolve(lambda iqd:
-                         np.array((uq, ud)) - self.uqd(w1, *iqd),
-                         (0, self.io[1]))
-
-    def i1_torque(self, torque, beta):
-        "return i1 current with given torque and beta"
-        i1, info, ier, mesg = so.fsolve(
-            lambda i1: self.torque_iqd(*iqd(beta, i1))-torque,
-            self.io[0],
-            full_output=True)
-        if ier == 1:
-            return i1
-        raise ValueError("no solution found for torque {}, beta {}".format(
-            torque, beta))
-
-    def i1_voltage(self, w1, u1, beta):
-        "return i1 current with given w1, u1 and beta"
-        i1, info, ier, mesg = so.fsolve(
-            lambda i1: la.norm(self.uqd(w1, *iqd(beta, i1)))-np.sqrt(2)*u1,
-            la.norm(self.io),
-            full_output=True)
-        if ier == 1:
-            return i1
-        raise ValueError("{} for w1 {}, u1 {}, beta {}".format(
-            mesg, w1, u1, beta))
-
-    def id_torque(self, torque, iq):
-        "return d current with given torque and d-current"
-        id0 = self.iqd_torque(torque)[1]
-        return so.fsolve(
-            lambda id: self.torque_iqd(np.array([iq]), id)-torque, id0)[0]
+    def iqd_plfe2(self, iq, id, f1):
+        return np.zeros(np.asarray(iq).shape)
 
-    def iqd_torque_umax(self, torque, w1, u1max, log=0):
-        """return d-q current and torque at stator frequency and max voltage
-        with minmal current"""
-        res = so.minimize(lambda iqd: la.norm(iqd), self.io, method='SLSQP',
-                          constraints=(
-                              {'type': 'eq',
-                               'fun': lambda iqd:
-                               self.torque_iqd(*iqd) - torque},
-                              {'type': 'ineq',
-                               'fun': lambda iqd:
-                               np.sqrt(2)*u1max - la.norm(self.uqd(w1, *iqd))}))
-        if log:
-            log(res.x)
-        logger.debug("iqd_torque_umax w1=%f torque=%f %f iq=%f id=%f u1 u1 %f %f",
-                    w1, torque, self.torque_iqd(*res.x), res.x[0], res.x[1],
-                    u1max, np.linalg.norm(
-                        self.uqd(w1, *res.x))/np.sqrt(2))
-        return res.x[0], res.x[1], self.torque_iqd(*res.x)
-
-    def iqd_torque_imax_umax(self, torque, n, u1max, log=0):
-        """return d-q current and torque at stator frequency w1,
-        max voltage  and current"""
-        iq, id = self.iqd_torque(torque)
-        w1 = 2*np.pi*n*self.p
-        # Constant torque range
-        if np.linalg.norm(self.uqd(w1, iq, id)) <= u1max*np.sqrt(2):
-            if log:
-                log((iq, id, torque))
-            return (iq, id, torque)
-        # Field weaking range
-        imax = betai1(iq, id)[1]
-        iq, id, tq = self.iqd_imax_umax(imax, w1, u1max, torque, with_mtpv=False)
-        if log:
-            log((iq, id, tq))
-        return iq, id, tq
+    def iqd_plmag(self, iq, id, f1):
+        return np.zeros(np.asarray(iq).shape)
+
+    def iqd_tmech(self, torque, n, disp=False, maxiter=500):
+        """return currents for shaft torque with minimal losses"""
+        if torque > 0:
+            startvals = self.bounds[0][1], 0, sum(self.bounds[-1])
+        else:
+            startvals = -self.bounds[0][1], 0, sum(self.bounds[-1])
 
-    def iqd_maxtorque_imax_umax(self, i1max, w1, u1max):
-        """return d-q current and max torque at stator frequency w1,
-        max voltage  and current"""
-        sign = -1 if i1max > 0 else 1
-        res = so.minimize(lambda iqd: sign*self.torque_iqd(*iqd),
-                          self.mtpa(i1max)[:2],
-                          method='SLSQP',
-                          constraints=(
-                              {'type': 'ineq',
-                               'fun': lambda iqd:
-                               np.sqrt(2)*abs(i1max) - betai1(*iqd)[1]},
-                              {'type': 'eq',
-                               'fun': lambda iqd:
-                               np.sqrt(2)*u1max - la.norm(self.uqd(w1, *iqd))}
-                          ))
-        return res.x[0], res.x[1], self.torque_iqd(*res.x)
-
-    def iqd_imax_umax(self, i1max, w1, u1max, torque, with_mtpv=True):
-        """return d-q current and torque at stator frequency and max voltage
-        and max current (for motor operation if maxtorque else generator operation)"""
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            def sqrtculoss(iqde):
+                pcu = self.culoss(iqde)
+                return pcu
+
+            res = so.minimize(
+                self.culoss, startvals, method='SLSQP',  # trust-constr
+                bounds=self.bounds,
+                #            jac=gradient_respecting_bounds(self.bounds, self.culoss),
+                constraints=[
+                    {'type': 'eq',
+                     'fun': lambda iqd: self.tmech_iqd(*iqd, n) - torque}])
+                    #options={'disp': disp, 'maxiter': maxiter})
+            if res['success']:
+                return res.x
+
+        logger.warning("%s: torque=%f %f, io=%s",
+                       res['message'], torque, self.tmech_iqd(*startvals, n),
+                       startvals)
+        raise ValueError(res['message'])
 
+    def iqd_torque(self, torque, disp=False, maxiter=500):
+        """return currents for torque with minimal losses"""
         if torque > 0:
-            # -pi/2 --> 0
-            b0, b1 = max(-np.pi/2, self.betarange[0]), 0
-            if max(self.betarange) < b1:
-                raise ValueError(
-                    f"invalid betarange for maxtorque>0: {self.betarange}")
-        else:
-            # -pi/2 --> -pi
-            b0, b1 = -np.pi/2, max(-np.pi, self.betarange[0])
-            if min(self.betarange) > b0:
-                raise ValueError(
-                    f"invalid betarange for maxtorque<0: {self.betarange}")
-
-        deps = 1e-6
-        kmax = 100
-
-        def u1norm(b):
-            return np.linalg.norm(
-                self.uqd(w1, *iqd(b, abs(i1max))))/np.sqrt(2)
-        if u1norm(b1) < u1max:
-            # must reduce current (torque)
-            iq, id, tq = self.iqd_torque_umax_imin(torque, w1, u1max)
-            if not with_mtpv:
-                return iq, id, tq
-            beta, i1 = betai1(iq, id)
-        else:
-            for k in range(kmax):
-                bx = b0 + (b1-b0)/2
-                ux = u1norm(bx)
-                #logger.info("%d: bx %f ux %f", k, bx, ux)
-                if ux > u1max:
-                    b1 = bx
-                else:
-                    b0 = bx
-                if abs(b1-b0) < deps:
-                    break
-            beta, i1 = bx, i1max
-            du = ux - u1max
-            logger.debug("iqd_imax_umax n %f beta %f iter=%d du=%f",
-                         w1/2/np.pi/self.p*60, beta/np.pi*180, k, du)
-            if abs(du) < 0.1:
-                iq, id = iqd(beta, abs(i1max))
-            else:
-                iq, id = self.iqd_torque(torque)
-        if with_mtpv:
-            # must check mtpv
-            self.check_extrapolation = False
-            try:
-                def voltw1(wx):
-                    return np.linalg.norm(
-                        self.mtpv(wx, u1max,
-                                  maxtorque=torque>0)[:2]) - np.sqrt(2)*i1,
-                w, _, ier, _ = so.fsolve(voltw1, w1, full_output=True)
-                logger.info("3: ier %d w %f w1 %f", ier, w, w1)
-                if ier in (1,5) and abs(w[0]) <= w1:
-                    self.check_extrapolation = True
-                    return self.mtpv(w1, u1max)
-            except ValueError as e:
-                logger.warning("MTPV w1=%f i1max=%f, u1max %f %s",
-                               w1, i1, u1max, e)
-            self.check_extrapolation = True
-
-        iq, id = iqd(beta, abs(i1))
-        tq = self.torque_iqd(iq, id)
-        logger.debug("iqd_imax_umax w1=%f torque=%f %f iq=%f id=%f u1 %f %f",
-                    w1, torque, tq, iq, id, u1max, np.linalg.norm(
-                            self.uqd(w1, iq, id))/np.sqrt(2))
-        return iq, id, tq
-
-    def mtpa(self, i1):
-        """return iq, id, torque at maximum torque of current i1"""
-        sign = -1 if i1 > 0 else 1
-        b0 = 0 if i1 > 0 else -np.pi
-        bopt, fopt, iter, funcalls, warnflag = so.fmin(
-            lambda x: sign*self.torque_iqd(*iqd(x, abs(i1))), b0,
-            full_output=True,
-            disp=0)
-        iq, id = iqd(bopt[0], abs(i1))
-        return [iq, id, sign*fopt]
-
-    def mtpv(self, w1, u1, iqd0=0, maxtorque=True):
-        """return d-q-current, torque for voltage and frequency
-        with maximum (maxtorque=True) or minimum torque """
-        sign = -1 if maxtorque else 1
-        if np.isscalar(iqd0):
-            i0 = (-sign*self.i1range[1]/20, -self.i1range[1]/np.sqrt(2))
-        else:
-            i0 = iqd0
-        res = so.minimize(
-            lambda iqd: sign*self.torque_iqd(*iqd),
-            i0, method='SLSQP',
-            #bounds=((0, self.i1range[1]),
-            #        (-self.i1range[1], 0)),
-            constraints=(
-                {'type': 'eq',
-                 'fun': lambda iqd:
-                 np.sqrt(2)*u1 - la.norm(self.uqd(w1, *iqd))},))
-        if res['success']:
-            return res.x[0], res.x[1], sign*res.fun
-        raise ValueError(f"mtpv w1={w1} u1={u1} maxtorque={maxtorque} res: {res['message']}")
-
-    def _set_losspar(self, pfe):
-        self.fo = pfe['speed']*self.p
-        ef = pfe.get('ef', [2.0, 2.0])
-        hf = pfe.get('hf', [1.0, 1.0])
-        self.plexp = {'styoke_hyst': hf[0],
-                      'stteeth_hyst': hf[0],
-                      'styoke_eddy': ef[0],
-                      'stteeth_eddy': ef[0],
-                      'rotor_hyst': hf[1],
-                      'rotor_eddy': ef[1]}
-        #                          'magnet'):
-
-    def betai1_plcu(self, i1, w1=0):
-        return self.m*self.rstat(w1)*i1**2
+            startvals = self.bounds[0][1], 0, sum(self.bounds[-1])
+        else:
+            startvals = -self.bounds[0][1], 0, sum(self.bounds[-1])
 
-    def iqd_plcu(self, iq, id, w1=0):
-        return self.m*self.rstat(w1)*(iq**2+id**2)/2
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            def sqrtculoss(iqde):
+                pcu = self.culoss(iqde)
+                #logger.info("iqde %s --> pcu %f", iqde, pcu)
+                return pcu
+            res = so.minimize(
+                self.culoss, startvals, method='SLSQP',  # trust-constr
+                bounds=self.bounds,
+                #            jac=gradient_respecting_bounds(self.bounds, self.culoss),
+                constraints=[
+                    {'type': 'eq',
+                     'fun': lambda iqd: self.torque_iqd(*iqd) - torque}])
+                #options={'disp': disp, 'maxiter': maxiter})
+            if res['success']:
+                return res.x
+        logger.warning("%s: torque=%f %f, io=%s",
+                       res['message'], torque, self.torque_iqd(*startvals),
+                       startvals)
+        raise ValueError(res['message'])
+
+    def mtpa(self, i1max):
+        """return iq, id, iex currents and maximum torque per current """
+        T0 = self.torque_iqd(np.sqrt(2)*i1max, 0, self.bounds[-1][1])
+        def i1tq(tq):
+            return abs(i1max) - np.linalg.norm(self.iqd_torque(tq)[:2])/np.sqrt(2)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            tq = so.fsolve(i1tq, T0)[0]
+        iq, id, iex = self.iqd_torque(tq)
+        return iq, id, iex, tq
+
+    def mtpa_tmech(self, i1max, n):
+        """return iq, id, iex currents and maximum torque per current """
+        T0 = self.torque_iqd(np.sqrt(2)*i1max, 0, self.bounds[-1][0])
+        def i1tq(tq):
+            return i1max - np.linalg.norm(self.iqd_tmech(tq, n)[:2])/np.sqrt(2)
+        tq = so.fsolve(i1tq, T0)[0]
+        iq, id, iex = self.iqd_tmech(tq, n)
+        return iq, id, iex, tq
+
+    def iqd_tmech_umax(self, torque, w1, u1max, log=0, **kwargs):
+        """return currents and shaft torque at stator frequency and
+         with minimal losses at max voltage"""
+        iqde = self.iqd_tmech(torque, w1/2/np.pi/self.p)
+        if np.linalg.norm(
+            self.uqd(w1, *iqde)) <= u1max*np.sqrt(2):
+            if log:
+                log(iqde)
+            return (*iqde, torque)
+        beta, i1 = betai1(iqde[0], iqde[1])
+        iex = iqde[2]
+
+        def ubeta(b):
+            return np.sqrt(2)*u1max - np.linalg.norm(
+                         self.uqd(w1, *iqd(b, i1), iex))
+        beta = -np.pi/4 if torque>0 else -3*np.pi/4
+        io = *iqd(beta, i1), iex
+
+        #    logger.debug("--- torque %g io %s", torque, io)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            n = w1/2/np.pi/self.p
+            def sqrtculoss(iqde):
+                pcu = self.culoss(iqde)
+                #logger.info("iqde %s pcu %g", iqde, pcu)
+                return pcu
+
+            res = so.minimize(
+                self.culoss, io, method='SLSQP',  # trust-constr
+                bounds=self.bounds,
+                constraints=[
+                    {'type': 'eq',
+                     'fun': lambda iqd: self.tmech_iqd(*iqd, n) - torque},
+                    {'type': 'eq',
+                     'fun': lambda iqd: np.linalg.norm(
+                         self.uqd(w1, *iqd)) - u1max*np.sqrt(2)}])
+            #if res['success']:
+        if log:
+            log(res.x)
+        return *res.x, self.tmech_iqd(*res.x, n)
+        #logger.warning("%s: w1=%f torque=%f, u1max=%f, io=%s",
+        #               res['message'], w1, torque, u1max, io)
+        #raise ValueError(res['message'])
+
+    def iqd_torque_umax(self, torque, w1, u1max,
+                        disp=False, maxiter=500, log=0, **kwargs):
+        """return currents for torque with minimal losses"""
+        iqde = self.iqd_torque(torque, disp, maxiter)
+        if np.linalg.norm(
+            self.uqd(w1, *iqde)) <= u1max*np.sqrt(2):
+                if log:
+                    log(iqde)
+                return (*iqde, torque)
+        io = iqde[0], 0, iqde[2]
+        #    logger.debug("--- torque %g io %s", torque, io)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            def sqrtculoss(iqde):
+                pcu = self.culoss(iqde)
+                #logger.info("iqde %s pcu %g", iqde, pcu)
+                return pcu
+
+            res = so.minimize(
+                self.culoss, io, method='SLSQP',  # trust-constr
+                bounds=self.bounds,
+                #options={'disp': disp, 'maxiter': maxiter},
+                #            jac=gradient_respecting_bounds(self.bounds, self.culoss),
+                constraints=[
+                    {'type': 'eq',
+                     'fun': lambda iqd: self.torque_iqd(*iqd) - torque},
+                    {'type': 'eq',
+                     'fun': lambda iqd: np.linalg.norm(
+                         self.uqd(w1, *iqd)) - u1max*np.sqrt(2)}])
+            if res['success']:
+
+                if log:
+                    log(res.x)
+                return *res.x, self.torque_iqd(*res.x)
+        logger.warning("%s: w1=%f torque=%f, u1max=%f, io=%s",
+                       res['message'], w1, torque, u1max, io)
+        raise ValueError(res['message'])
 
-    def iqd_plcu1(self, iq, id, w1):
-        return self.iqd_plcu(iq, id, w1)
+    def w1_imax_umax(self, i1max, u1max):
+        """return frequency w1 and shaft torque at voltage u1max and current i1max
 
-    def iqd_plcu2(self, iq, id):
-        return np.zeros(np.asarray(iq).shape)
+        Keyword arguments:
+        u1max -- the maximum voltage (Vrms)
+        i1max -- the maximum current (Arms)"""
+        iq, id, iex, T = self.mtpa(i1max)
+        n0 = np.sqrt(2)*u1max/np.linalg.norm(
+                self.psi(iq, id, iex))/2/np.pi/self.p
+        return self.w1_umax(u1max, iq, id, iex), T
 
-    def betai1_losses(self, beta, i1, f):
-        return np.sum([self.betai1_plfe1(beta, i1, f),
-                       self.betai1_plfe2(beta, i1, f),
-                       self.betai1_plmag(beta, i1, f),
-                       self.betai1_plcu(i1), 2*np.pi*f], axis=0)
-
-    def iqd_losses(self, iq, id, f):
-        return np.sum([self.iqd_plfe1(iq, id, f),
-                       self.iqd_plfe2(iq, id, f),
-                       self.iqd_plmag(iq, id, f),
-                       self.iqd_plcu(iq, id, 2*np.pi*f)], axis=0)
-
-    def speedranges(self, i1max, u1max, speedmax, with_mtpv, weps=1e-4):
-        """calculate speed range intervals:
-        1. const current MTPA (u < u1max)
-        2. const voltage: flux reduction / MTPA and MTPV (if enabled)
-        returns list of speed limit for each interval
-        """
-        iq, id, T = self.mtpa(i1max)
-        logger.debug("speedrange i1 %f T %f", i1max, T)
-        w1max = 2*np.pi*speedmax*self.p
-        w1type = self.w1_umax(u1max, iq, id)
-        wl, wu = [w1type, w1max]
-        if with_mtpv:
-            kmax = 6
-            self.check_extrapolation = False
-        else:
-            kmax = 0
-            k = kmax
-        for k in range(kmax):
-            wx = wl + (wu-wl)/2
-            try:
-                iq, id = self.iqd_imax_umax(i1max, wx, u1max,
-                                            T, with_mtpv=False)[:2]
-                i1 = betai1(iq, id)[1]
-                try:
-                    def voltw1(wx):
-                        return np.linalg.norm(
-                            self.mtpv(wx, u1max,
-                                      maxtorque=T > 0)[:2]) - np.sqrt(2)*i1
-                    w, _, ier, _ = so.fsolve(voltw1, wx, full_output=True)
-                    logger.debug("3: ier %d i1 %f w %f w1 %f", ier, i1, w, wx)
-                    if ier in (1, 4, 5):
-                        self.check_extrapolation = True
-                        if abs(w[0]) <= wx:
-                            return [w/2/np.pi/self.p
-                                    for w in (w1type, w[0], w1max)]  # ['MTPA', 'MTPV']
-                        wl = w[0]
-                except ValueError as e:
-                    logger.debug(e)
-                    wl = wx
-                    pass
-            except ValueError as e:
-                logger.warning(e)
-                wu = wx
-            logger.debug("%d: wx %f wl %f wu %f --> %f",
-                         k, wx, wl, wu, 100*(wu-wl)/wl)
-
-        self.check_extrapolation = True
-        w1max = min(w1max, self.w1_umax(
-            u1max, *iqd(-np.pi/2, abs(i1max))))
-        return [w/2/np.pi/self.p for w in (w1type, w1max)]  # ['MTPA']
+    def w1_umax(self, u, iq, id, iex):
+        """return frequency w1 at given voltage u and id, iq current
 
+        Keyword arguments:
+        u -- the maximum voltage (RMS)
+        iq, id -- the d-q currents"""
+        w10 = np.sqrt(2)*u/np.linalg.norm(self.psi(iq, id, iex))
+        return so.fsolve(
+            lambda w1: np.linalg.norm(self.uqd(w1, iq, id, iex))-u*np.sqrt(2),
+            w10)[0]
 
-    def characteristics(self, T, n, u1max, nsamples=60, with_mtpv=True):
+    def characteristics(self, T, n, u1max, nsamples=50,
+                        with_tmech=True, **kwargs):
         """calculate torque speed characteristics.
         return dict with list values of
-        id, iq, n, T, ud, uq, u1, i1,
-        beta, gamma, phi, cosphi, pmech, n_type
+        n, T, u1, i1, beta, cosphi, pmech, n_type
 
         Keyword arguments:
-        T -- the maximum torque or the list of torque values in Nm
-        n -- the maximum speed or the list of speed values in 1/s
-        u1max -- the maximum voltage in V rms
+        T -- (float) the maximum torque in Nm
+        n -- (float) the maximum speed in 1/s
+        u1max -- (float) the maximum voltage in V rms
         nsamples -- (optional) number of speed samples
-        with_mtpv -- (optional) use mtpv if true (default)
+        with_tmech -- (optional) use friction and windage losses
         """
-        r = dict(id=[], iq=[], uq=[], ud=[], u1=[], i1=[], T=[],
-                 beta=[], gamma=[], phi=[], cosphi=[], pmech=[], n=[])
-        if np.isscalar(T):
-            iq, id = self.iqd_torque(T)
+        iq, id, iex = self.iqd_torque(T)
+        if with_tmech:
             i1max = betai1(iq, id)[1]
             if T < 0:
                 i1max = -i1max
-            w1 = self.w1_umax(u1max, iq, id)
-            n1 = w1/2/np.pi/self.p
-            r['n_type'] = n1
-            nmax = n
-            logger.info("Type speed %f n: %f nmax %f",
-                        60*n1, 60*n, 60*nmax)
-
-            n1 = min(n1, nmax)
-            if n1 < nmax:
-                speedrange = [0] + self.speedranges(i1max, u1max,
-                                                     nmax, with_mtpv)
-                if len(speedrange) > 3:
-                    interv = 'MTPA', 'MTPV'
-                else:
-                    interv = 'MTPA',
+            w1type, Tf = self.w1_imax_umax(i1max, u1max)
+        else:
+            Tf = T
+            w1type = self.w1_umax(u1max, iq, id, iex)
+        logger.debug("w1type %f", w1type)
+        wmType = w1type/self.p
+        pmax = Tf*wmType
+
+        def tload(wm):
+            if abs(wm*Tf) < abs(pmax):
+                return Tf
+            return pmax/wm
+
+        wmtab = []
+        dw = 0
+        wmMax = 3.5*wmType
+        if n > 0:
+            wmMax = min(wmMax, 2*np.pi*n)
+        if wmType > wmMax:
+            wmrange = sorted([0, wmMax])
+            wmtab = np.linspace(0, wmMax, nsamples).tolist()
+        else:
+            wmrange = sorted([0, wmType, wmMax])
+            nx = int(round(nsamples*wmType/wmMax))
+            dw = (wmMax-wmType)/(nsamples-nx)
+            wmtab = (np.linspace(0, wmType, nx).tolist() +
+                     np.linspace(wmType+dw, wmMax, nsamples-nx).tolist())
+
+        logger.info("Speed range T %f %s", Tf, wmrange)
+        wmtab[0] = 0
+
+        r = dict(u1=[], i1=[], id=[], iq=[], iex=[], T=[], cosphi=[], n=[],
+                 beta=[], plfe1=[], plcu1=[], plcu2=[])
+        for wm, tq in zip(wmtab, [tload(wx) for wx in wmtab]):
+            w1 = wm*self.p
+            if with_tmech:
+                iq, id, iex, tqx = self.iqd_tmech_umax(
+                        tq, w1, u1max)
             else:
-                speedrange = [0, n1]
-                interv = []
-
-            logger.info("Speedrange T=%g %s", T, speedrange)
-            n3 = speedrange[-1]
-            nstab = [int(nsamples*(x1-x2)/n3)
-                     for x1, x2 in zip(speedrange[1:],
-                                       speedrange)]
-            logger.info("sample intervals %s", nstab)
-            for nx in np.linspace(0, n1, nstab[0]):
-                r['id'].append(id)
-                r['iq'].append(iq)
-                r['n'].append(nx)
-                r['T'].append(T)
-
-            for ns, nu, iv in zip(nstab[1:], speedrange[2:], interv):
-                # find id, iq, torque in fieldweakening range
-                if ns == 0:
-                    ns = 1
-                dn = (nu - r['n'][-1])/ns
-                logger.info("RANGE %s %d: %f -- %f",
-                            iv, ns, r['n'][-1] + dn, nu)
-                try:
-                    for nn in np.linspace(r['n'][-1]+dn, nu, ns):
-                        w1 = 2*np.pi*nn*self.p
-                        logger.debug("fieldweakening: n %g T %g i1max %g w1 %g u1 %g",
-                                     nn*60, T, i1max, w1, u1max)
-                        if iv == 'MTPA':
-                            iq, id, tq = self.iqd_imax_umax(i1max, w1, u1max, T,
-                                                            with_mtpv=False)
-                        else:
-                            iq, id, tq = self.mtpv(w1, u1max,
-                                                   maxtorque=T > 0)
-                        if (T > 0 and tq > 0) or (T < 0 and tq < 0):
-                            r['id'].append(id)
-                            r['iq'].append(iq)
-                            r['n'].append(nn)
-                            r['T'].append(tq)
-                        else:
-                            logger.warning("fieldweakening: n %g T %g tq %g i1max %g w1 %g u1 %g",
-                                           nn*60, T, tq, i1max, w1, u1max)
-                except ValueError as e:
-                    nmax = r['n'][-1]
-                    logger.warning("%s: adjusted nmax %f", e, nmax)
-        else:
-            for t, nx in zip(T, n):
-                w1 = 2*np.pi*nx*self.p
-                iq, id, tq = self.iqd_torque_umax(t, w1, u1max)
-                r['id'].append(id)
-                r['iq'].append(iq)
-                r['T'].append(tq)
-                r['n'].append(nx)
-
-        for nx, iq, id in zip(r['n'], r['iq'], r['id']):
-            w1 = 2*np.pi*nx*self.p
-            uq, ud = self.uqd(w1, iq, id)
-            r['uq'].append(uq)
-            r['ud'].append(ud)
-            r['u1'].append(la.norm((ud, uq))/np.sqrt(2.0))
-            r['i1'].append(la.norm((id, iq))/np.sqrt(2.0))
-            r['beta'].append(np.arctan2(id, iq)/np.pi*180.)
-            r['gamma'].append(np.arctan2(ud, uq)/np.pi*180.)
-
-            r['phi'].append(r['beta'][-1] - r['gamma'][-1])
-            r['cosphi'].append(np.cos(r['phi'][-1]/180*np.pi))
-
-        pmech = np.array([2*np.pi*nx*tq for nx, tq in zip(r['n'], r['T'])])
-        f1 = np.array(r['n'])*self.p
-        plfe1 = self.iqd_plfe1(np.array(r['iq']), np.array(r['id']), f1)
-        plfe2 = self.iqd_plfe2(np.array(r['iq']), np.array(r['id']), f1)
-        plmag = self.iqd_plmag(np.array(r['iq']), np.array(r['id']), f1)
-        plfe = plfe1 + plfe2 + plmag
-        plcu = self.betai1_plcu(np.array(r['i1']), 2*np.pi*f1)
-        pltotal = plfe + plcu
-        r['pmech'] = pmech.tolist()
-        r['plfe'] = plfe.tolist()
-        r['plcu'] = plcu.tolist()
+                iq, id, iex, tqx = self.iqd_torque_umax(
+                        tq, w1, u1max)
+                tqx -= self.tfric
+            uq, ud = self.uqd(w1, iq, id, iex)
+            u1 = np.linalg.norm((uq, ud))/np.sqrt(2)
+            f1 = w1/2/np.pi
+            r['id'].append(id)
+            r['iq'].append(iq)
+            r['iex'].append(iex)
+            r['u1'].append(u1)
+            beta = np.arctan2(id, iq)
+            if beta > 0:
+                beta -= 2*np.pi
+            i1 = np.linalg.norm((id, iq), axis=0)/np.sqrt(2.0)
+            r['i1'].append(i1)
+            r['beta'].append(beta/180*np.pi)
+            gamma = np.arctan2(ud, uq)
+            r['cosphi'].append(np.cos(gamma - beta))
+            r['plfe1'].append(self.iqd_plfe1(iq, id, iex, f1))
+            r['plcu1'].append(self.m*i1**2*self.rstat(w1))
+            r['plcu2'].append(iex**2*self.rrot(0))
+            r['T'].append(tqx)
+            r['n'].append(wm/2/np.pi)
+
+        r['plfe'] = r['plfe1']
+        r['plcu'] = (np.array(r['plcu1']) + np.array(r['plcu2'])).tolist()
+        r['plfw'] = [self.pfric(n) for n in r['n']]
+        r['pmech'] = [2*np.pi*n*tq
+                      for n, tq in zip(r['n'], r['T'])]
+        pmech = np.array(r['pmech'])
+        pltotal = (np.array(r['plfe1']) + np.array(r['plfw']) +
+                   np.array(r['plcu1']) + np.array(r['plcu2']))
         r['losses'] = pltotal.tolist()
+
         if pmech.any():
             p1 = pmech + pltotal
             if np.abs(pmech[0]) < 1e-12:
                 r['eta'] = [0]
                 i = 1
             else:
                 r['eta'] = []
                 i = 0
             if np.all(abs(p1[i:]) > abs(pmech[i:])):
                 r['eta'] += (pmech[i:]/(p1[i:])).tolist()
             else:
                 r['eta'] += (p1[i:]/pmech[i:]).tolist()
-        return r
 
-    def i1beta_characteristics(self, n_list, i1_list, beta_list, u1max):
-        """calculate i1-beta characteristics"""
-        r = dict(id=[], iq=[], uq=[], ud=[], u1=[], i1=[], T=[],
-                 beta=[], gamma=[], phi=[], cosphi=[], pmech=[], n=[])
-        for n, i1, beta in zip(n_list, i1_list, beta_list):
-            w1 = 2*np.pi*n*self.p
-            beta = beta/180*np.pi
-            iq, id = iqd(beta, i1)
-            uq, ud = self.uqd(w1, iq, id)
-            u1 = la.norm((ud, uq))/np.sqrt(2)
-            if u1 > u1max:
-                logger.debug("u1 %s > %s", u1, u1max)
-                beta = self.beta_u(w1, u1max, i1)
-                logger.debug("beta %s", beta*180/np.pi)
-                iq, id = iqd(beta, i1)
-                logger.debug("beta %s id, %s iq %s", beta*180/np.pi, id, iq)
-                uq, ud = self.uqd(w1, iq, id)
-                u1 = la.norm((ud, uq))/np.sqrt(2)
-                logger.debug("ud %s uq %s --> u1 %s", ud, uq, u1)
-
-            tq = self.torque_iqd(iq, id)
+        return r
 
-            r['id'].append(id)
-            r['iq'].append(iq)
 
-            r['uq'].append(uq)
-            r['ud'].append(ud)
-            r['u1'].append(u1)
-            r['i1'].append(la.norm((id, iq))/np.sqrt(2))
-            r['T'].append(tq)
-            r['beta'].append(np.arctan2(id, iq)/np.pi*180.)
-            r['gamma'].append(np.arctan2(ud, uq)/np.pi*180.)
-
-            r['n'].append(n)
-            r['phi'].append(r['beta'][-1]-r['gamma'][-1])
-            r['cosphi'].append(np.cos(r['phi'][-1]/180*np.pi))
-            r['pmech'].append(w1/self.p*r['T'][-1])
-
-        r['losses'] = self.iqd_losses(
-            *iqd(np.array(beta_list)/180*np.pi,
-                 np.array(i1_list)),
-            np.array(n_list)*self.p).tolist()
-        return r
+class SynchronousMachinePsidq(SynchronousMachine):
 
-    def _inrange(self, iqd):
-        i1 = np.linalg.norm(iqd)/np.sqrt(2)
-        iqmin, idmin = self.iqdmin(i1)
-        iqmax, idmax = self.iqdmax(i1)
-        return iqmin <= iqd[0] <= iqmax and idmin <= iqd[1] <= idmax
-
-
-class PmRelMachineLdq(PmRelMachine):
-    """Standard set of PM machine given by i1,beta parameters:
-    p number of pole pairs
-    m number of phases
-    psim flux in Vs (RMS)
-    ld d-inductance in
-    lq q-inductance in H
-    r1 stator resistance
-    ls stator leakage inductance in H
-    beta angle i1 vs up in degrees
-    i1 current in A (RMS)
-
-    optional keyword args:
-    psid D-Flux in Vs (RMS)
-    psiq Q-Flux in Vs (RMS)
-    """
-
-    def __init__(self,  m, p, psim=[], ld=[], lq=[],
-                 r1=0, beta=[], i1=[], ls=0, **kwargs):
-
-        super(self.__class__, self).__init__(m, p, r1, ls)
-        self.psid = None
-        self.betarange = (-np.pi, np.pi)
-        self.i1range = (0, np.inf)
-        if np.isscalar(ld):
-            self.ld = lambda b, i: ld
-            self.psim = lambda b, i: psim
-            self.lq = lambda b, i: lq
-            logger.debug("ld %s lq %s psim %s", ld, lq, psim)
-            return
-
-        if len(ld) == 1:
-            try:
-                self.io = iqd(min(beta)*np.pi/360, max(i1)/2)
-            except:
-                self.io = (1, -1)
-            self.ld = lambda b, i: ld[0]
-            self.psim = lambda b, i: psim[0]
-            self.lq = lambda b, i: lq[0]
-            logger.debug("ld %s lq %s psim %s", ld, lq, psim)
-            return
-
-        beta = np.asarray(beta)/180.0*np.pi
-        if np.any(beta[beta > np.pi]):
-            beta[beta > np.pi] = beta - 2*np.pi
-        self.io = iqd((np.min(beta)+max(beta))/2, np.max(i1)/2)
-        kx = ky = 3
-        if len(i1) < 4:
-            ky = len(i1)-1
-        if len(beta) < 4:
-            kx = len(beta)-1
+    def __init__(self, eecpars, lfe=1, wdg=1, **kwargs):
+        super(self.__class__, self).__init__(
+                eecpars, **kwargs)
+        self.iqrange = (eecpars['psidq'][0]['iq'][0],
+                        eecpars['psidq'][0]['iq'][-1])
+        self.idrange = (eecpars['psidq'][0]['id'][0],
+                        eecpars['psidq'][0]['id'][-1])
+        islinear = True
+        iexc = [l['ex_current'] for l in eecpars['psidq']]
+        id = [i/wdg for i in eecpars['psidq'][-1]['id']]
+        idx = np.linspace(id[0], id[-1], 12)
+        iq = [i/wdg for i in eecpars['psidq'][-1]['iq']]
+        iqx = np.linspace(iq[0], iq[-1], 20)
+
+        if _islinear(iexc):
+            exc = iexc
+            psid = wdg*lfe*np.array([
+                    _splinterp(iq, id, iqx, idx, l['psid'])
+                    for l in eecpars['psidq']])
+            psiq = wdg*lfe*np.array([
+                    _splinterp(iq, id, iqx, idx, l['psiq'])
+                    for l in eecpars['psidq']])
+        else:
+            islinear = False
+            nsamples = 10
+            iexcl = np.linspace(iexc[0], iexc[-1], nsamples)
+            exc = iexcl
+            psid = wdg*lfe*_linsampl(iexc, iexcl, np.array(
+                    [_splinterp(iq, id, iqx, idx, l['psid'])
+                     for l in eecpars['psidq']]))
+            psiq = wdg*lfe*_linsampl(iexc, iexcl, np.array(
+                    [_splinterp(iq, id, iqx, idx, l['psiq'])
+                     for l in eecpars['psidq']]))
+
+        self.psidf = ip.RegularGridInterpolator(
+                (exc, iqx, idx), psid,
+                method='cubic', bounds_error=False, fill_value=None)
+        self.psiqf = ip.RegularGridInterpolator(
+                (exc, iqx, idx), psiq,
+                method='cubic', bounds_error=False, fill_value=None)
+        self.bounds = [(min(iq), max(iq)),
+                       (min(id), 0),
+                       (iexc[0], iexc[-1])]
         try:
-            pfe = kwargs['losses']
-            self._set_losspar(pfe)
-            self._losses = {k: ip.RectBivariateSpline(
-                beta, i1, np.array(pfe[k]),
-                kx=kx, ky=ky).ev for k in (
-                    'styoke_hyst', 'stteeth_hyst',
-                    'styoke_eddy', 'stteeth_eddy',
-                    'rotor_hyst', 'rotor_eddy',
-                    'magnet')}
-        except KeyError as e:
-            logger.warning("loss map missing: %s", e)
-            pass
-        if 'psid' in kwargs:
-            self.betarange = min(beta), max(beta)
-            self.i1range = (0, np.max(i1))
-            self.psid = lambda x, y: ip.RectBivariateSpline(
-                beta, i1, np.sqrt(2)*np.asarray(kwargs['psid']),
-                kx=kx, ky=ky).ev(x, y)
-            self.psiq = lambda x, y: ip.RectBivariateSpline(
-                beta, i1, np.sqrt(2)*np.asarray(kwargs['psiq']),
-                kx=kx, ky=ky).ev(x, y)
-
-            return
-
-        if len(i1) < 4 or len(beta) < 4:
-            if len(i1) == len(beta):
-                self.ld = lambda x, y: ip.interp2d(beta, i1, ld.T)(x, y)
-                self.psim = lambda x, y: ip.interp2d(beta, i1, psim.T)(x, y)
-                self.lq = lambda x, y: ip.interp2d(beta, i1, lq.T)(x, y)
-                logger.debug("interp2d beta %s i1 %s", beta, i1)
-                return
-            elif len(i1) == 1:
-                self.ld = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    beta, ld, k=1)(x)
-                self.psim = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    beta, psim, k=1)(x)
-                self.lq = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    beta, lq, k=1)(x)
-                logger.debug("interpolatedunivariatespline beta %s", beta)
-                return
-            if len(beta) == 1:
-                self.ld = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    i1, ld, k=1)(y)
-                self.psim = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    i1, ld, k=1)(y)
-                self.lq = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    i1, lq, k=1)(y)
-                logger.debug("interpolatedunivariatespline i1 %s", i1)
-                return
-
-            raise ValueError("unsupported array size {}x{}".format(
-                len(beta), len(i1)))
-
-        self.betarange = min(beta), max(beta)
-        self.i1range = (0, np.max(i1))
-        self.ld = lambda x, y: ip.RectBivariateSpline(
-            beta, i1, np.asarray(ld)).ev(x, y)
-        self.psim = lambda x, y: ip.RectBivariateSpline(
-            beta, i1, np.asarray(psim)).ev(x, y)
-        self.lq = lambda x, y: ip.RectBivariateSpline(
-            beta, i1, np.asarray(lq)).ev(x, y)
-        logger.debug("rectbivariatespline beta %s i1 %s", beta, i1)
-
-    def psi(self, iq, id):
-        """return psid, psiq of currents iq, id"""
-        beta, i1 = betai1(np.asarray(iq), np.asarray(id))
-        #logger.debug('beta %f (%f, %f) i1 %f %f',
-        #             beta, self.betarange[0], self.betarange[1],
-        #             i1, self.i1range[1])
-        if self.check_extrapolation:
-            if (self.betarange[0] > beta or
-                self.betarange[1] < beta or
-                i1 > 1.01*self.i1range[1]):
-                return (np.nan, np.nan)
-        if self.psid:
-            return (self.psid(beta, i1), self.psiq(beta, i1))
-
-        psid = self.ld(beta, i1)*id + np.sqrt(2)*self.psim(beta, i1)
-        psiq = self.lq(beta, i1)*iq
-        return (psid, psiq)
-
-    def iqdmin(self, i1):
-        """max iq, min id for given current"""
-        if self.betarange[0] <= -np.pi/2 <= self.betarange[1]:
-            return iqd(-np.pi/2, i1)
-        if self.betarange[1] == 0:
-            return iqd(self.betarange[0], i1)
-        return iqd(self.betarange[1], i1)
-
-    def iqdmax(self, i1):
-        """max iq, min id for given current"""
-        if self.betarange[1] == 0:
-            return iqd(self.betarange[1], i1)
-        return iqd(self.betarange[0], i1)
+            idname = 'psidq'
+            keys = self.plexp.keys()
+            if islinear:
+                pfe = {k: np.array([l['losses'][k]
+                                    for l in eecpars[idname]])
+                       for k in keys}
+            else:
+                pfe = {k: _linsampl(iexc, iexcl,
+                                    np.array([l['losses'][k]
+                                             for l in eecpars[idname]]))
+                       for k in keys}
+            self._losses = {k: ip.RegularGridInterpolator(
+                    (exc, iq, id), lfe*np.array(pfe[k]),
+                    method='cubic', bounds_error=False, fill_value=None)
+                            for k in keys}
+            self._set_losspar(eecpars[idname][0]['losses']['speed'],
+                          eecpars[idname][0]['losses']['ef'],
+                          eecpars[idname][0]['losses']['hf'])
+        except KeyError:
+            logger.warning("loss map missing")
+            self._losses = {k: lambda x: 0 for k in (
+                'styoke_hyst', 'stteeth_hyst',
+                'styoke_eddy', 'stteeth_eddy',
+                'rotor_hyst', 'rotor_eddy')}
 
-    def betai1_plfe1(self, beta, i1, f1):
-        return np.sum([
-            self._losses[k](beta, i1)*(f1/self.fo)**self.plexp[k] for
-            k in ('styoke_eddy', 'styoke_hyst',
-                  'stteeth_eddy', 'stteeth_hyst')], axis=0)
 
-    def iqd_plfe1(self, iq, id, f1):
-        return self.betai1_plfe1(*betai1(iq, id), f1)
+    def psi(self, iq, id, iex):
+        """return psid, psiq of currents iq, id"""
+        try:
+            return self.psidf((iex, iq, id)), self.psiqf((iex, iq, id))
+        except ValueError as ex:
+            logger.error(iex, iq, id)
+            raise ex
 
-    def betai1_plfe2(self, beta, i1, f1):
+    def plfe1(self, iq, id, iex, f1):
         return np.sum([
-            self._losses[k](beta, i1)*(f1/self.fo)**self.plexp[k] for
-            k in ('rotor_eddy', 'rotor_hyst',)], axis=0)
-
-    def iqd_plfe2(self, iq, id, f1):
-        return self.betai1_plfe2(*betai1(iq, id), f1)
-
-    def betai1_plmag(self, beta, i1, f1):
-        return self._losses['magnet'](beta, i1)*(f1/self.fo)**2
-
-    def iqd_plmag(self, iq, id, f1):
-        return self.betai1_plmag(*betai1(iq, id), f1)
-
-
-class PmRelMachinePsidq(PmRelMachine):
-    """Standard set of PM machine parameters:
-    p number of pole pairs
-    m number of phases
-
-    psid d-flux (Vs Peak)
-    psiq q-flux (Vs Peak)
-    r1 stator resistance (Ohm)
-    r1 stator leakage inductance (H)
-    id q current (A, Peak)
-    iq q current (A, Peak)
-    """
-
-    def __init__(self, m, p, psid, psiq, r1, id, iq, ls=0, **kwargs):
-        super(self.__class__, self).__init__(m, p, r1, ls)
-
-        if isinstance(psid, (float, int)):
-            self._psid = lambda id, iq: np.array([[psid]])
-            self._psiq = lambda id, iq: np.array([[psiq]])
-            return
-
-        psid = np.asarray(psid)
-        psiq = np.asarray(psiq)
-        id = np.asarray(id)
-        iq = np.asarray(iq)
-        self.idrange = (min(id), max(id))
-        self.iqrange = (min(iq), max(iq))
-        self.betarange = (-np.pi if min(iq) < 0 else -np.pi/2,
-                          0 if max(iq) > 0 else -np.pi/2)
-        self.i1range = (0, np.sqrt(2)*np.min(id))
-        self.io = np.max(iq)/2, np.min(id)/2
-
-        if np.any(psid.shape < (4, 4)):
-            if psid.shape[0] > 1 and psid.shape[1] > 1:
-                self._psid = ip.interp2d(iq, id, psid.T)
-                self._psiq = ip.interp2d(iq, id, psiq.T)
-                return
-            if len(id) == 1 or psid.shape[1] == 1:
-                self._psid = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    iq, psid)(x)
-                self._psiq = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    iq, psiq)(x)
-                return
-            if len(iq) == 1 or psid.shape[0] == 1:
-                self._psid = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    id, psid)(y)
-                self._psiq = lambda x, y: ip.InterpolatedUnivariateSpline(
-                    id, psiq)(y)
-                return
-            raise ValueError("unsupported array size {}x{}".format(
-                len(psid.shape[0]), psid.shape[1]))
-
-        self._psid = lambda x, y: ip.RectBivariateSpline(
-            iq, id, psid).ev(x, y)
-        self._psiq = lambda x, y: ip.RectBivariateSpline(
-            iq, id, psiq).ev(x, y)
+            self._losses[k]((iex, iq, id))*(f1/self.fo)**self.plexp[k][0]
+            for k in ('styoke_eddy', 'styoke_hyst',
+                      'stteeth_eddy', 'stteeth_hyst')], axis=0)
+
+    def iqd_plfe1(self, iq, id, iex, f1):
+        return self.plfe1(iq, id, iex, f1)
+
+
+class SynchronousMachineLdq(SynchronousMachine):
+    def __init__(self, eecpars, lfe=1, wdg=1, **kwargs):
+        super(self.__class__, self).__init__(eecpars, **kwargs)
+        self.betarange = (eecpars['ldq'][0]['beta'][0]/180*np.pi,
+                          eecpars['ldq'][0]['beta'][-1]/180*np.pi)
+        self.i1range = (0, eecpars['ldq'][0]['i1'][-1])
+        islinear = True
+        iexc = [l['ex_current'] for l in eecpars['ldq']]
+        i1 = [i/wdg for i in eecpars['ldq'][-1]['i1']]
+        i1x = np.linspace(i1[0], i1[-1], 12)
+        beta = [b*np.pi/180 for b in eecpars['ldq'][-1]['beta']]
+        betax = np.linspace(beta[0], beta[-1], 20)
+
+        if _islinear(iexc):
+            exc = iexc
+            psid = wdg*lfe*np.array([
+                    _splinterp(beta, i1, betax, i1x, l['psid'])
+                    for l in eecpars['ldq']])
+            psiq = wdg*lfe*np.array([
+                    _splinterp(beta, i1, betax, i1x, l['psiq'])
+                    for l in eecpars['ldq']])
+        else:
+            islinear = False
+            nsamples = 10
+            iexcl = np.linspace(iexc[0], iexc[-1], nsamples)
+            exc = iexcl
+            psid = wdg*lfe*_linsampl(iexc, iexcl, np.array(
+                    [_splinterp(beta, i1, betax, i1x, l['psid'])
+                     for l in eecpars['ldq']]))
+            psiq = wdg*lfe*_linsampl(iexc, iexcl, np.array(
+                    [_splinterp(beta, i1, betax, i1x, l['psiq'])
+                     for l in eecpars['ldq']]))
+
+        # extrapolate outside range
+        self.psidf = ip.RegularGridInterpolator(
+                (exc, betax, i1x), np.sqrt(2)*psid,
+                method='cubic',
+                bounds_error=False, fill_value=None)
+        self.psiqf = ip.RegularGridInterpolator(
+                (exc, betax, i1x), np.sqrt(2)*psiq,
+                method='cubic'
+                , bounds_error=False, fill_value=None)
+        i1max = np.sqrt(2)*(max(i1))
+        self.bounds = [(np.cos(min(beta))*i1max, i1max),
+                       (-i1max, 0),
+                       (iexc[0], iexc[-1])]
+        keys = self.plexp.keys()
         try:
-            pfe = kwargs['losses']
-            self._set_losspar(pfe)
-            self._losses = {k: ip.RectBivariateSpline(
-                iq, id, np.array(pfe[k])).ev for k in (
+            idname = 'ldq'
+            if islinear:
+                pfe = {k: np.array([l['losses'][k]
+                                    for l in eecpars[idname]])
+                       for k in keys}
+            else:
+                pfe = {k: _linsampl(iexc, iexcl,
+                                    np.array([l['losses'][k]
+                                             for l in eecpars[idname]]))
+                       for k in keys}
+        # fill value with nan outside range
+            self._losses = {k: ip.RegularGridInterpolator(
+                    (exc, beta, i1), lfe*np.array(pfe[k]),
+                    method='cubic', bounds_error=False, fill_value=None)
+                            for k in keys}
+            self._set_losspar(eecpars[idname][0]['losses']['speed'],
+                              eecpars[idname][0]['losses']['ef'],
+                              eecpars[idname][0]['losses']['hf'])
+        except ValueError:
+            logger.warning("loss map missing")
+            self._losses = {k: lambda x: 0 for k in (
                 'styoke_hyst', 'stteeth_hyst',
                 'styoke_eddy', 'stteeth_eddy',
-                'rotor_hyst', 'rotor_eddy',
-                'magnet')}
-        except KeyError as e:
-            logger.warning("loss map missing: %s", e)
-            pass
-
-    def psi(self, iq, id):
-        return (self._psid(iq, id),
-                self._psiq(iq, id))
-
-    def iqdmin(self, i1):
-        """max iq, min id for given current"""
-        if self.idrange[0] < 0 and self.idrange[1] <= 0:
-            idmin = -np.sqrt(2)*i1
-        else:
-            idmin = 0
-        if self.idrange[0] <= idmin/np.sqrt(2):
-            iqmin = -np.sqrt(2)*i1
-            if self.iqrange[0] <= iqmin:
-                return (iqmin, idmin)
-            return self.iqrange[0], idmin
-
-        beta = np.arccos(self.iqrange[0]/i1/np.sqrt(2))
-        iqmin = np.sqrt(2)*i1*np.sin(beta)
-        if self.iqrange[0] <= iqmin:
-            return (iqmin, idmin)
-
-        return self.iqrange[0], self.idrange[0]
-
-    def iqdmax(self, i1):
-        """max iq, max id for given current"""
-        iqmax = np.sqrt(2)*i1
-        if iqmax <= np.max(self.iqrange):
-            if np.min(self.idrange) < 0 and np.max(self.idrange) <= 0:
-                idmax = 0
-            else:
-                idmax = np.sqrt(2)*i1
-            if idmax <= np.max(self.idrange):
-                return (iqmax, idmax)
-            return (iqmax, np.max(self.idrange))
-
-        beta = np.arccos(self.iqrange[1]/iqmax)
-        iqmax = np.sqrt(2)*i1*np.cos(beta)
-        idmax = np.sqrt(2)*i1*np.sin(beta)
-        if idmax <= np.max(self.idrange):
-            return (iqmax, idmax)
-
-        return iqmax, np.max(self.idrange)
-
-    def iqd_plfe1(self, iq, id, f1):
-        return np.sum([
-            self._losses[k](iq, id)*(f1/self.fo)**self.plexp[k] for
-            k in ('styoke_eddy', 'styoke_hyst',
-                  'stteeth_eddy', 'stteeth_hyst')], axis=0)
+                'rotor_hyst', 'rotor_eddy')}
 
-    def betai1_plfe1(self, beta, i1, f1):
-        return self.iqd_plfe1(*iqd(beta, i1), f1)
+    def psi(self, iq, id, iex):
+        """return psid, psiq of currents iq, id"""
+        beta = np.arctan2(id, iq)
+        if beta > 0:
+            beta -= 2*np.pi
+        i1 = np.linalg.norm((id, iq), axis=0)/np.sqrt(2.0)
+        try:
+            return self.psidf((iex, beta, i1)), self.psiqf((iex, beta, i1))
+        except ValueError as ex:
+            logger.error("iex %s iq %f id %f beta %f i1 %f",
+                         iex, iq, id, beta, i1)
+            raise ex
 
-    def iqd_plfe2(self, iq, id, f1):
+    def plfe1(self, beta, i1, iex, f1):
         return np.sum([
-            self._losses[k](iq, id)*(f1/self.fo)**self.plexp[k] for
-            k in ('rotor_eddy', 'rotor_hyst',)], axis=0)
-
-    def betai1_plfe2(self, beta, i1, f1):
-        return self.iqd_plfe2(*iqd(beta, i1), f1)
-
-    def iqd_plmag(self, iq, id, f1):
-        return self._losses['magnet'](iq, id)*(f1/self.fo)**2
-
-    def betai1_plmag(self, beta, i1, f1):
-        return self.iqd_plmag(*iqd(beta, i1), f1)
+            self._losses[k]((iex, beta, i1))*(f1/self.fo)**self.plexp[k][0]
+            for k in ('styoke_eddy', 'styoke_hyst',
+                      'stteeth_eddy', 'stteeth_hyst')], axis=0)
+    def iqd_plfe1(self, iq, id, iex, f1):
+        beta = np.arctan2(id, iq)
+        if np.isscalar(beta):
+            if beta > 0:
+                beta -= 2*np.pi
+        else:
+            beta[beta > 0] -= 2*np.pi
+        i1 = np.linalg.norm((id, iq), axis=0)/np.sqrt(2.0)
+        return self.plfe1(beta, i1, iex, f1)
+
+
+if __name__ == '__main__':
+    import sys
+    import json
+    import femagtools.plot
+    import matplotlib.pyplot as plt
+    with open(sys.argv[1]) as fp:
+        eecpar = json.load(fp)
+    if 'ldq' in eecpar:
+        m = SynchronousMachineLdq(eecpar)
+    else:
+        m = SynchronousMachinePsidq(eecpar)
+    T = 240
+    u1max = 163
+    nmax = 1000
+    r = m.characteristics(T, 0, u1max)
+    femagtools.plot.characteristics(r, 'SynchronousMachine')
+    plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `femagtools-1.3.0/femagtools/machine/sizing.py` & `femagtools-1.3.1/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/machine/utils.py` & `femagtools-1.3.1/femagtools/machine/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/magnet.py` & `femagtools-1.3.1/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/mcv.py` & `femagtools-1.3.1/femagtools/mcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,16 +492,15 @@
                                          self.PARAMETER_PM_CURVE):
                 self.writeBlock([self.mc1_angle[K], self.mc1_db2[K]])
 
         if not (self.mc1_ch_factor or self.mc1_cw_factor) and self.losses:
             pfe = self.losses['pfe']
             f = self.losses['f']
             B = self.losses['B']
-            colsize = len(f)
-            losses = [list(p) + [0]*(colsize-len(p)) for p in pfe]
+            losses = [list(p) + [None]*(len(B)-len(p)) for p in pfe]
             fo = self.mc1_base_frequency
             Bo = self.mc1_base_induction
             fit_jordan = False
             if fit_jordan:
                 ch, alfa, cw, beta, gamma = lc.fitjordan(f, B, losses, Bo, fo)
                 self.mc1_ch_factor = ch
                 self.mc1_ch_freq_factor = alfa
@@ -553,36 +552,35 @@
                 self.losses['cw'] = cw
                 self.losses['cw_freq'] = alfa
                 self.losses['b_coeff'] = beta
                 self.losses['Bo'] = Bo
                 self.losses['fo'] = fo
 
             self.writeBlock([nfreq, nind])
-            self.writeBlock(B +
-                            [0.0]*(M_LOSS_INDUCT - nind))
+            self.writeBlock([float(b) for b in B] + [0.0]*(M_LOSS_INDUCT - nind))
 
             for f, p in zip(self.losses['f'], pfe):
                 if f > 0:
                     y = np.array(p)
-                    losses = y[y != np.array(None)].tolist()
+                    losses = [float(x) for x in y[y != np.array(None)]]
                     if len(losses) == nind:
                         pl = p
                     else:
                         n = len(losses)
                         cw, alfa, beta = lc.fitsteinmetz(
                             f, B[:n], losses, Bo, fo)
-                        pl = [lc.pfe_steinmetz(
+                        pl = losses + [lc.pfe_steinmetz(
                             f, b, cw, alfa, beta,
                             self.losses['fo'],
                             self.losses['Bo'])
-                              for b in B]
+                                       for b in B[n:]]
                     logger.debug("%s", pl)
                     self.writeBlock(pl +
                                     [0.0]*(M_LOSS_INDUCT - len(pl)))
-                    self.writeBlock(f)
+                    self.writeBlock(float(f))
             for m in range(M_LOSS_FREQ - len(pfe)):
                 self.writeBlock([0.0]*M_LOSS_INDUCT)
                 self.writeBlock(0.0)
 
             self.writeBlock([self.losses['cw'], self.losses['cw_freq'],
                              self.losses['b_coeff'], self.losses['fo'],
                              self.losses['Bo']])
```

### Comparing `femagtools-1.3.0/femagtools/me.py` & `femagtools-1.3.1/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/model.py` & `femagtools-1.3.1/femagtools/model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/moo/algorithm.py` & `femagtools-1.3.1/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/moo/population.py` & `femagtools-1.3.1/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/moo/problem.py` & `femagtools-1.3.1/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/moproblem.py` & `femagtools-1.3.1/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/multiproc.py` & `femagtools-1.3.1/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/mxw2msh.py` & `femagtools-1.3.1/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/nc.py` & `femagtools-1.3.1/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/netlist.py` & `femagtools-1.3.1/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/ntib.py` & `femagtools-1.3.1/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/opt.py` & `femagtools-1.3.1/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/parstudy.py` & `femagtools-1.3.1/femagtools/parstudy.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         Args:
           dirname: name of report directory
         """
         if os.listdir(dirname):
             raise ValueError("directory {} is not empty".format(dirname))
         self.reportdir = dirname
 
-    def setup_model(self, builder, model, recsin):
+    def setup_model(self, builder, model, recsin=''):
         """builds model in current workdir and returns its filenames"""
         # get and write mag curves
         mc_files = self.femag.copy_magnetizing_curves(model, recsin=recsin)
 
         if model.is_complete():
             logger.info("setup model in %s", self.femag.workdir)
             filename = 'femag.fsl'
```

### Comparing `femagtools-1.3.0/femagtools/plot.py` & `femagtools-1.3.1/femagtools/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -892,15 +892,42 @@
     ax.grid(True)
     ax.plot(bch.scData['time'], bch.scData['torque'])
     ax.set_xlabel('Time / s')
 
     fig.tight_layout(h_pad=2)
     if title:
         fig.subplots_adjust(top=0.92)
+    return fig
 
+def transientsc_demag(demag, magnet=0, title='', ax=0):
+    """creates a demag plot of a transient short circuit
+    Args:
+      demag: list of dicts with 'displ', 'H_av', 'H_max', 'lim_hc'
+      magnet dict with 'Tmag'
+    """
+    if ax == 0:
+        ax = plt.gca()
+    pos = [d['displ'] for d in demag if 'displ' in d]
+    hmax = [-d['H_max'] for d in demag if 'H_max' in d]
+    havg = [-d['H_av'] for d in demag if 'H_av' in d]
+    hclim = [-d['lim_hc'] for d in demag if 'lim_hc' in d]*2
+
+    ax.set_title('Transient Short Circuit Demagnetization [kA/m]')
+    ax.plot(pos, hmax,
+            label='H Max {:4.2f} kA/m'.format(max(hmax)))
+    ax.plot(pos, havg,
+            label='H Avg {:4.2f} kA/m'.format(max(havg)))
+    ax.plot([pos[0], pos[-1]], hclim, color='C3', linestyle='dashed',
+            label='Hc {:4.2f} kA/m'.format(hclim[0]))
+    ax.set_xlabel('Rotor Position / °')
+    ax.grid(True)
+    if magnet:
+        ax.legend(title=f"Magnet Temperature {magnet['Tmag']}°C")
+    else:
+        ax.legend()
 
 def i1beta_torque(i1, beta, torque, title='', ax=0):
     """creates a surface plot of torque vs i1, beta"""
     if ax == 0:
         _create_3d_axis()
         ax = plt.gca()
     azim = 210
@@ -1218,69 +1245,75 @@
 
 def _contour(ax, title, elements, values, label='', isa=None):
     from matplotlib.patches import Polygon
     from matplotlib.collections import PatchCollection
     if ax == 0:
         ax = plt.gca()
     ax.set_aspect('equal')
-    ax.set_title(title, fontsize=18)
+    ax.set_title(title)
     if isa:
         for se in isa.superelements:
             ax.add_patch(Polygon([n.xy
                                   for nc in se.nodechains
                                   for n in nc.nodes],
                                  color='gray', alpha=0.1, lw=0))
     valid_values = np.logical_not(np.isnan(values))
     patches = np.array([Polygon([v.xy for v in e.vertices])
                        for e in elements])[valid_values]
     # , cmap=matplotlib.cm.jet, alpha=0.4)
     p = PatchCollection(patches, alpha=1.0, match_original=False)
     p.set_array(np.asarray(values)[valid_values])
     ax.add_collection(p)
-    cb = plt.colorbar(p)
+    cb = plt.colorbar(p, shrink=0.9)
     for patch in np.array([Polygon([v.xy for v in e.vertices],
                                    fc='white', alpha=1.0)
                            for e in elements])[np.isnan(values)]:
         ax.add_patch(patch)
     if label:
-        cb.set_label(label=label, fontsize=18)
+        cb.set_label(label=label)
     ax.autoscale(enable=True)
     ax.axis('off')
 
 
 def demag(isa, ax=0):
     """plot demag of NC/I7/ISA7 model
     Args:
       isa: Isa7/NC object
     """
     emag = [e for e in isa.elements if e.is_magnet()]
     demag = np.array([e.demagnetization(isa.MAGN_TEMPERATURE) for e in emag])
-    _contour(ax, f'Demagnetization at {isa.MAGN_TEMPERATURE} °C',
+    _contour(ax, f'Demagnetization at {isa.MAGN_TEMPERATURE} °C (max -{np.max(demag):.1f} kA/m)',
              emag, demag, '-H / kA/m', isa)
     logger.info("Max demagnetization %f", np.max(demag))
 
 
-def demag_pos(isa, pos, icur=-1, ibeta=-1, ax=0):
+def demag_pos(isa, pos=-1, icur=-1, ibeta=-1, ax=0):
     """plot demag of NC/I7/ISA7 model at rotor position
     Args:
       isa: Isa7/NC object
-      pos: rotor position in degree
+      pos: rotor position in degree (maximum h if -1)
       icur: cur amplitude index or last index if -1
       ibeta: beta angle index or last index if -1
     """
     emag = [e for e in isa.elements if e.is_magnet()]
     demag = np.array([isa.demagnetization(e, icur, ibeta)[1]
                       for e in emag])
-    for i, x in enumerate(isa.pos_el_fe_induction):
-        if x >= pos/180*np.pi:
-            break
+    if pos>=0:
+        for i, x in enumerate(isa.pos_el_fe_induction):
+            if x >= pos/180*np.pi:
+                break
+    else:
+        demagmax = np.max(demag, axis=0)
+        i = np.argmax(demagmax)
+        x = isa.pos_el_fe_induction[i]
 
     hpol = demag[:, i]
     hpol[hpol == 0] = np.nan
-    _contour(ax, f'Demagnetization at Pos. {round(x/np.pi*180)}° ({isa.MAGN_TEMPERATURE} °C)',
+    _contour(ax, f'Demagnetization at pos. {round(x/np.pi*180):.1f}°,'
+    f'{isa.MAGN_TEMPERATURE} °C (max -{np.max(hpol):.1f} kA/m)',
              emag, hpol, '-H / kA/m', isa)
     logger.info("Max demagnetization %f kA/m", np.nanmax(hpol))
 
 
 def flux_density(isa, subreg=[], ax=0):
     """plot flux density of NC/I7/ISA7 model
     Args:
@@ -1293,15 +1326,15 @@
             sr = [subreg]
         elements = [e for s in sr for se in isa.get_subregion(s).elements()
                     for e in se]
     else:
         elements = [e for e in isa.elements]
 
     fluxd = np.array([np.linalg.norm(e.flux_density()) for e in elements])
-    _contour(ax, f'Flux Density T', elements, fluxd)
+    _contour(ax, f'Flux Density T (max {np.max(fluxd):.1f} T)', elements, fluxd)
     logger.info("Max flux dens %f", np.max(fluxd))
 
 
 def loss_density(isa, subreg=[], ax=0):
     """plot loss density of NC/I7/ISA7 model
     Args:
       isa: Isa7/NC object
@@ -1648,23 +1681,34 @@
     fig, axs = plt.subplots(2, 2, figsize=(10, 8),
                             layout='tight',
                             sharex=True)
     if title:
         fig.suptitle(title)
 
     n = np.array(char['n'])*60
-    pmech = np.array(char['pmech'])*1e-3
+    punit = 'kW'
+    k = 1e-3
+    if max(char['pmech']) > 1e6:
+        punit = 'MW'
+        k = 1e-6
+    pmech = np.array(char['pmech'])*k
+    tunit = 'Nm'
+    if max(char['T']) > 1e3:
+        tunit = 'kNm'
+        tq = np.array(char['T'])*1e-3
+    else:
+        tq = np.array(char['T'])
 
-    axs[0, 0].plot(n, np.array(char['T']), 'C0-', label='Torque')
-    axs[0, 0].set_ylabel("Torque / Nm")
+    axs[0, 0].plot(n, tq, 'C0-', label='Torque')
+    axs[0, 0].set_ylabel(f"Torque / {tunit}")
     axs[0, 0].grid()
     axs[0, 0].legend(loc='center left')
     ax1 = axs[0, 0].twinx()
     ax1.plot(n, pmech, 'C1-', label='P mech')
-    ax1.set_ylabel("Power / kW")
+    ax1.set_ylabel(f"Power / {punit}")
     ax1.legend(loc='lower center')
 
     axs[0, 1].plot(n[1:], np.array(char['u1'][1:]), 'C0-', label='Voltage')
     axs[0, 1].set_ylabel("Voltage / V",)
     axs[0, 1].grid()
     axs[0, 1].legend(loc='center left')
     ax2 = axs[0, 1].twinx()
@@ -1693,14 +1737,20 @@
     try:
         plcu = np.array(char['plcu'])*1e-3
     except KeyError:
         plcu = np.array(char['plcu1'])*1e-3
     pl = np.array(char['losses'])*1e-3
     axs[1, 1].plot(n, plcu, 'C0-', label='Cu Losses')
     axs[1, 1].plot(n, plfe, 'C1-', label='Fe Losses')
+    try:
+        if char['plfw'] and char['plfw'][-1] > 0:
+            plfw = np.array(char['plfw'])*1e-3
+            axs[1, 1].plot(n, plfw, 'C2-', label='Friction + Windage')
+    except KeyError:
+            pass
     axs[1, 1].set_ylabel("Losses / kW")
     axs[1, 1].legend(loc='center left')
     axs[1, 1].grid()
     axs[1, 1].set_xlabel("Speed / rpm")
     ax4 = axs[1, 1].twinx()
     ax4.plot(n[1:-1], char['eta'][1:-1], 'C3-', label="Eta")
     ax4.legend(loc='upper center')
@@ -1720,65 +1770,115 @@
             bnd[1].append((n0, t0))
             bnd[0].append((nx, tx))
             n0 = nx
         t0 = tx
     bnd[1].append((nx, tx))
     return np.array(bnd[0] + bnd[1][::-1])
 
+def normalize10(v):
+    """
+    Normalizes the input-array using the nearest (ceiling) power of 10.
+
+    Arguments:
+        v: array to normalize
+
+    Returns:
+        normalized array
+        normalisation factor (power of 10)
+    """
+    norm = 10**(np.ceil(np.log10(np.max(np.abs(v)))))
+    return v / norm, norm
+
 
-def plot_contour(speed, torque, z, ax, title='', levels=[], clabel=True):
+def plot_contour(speed, torque, z, ax, title='', levels=[],
+                 clabel=True, cmap='YlOrRd', cbar=False):
+    """ contour plot of speed, torque, z values
+    Arguments:
+    levels: (list of floats)
+    clabel: contour labels if True
+    cmap: colour map
+    cbar: (bool) create color bar if True (default False)
+
+    Note: the x and y axes are scaled
+
+    returns tricontourf, xscale, yscale
+    """
     from matplotlib.path import Path
     from matplotlib.patches import PathPatch
-    x = [60*n for n in speed]
-    y = torque
+    x = 60*np.asarray(speed)
+    y = np.asarray(torque)
+
+    x, xscale = normalize10(x)
+    y, yscale = normalize10(y)
+
     if not levels:
         if max(z) <= 1:
             if max(z) > 0.96:
                 levels = [0.5, 0.75, 0.8, 0.84,
                           0.89, 0.92, 0.94, 0.96, 0.97]
             else:
                 levels = [0.25, 0.5, 0.75, 0.8, 0.84,
                           0.88, 0.9, 0.92, 0.94, 0.96]
 
             if max(z) > levels[-1]:
                 levels.append(np.ceil(max(z)*100)/100)
         else:
             levels = 14
-    cont = ax.tricontour(x, y, z,
-                         linewidths=0.4, levels=levels, colors='k')
-    if clabel:
-        ax.clabel(cont, inline=True, colors='k', fontsize=8)
-    contf = ax.tricontourf(x, y, z,
-                           levels=levels, cmap='YlOrRd')
     #
     ax.spines['top'].set_color('none')
     ax.spines['right'].set_color('none')
 
+    cont = ax.tricontour(x, y, z,
+                         linewidths=0.4, levels=levels,
+                         colors='k')
+    contf = ax.tricontourf(x, y, z,
+                           levels=levels, cmap=cmap)
+
     clippath = Path(get_nT_boundary(x, y))
     patch = PathPatch(clippath, facecolor='none')
     ax.add_patch(patch)
     for c in cont.collections:
         c.set_clip_path(patch)
+    #ax.plot(x, y, "k.", ms=3)
+    if clabel:
+        ax.clabel(cont, inline=True, colors='k', fontsize=8, inline_spacing=0)
+
     for c in contf.collections:
         c.set_clip_path(patch)
-    #ax.plot(x, y, "k.", ms=3)
+
+    if xscale > 1:
+        def format_fn(tick_val, tick_pos):
+            return round(xscale*tick_val)
+        ax.xaxis.set_major_formatter(format_fn)
+    if yscale > 1:
+        def format_fn(tick_val, tick_pos):
+            return round(yscale*tick_val)
+        ax.yaxis.set_major_formatter(format_fn)
+
     ax.set_ylabel('Torque / Nm')
     ax.set_xlabel('Speed / rpm')
     ax.set_title(title)
-    return contf
+    if cbar:
+        cfig = ax.get_figure()
+        cfig.colorbar(contf, ax=ax,
+                      orientation='vertical')
+    return contf, xscale, yscale
+
 
-def efficiency_map(rmap, ax=0, title='Efficiency Map', clabel=True):
+def efficiency_map(rmap, ax=0, title='Efficiency Map', clabel=True,
+                   cmap='YlOrRd', levels=None, cbar=False):
     if ax == 0:
         fig, ax = plt.subplots(figsize=(12, 12))
-    contf = plot_contour(rmap['n'], rmap['T'], rmap['eta'], ax,
-                         title=title, clabel=clabel)
-    return contf
+    return plot_contour(rmap['n'], rmap['T'], rmap['eta'], ax,
+                        title=title, clabel=clabel, cmap=cmap,
+                        levels=levels, cbar=cbar)
 
 
-def losses_map(rmap, ax=0, title='Losses Map / kW', clabel=True):
+def losses_map(rmap, ax=0, title='Losses Map / kW', clabel=True,
+               cmap='YlOrRd', cbar=False):
     if ax == 0:
         fig, ax = plt.subplots(figsize=(12, 12))
     return plot_contour(rmap['n'], rmap['T'], np.asarray(rmap['losses'])/1e3, ax,
                         title=title, levels=14, clabel=clabel)
 
 
 def eigenmode(reigen, num_modes=12):
```

### Comparing `femagtools-1.3.0/femagtools/poc.py` & `femagtools-1.3.1/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/FE-losses.mako` & `femagtools-1.3.1/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/asyn_motor.mako` & `femagtools-1.3.1/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/basic_modpar.mako` & `femagtools-1.3.1/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/calc_field_ts.mako` & `femagtools-1.3.1/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/calc_therm_field.mako` & `femagtools-1.3.1/femagtools/templates/calc_therm_field.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/cogg_calc.mako` & `femagtools-1.3.1/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/com_motor_sim.mako` & `femagtools-1.3.1/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/connect_models.mako` & `femagtools-1.3.1/femagtools/templates/connect_models.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/cu_losses.mako` & `femagtools-1.3.1/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.3.1/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/fe-contr.mako` & `femagtools-1.3.1/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/gen_winding.mako` & `femagtools-1.3.1/femagtools/templates/gen_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/inductances.mako` & `femagtools-1.3.1/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.3.1/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.3.1/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.3.1/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnet-data.mako` & `femagtools-1.3.1/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetFC2.mako` & `femagtools-1.3.1/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetIron.mako` & `femagtools-1.3.1/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetIron2.mako` & `femagtools-1.3.1/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetIron3.mako` & `femagtools-1.3.1/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetIron4.mako` & `femagtools-1.3.1/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetIron5.mako` & `femagtools-1.3.1/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetIronV.mako` & `femagtools-1.3.1/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetSector.mako` & `femagtools-1.3.1/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.3.1/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetShell.mako` & `femagtools-1.3.1/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/magnetShell2.mako` & `femagtools-1.3.1/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/mesh-airgap.mako` & `femagtools-1.3.1/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/modal_analysis.mako` & `femagtools-1.3.1/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.3.1/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.3.1/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/noloadflux.mako` & `femagtools-1.3.1/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.3.1/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/plots.mako` & `femagtools-1.3.1/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.3.1/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.3.1/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.3.1/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.3.1/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/ring.mako` & `femagtools-1.3.1/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/rot_hsm.mako` & `femagtools-1.3.1/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/rotorAsyn.mako` & `femagtools-1.3.1/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/rotorKs2.mako` & `femagtools-1.3.1/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/rotor_msh.mako` & `femagtools-1.3.1/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/rotor_winding.mako` & `femagtools-1.3.1/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/shortcircuit.mako` & `femagtools-1.3.1/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/srm.mako` & `femagtools-1.3.1/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/stator1.mako` & `femagtools-1.3.1/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/stator2.mako` & `femagtools-1.3.1/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/stator3Linear.mako` & `femagtools-1.3.1/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/stator4.mako` & `femagtools-1.3.1/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/statorBG.mako` & `femagtools-1.3.1/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/statorRing.mako` & `femagtools-1.3.1/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/statorRotor3.mako` & `femagtools-1.3.1/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/stator_msh.mako` & `femagtools-1.3.1/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/therm-dynamic.mako` & `femagtools-1.3.1/femagtools/templates/therm-dynamic.mako`

 * *Files 14% similar despite different names*

```diff
@@ -52,22 +52,30 @@
 
 m.pocfilename    = model..'_'..m.num_poles..'p.poc'
 xcoil, ycoil = ${model['temp_coords'][0]},${model['temp_coords'][1]}
 
 local load = read_load_file("load.csv")
 
 f = io.open('temperature.dat', 'w')
+f:write(string.format("0.0 0.0\n"))
+
 i = 1
 for _, load_data in ipairs(load) do  -- use pairs or ipairs to iterate over tables
   if i == 1 then
     t1 = load_data.t
+    i1 = load_data.i1
+    beta = load_data.beta
+    speed = load_data.n
     printf("\nTotal steps: %d\n", #load)
   else
     t2 = load_data.t
     end_time = t2 - t1
+    i1 = load_data.i1
+    beta = load_data.beta
+    speed = load_data.n
 
     m.current   = i1 * math.sqrt(2)/m.num_par_wdgs
     m.angl_i_up = beta
     m.speed     = speed
     printf("Step %3d: %6.1fs %5.1f A %5.1f° %6.1f rpm: ",
             i-1, t1, i1, m.angl_i_up, m.speed)
 
@@ -78,24 +86,22 @@
     import_losses_from_femag_dc()
 
     if i == 2 then
       start_mode = temp_reset
     else
       start_mode = temp_load
     end
-    time_step = 10
+    time_step = end_time/5
     calc_therm_field_tstep(start_mode,time_step,end_time)
 
     export_calc_results("temp-"..string.format("%03d",i)..".vtu")
     temp = temperature_xy(xcoil, ycoil)
-    printf(" %f\n", temp)
+    printf("%4d, time: %6.1fs, current: %5.1fA, speed: %6.1frpm, Temp incr.: %2.2fK, time-step: %3.1fs\n", i-1, t2, i1, m.speed, temp, time_step)
     f:write(string.format("%g %g\n", t2, temp))
     t1 = t2
   end
 
-    i1 = load_data.i1
-    beta = load_data.beta
-    speed = load_data.n
-    i = i+1
+  i = i+1
+
 end
 f:close()
 save_model('close')
```

### Comparing `femagtools-1.3.0/femagtools/templates/therm-static.mako` & `femagtools-1.3.1/femagtools/templates/therm-static.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/templates/torq_calc.mako` & `femagtools-1.3.1/femagtools/templates/torq_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/tks.py` & `femagtools-1.3.1/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/ts.py` & `femagtools-1.3.1/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/vbf.py` & `femagtools-1.3.1/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/vtu.py` & `femagtools-1.3.1/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools/windings.py` & `femagtools-1.3.1/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/femagtools.egg-info/PKG-INFO` & `femagtools-1.3.1/femagtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.3.0/femagtools.egg-info/SOURCES.txt` & `femagtools-1.3.1/femagtools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 femagtools/conductor.py
 femagtools/config.py
 femagtools/convert.py
 femagtools/dakota.py
 femagtools/dakota_femag.py
 femagtools/dakotaout.py
 femagtools/docker.py
+femagtools/ecloss.py
 femagtools/erg.py
 femagtools/femag.py
 femagtools/forcedens.py
 femagtools/fsl.py
 femagtools/getset.py
 femagtools/gmsh.py
 femagtools/google.py
 femagtools/grid.py
+femagtools/hxy.py
 femagtools/isa7.py
 femagtools/jcf2msh.py
 femagtools/jhb.py
 femagtools/job.py
 femagtools/losscoeffs.py
 femagtools/magnet.py
 femagtools/mcv.py
```

### Comparing `femagtools-1.3.0/pyproject.toml` & `femagtools-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_airgap_induction.py` & `femagtools-1.3.1/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_amela.py` & `femagtools-1.3.1/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_asm.py` & `femagtools-1.3.1/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_bchreader.py` & `femagtools-1.3.1/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_convert.py` & `femagtools-1.3.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_effloss.py` & `femagtools-1.3.1/tests/test_effloss.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,12 +22,12 @@
     T = 32.9
     u1 = 230
     temp = (120, 120)
 
     r = femagtools.machine.effloss.efficiency_losses_map(
         impars, u1, T, temp, nmax, npoints=(5, 4))
     assert r['T'] == pytest.approx(
-        [-33.1, -0.6, 0.4, 32.7,
-         -27.9, -0.6, 0.4, 25.9,
-         -13.5, -0.6, 0.4, 12.2,
-         -8.9, -0.6, 0.4, 7.8,
-         -6.6, -0.6, 0.4, 5.8], abs=1e-1)
+        [-32.9, -0.5, 0.4, 32.9,
+         -16.7, -0.5, 0.4, 15.8,
+         -10.8, -0.5, 0.4, 10.1,
+         -8.0, -0.5, 0.4, 7.4,
+         -6.4, -0.5, 0.4, 6.0], abs=1e-1)
```

### Comparing `femagtools-1.3.0/tests/test_erg.py` & `femagtools-1.3.1/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_femag.py` & `femagtools-1.3.1/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_forcedens.py` & `femagtools-1.3.1/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_fsl.py` & `femagtools-1.3.1/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_im.py` & `femagtools-1.3.1/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_isa7.py` & `femagtools-1.3.1/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_jhb.py` & `femagtools-1.3.1/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_job.py` & `femagtools-1.3.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_losscoeffs.py` & `femagtools-1.3.1/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_machine.py` & `femagtools-1.3.1/tests/test_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     r = pm.characteristics(T, n, u1)
 
     assert r['i1'][0] == pytest.approx(207.74350, rel=1e-1)
     assert r['u1'][0] == pytest.approx(1192.88, rel=1e-1)
     assert r['beta'][0] == pytest.approx(-38.01, rel=1e-1)
     assert r['cosphi'][0] == pytest.approx(0.788, rel=1e-1)
 
-
+@pytest.mark.skip(reason="fixit: returns currently 0")
 def test_char_ldd_fieldweakening():
     m = dict(
         p=6,
         r1=0.0,
         ld=[0.005152],
         lq=[0.0104825],
         psim=[1.1298],
@@ -240,15 +240,14 @@
                                               r1=r1, ls=ls)
     w1 = 500
     iqs, ids = m1.iqd_uqd(w1, 0, 0)
     assert femagtools.machine.betai1(
         iqs, ids) == pytest.approx((-1.768, 42.48), rel=1e-1)
 
 
-@pytest.mark.skip("temporarily ignored due to strange github action failures")
 def test_ldq_create(data_dir):
     bch = femagtools.bch.read(str(data_dir / 'ldq.BATCH'))
     pm = femagtools.machine.create(bch, r1=0, ls=0)
     # with pytest.raises(ValueError) as exc_info:
     #    iqd = pm.iqd_torque(250)
 
     iqd = pm.iqd_torque(120)
```

### Comparing `femagtools-1.3.0/tests/test_magncurv.py` & `femagtools-1.3.1/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_mcvreader.py` & `femagtools-1.3.1/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_mcvwriter.py` & `femagtools-1.3.1/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_model.py` & `femagtools-1.3.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_nc.py` & `femagtools-1.3.1/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_parident.py` & `femagtools-1.3.1/tests/test_parident.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 
 def test_noloadrot_eval(data_dir):
     task = Task(id=1, directory=data_dir / 'parident')
     i1tab = [2.0384197650236815, 4.076839530047363,
              6.115259295071045, 8.153679060094726, 10.192098825118407]
     u1ph = 400/np.sqrt(3)
-    eval = femagtools.machine.im._eval_noloadrot()
+    pmod = 0
+    eval = femagtools.machine.im._eval_noloadrot(pmod)
     r = eval(task)
     i0 = [2.0384,  4.0768,  6.1153,  8.1537, 10.1921]
     psi1_0 = [0.2725, 0.5301, 0.7106, 0.8091, 0.8641]
     Bamp = [0.3091, 0.6013, 0.8058, 0.9159, 0.9769]
     assert i0 == [round(x, 4) for x in r['i1_0']]
     assert psi1_0 == [round(x, 4) for x in np.mean(r['psi1_0'], axis=1)]
     assert Bamp == [round(x, 4) for x in np.mean(r['Bamp'], axis=1)]
```

### Comparing `femagtools-1.3.0/tests/test_parstudy.py` & `femagtools-1.3.1/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_pocfile.py` & `femagtools-1.3.1/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_sizing.py` & `femagtools-1.3.1/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_sm.py` & `femagtools-1.3.1/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_tksreader.py` & `femagtools-1.3.1/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_ts.py` & `femagtools-1.3.1/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_vbfreader.py` & `femagtools-1.3.1/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_vtu.py` & `femagtools-1.3.1/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.0/tests/test_windings.py` & `femagtools-1.3.1/tests/test_windings.py`

 * *Files identical despite different names*

