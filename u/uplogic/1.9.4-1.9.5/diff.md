# Comparing `tmp/uplogic-1.9.4.tar.gz` & `tmp/uplogic-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplogic-1.9.4.tar", last modified: Fri Jul  7 13:44:08 2023, max compression
+gzip compressed data, was "uplogic-1.9.5.tar", last modified: Fri Jul  7 13:58:28 2023, max compression
```

## Comparing `uplogic-1.9.4.tar` & `uplogic-1.9.5.tar`

### file list

```diff
@@ -1,393 +1,393 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.594940 uplogic-1.9.4/
--rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-1.9.4/LICENSE.md
--rw-rw-rw-   0        0        0     1049 2023-07-07 13:44:08.594940 uplogic-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-1.9.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 13:44:08.594940 uplogic-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1743 2023-07-07 13:43:57.000000 uplogic-1.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.771221 uplogic-1.9.4/uplogic/
--rw-rw-rw-   0        0        0     5944 2023-07-05 13:56:27.000000 uplogic-1.9.4/uplogic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.822233 uplogic-1.9.4/uplogic/animation/
--rw-rw-rw-   0        0        0      343 2023-03-08 12:02:42.000000 uplogic-1.9.4/uplogic/animation/__init__.py
--rw-rw-rw-   0        0        0    12544 2023-07-07 11:38:36.000000 uplogic-1.9.4/uplogic/animation/action.py
--rw-rw-rw-   0        0        0     4016 2023-05-01 17:00:05.000000 uplogic-1.9.4/uplogic/animation/actionsystem.py
--rw-rw-rw-   0        0        0     6224 2023-05-14 08:46:37.000000 uplogic-1.9.4/uplogic/animation/sequence.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.855232 uplogic-1.9.4/uplogic/audio/
--rw-rw-rw-   0        0        0      606 2023-03-06 09:07:59.000000 uplogic-1.9.4/uplogic/audio/__init__.py
--rw-rw-rw-   0        0        0     7689 2023-04-24 21:26:30.000000 uplogic-1.9.4/uplogic/audio/audiosystem.py
--rw-rw-rw-   0        0        0     6839 2023-05-14 08:47:09.000000 uplogic-1.9.4/uplogic/audio/music.py
--rw-rw-rw-   0        0        0    23984 2023-07-05 14:14:26.000000 uplogic-1.9.4/uplogic/audio/sound.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.888276 uplogic-1.9.4/uplogic/data/
--rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-1.9.4/uplogic/data/__init__.py
--rw-rw-rw-   0        0        0     3122 2023-04-07 16:35:00.000000 uplogic-1.9.4/uplogic/data/file.py
--rw-rw-rw-   0        0        0     7148 2023-05-14 08:48:26.000000 uplogic-1.9.4/uplogic/data/globaldb.py
--rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-1.9.4/uplogic/data/serializers.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.898278 uplogic-1.9.4/uplogic/decorators/
--rw-rw-rw-   0        0        0    11024 2023-06-20 15:01:27.000000 uplogic-1.9.4/uplogic/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.907290 uplogic-1.9.4/uplogic/events/
--rw-rw-rw-   0        0        0     7615 2023-04-04 13:17:19.000000 uplogic-1.9.4/uplogic/events/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.954301 uplogic-1.9.4/uplogic/input/
--rw-rw-rw-   0        0        0     1494 2023-03-06 08:52:33.000000 uplogic-1.9.4/uplogic/input/__init__.py
--rw-rw-rw-   0        0        0    15064 2023-06-13 14:39:52.000000 uplogic-1.9.4/uplogic/input/gamepad.py
--rw-rw-rw-   0        0        0     9607 2023-01-16 12:00:44.000000 uplogic-1.9.4/uplogic/input/keyboard.py
--rw-rw-rw-   0        0        0    14930 2023-05-14 08:49:32.000000 uplogic-1.9.4/uplogic/input/mouse.py
--rw-rw-rw-   0        0        0     9131 2023-05-14 08:49:48.000000 uplogic-1.9.4/uplogic/input/vr.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.963294 uplogic-1.9.4/uplogic/logging/
--rw-rw-rw-   0        0        0     6115 2023-06-06 15:11:05.000000 uplogic-1.9.4/uplogic/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.987308 uplogic-1.9.4/uplogic/network/
--rw-rw-rw-   0        0        0       56 2023-06-05 09:06:00.000000 uplogic-1.9.4/uplogic/network/__init__.py
--rw-rw-rw-   0        0        0     3351 2023-06-05 09:11:35.000000 uplogic-1.9.4/uplogic/network/client.py
--rw-rw-rw-   0        0        0     4756 2023-06-13 19:02:29.000000 uplogic-1.9.4/uplogic/network/server.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.998310 uplogic-1.9.4/uplogic/nodes/
--rw-rw-rw-   0        0        0     5176 2023-05-19 05:22:01.000000 uplogic-1.9.4/uplogic/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:07.194010 uplogic-1.9.4/uplogic/nodes/actions/
--rw-rw-rw-   0        0        0     8023 2023-05-16 08:46:11.000000 uplogic-1.9.4/uplogic/nodes/actions/__init__.py
--rw-rw-rw-   0        0        0     4065 2022-11-02 09:25:32.000000 uplogic-1.9.4/uplogic/nodes/actions/addfilter.py
--rw-rw-rw-   0        0        0     1308 2022-08-21 23:02:22.000000 uplogic-1.9.4/uplogic/nodes/actions/addobject.py
--rw-rw-rw-   0        0        0     2710 2022-04-24 07:51:50.000000 uplogic-1.9.4/uplogic/nodes/actions/addphysicsconstraint.py
--rw-rw-rw-   0        0        0      797 2023-03-01 15:33:33.000000 uplogic-1.9.4/uplogic/nodes/actions/adduiwidget.py
--rw-rw-rw-   0        0        0     1420 2022-10-28 14:13:34.000000 uplogic-1.9.4/uplogic/nodes/actions/alignaxistovector.py
--rw-rw-rw-   0        0        0     1056 2022-01-12 11:55:23.000000 uplogic-1.9.4/uplogic/nodes/actions/appendlistitem.py
--rw-rw-rw-   0        0        0     1007 2022-01-12 13:37:33.000000 uplogic-1.9.4/uplogic/nodes/actions/applyforce.py
--rw-rw-rw-   0        0        0     1187 2022-01-12 13:38:47.000000 uplogic-1.9.4/uplogic/nodes/actions/applyimpulse.py
--rw-rw-rw-   0        0        0     1074 2022-01-12 13:36:04.000000 uplogic-1.9.4/uplogic/nodes/actions/applymovement.py
--rw-rw-rw-   0        0        0     1237 2023-01-05 15:34:33.000000 uplogic-1.9.4/uplogic/nodes/actions/applyrotation.py
--rw-rw-rw-   0        0        0      984 2022-01-12 14:18:21.000000 uplogic-1.9.4/uplogic/nodes/actions/applytorque.py
--rw-rw-rw-   0        0        0     2560 2022-01-10 18:02:58.000000 uplogic-1.9.4/uplogic/nodes/actions/cameraraycast.py
--rw-rw-rw-   0        0        0     1014 2022-01-12 14:08:55.000000 uplogic-1.9.4/uplogic/nodes/actions/characterjump.py
--rw-rw-rw-   0        0        0     1536 2022-04-10 10:15:42.000000 uplogic-1.9.4/uplogic/nodes/actions/clampedmodifyproperty.py
--rw-rw-rw-   0        0        0     1610 2023-05-14 08:51:40.000000 uplogic-1.9.4/uplogic/nodes/actions/clearvariables.py
--rw-rw-rw-   0        0        0     1395 2022-04-09 10:45:53.000000 uplogic-1.9.4/uplogic/nodes/actions/copyproperty.py
--rw-rw-rw-   0        0        0     3577 2023-06-14 11:06:15.000000 uplogic-1.9.4/uplogic/nodes/actions/createuibutton.py
--rw-rw-rw-   0        0        0      821 2023-03-01 15:34:01.000000 uplogic-1.9.4/uplogic/nodes/actions/createuicanvas.py
--rw-rw-rw-   0        0        0     1789 2023-06-14 11:06:17.000000 uplogic-1.9.4/uplogic/nodes/actions/createuiimage.py
--rw-rw-rw-   0        0        0     2599 2023-06-14 11:06:17.000000 uplogic-1.9.4/uplogic/nodes/actions/createuilabel.py
--rw-rw-rw-   0        0        0     2386 2023-06-14 11:06:17.000000 uplogic-1.9.4/uplogic/nodes/actions/createuilayout.py
--rw-rw-rw-   0        0        0     2003 2023-05-14 08:51:47.000000 uplogic-1.9.4/uplogic/nodes/actions/createvehicle.py
--rw-rw-rw-   0        0        0     1523 2022-09-11 14:27:22.000000 uplogic-1.9.4/uplogic/nodes/actions/cursorbehavior.py
--rw-rw-rw-   0        0        0      797 2023-03-02 21:19:09.000000 uplogic-1.9.4/uplogic/nodes/actions/cursorvisibility.py
--rw-rw-rw-   0        0        0     1245 2023-05-14 08:51:57.000000 uplogic-1.9.4/uplogic/nodes/actions/dispatchevent.py
--rw-rw-rw-   0        0        0     1188 2023-05-14 08:52:09.000000 uplogic-1.9.4/uplogic/nodes/actions/drawbox.py
--rw-rw-rw-   0        0        0     1028 2023-05-14 08:52:17.000000 uplogic-1.9.4/uplogic/nodes/actions/drawcube.py
--rw-rw-rw-   0        0        0      980 2022-08-23 18:34:20.000000 uplogic-1.9.4/uplogic/nodes/actions/drawline.py
--rw-rw-rw-   0        0        0     3560 2022-01-12 12:12:44.000000 uplogic-1.9.4/uplogic/nodes/actions/editbone.py
--rw-rw-rw-   0        0        0      530 2022-07-18 15:47:27.000000 uplogic-1.9.4/uplogic/nodes/actions/endgame.py
--rw-rw-rw-   0        0        0     1019 2022-01-12 13:25:49.000000 uplogic-1.9.4/uplogic/nodes/actions/endobject.py
--rw-rw-rw-   0        0        0     1237 2022-02-07 22:47:57.000000 uplogic-1.9.4/uplogic/nodes/actions/executesubnetwork.py
--rw-rw-rw-   0        0        0     5575 2023-07-07 10:14:02.000000 uplogic-1.9.4/uplogic/nodes/actions/followpath.py
--rw-rw-rw-   0        0        0     4138 2023-05-16 16:57:59.000000 uplogic-1.9.4/uplogic/nodes/actions/gamepadlook.py
--rw-rw-rw-   0        0        0     1395 2023-05-14 08:53:21.000000 uplogic-1.9.4/uplogic/nodes/actions/gamepadvibration.py
--rw-rw-rw-   0        0        0     2383 2022-01-12 12:04:24.000000 uplogic-1.9.4/uplogic/nodes/actions/getperformanceprofile.py
--rw-rw-rw-   0        0        0     1373 2022-02-07 22:56:45.000000 uplogic-1.9.4/uplogic/nodes/actions/installsubnetwork.py
--rw-rw-rw-   0        0        0     1976 2023-04-26 12:34:19.000000 uplogic-1.9.4/uplogic/nodes/actions/instream.py
--rw-rw-rw-   0        0        0     1338 2023-06-07 19:15:20.000000 uplogic-1.9.4/uplogic/nodes/actions/listglobalvalues.py
--rw-rw-rw-   0        0        0     2110 2023-05-14 08:53:38.000000 uplogic-1.9.4/uplogic/nodes/actions/listvariables.py
--rw-rw-rw-   0        0        0      674 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/loadblendfile.py
--rw-rw-rw-   0        0        0     1586 2023-05-14 08:53:49.000000 uplogic-1.9.4/uplogic/nodes/actions/loadfilecontent.py
--rw-rw-rw-   0        0        0     4266 2023-05-14 08:54:00.000000 uplogic-1.9.4/uplogic/nodes/actions/loadgame.py
--rw-rw-rw-   0        0        0     1658 2023-05-14 08:54:06.000000 uplogic-1.9.4/uplogic/nodes/actions/loadscene.py
--rw-rw-rw-   0        0        0     2515 2023-05-16 10:27:44.000000 uplogic-1.9.4/uplogic/nodes/actions/localclient.py
--rw-rw-rw-   0        0        0     2391 2023-05-16 10:27:30.000000 uplogic-1.9.4/uplogic/nodes/actions/localserver.py
--rw-rw-rw-   0        0        0     1051 2022-01-12 15:17:30.000000 uplogic-1.9.4/uplogic/nodes/actions/makeuniquelight.py
--rw-rw-rw-   0        0        0     1363 2022-04-10 10:15:35.000000 uplogic-1.9.4/uplogic/nodes/actions/modifyproperty.py
--rw-rw-rw-   0        0        0     4855 2023-05-19 05:22:01.000000 uplogic-1.9.4/uplogic/nodes/actions/mouselook.py
--rw-rw-rw-   0        0        0     2144 2022-01-10 18:01:11.000000 uplogic-1.9.4/uplogic/nodes/actions/mouseraycast.py
--rw-rw-rw-   0        0        0     1012 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/mousesetposition.py
--rw-rw-rw-   0        0        0     1521 2023-05-14 08:54:30.000000 uplogic-1.9.4/uplogic/nodes/actions/moveto.py
--rw-rw-rw-   0        0        0     5241 2023-07-07 10:14:02.000000 uplogic-1.9.4/uplogic/nodes/actions/movetowithnavmesh.py
--rw-rw-rw-   0        0        0      626 2022-01-12 14:35:38.000000 uplogic-1.9.4/uplogic/nodes/actions/pausesound.py
--rw-rw-rw-   0        0        0     5400 2023-05-14 08:54:59.000000 uplogic-1.9.4/uplogic/nodes/actions/playaction.py
--rw-rw-rw-   0        0        0     2476 2023-02-12 11:22:41.000000 uplogic-1.9.4/uplogic/nodes/actions/playsequence.py
--rw-rw-rw-   0        0        0     1338 2023-05-14 08:55:21.000000 uplogic-1.9.4/uplogic/nodes/actions/popdictkey.py
--rw-rw-rw-   0        0        0      762 2023-05-16 10:26:49.000000 uplogic-1.9.4/uplogic/nodes/actions/printvalue.py
--rw-rw-rw-   0        0        0     3218 2023-05-16 10:40:40.000000 uplogic-1.9.4/uplogic/nodes/actions/projectileraycast.py
--rw-rw-rw-   0        0        0     3516 2022-09-11 15:14:18.000000 uplogic-1.9.4/uplogic/nodes/actions/raycast.py
--rw-rw-rw-   0        0        0      842 2022-09-06 10:05:33.000000 uplogic-1.9.4/uplogic/nodes/actions/removefilter.py
--rw-rw-rw-   0        0        0     1176 2022-01-12 11:59:50.000000 uplogic-1.9.4/uplogic/nodes/actions/removelistindex.py
--rw-rw-rw-   0        0        0     1207 2022-01-12 11:59:09.000000 uplogic-1.9.4/uplogic/nodes/actions/removelistvalue.py
--rw-rw-rw-   0        0        0      779 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/removeoverlaycollection.py
--rw-rw-rw-   0        0        0      969 2022-02-01 19:49:18.000000 uplogic-1.9.4/uplogic/nodes/actions/removeparent.py
--rw-rw-rw-   0        0        0      974 2022-01-12 15:45:41.000000 uplogic-1.9.4/uplogic/nodes/actions/removephysicsconstraint.py
--rw-rw-rw-   0        0        0     1834 2023-02-14 10:14:02.000000 uplogic-1.9.4/uplogic/nodes/actions/removevariable.py
--rw-rw-rw-   0        0        0     1255 2022-01-12 15:43:12.000000 uplogic-1.9.4/uplogic/nodes/actions/replacemesh.py
--rw-rw-rw-   0        0        0      633 2022-02-10 19:19:01.000000 uplogic-1.9.4/uplogic/nodes/actions/restartgame.py
--rw-rw-rw-   0        0        0      628 2022-01-12 14:37:05.000000 uplogic-1.9.4/uplogic/nodes/actions/resumesound.py
--rw-rw-rw-   0        0        0     1611 2023-07-07 11:05:26.000000 uplogic-1.9.4/uplogic/nodes/actions/rotateto.py
--rw-rw-rw-   0        0        0     1199 2022-02-09 13:38:34.000000 uplogic-1.9.4/uplogic/nodes/actions/runactuator.py
--rw-rw-rw-   0        0        0     1716 2023-05-15 10:27:54.000000 uplogic-1.9.4/uplogic/nodes/actions/runpython.py
--rw-rw-rw-   0        0        0     7976 2022-02-08 15:48:21.000000 uplogic-1.9.4/uplogic/nodes/actions/savegame.py
--rw-rw-rw-   0        0        0     2005 2023-02-14 10:08:13.000000 uplogic-1.9.4/uplogic/nodes/actions/savevariable.py
--rw-rw-rw-   0        0        0     1738 2023-02-14 10:08:29.000000 uplogic-1.9.4/uplogic/nodes/actions/savevariabledict.py
--rw-rw-rw-   0        0        0     1180 2022-01-10 17:48:43.000000 uplogic-1.9.4/uplogic/nodes/actions/sendmessage.py
--rw-rw-rw-   0        0        0      849 2023-05-16 09:59:36.000000 uplogic-1.9.4/uplogic/nodes/actions/sendnetworkmessage.py
--rw-rw-rw-   0        0        0     2608 2023-02-13 17:09:10.000000 uplogic-1.9.4/uplogic/nodes/actions/setactionframe.py
--rw-rw-rw-   0        0        0     1135 2022-02-26 12:20:29.000000 uplogic-1.9.4/uplogic/nodes/actions/setactuatorvalue.py
--rw-rw-rw-   0        0        0     1532 2022-01-12 13:30:41.000000 uplogic-1.9.4/uplogic/nodes/actions/setboneconstraintattr.py
--rw-rw-rw-   0        0        0     1389 2022-01-12 12:09:35.000000 uplogic-1.9.4/uplogic/nodes/actions/setboneconstraintinfluence.py
--rw-rw-rw-   0        0        0     1382 2022-01-12 12:08:54.000000 uplogic-1.9.4/uplogic/nodes/actions/setboneconstrainttarget.py
--rw-rw-rw-   0        0        0     1488 2022-01-12 12:15:32.000000 uplogic-1.9.4/uplogic/nodes/actions/setboneposition.py
--rw-rw-rw-   0        0        0      944 2022-01-10 18:05:42.000000 uplogic-1.9.4/uplogic/nodes/actions/setcamera.py
--rw-rw-rw-   0        0        0      941 2022-01-23 23:21:22.000000 uplogic-1.9.4/uplogic/nodes/actions/setcamerafov.py
--rw-rw-rw-   0        0        0      966 2022-01-10 18:09:57.000000 uplogic-1.9.4/uplogic/nodes/actions/setcameraorthoscale.py
--rw-rw-rw-   0        0        0     1154 2022-01-12 14:13:53.000000 uplogic-1.9.4/uplogic/nodes/actions/setcharactergravity.py
--rw-rw-rw-   0        0        0     1102 2022-01-12 14:08:37.000000 uplogic-1.9.4/uplogic/nodes/actions/setcharacterjumpspeed.py
--rw-rw-rw-   0        0        0     1096 2022-01-12 14:09:24.000000 uplogic-1.9.4/uplogic/nodes/actions/setcharactermaxjumps.py
--rw-rw-rw-   0        0        0     1200 2022-01-12 14:17:03.000000 uplogic-1.9.4/uplogic/nodes/actions/setcharactervelocity.py
--rw-rw-rw-   0        0        0     1795 2022-01-12 14:14:18.000000 uplogic-1.9.4/uplogic/nodes/actions/setcharacterwalkdir.py
--rw-rw-rw-   0        0        0     1030 2022-01-12 13:44:27.000000 uplogic-1.9.4/uplogic/nodes/actions/setcollisiongroup.py
--rw-rw-rw-   0        0        0     1028 2022-01-12 13:45:39.000000 uplogic-1.9.4/uplogic/nodes/actions/setcollisionmask.py
--rw-rw-rw-   0        0        0     1493 2022-02-16 14:17:45.000000 uplogic-1.9.4/uplogic/nodes/actions/setcurvepoints.py
--rw-rw-rw-   0        0        0     1095 2023-05-03 10:24:19.000000 uplogic-1.9.4/uplogic/nodes/actions/setcustomcursor.py
--rw-rw-rw-   0        0        0     1105 2022-01-12 11:43:10.000000 uplogic-1.9.4/uplogic/nodes/actions/setdictkey.py
--rw-rw-rw-   0        0        0     1166 2022-09-07 10:43:04.000000 uplogic-1.9.4/uplogic/nodes/actions/setdynamics.py
--rw-rw-rw-   0        0        0      887 2022-01-12 15:03:06.000000 uplogic-1.9.4/uplogic/nodes/actions/seteeveeao.py
--rw-rw-rw-   0        0        0      891 2022-01-12 16:00:43.000000 uplogic-1.9.4/uplogic/nodes/actions/seteeveebloom.py
--rw-rw-rw-   0        0        0      895 2022-01-12 15:08:25.000000 uplogic-1.9.4/uplogic/nodes/actions/seteeveesmaa.py
--rw-rw-rw-   0        0        0      902 2022-01-12 15:12:11.000000 uplogic-1.9.4/uplogic/nodes/actions/seteeveesmaaquality.py
--rw-rw-rw-   0        0        0      887 2022-01-12 15:04:58.000000 uplogic-1.9.4/uplogic/nodes/actions/seteeveessr.py
--rw-rw-rw-   0        0        0      933 2022-01-12 15:05:54.000000 uplogic-1.9.4/uplogic/nodes/actions/seteeveevolumetrics.py
--rw-rw-rw-   0        0        0      920 2022-02-06 14:06:39.000000 uplogic-1.9.4/uplogic/nodes/actions/setexposure.py
--rw-rw-rw-   0        0        0      935 2022-09-06 10:37:29.000000 uplogic-1.9.4/uplogic/nodes/actions/setfilterstate.py
--rw-rw-rw-   0        0        0      858 2022-01-10 18:13:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setfullscreen.py
--rw-rw-rw-   0        0        0     1938 2023-07-07 11:20:03.000000 uplogic-1.9.4/uplogic/nodes/actions/setgameobjectattr.py
--rw-rw-rw-   0        0        0      914 2022-01-12 15:01:16.000000 uplogic-1.9.4/uplogic/nodes/actions/setgamma.py
--rw-rw-rw-   0        0        0     1456 2022-01-12 15:57:52.000000 uplogic-1.9.4/uplogic/nodes/actions/setglobalvalue.py
--rw-rw-rw-   0        0        0      933 2022-01-12 13:28:24.000000 uplogic-1.9.4/uplogic/nodes/actions/setgravity.py
--rw-rw-rw-   0        0        0     1012 2022-01-12 15:24:08.000000 uplogic-1.9.4/uplogic/nodes/actions/setlightcolor.py
--rw-rw-rw-   0        0        0      959 2022-01-12 15:16:33.000000 uplogic-1.9.4/uplogic/nodes/actions/setlightenergy.py
--rw-rw-rw-   0        0        0      983 2022-01-12 15:19:36.000000 uplogic-1.9.4/uplogic/nodes/actions/setlightshadow.py
--rw-rw-rw-   0        0        0     1137 2022-01-12 11:56:28.000000 uplogic-1.9.4/uplogic/nodes/actions/setlistindex.py
--rw-rw-rw-   0        0        0     1321 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setmaterial.py
--rw-rw-rw-   0        0        0     1412 2022-01-10 12:35:51.000000 uplogic-1.9.4/uplogic/nodes/actions/setmatnodesocket.py
--rw-rw-rw-   0        0        0     1610 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setmatnodevalue.py
--rw-rw-rw-   0        0        0     1388 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setnodesocket.py
--rw-rw-rw-   0        0        0     1622 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setnodevalue.py
--rw-rw-rw-   0        0        0      863 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setoverlaycollection.py
--rw-rw-rw-   0        0        0     1188 2022-01-12 12:01:10.000000 uplogic-1.9.4/uplogic/nodes/actions/setparent.py
--rw-rw-rw-   0        0        0     1188 2022-01-12 16:00:43.000000 uplogic-1.9.4/uplogic/nodes/actions/setphysics.py
--rw-rw-rw-   0        0        0      838 2022-01-10 18:14:35.000000 uplogic-1.9.4/uplogic/nodes/actions/setprofile.py
--rw-rw-rw-   0        0        0     1383 2022-10-05 12:35:18.000000 uplogic-1.9.4/uplogic/nodes/actions/setproperty.py
--rw-rw-rw-   0        0        0      736 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/actions/setpyinstanceattr.py
--rw-rw-rw-   0        0        0      898 2022-01-23 23:21:22.000000 uplogic-1.9.4/uplogic/nodes/actions/setresolution.py
--rw-rw-rw-   0        0        0     1085 2022-01-12 13:12:07.000000 uplogic-1.9.4/uplogic/nodes/actions/setrigidbody.py
--rw-rw-rw-   0        0        0      820 2022-10-04 11:00:44.000000 uplogic-1.9.4/uplogic/nodes/actions/setscene.py
--rw-rw-rw-   0        0        0     1200 2022-02-04 18:03:35.000000 uplogic-1.9.4/uplogic/nodes/actions/setsensorvalue.py
--rw-rw-rw-   0        0        0      949 2022-01-12 13:27:30.000000 uplogic-1.9.4/uplogic/nodes/actions/settimescale.py
--rw-rw-rw-   0        0        0     2417 2023-06-14 11:15:48.000000 uplogic-1.9.4/uplogic/nodes/actions/setuiwidgetattr.py
--rw-rw-rw-   0        0        0     2913 2022-02-06 12:41:13.000000 uplogic-1.9.4/uplogic/nodes/actions/setvisibility.py
--rw-rw-rw-   0        0        0      828 2022-01-12 11:22:14.000000 uplogic-1.9.4/uplogic/nodes/actions/setvsync.py
--rw-rw-rw-   0        0        0      853 2022-01-10 18:19:10.000000 uplogic-1.9.4/uplogic/nodes/actions/showframerate.py
--rw-rw-rw-   0        0        0     1519 2023-05-14 08:56:41.000000 uplogic-1.9.4/uplogic/nodes/actions/slowfollow.py
--rw-rw-rw-   0        0        0     3572 2023-05-16 11:15:30.000000 uplogic-1.9.4/uplogic/nodes/actions/spawnpool.py
--rw-rw-rw-   0        0        0     2051 2023-03-06 08:53:53.000000 uplogic-1.9.4/uplogic/nodes/actions/startsound.py
--rw-rw-rw-   0        0        0     3107 2023-03-06 08:54:22.000000 uplogic-1.9.4/uplogic/nodes/actions/startsound3d.py
--rw-rw-rw-   0        0        0     2541 2023-03-06 08:54:22.000000 uplogic-1.9.4/uplogic/nodes/actions/startspeaker.py
--rw-rw-rw-   0        0        0     1436 2023-05-14 08:57:02.000000 uplogic-1.9.4/uplogic/nodes/actions/startsubnetwork.py
--rw-rw-rw-   0        0        0     1597 2022-10-07 11:19:16.000000 uplogic-1.9.4/uplogic/nodes/actions/stopaction.py
--rw-rw-rw-   0        0        0      591 2022-01-12 14:34:57.000000 uplogic-1.9.4/uplogic/nodes/actions/stopallsounds.py
--rw-rw-rw-   0        0        0      624 2022-01-12 14:28:14.000000 uplogic-1.9.4/uplogic/nodes/actions/stopsound.py
--rw-rw-rw-   0        0        0     1209 2022-02-07 22:56:33.000000 uplogic-1.9.4/uplogic/nodes/actions/stopsubnetwork.py
--rw-rw-rw-   0        0        0      842 2022-09-06 10:25:56.000000 uplogic-1.9.4/uplogic/nodes/actions/togglefilter.py
--rw-rw-rw-   0        0        0     1227 2022-04-09 10:37:36.000000 uplogic-1.9.4/uplogic/nodes/actions/toggleproperty.py
--rw-rw-rw-   0        0        0     2809 2022-01-12 14:57:52.000000 uplogic-1.9.4/uplogic/nodes/actions/translate.py
--rw-rw-rw-   0        0        0     1391 2023-05-14 08:57:16.000000 uplogic-1.9.4/uplogic/nodes/actions/vehicleapplybraking.py
--rw-rw-rw-   0        0        0     1379 2023-05-14 08:57:23.000000 uplogic-1.9.4/uplogic/nodes/actions/vehicleapplyforce.py
--rw-rw-rw-   0        0        0     1392 2023-05-14 08:57:30.000000 uplogic-1.9.4/uplogic/nodes/actions/vehicleapplysteering.py
--rw-rw-rw-   0        0        0     3473 2023-05-14 08:57:36.000000 uplogic-1.9.4/uplogic/nodes/actions/vehiclesetattributes.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:07.508090 uplogic-1.9.4/uplogic/nodes/conditions/
--rw-rw-rw-   0        0        0     1946 2022-01-20 14:15:37.000000 uplogic-1.9.4/uplogic/nodes/conditions/__init__.py
--rw-rw-rw-   0        0        0      935 2022-01-12 13:06:20.000000 uplogic-1.9.4/uplogic/nodes/conditions/barrier.py
--rw-rw-rw-   0        0        0     2397 2023-05-14 08:57:52.000000 uplogic-1.9.4/uplogic/nodes/conditions/checkdistance.py
--rw-rw-rw-   0        0        0     4852 2023-05-23 10:33:12.000000 uplogic-1.9.4/uplogic/nodes/conditions/collision.py
--rw-rw-rw-   0        0        0     1508 2023-05-14 08:58:21.000000 uplogic-1.9.4/uplogic/nodes/conditions/compare.py
--rw-rw-rw-   0        0        0     2175 2023-05-14 08:58:27.000000 uplogic-1.9.4/uplogic/nodes/conditions/comparevectors.py
--rw-rw-rw-   0        0        0     3288 2022-01-10 17:39:46.000000 uplogic-1.9.4/uplogic/nodes/conditions/controllerstatus.py
--rw-rw-rw-   0        0        0     1497 2023-05-14 08:58:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/evaluateproperty.py
--rw-rw-rw-   0        0        0      756 2022-01-28 16:50:48.000000 uplogic-1.9.4/uplogic/nodes/conditions/gamepadactive.py
--rw-rw-rw-   0        0        0     1503 2023-05-14 08:58:39.000000 uplogic-1.9.4/uplogic/nodes/conditions/gamepadbutton.py
--rw-rw-rw-   0        0        0     1782 2023-05-14 08:58:43.000000 uplogic-1.9.4/uplogic/nodes/conditions/gamepadbuttonup.py
--rw-rw-rw-   0        0        0     1093 2023-05-14 08:58:51.000000 uplogic-1.9.4/uplogic/nodes/conditions/handleevent.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 08:58:56.000000 uplogic-1.9.4/uplogic/nodes/conditions/hasproperty.py
--rw-rw-rw-   0        0        0      303 2021-12-21 09:41:07.000000 uplogic-1.9.4/uplogic/nodes/conditions/keyboardactive.py
--rw-rw-rw-   0        0        0      812 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/keypressed.py
--rw-rw-rw-   0        0        0      756 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/keyreleased.py
--rw-rw-rw-   0        0        0     1705 2022-02-04 11:39:59.000000 uplogic-1.9.4/uplogic/nodes/conditions/logicand.py
--rw-rw-rw-   0        0        0      621 2022-02-04 11:45:26.000000 uplogic-1.9.4/uplogic/nodes/conditions/logicandnot.py
--rw-rw-rw-   0        0        0      325 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/logicnone.py
--rw-rw-rw-   0        0        0      768 2023-05-14 08:59:42.000000 uplogic-1.9.4/uplogic/nodes/conditions/logicnot.py
--rw-rw-rw-   0        0        0      334 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/logicnotnone.py
--rw-rw-rw-   0        0        0     1168 2023-05-14 09:15:28.000000 uplogic-1.9.4/uplogic/nodes/conditions/logicor.py
--rw-rw-rw-   0        0        0     1681 2023-05-14 09:15:55.000000 uplogic-1.9.4/uplogic/nodes/conditions/logictreestatus.py
--rw-rw-rw-   0        0        0      494 2022-09-11 14:46:42.000000 uplogic-1.9.4/uplogic/nodes/conditions/mousemoved.py
--rw-rw-rw-   0        0        0     3567 2022-09-11 14:47:44.000000 uplogic-1.9.4/uplogic/nodes/conditions/mouseover.py
--rw-rw-rw-   0        0        0     1313 2023-05-14 09:00:04.000000 uplogic-1.9.4/uplogic/nodes/conditions/mousepressed.py
--rw-rw-rw-   0        0        0     1740 2023-05-14 09:00:09.000000 uplogic-1.9.4/uplogic/nodes/conditions/mousepressedon.py
--rw-rw-rw-   0        0        0     1302 2023-05-14 09:00:16.000000 uplogic-1.9.4/uplogic/nodes/conditions/mousereleased.py
--rw-rw-rw-   0        0        0      700 2022-09-11 14:54:01.000000 uplogic-1.9.4/uplogic/nodes/conditions/mousescroll.py
--rw-rw-rw-   0        0        0     1071 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/once.py
--rw-rw-rw-   0        0        0      358 2023-05-14 09:00:22.000000 uplogic-1.9.4/uplogic/nodes/conditions/oninit.py
--rw-rw-rw-   0        0        0      704 2023-04-06 11:05:27.000000 uplogic-1.9.4/uplogic/nodes/conditions/onnexttick.py
--rw-rw-rw-   0        0        0      359 2023-05-14 09:00:29.000000 uplogic-1.9.4/uplogic/nodes/conditions/onupdate.py
--rw-rw-rw-   0        0        0     1270 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/conditions/onvaluechanged.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 09:00:33.000000 uplogic-1.9.4/uplogic/nodes/conditions/onvaluechangedto.py
--rw-rw-rw-   0        0        0     1474 2022-05-25 09:41:06.000000 uplogic-1.9.4/uplogic/nodes/conditions/pulsify.py
--rw-rw-rw-   0        0        0     1105 2023-05-14 09:16:25.000000 uplogic-1.9.4/uplogic/nodes/conditions/sensorpositive.py
--rw-rw-rw-   0        0        0      940 2022-01-17 10:41:45.000000 uplogic-1.9.4/uplogic/nodes/conditions/timedelay.py
--rw-rw-rw-   0        0        0      918 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/timer.py
--rw-rw-rw-   0        0        0      548 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/truefalse.py
--rw-rw-rw-   0        0        0      377 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/conditions/valuevalid.py
--rw-rw-rw-   0        0        0     8472 2023-05-19 05:22:01.000000 uplogic-1.9.4/uplogic/nodes/logictree.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.232858 uplogic-1.9.4/uplogic/nodes/parameters/
--rw-rw-rw-   0        0        0     4767 2023-06-13 19:48:28.000000 uplogic-1.9.4/uplogic/nodes/parameters/__init__.py
--rw-rw-rw-   0        0        0      648 2023-05-14 09:00:44.000000 uplogic-1.9.4/uplogic/nodes/parameters/absolutevalue.py
--rw-rw-rw-   0        0        0     1713 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/actionstatus.py
--rw-rw-rw-   0        0        0      585 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/activecamera.py
--rw-rw-rw-   0        0        0      909 2023-05-14 09:01:31.000000 uplogic-1.9.4/uplogic/nodes/parameters/axisvector.py
--rw-rw-rw-   0        0        0     1923 2023-05-14 09:01:36.000000 uplogic-1.9.4/uplogic/nodes/parameters/bonestatus.py
--rw-rw-rw-   0        0        0     1911 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/parameters/characterinfo.py
--rw-rw-rw-   0        0        0     1158 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/childbyindex.py
--rw-rw-rw-   0        0        0      903 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/childbyname.py
--rw-rw-rw-   0        0        0     1116 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/clamp.py
--rw-rw-rw-   0        0        0      792 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/colorrgb.py
--rw-rw-rw-   0        0        0      719 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/parameters/colorrgba.py
--rw-rw-rw-   0        0        0      911 2022-02-17 16:47:54.000000 uplogic-1.9.4/uplogic/nodes/parameters/dictvalue.py
--rw-rw-rw-   0        0        0      920 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/distance.py
--rw-rw-rw-   0        0        0      910 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/parameters/euler.py
--rw-rw-rw-   0        0        0      786 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/parameters/eulertomatrix.py
--rw-rw-rw-   0        0        0     1284 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/formattedstring.py
--rw-rw-rw-   0        0        0     2158 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/parameters/formula.py
--rw-rw-rw-   0        0        0     1858 2023-07-07 11:36:29.000000 uplogic-1.9.4/uplogic/nodes/parameters/gamepadsticks.py
--rw-rw-rw-   0        0        0     1563 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/gamepadtrigger.py
--rw-rw-rw-   0        0        0     1097 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getactuatorvalue.py
--rw-rw-rw-   0        0        0      612 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getcollection.py
--rw-rw-rw-   0        0        0     1056 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getcollectionobjectnames.py
--rw-rw-rw-   0        0        0     1047 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getcollectionobjects.py
--rw-rw-rw-   0        0        0     1055 2022-01-10 11:25:35.000000 uplogic-1.9.4/uplogic/nodes/parameters/getcurvepoints.py
--rw-rw-rw-   0        0        0      527 2023-03-02 19:33:55.000000 uplogic-1.9.4/uplogic/nodes/parameters/getfont.py
--rw-rw-rw-   0        0        0      401 2023-06-07 19:15:13.000000 uplogic-1.9.4/uplogic/nodes/parameters/getfullscreen.py
--rw-rw-rw-   0        0        0     1100 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getglobalvalue.py
--rw-rw-rw-   0        0        0      432 2021-12-21 09:41:07.000000 uplogic-1.9.4/uplogic/nodes/parameters/getgravity.py
--rw-rw-rw-   0        0        0      534 2022-01-10 11:08:34.000000 uplogic-1.9.4/uplogic/nodes/parameters/getimage.py
--rw-rw-rw-   0        0        0      648 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getlightcolor.py
--rw-rw-rw-   0        0        0      654 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getlightenergy.py
--rw-rw-rw-   0        0        0     1420 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getnodeattribute.py
--rw-rw-rw-   0        0        0     1294 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getnodesocket.py
--rw-rw-rw-   0        0        0      762 2023-05-16 10:12:45.000000 uplogic-1.9.4/uplogic/nodes/parameters/getobject.py
--rw-rw-rw-   0        0        0      442 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getowner.py
--rw-rw-rw-   0        0        0      614 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getparent.py
--rw-rw-rw-   0        0        0     1080 2023-05-14 16:12:28.000000 uplogic-1.9.4/uplogic/nodes/parameters/getproperty.py
--rw-rw-rw-   0        0        0      715 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getpyinstanceattr.py
--rw-rw-rw-   0        0        0      760 2022-01-12 11:11:52.000000 uplogic-1.9.4/uplogic/nodes/parameters/getresolution.py
--rw-rw-rw-   0        0        0      384 2021-12-21 09:41:07.000000 uplogic-1.9.4/uplogic/nodes/parameters/getscene.py
--rw-rw-rw-   0        0        0      954 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getsensorvalue.py
--rw-rw-rw-   0        0        0      572 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/getsound.py
--rw-rw-rw-   0        0        0      385 2021-12-21 09:41:07.000000 uplogic-1.9.4/uplogic/nodes/parameters/gettimescale.py
--rw-rw-rw-   0        0        0     1070 2023-03-02 22:50:45.000000 uplogic-1.9.4/uplogic/nodes/parameters/getuiwidgetattr.py
--rw-rw-rw-   0        0        0      381 2023-06-07 19:15:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/getvsync.py
--rw-rw-rw-   0        0        0      429 2022-01-12 11:37:03.000000 uplogic-1.9.4/uplogic/nodes/parameters/initemptydict.py
--rw-rw-rw-   0        0        0      599 2022-01-26 18:13:15.000000 uplogic-1.9.4/uplogic/nodes/parameters/initemptylist.py
--rw-rw-rw-   0        0        0      652 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/initnewdict.py
--rw-rw-rw-   0        0        0      873 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/interpolate.py
--rw-rw-rw-   0        0        0      620 2022-01-10 14:18:19.000000 uplogic-1.9.4/uplogic/nodes/parameters/invertvalue.py
--rw-rw-rw-   0        0        0      316 2022-01-10 11:08:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/keycode.py
--rw-rw-rw-   0        0        0     1475 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/limitrange.py
--rw-rw-rw-   0        0        0      620 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/listduplicate.py
--rw-rw-rw-   0        0        0      823 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/listextend.py
--rw-rw-rw-   0        0        0      697 2022-12-21 14:09:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/listfromitems.py
--rw-rw-rw-   0        0        0      827 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/listindex.py
--rw-rw-rw-   0        0        0      835 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/listindexrandom.py
--rw-rw-rw-   0        0        0     1951 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/loadvariable.py
--rw-rw-rw-   0        0        0     1479 2023-02-14 10:12:26.000000 uplogic-1.9.4/uplogic/nodes/parameters/loadvariabledict.py
--rw-rw-rw-   0        0        0     1432 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/materialgetattribute.py
--rw-rw-rw-   0        0        0      799 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/materialgetnode.py
--rw-rw-rw-   0        0        0     1300 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/materialgetsocket.py
--rw-rw-rw-   0        0        0     2549 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/math.py
--rw-rw-rw-   0        0        0      672 2022-01-30 10:48:51.000000 uplogic-1.9.4/uplogic/nodes/parameters/matrixtoxyz.py
--rw-rw-rw-   0        0        0     1278 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/mousedata.py
--rw-rw-rw-   0        0        0     1144 2023-07-07 13:41:52.000000 uplogic-1.9.4/uplogic/nodes/parameters/objectattr.py
--rw-rw-rw-   0        0        0      601 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/objectdataname.py
--rw-rw-rw-   0        0        0     1146 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/objectdatavertices.py
--rw-rw-rw-   0        0        0     1222 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/randomfloat.py
--rw-rw-rw-   0        0        0     1167 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/randomint.py
--rw-rw-rw-   0        0        0      979 2022-01-16 18:24:15.000000 uplogic-1.9.4/uplogic/nodes/parameters/randomvect.py
--rw-rw-rw-   0        0        0     1032 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/rangedthreshold.py
--rw-rw-rw-   0        0        0      789 2023-06-13 19:51:24.000000 uplogic-1.9.4/uplogic/nodes/parameters/rebuilddata.py
--rw-rw-rw-   0        0        0      871 2023-05-14 16:12:38.000000 uplogic-1.9.4/uplogic/nodes/parameters/screenposition.py
--rw-rw-rw-   0        0        0      829 2023-05-16 09:25:56.000000 uplogic-1.9.4/uplogic/nodes/parameters/serializedata.py
--rw-rw-rw-   0        0        0      417 2022-01-10 11:08:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/simplevalue.py
--rw-rw-rw-   0        0        0      775 2023-06-16 18:58:38.000000 uplogic-1.9.4/uplogic/nodes/parameters/storevalue.py
--rw-rw-rw-   0        0        0     1102 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/threshold.py
--rw-rw-rw-   0        0        0     1007 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/timedata.py
--rw-rw-rw-   0        0        0      988 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/typecastvalue.py
--rw-rw-rw-   0        0        0     4507 2023-05-14 09:01:49.000000 uplogic-1.9.4/uplogic/nodes/parameters/valueswitch.py
--rw-rw-rw-   0        0        0      751 2023-05-14 16:12:43.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorabsolute.py
--rw-rw-rw-   0        0        0      886 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorangle.py
--rw-rw-rw-   0        0        0     1385 2023-05-14 09:01:59.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectoranglecheck.py
--rw-rw-rw-   0        0        0      646 2023-05-14 16:12:48.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorlength.py
--rw-rw-rw-   0        0        0     3625 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectormath.py
--rw-rw-rw-   0        0        0      717 2022-01-10 11:08:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorsplitxy.py
--rw-rw-rw-   0        0        0     1032 2022-01-30 14:47:33.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorsplitxyz.py
--rw-rw-rw-   0        0        0      691 2023-03-03 08:53:48.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorxy.py
--rw-rw-rw-   0        0        0      818 2022-01-10 11:08:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorxyz.py
--rw-rw-rw-   0        0        0      945 2022-01-10 11:08:17.000000 uplogic-1.9.4/uplogic/nodes/parameters/vectorxyzw.py
--rw-rw-rw-   0        0        0     1378 2023-03-06 09:01:43.000000 uplogic-1.9.4/uplogic/nodes/parameters/vrcontrollervalues.py
--rw-rw-rw-   0        0        0      583 2023-03-06 09:01:01.000000 uplogic-1.9.4/uplogic/nodes/parameters/vrheadsetvalues.py
--rw-rw-rw-   0        0        0     1026 2023-05-14 09:01:09.000000 uplogic-1.9.4/uplogic/nodes/parameters/withinrange.py
--rw-rw-rw-   0        0        0     1293 2023-05-14 16:12:52.000000 uplogic-1.9.4/uplogic/nodes/parameters/worldposition.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.280869 uplogic-1.9.4/uplogic/physics/
--rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-1.9.4/uplogic/physics/__init__.py
--rw-rw-rw-   0        0        0     4196 2023-05-14 08:28:32.000000 uplogic-1.9.4/uplogic/physics/buoyancy.py
--rw-rw-rw-   0        0        0     4099 2023-07-05 14:13:35.000000 uplogic-1.9.4/uplogic/physics/character.py
--rw-rw-rw-   0        0        0     3450 2023-05-14 08:29:19.000000 uplogic-1.9.4/uplogic/physics/collision.py
--rw-rw-rw-   0        0        0     8370 2023-05-14 08:38:03.000000 uplogic-1.9.4/uplogic/physics/constraints.py
--rw-rw-rw-   0        0        0    10072 2023-05-14 08:30:19.000000 uplogic-1.9.4/uplogic/physics/vehicle.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.289872 uplogic-1.9.4/uplogic/serialize/
--rw-rw-rw-   0        0        0     2945 2023-05-16 08:33:09.000000 uplogic-1.9.4/uplogic/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.423911 uplogic-1.9.4/uplogic/shaders/
--rw-rw-rw-   0        0        0      675 2023-04-01 06:53:28.000000 uplogic-1.9.4/uplogic/shaders/__init__.py
--rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-1.9.4/uplogic/shaders/adaptivetonemapping.py
--rw-rw-rw-   0        0        0     1631 2023-04-01 06:53:32.000000 uplogic-1.9.4/uplogic/shaders/blur.py
--rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/brightness.py
--rw-rw-rw-   0        0        0     1050 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/chromaticaberration.py
--rw-rw-rw-   0        0        0     8869 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/distort.py
--rw-rw-rw-   0        0        0     9818 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/dof.py
--rw-rw-rw-   0        0        0     9106 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/droplets.py
--rw-rw-rw-   0        0        0    33424 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/fxaa.py
--rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/grayscale.py
--rw-rw-rw-   0        0        0     9683 2023-07-05 14:45:48.000000 uplogic-1.9.4/uplogic/shaders/hbao.py
--rw-rw-rw-   0        0        0     1173 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/letterbox.py
--rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/levels.py
--rw-rw-rw-   0        0        0     4209 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/mist.py
--rw-rw-rw-   0        0        0     5411 2023-04-01 07:02:38.000000 uplogic-1.9.4/uplogic/shaders/shader.py
--rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/sharpen.py
--rw-rw-rw-   0        0        0     5738 2023-06-20 15:34:55.000000 uplogic-1.9.4/uplogic/shaders/ssao.py
--rw-rw-rw-   0        0        0     1190 2023-04-01 06:54:25.000000 uplogic-1.9.4/uplogic/shaders/vignette.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.493918 uplogic-1.9.4/uplogic/ui/
--rw-rw-rw-   0        0        0      367 2023-06-20 17:11:49.000000 uplogic-1.9.4/uplogic/ui/__init__.py
--rw-rw-rw-   0        0        0      579 2023-04-02 14:03:20.000000 uplogic-1.9.4/uplogic/ui/behaviors.py
--rw-rw-rw-   0        0        0     5139 2023-06-05 09:06:00.000000 uplogic-1.9.4/uplogic/ui/button.py
--rw-rw-rw-   0        0        0     1301 2023-06-05 09:06:00.000000 uplogic-1.9.4/uplogic/ui/canvas.py
--rw-rw-rw-   0        0        0     2438 2023-04-26 12:34:19.000000 uplogic-1.9.4/uplogic/ui/cursor.py
--rw-rw-rw-   0        0        0     4179 2023-06-26 10:59:15.000000 uplogic-1.9.4/uplogic/ui/image.py
--rw-rw-rw-   0        0        0     6180 2023-06-05 09:06:00.000000 uplogic-1.9.4/uplogic/ui/label.py
--rw-rw-rw-   0        0        0     6441 2023-06-14 10:42:03.000000 uplogic-1.9.4/uplogic/ui/layout.py
--rw-rw-rw-   0        0        0    11258 2023-06-14 10:56:40.000000 uplogic-1.9.4/uplogic/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:08.592941 uplogic-1.9.4/uplogic/utils/
--rw-rw-rw-   0        0        0     7036 2023-07-07 10:14:02.000000 uplogic-1.9.4/uplogic/utils/__init__.py
--rw-rw-rw-   0        0        0     1429 2023-07-05 18:18:21.000000 uplogic-1.9.4/uplogic/utils/constants.py
--rw-rw-rw-   0        0        0     1089 2023-06-20 14:44:01.000000 uplogic-1.9.4/uplogic/utils/engine.py
--rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-1.9.4/uplogic/utils/errors.py
--rw-rw-rw-   0        0        0     7571 2023-06-05 09:06:00.000000 uplogic-1.9.4/uplogic/utils/lights.py
--rw-rw-rw-   0        0        0     7975 2023-07-05 15:28:25.000000 uplogic-1.9.4/uplogic/utils/math.py
--rw-rw-rw-   0        0        0     4801 2022-08-22 17:00:51.000000 uplogic-1.9.4/uplogic/utils/nodetrees.py
--rw-rw-rw-   0        0        0    11155 2023-07-07 11:02:08.000000 uplogic-1.9.4/uplogic/utils/objects.py
--rw-rw-rw-   0        0        0     6193 2023-07-07 11:33:19.000000 uplogic-1.9.4/uplogic/utils/pooling.py
--rw-rw-rw-   0        0        0    13346 2023-05-14 16:52:14.000000 uplogic-1.9.4/uplogic/utils/raycasting.py
--rw-rw-rw-   0        0        0     5831 2022-10-05 11:16:36.000000 uplogic-1.9.4/uplogic/utils/scene.py
--rw-rw-rw-   0        0        0     2037 2023-06-05 09:06:00.000000 uplogic-1.9.4/uplogic/utils/visuals.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:44:05.796218 uplogic-1.9.4/uplogic.egg-info/
--rw-rw-rw-   0        0        0     1049 2023-07-07 13:44:05.000000 uplogic-1.9.4/uplogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13638 2023-07-07 13:44:05.000000 uplogic-1.9.4/uplogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:44:05.000000 uplogic-1.9.4/uplogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 13:44:05.000000 uplogic-1.9.4/uplogic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-07 13:44:05.000000 uplogic-1.9.4/uplogic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-1.9.4/uplogic.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.473856 uplogic-1.9.5/
+-rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-1.9.5/LICENSE.md
+-rw-rw-rw-   0        0        0     1049 2023-07-07 13:58:28.473856 uplogic-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-1.9.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:58:28.474855 uplogic-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1743 2023-07-07 13:57:56.000000 uplogic-1.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.058233 uplogic-1.9.5/uplogic/
+-rw-rw-rw-   0        0        0     5944 2023-07-05 13:56:27.000000 uplogic-1.9.5/uplogic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.090241 uplogic-1.9.5/uplogic/animation/
+-rw-rw-rw-   0        0        0      343 2023-03-08 12:02:42.000000 uplogic-1.9.5/uplogic/animation/__init__.py
+-rw-rw-rw-   0        0        0    12544 2023-07-07 11:38:36.000000 uplogic-1.9.5/uplogic/animation/action.py
+-rw-rw-rw-   0        0        0     4016 2023-05-01 17:00:05.000000 uplogic-1.9.5/uplogic/animation/actionsystem.py
+-rw-rw-rw-   0        0        0     6224 2023-05-14 08:46:37.000000 uplogic-1.9.5/uplogic/animation/sequence.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.094243 uplogic-1.9.5/uplogic/audio/
+-rw-rw-rw-   0        0        0      606 2023-03-06 09:07:59.000000 uplogic-1.9.5/uplogic/audio/__init__.py
+-rw-rw-rw-   0        0        0     7689 2023-04-24 21:26:30.000000 uplogic-1.9.5/uplogic/audio/audiosystem.py
+-rw-rw-rw-   0        0        0     6839 2023-05-14 08:47:09.000000 uplogic-1.9.5/uplogic/audio/music.py
+-rw-rw-rw-   0        0        0    23984 2023-07-05 14:14:26.000000 uplogic-1.9.5/uplogic/audio/sound.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.098242 uplogic-1.9.5/uplogic/data/
+-rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-1.9.5/uplogic/data/__init__.py
+-rw-rw-rw-   0        0        0     3122 2023-04-07 16:35:00.000000 uplogic-1.9.5/uplogic/data/file.py
+-rw-rw-rw-   0        0        0     7148 2023-05-14 08:48:26.000000 uplogic-1.9.5/uplogic/data/globaldb.py
+-rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-1.9.5/uplogic/data/serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.099243 uplogic-1.9.5/uplogic/decorators/
+-rw-rw-rw-   0        0        0    11024 2023-06-20 15:01:27.000000 uplogic-1.9.5/uplogic/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.100242 uplogic-1.9.5/uplogic/events/
+-rw-rw-rw-   0        0        0     7615 2023-04-04 13:17:19.000000 uplogic-1.9.5/uplogic/events/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.107245 uplogic-1.9.5/uplogic/input/
+-rw-rw-rw-   0        0        0     1494 2023-03-06 08:52:33.000000 uplogic-1.9.5/uplogic/input/__init__.py
+-rw-rw-rw-   0        0        0    15064 2023-06-13 14:39:52.000000 uplogic-1.9.5/uplogic/input/gamepad.py
+-rw-rw-rw-   0        0        0     9607 2023-01-16 12:00:44.000000 uplogic-1.9.5/uplogic/input/keyboard.py
+-rw-rw-rw-   0        0        0    14930 2023-05-14 08:49:32.000000 uplogic-1.9.5/uplogic/input/mouse.py
+-rw-rw-rw-   0        0        0     9131 2023-05-14 08:49:48.000000 uplogic-1.9.5/uplogic/input/vr.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.109245 uplogic-1.9.5/uplogic/logging/
+-rw-rw-rw-   0        0        0     6115 2023-06-06 15:11:05.000000 uplogic-1.9.5/uplogic/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.111245 uplogic-1.9.5/uplogic/network/
+-rw-rw-rw-   0        0        0       56 2023-06-05 09:06:00.000000 uplogic-1.9.5/uplogic/network/__init__.py
+-rw-rw-rw-   0        0        0     3351 2023-06-05 09:11:35.000000 uplogic-1.9.5/uplogic/network/client.py
+-rw-rw-rw-   0        0        0     4756 2023-06-13 19:02:29.000000 uplogic-1.9.5/uplogic/network/server.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.113247 uplogic-1.9.5/uplogic/nodes/
+-rw-rw-rw-   0        0        0     5176 2023-05-19 05:22:01.000000 uplogic-1.9.5/uplogic/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.274811 uplogic-1.9.5/uplogic/nodes/actions/
+-rw-rw-rw-   0        0        0     8023 2023-05-16 08:46:11.000000 uplogic-1.9.5/uplogic/nodes/actions/__init__.py
+-rw-rw-rw-   0        0        0     4065 2022-11-02 09:25:32.000000 uplogic-1.9.5/uplogic/nodes/actions/addfilter.py
+-rw-rw-rw-   0        0        0     1308 2022-08-21 23:02:22.000000 uplogic-1.9.5/uplogic/nodes/actions/addobject.py
+-rw-rw-rw-   0        0        0     2710 2022-04-24 07:51:50.000000 uplogic-1.9.5/uplogic/nodes/actions/addphysicsconstraint.py
+-rw-rw-rw-   0        0        0      797 2023-03-01 15:33:33.000000 uplogic-1.9.5/uplogic/nodes/actions/adduiwidget.py
+-rw-rw-rw-   0        0        0     1420 2022-10-28 14:13:34.000000 uplogic-1.9.5/uplogic/nodes/actions/alignaxistovector.py
+-rw-rw-rw-   0        0        0     1056 2022-01-12 11:55:23.000000 uplogic-1.9.5/uplogic/nodes/actions/appendlistitem.py
+-rw-rw-rw-   0        0        0     1007 2022-01-12 13:37:33.000000 uplogic-1.9.5/uplogic/nodes/actions/applyforce.py
+-rw-rw-rw-   0        0        0     1187 2022-01-12 13:38:47.000000 uplogic-1.9.5/uplogic/nodes/actions/applyimpulse.py
+-rw-rw-rw-   0        0        0     1074 2022-01-12 13:36:04.000000 uplogic-1.9.5/uplogic/nodes/actions/applymovement.py
+-rw-rw-rw-   0        0        0     1237 2023-01-05 15:34:33.000000 uplogic-1.9.5/uplogic/nodes/actions/applyrotation.py
+-rw-rw-rw-   0        0        0      984 2022-01-12 14:18:21.000000 uplogic-1.9.5/uplogic/nodes/actions/applytorque.py
+-rw-rw-rw-   0        0        0     2560 2022-01-10 18:02:58.000000 uplogic-1.9.5/uplogic/nodes/actions/cameraraycast.py
+-rw-rw-rw-   0        0        0     1014 2022-01-12 14:08:55.000000 uplogic-1.9.5/uplogic/nodes/actions/characterjump.py
+-rw-rw-rw-   0        0        0     1536 2022-04-10 10:15:42.000000 uplogic-1.9.5/uplogic/nodes/actions/clampedmodifyproperty.py
+-rw-rw-rw-   0        0        0     1610 2023-05-14 08:51:40.000000 uplogic-1.9.5/uplogic/nodes/actions/clearvariables.py
+-rw-rw-rw-   0        0        0     1395 2022-04-09 10:45:53.000000 uplogic-1.9.5/uplogic/nodes/actions/copyproperty.py
+-rw-rw-rw-   0        0        0     3577 2023-06-14 11:06:15.000000 uplogic-1.9.5/uplogic/nodes/actions/createuibutton.py
+-rw-rw-rw-   0        0        0      821 2023-03-01 15:34:01.000000 uplogic-1.9.5/uplogic/nodes/actions/createuicanvas.py
+-rw-rw-rw-   0        0        0     1789 2023-06-14 11:06:17.000000 uplogic-1.9.5/uplogic/nodes/actions/createuiimage.py
+-rw-rw-rw-   0        0        0     2599 2023-06-14 11:06:17.000000 uplogic-1.9.5/uplogic/nodes/actions/createuilabel.py
+-rw-rw-rw-   0        0        0     2386 2023-06-14 11:06:17.000000 uplogic-1.9.5/uplogic/nodes/actions/createuilayout.py
+-rw-rw-rw-   0        0        0     2003 2023-05-14 08:51:47.000000 uplogic-1.9.5/uplogic/nodes/actions/createvehicle.py
+-rw-rw-rw-   0        0        0     1523 2022-09-11 14:27:22.000000 uplogic-1.9.5/uplogic/nodes/actions/cursorbehavior.py
+-rw-rw-rw-   0        0        0      797 2023-03-02 21:19:09.000000 uplogic-1.9.5/uplogic/nodes/actions/cursorvisibility.py
+-rw-rw-rw-   0        0        0     1245 2023-05-14 08:51:57.000000 uplogic-1.9.5/uplogic/nodes/actions/dispatchevent.py
+-rw-rw-rw-   0        0        0     1188 2023-05-14 08:52:09.000000 uplogic-1.9.5/uplogic/nodes/actions/drawbox.py
+-rw-rw-rw-   0        0        0     1028 2023-05-14 08:52:17.000000 uplogic-1.9.5/uplogic/nodes/actions/drawcube.py
+-rw-rw-rw-   0        0        0      980 2022-08-23 18:34:20.000000 uplogic-1.9.5/uplogic/nodes/actions/drawline.py
+-rw-rw-rw-   0        0        0     3560 2022-01-12 12:12:44.000000 uplogic-1.9.5/uplogic/nodes/actions/editbone.py
+-rw-rw-rw-   0        0        0      530 2022-07-18 15:47:27.000000 uplogic-1.9.5/uplogic/nodes/actions/endgame.py
+-rw-rw-rw-   0        0        0     1019 2022-01-12 13:25:49.000000 uplogic-1.9.5/uplogic/nodes/actions/endobject.py
+-rw-rw-rw-   0        0        0     1237 2022-02-07 22:47:57.000000 uplogic-1.9.5/uplogic/nodes/actions/executesubnetwork.py
+-rw-rw-rw-   0        0        0     5575 2023-07-07 10:14:02.000000 uplogic-1.9.5/uplogic/nodes/actions/followpath.py
+-rw-rw-rw-   0        0        0     4138 2023-05-16 16:57:59.000000 uplogic-1.9.5/uplogic/nodes/actions/gamepadlook.py
+-rw-rw-rw-   0        0        0     1395 2023-05-14 08:53:21.000000 uplogic-1.9.5/uplogic/nodes/actions/gamepadvibration.py
+-rw-rw-rw-   0        0        0     2383 2022-01-12 12:04:24.000000 uplogic-1.9.5/uplogic/nodes/actions/getperformanceprofile.py
+-rw-rw-rw-   0        0        0     1373 2022-02-07 22:56:45.000000 uplogic-1.9.5/uplogic/nodes/actions/installsubnetwork.py
+-rw-rw-rw-   0        0        0     1976 2023-04-26 12:34:19.000000 uplogic-1.9.5/uplogic/nodes/actions/instream.py
+-rw-rw-rw-   0        0        0     1338 2023-06-07 19:15:20.000000 uplogic-1.9.5/uplogic/nodes/actions/listglobalvalues.py
+-rw-rw-rw-   0        0        0     2110 2023-05-14 08:53:38.000000 uplogic-1.9.5/uplogic/nodes/actions/listvariables.py
+-rw-rw-rw-   0        0        0      674 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/loadblendfile.py
+-rw-rw-rw-   0        0        0     1586 2023-05-14 08:53:49.000000 uplogic-1.9.5/uplogic/nodes/actions/loadfilecontent.py
+-rw-rw-rw-   0        0        0     4266 2023-05-14 08:54:00.000000 uplogic-1.9.5/uplogic/nodes/actions/loadgame.py
+-rw-rw-rw-   0        0        0     1658 2023-05-14 08:54:06.000000 uplogic-1.9.5/uplogic/nodes/actions/loadscene.py
+-rw-rw-rw-   0        0        0     2515 2023-05-16 10:27:44.000000 uplogic-1.9.5/uplogic/nodes/actions/localclient.py
+-rw-rw-rw-   0        0        0     2391 2023-05-16 10:27:30.000000 uplogic-1.9.5/uplogic/nodes/actions/localserver.py
+-rw-rw-rw-   0        0        0     1051 2022-01-12 15:17:30.000000 uplogic-1.9.5/uplogic/nodes/actions/makeuniquelight.py
+-rw-rw-rw-   0        0        0     1363 2022-04-10 10:15:35.000000 uplogic-1.9.5/uplogic/nodes/actions/modifyproperty.py
+-rw-rw-rw-   0        0        0     4855 2023-05-19 05:22:01.000000 uplogic-1.9.5/uplogic/nodes/actions/mouselook.py
+-rw-rw-rw-   0        0        0     2144 2022-01-10 18:01:11.000000 uplogic-1.9.5/uplogic/nodes/actions/mouseraycast.py
+-rw-rw-rw-   0        0        0     1012 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/mousesetposition.py
+-rw-rw-rw-   0        0        0     1521 2023-05-14 08:54:30.000000 uplogic-1.9.5/uplogic/nodes/actions/moveto.py
+-rw-rw-rw-   0        0        0     5241 2023-07-07 10:14:02.000000 uplogic-1.9.5/uplogic/nodes/actions/movetowithnavmesh.py
+-rw-rw-rw-   0        0        0      626 2022-01-12 14:35:38.000000 uplogic-1.9.5/uplogic/nodes/actions/pausesound.py
+-rw-rw-rw-   0        0        0     5400 2023-05-14 08:54:59.000000 uplogic-1.9.5/uplogic/nodes/actions/playaction.py
+-rw-rw-rw-   0        0        0     2476 2023-02-12 11:22:41.000000 uplogic-1.9.5/uplogic/nodes/actions/playsequence.py
+-rw-rw-rw-   0        0        0     1338 2023-05-14 08:55:21.000000 uplogic-1.9.5/uplogic/nodes/actions/popdictkey.py
+-rw-rw-rw-   0        0        0      762 2023-05-16 10:26:49.000000 uplogic-1.9.5/uplogic/nodes/actions/printvalue.py
+-rw-rw-rw-   0        0        0     3218 2023-05-16 10:40:40.000000 uplogic-1.9.5/uplogic/nodes/actions/projectileraycast.py
+-rw-rw-rw-   0        0        0     3516 2022-09-11 15:14:18.000000 uplogic-1.9.5/uplogic/nodes/actions/raycast.py
+-rw-rw-rw-   0        0        0      842 2022-09-06 10:05:33.000000 uplogic-1.9.5/uplogic/nodes/actions/removefilter.py
+-rw-rw-rw-   0        0        0     1176 2022-01-12 11:59:50.000000 uplogic-1.9.5/uplogic/nodes/actions/removelistindex.py
+-rw-rw-rw-   0        0        0     1207 2022-01-12 11:59:09.000000 uplogic-1.9.5/uplogic/nodes/actions/removelistvalue.py
+-rw-rw-rw-   0        0        0      779 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/removeoverlaycollection.py
+-rw-rw-rw-   0        0        0      969 2022-02-01 19:49:18.000000 uplogic-1.9.5/uplogic/nodes/actions/removeparent.py
+-rw-rw-rw-   0        0        0      974 2022-01-12 15:45:41.000000 uplogic-1.9.5/uplogic/nodes/actions/removephysicsconstraint.py
+-rw-rw-rw-   0        0        0     1834 2023-02-14 10:14:02.000000 uplogic-1.9.5/uplogic/nodes/actions/removevariable.py
+-rw-rw-rw-   0        0        0     1255 2022-01-12 15:43:12.000000 uplogic-1.9.5/uplogic/nodes/actions/replacemesh.py
+-rw-rw-rw-   0        0        0      633 2022-02-10 19:19:01.000000 uplogic-1.9.5/uplogic/nodes/actions/restartgame.py
+-rw-rw-rw-   0        0        0      628 2022-01-12 14:37:05.000000 uplogic-1.9.5/uplogic/nodes/actions/resumesound.py
+-rw-rw-rw-   0        0        0     1611 2023-07-07 11:05:26.000000 uplogic-1.9.5/uplogic/nodes/actions/rotateto.py
+-rw-rw-rw-   0        0        0     1199 2022-02-09 13:38:34.000000 uplogic-1.9.5/uplogic/nodes/actions/runactuator.py
+-rw-rw-rw-   0        0        0     1716 2023-05-15 10:27:54.000000 uplogic-1.9.5/uplogic/nodes/actions/runpython.py
+-rw-rw-rw-   0        0        0     7976 2022-02-08 15:48:21.000000 uplogic-1.9.5/uplogic/nodes/actions/savegame.py
+-rw-rw-rw-   0        0        0     2005 2023-02-14 10:08:13.000000 uplogic-1.9.5/uplogic/nodes/actions/savevariable.py
+-rw-rw-rw-   0        0        0     1738 2023-02-14 10:08:29.000000 uplogic-1.9.5/uplogic/nodes/actions/savevariabledict.py
+-rw-rw-rw-   0        0        0     1180 2022-01-10 17:48:43.000000 uplogic-1.9.5/uplogic/nodes/actions/sendmessage.py
+-rw-rw-rw-   0        0        0      849 2023-05-16 09:59:36.000000 uplogic-1.9.5/uplogic/nodes/actions/sendnetworkmessage.py
+-rw-rw-rw-   0        0        0     2608 2023-02-13 17:09:10.000000 uplogic-1.9.5/uplogic/nodes/actions/setactionframe.py
+-rw-rw-rw-   0        0        0     1135 2022-02-26 12:20:29.000000 uplogic-1.9.5/uplogic/nodes/actions/setactuatorvalue.py
+-rw-rw-rw-   0        0        0     1532 2022-01-12 13:30:41.000000 uplogic-1.9.5/uplogic/nodes/actions/setboneconstraintattr.py
+-rw-rw-rw-   0        0        0     1389 2022-01-12 12:09:35.000000 uplogic-1.9.5/uplogic/nodes/actions/setboneconstraintinfluence.py
+-rw-rw-rw-   0        0        0     1382 2022-01-12 12:08:54.000000 uplogic-1.9.5/uplogic/nodes/actions/setboneconstrainttarget.py
+-rw-rw-rw-   0        0        0     1488 2022-01-12 12:15:32.000000 uplogic-1.9.5/uplogic/nodes/actions/setboneposition.py
+-rw-rw-rw-   0        0        0      944 2022-01-10 18:05:42.000000 uplogic-1.9.5/uplogic/nodes/actions/setcamera.py
+-rw-rw-rw-   0        0        0      941 2022-01-23 23:21:22.000000 uplogic-1.9.5/uplogic/nodes/actions/setcamerafov.py
+-rw-rw-rw-   0        0        0      966 2022-01-10 18:09:57.000000 uplogic-1.9.5/uplogic/nodes/actions/setcameraorthoscale.py
+-rw-rw-rw-   0        0        0     1154 2022-01-12 14:13:53.000000 uplogic-1.9.5/uplogic/nodes/actions/setcharactergravity.py
+-rw-rw-rw-   0        0        0     1102 2022-01-12 14:08:37.000000 uplogic-1.9.5/uplogic/nodes/actions/setcharacterjumpspeed.py
+-rw-rw-rw-   0        0        0     1096 2022-01-12 14:09:24.000000 uplogic-1.9.5/uplogic/nodes/actions/setcharactermaxjumps.py
+-rw-rw-rw-   0        0        0     1200 2022-01-12 14:17:03.000000 uplogic-1.9.5/uplogic/nodes/actions/setcharactervelocity.py
+-rw-rw-rw-   0        0        0     1795 2022-01-12 14:14:18.000000 uplogic-1.9.5/uplogic/nodes/actions/setcharacterwalkdir.py
+-rw-rw-rw-   0        0        0     1030 2022-01-12 13:44:27.000000 uplogic-1.9.5/uplogic/nodes/actions/setcollisiongroup.py
+-rw-rw-rw-   0        0        0     1028 2022-01-12 13:45:39.000000 uplogic-1.9.5/uplogic/nodes/actions/setcollisionmask.py
+-rw-rw-rw-   0        0        0     1493 2022-02-16 14:17:45.000000 uplogic-1.9.5/uplogic/nodes/actions/setcurvepoints.py
+-rw-rw-rw-   0        0        0     1095 2023-05-03 10:24:19.000000 uplogic-1.9.5/uplogic/nodes/actions/setcustomcursor.py
+-rw-rw-rw-   0        0        0     1105 2022-01-12 11:43:10.000000 uplogic-1.9.5/uplogic/nodes/actions/setdictkey.py
+-rw-rw-rw-   0        0        0     1166 2022-09-07 10:43:04.000000 uplogic-1.9.5/uplogic/nodes/actions/setdynamics.py
+-rw-rw-rw-   0        0        0      887 2022-01-12 15:03:06.000000 uplogic-1.9.5/uplogic/nodes/actions/seteeveeao.py
+-rw-rw-rw-   0        0        0      891 2022-01-12 16:00:43.000000 uplogic-1.9.5/uplogic/nodes/actions/seteeveebloom.py
+-rw-rw-rw-   0        0        0      895 2022-01-12 15:08:25.000000 uplogic-1.9.5/uplogic/nodes/actions/seteeveesmaa.py
+-rw-rw-rw-   0        0        0      902 2022-01-12 15:12:11.000000 uplogic-1.9.5/uplogic/nodes/actions/seteeveesmaaquality.py
+-rw-rw-rw-   0        0        0      887 2022-01-12 15:04:58.000000 uplogic-1.9.5/uplogic/nodes/actions/seteeveessr.py
+-rw-rw-rw-   0        0        0      933 2022-01-12 15:05:54.000000 uplogic-1.9.5/uplogic/nodes/actions/seteeveevolumetrics.py
+-rw-rw-rw-   0        0        0      920 2022-02-06 14:06:39.000000 uplogic-1.9.5/uplogic/nodes/actions/setexposure.py
+-rw-rw-rw-   0        0        0      935 2022-09-06 10:37:29.000000 uplogic-1.9.5/uplogic/nodes/actions/setfilterstate.py
+-rw-rw-rw-   0        0        0      858 2022-01-10 18:13:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setfullscreen.py
+-rw-rw-rw-   0        0        0     1938 2023-07-07 11:20:03.000000 uplogic-1.9.5/uplogic/nodes/actions/setgameobjectattr.py
+-rw-rw-rw-   0        0        0      914 2022-01-12 15:01:16.000000 uplogic-1.9.5/uplogic/nodes/actions/setgamma.py
+-rw-rw-rw-   0        0        0     1456 2022-01-12 15:57:52.000000 uplogic-1.9.5/uplogic/nodes/actions/setglobalvalue.py
+-rw-rw-rw-   0        0        0      933 2022-01-12 13:28:24.000000 uplogic-1.9.5/uplogic/nodes/actions/setgravity.py
+-rw-rw-rw-   0        0        0     1012 2022-01-12 15:24:08.000000 uplogic-1.9.5/uplogic/nodes/actions/setlightcolor.py
+-rw-rw-rw-   0        0        0      959 2022-01-12 15:16:33.000000 uplogic-1.9.5/uplogic/nodes/actions/setlightenergy.py
+-rw-rw-rw-   0        0        0      983 2022-01-12 15:19:36.000000 uplogic-1.9.5/uplogic/nodes/actions/setlightshadow.py
+-rw-rw-rw-   0        0        0     1137 2022-01-12 11:56:28.000000 uplogic-1.9.5/uplogic/nodes/actions/setlistindex.py
+-rw-rw-rw-   0        0        0     1321 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setmaterial.py
+-rw-rw-rw-   0        0        0     1412 2022-01-10 12:35:51.000000 uplogic-1.9.5/uplogic/nodes/actions/setmatnodesocket.py
+-rw-rw-rw-   0        0        0     1610 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setmatnodevalue.py
+-rw-rw-rw-   0        0        0     1388 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setnodesocket.py
+-rw-rw-rw-   0        0        0     1622 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setnodevalue.py
+-rw-rw-rw-   0        0        0      863 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setoverlaycollection.py
+-rw-rw-rw-   0        0        0     1188 2022-01-12 12:01:10.000000 uplogic-1.9.5/uplogic/nodes/actions/setparent.py
+-rw-rw-rw-   0        0        0     1188 2022-01-12 16:00:43.000000 uplogic-1.9.5/uplogic/nodes/actions/setphysics.py
+-rw-rw-rw-   0        0        0      838 2022-01-10 18:14:35.000000 uplogic-1.9.5/uplogic/nodes/actions/setprofile.py
+-rw-rw-rw-   0        0        0     1383 2022-10-05 12:35:18.000000 uplogic-1.9.5/uplogic/nodes/actions/setproperty.py
+-rw-rw-rw-   0        0        0      736 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/actions/setpyinstanceattr.py
+-rw-rw-rw-   0        0        0      898 2022-01-23 23:21:22.000000 uplogic-1.9.5/uplogic/nodes/actions/setresolution.py
+-rw-rw-rw-   0        0        0     1085 2022-01-12 13:12:07.000000 uplogic-1.9.5/uplogic/nodes/actions/setrigidbody.py
+-rw-rw-rw-   0        0        0      820 2022-10-04 11:00:44.000000 uplogic-1.9.5/uplogic/nodes/actions/setscene.py
+-rw-rw-rw-   0        0        0     1200 2022-02-04 18:03:35.000000 uplogic-1.9.5/uplogic/nodes/actions/setsensorvalue.py
+-rw-rw-rw-   0        0        0      949 2022-01-12 13:27:30.000000 uplogic-1.9.5/uplogic/nodes/actions/settimescale.py
+-rw-rw-rw-   0        0        0     2417 2023-06-14 11:15:48.000000 uplogic-1.9.5/uplogic/nodes/actions/setuiwidgetattr.py
+-rw-rw-rw-   0        0        0     2913 2022-02-06 12:41:13.000000 uplogic-1.9.5/uplogic/nodes/actions/setvisibility.py
+-rw-rw-rw-   0        0        0      828 2022-01-12 11:22:14.000000 uplogic-1.9.5/uplogic/nodes/actions/setvsync.py
+-rw-rw-rw-   0        0        0      853 2022-01-10 18:19:10.000000 uplogic-1.9.5/uplogic/nodes/actions/showframerate.py
+-rw-rw-rw-   0        0        0     1519 2023-05-14 08:56:41.000000 uplogic-1.9.5/uplogic/nodes/actions/slowfollow.py
+-rw-rw-rw-   0        0        0     3572 2023-05-16 11:15:30.000000 uplogic-1.9.5/uplogic/nodes/actions/spawnpool.py
+-rw-rw-rw-   0        0        0     2051 2023-03-06 08:53:53.000000 uplogic-1.9.5/uplogic/nodes/actions/startsound.py
+-rw-rw-rw-   0        0        0     3107 2023-03-06 08:54:22.000000 uplogic-1.9.5/uplogic/nodes/actions/startsound3d.py
+-rw-rw-rw-   0        0        0     2541 2023-03-06 08:54:22.000000 uplogic-1.9.5/uplogic/nodes/actions/startspeaker.py
+-rw-rw-rw-   0        0        0     1436 2023-05-14 08:57:02.000000 uplogic-1.9.5/uplogic/nodes/actions/startsubnetwork.py
+-rw-rw-rw-   0        0        0     1597 2022-10-07 11:19:16.000000 uplogic-1.9.5/uplogic/nodes/actions/stopaction.py
+-rw-rw-rw-   0        0        0      591 2022-01-12 14:34:57.000000 uplogic-1.9.5/uplogic/nodes/actions/stopallsounds.py
+-rw-rw-rw-   0        0        0      624 2022-01-12 14:28:14.000000 uplogic-1.9.5/uplogic/nodes/actions/stopsound.py
+-rw-rw-rw-   0        0        0     1209 2022-02-07 22:56:33.000000 uplogic-1.9.5/uplogic/nodes/actions/stopsubnetwork.py
+-rw-rw-rw-   0        0        0      842 2022-09-06 10:25:56.000000 uplogic-1.9.5/uplogic/nodes/actions/togglefilter.py
+-rw-rw-rw-   0        0        0     1227 2022-04-09 10:37:36.000000 uplogic-1.9.5/uplogic/nodes/actions/toggleproperty.py
+-rw-rw-rw-   0        0        0     2809 2022-01-12 14:57:52.000000 uplogic-1.9.5/uplogic/nodes/actions/translate.py
+-rw-rw-rw-   0        0        0     1391 2023-05-14 08:57:16.000000 uplogic-1.9.5/uplogic/nodes/actions/vehicleapplybraking.py
+-rw-rw-rw-   0        0        0     1379 2023-05-14 08:57:23.000000 uplogic-1.9.5/uplogic/nodes/actions/vehicleapplyforce.py
+-rw-rw-rw-   0        0        0     1392 2023-05-14 08:57:30.000000 uplogic-1.9.5/uplogic/nodes/actions/vehicleapplysteering.py
+-rw-rw-rw-   0        0        0     3473 2023-05-14 08:57:36.000000 uplogic-1.9.5/uplogic/nodes/actions/vehiclesetattributes.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.316820 uplogic-1.9.5/uplogic/nodes/conditions/
+-rw-rw-rw-   0        0        0     1946 2022-01-20 14:15:37.000000 uplogic-1.9.5/uplogic/nodes/conditions/__init__.py
+-rw-rw-rw-   0        0        0      935 2022-01-12 13:06:20.000000 uplogic-1.9.5/uplogic/nodes/conditions/barrier.py
+-rw-rw-rw-   0        0        0     2397 2023-05-14 08:57:52.000000 uplogic-1.9.5/uplogic/nodes/conditions/checkdistance.py
+-rw-rw-rw-   0        0        0     4852 2023-05-23 10:33:12.000000 uplogic-1.9.5/uplogic/nodes/conditions/collision.py
+-rw-rw-rw-   0        0        0     1508 2023-05-14 08:58:21.000000 uplogic-1.9.5/uplogic/nodes/conditions/compare.py
+-rw-rw-rw-   0        0        0     2175 2023-05-14 08:58:27.000000 uplogic-1.9.5/uplogic/nodes/conditions/comparevectors.py
+-rw-rw-rw-   0        0        0     3288 2022-01-10 17:39:46.000000 uplogic-1.9.5/uplogic/nodes/conditions/controllerstatus.py
+-rw-rw-rw-   0        0        0     1497 2023-05-14 08:58:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/evaluateproperty.py
+-rw-rw-rw-   0        0        0      756 2022-01-28 16:50:48.000000 uplogic-1.9.5/uplogic/nodes/conditions/gamepadactive.py
+-rw-rw-rw-   0        0        0     1503 2023-05-14 08:58:39.000000 uplogic-1.9.5/uplogic/nodes/conditions/gamepadbutton.py
+-rw-rw-rw-   0        0        0     1782 2023-05-14 08:58:43.000000 uplogic-1.9.5/uplogic/nodes/conditions/gamepadbuttonup.py
+-rw-rw-rw-   0        0        0     1093 2023-05-14 08:58:51.000000 uplogic-1.9.5/uplogic/nodes/conditions/handleevent.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 08:58:56.000000 uplogic-1.9.5/uplogic/nodes/conditions/hasproperty.py
+-rw-rw-rw-   0        0        0      303 2021-12-21 09:41:07.000000 uplogic-1.9.5/uplogic/nodes/conditions/keyboardactive.py
+-rw-rw-rw-   0        0        0      812 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/keypressed.py
+-rw-rw-rw-   0        0        0      756 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/keyreleased.py
+-rw-rw-rw-   0        0        0     1705 2022-02-04 11:39:59.000000 uplogic-1.9.5/uplogic/nodes/conditions/logicand.py
+-rw-rw-rw-   0        0        0      621 2022-02-04 11:45:26.000000 uplogic-1.9.5/uplogic/nodes/conditions/logicandnot.py
+-rw-rw-rw-   0        0        0      325 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/logicnone.py
+-rw-rw-rw-   0        0        0      768 2023-05-14 08:59:42.000000 uplogic-1.9.5/uplogic/nodes/conditions/logicnot.py
+-rw-rw-rw-   0        0        0      334 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/logicnotnone.py
+-rw-rw-rw-   0        0        0     1168 2023-05-14 09:15:28.000000 uplogic-1.9.5/uplogic/nodes/conditions/logicor.py
+-rw-rw-rw-   0        0        0     1681 2023-05-14 09:15:55.000000 uplogic-1.9.5/uplogic/nodes/conditions/logictreestatus.py
+-rw-rw-rw-   0        0        0      494 2022-09-11 14:46:42.000000 uplogic-1.9.5/uplogic/nodes/conditions/mousemoved.py
+-rw-rw-rw-   0        0        0     3567 2022-09-11 14:47:44.000000 uplogic-1.9.5/uplogic/nodes/conditions/mouseover.py
+-rw-rw-rw-   0        0        0     1313 2023-05-14 09:00:04.000000 uplogic-1.9.5/uplogic/nodes/conditions/mousepressed.py
+-rw-rw-rw-   0        0        0     1740 2023-05-14 09:00:09.000000 uplogic-1.9.5/uplogic/nodes/conditions/mousepressedon.py
+-rw-rw-rw-   0        0        0     1302 2023-05-14 09:00:16.000000 uplogic-1.9.5/uplogic/nodes/conditions/mousereleased.py
+-rw-rw-rw-   0        0        0      700 2022-09-11 14:54:01.000000 uplogic-1.9.5/uplogic/nodes/conditions/mousescroll.py
+-rw-rw-rw-   0        0        0     1071 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/once.py
+-rw-rw-rw-   0        0        0      358 2023-05-14 09:00:22.000000 uplogic-1.9.5/uplogic/nodes/conditions/oninit.py
+-rw-rw-rw-   0        0        0      704 2023-04-06 11:05:27.000000 uplogic-1.9.5/uplogic/nodes/conditions/onnexttick.py
+-rw-rw-rw-   0        0        0      359 2023-05-14 09:00:29.000000 uplogic-1.9.5/uplogic/nodes/conditions/onupdate.py
+-rw-rw-rw-   0        0        0     1270 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/conditions/onvaluechanged.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 09:00:33.000000 uplogic-1.9.5/uplogic/nodes/conditions/onvaluechangedto.py
+-rw-rw-rw-   0        0        0     1474 2022-05-25 09:41:06.000000 uplogic-1.9.5/uplogic/nodes/conditions/pulsify.py
+-rw-rw-rw-   0        0        0     1105 2023-05-14 09:16:25.000000 uplogic-1.9.5/uplogic/nodes/conditions/sensorpositive.py
+-rw-rw-rw-   0        0        0      940 2022-01-17 10:41:45.000000 uplogic-1.9.5/uplogic/nodes/conditions/timedelay.py
+-rw-rw-rw-   0        0        0      918 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/timer.py
+-rw-rw-rw-   0        0        0      548 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/truefalse.py
+-rw-rw-rw-   0        0        0      377 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/conditions/valuevalid.py
+-rw-rw-rw-   0        0        0     8472 2023-05-19 05:22:01.000000 uplogic-1.9.5/uplogic/nodes/logictree.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.423847 uplogic-1.9.5/uplogic/nodes/parameters/
+-rw-rw-rw-   0        0        0     4767 2023-06-13 19:48:28.000000 uplogic-1.9.5/uplogic/nodes/parameters/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-05-14 09:00:44.000000 uplogic-1.9.5/uplogic/nodes/parameters/absolutevalue.py
+-rw-rw-rw-   0        0        0     1713 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/actionstatus.py
+-rw-rw-rw-   0        0        0      585 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/activecamera.py
+-rw-rw-rw-   0        0        0      909 2023-05-14 09:01:31.000000 uplogic-1.9.5/uplogic/nodes/parameters/axisvector.py
+-rw-rw-rw-   0        0        0     1923 2023-05-14 09:01:36.000000 uplogic-1.9.5/uplogic/nodes/parameters/bonestatus.py
+-rw-rw-rw-   0        0        0     1911 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/parameters/characterinfo.py
+-rw-rw-rw-   0        0        0     1158 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/childbyindex.py
+-rw-rw-rw-   0        0        0      903 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/childbyname.py
+-rw-rw-rw-   0        0        0     1116 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/clamp.py
+-rw-rw-rw-   0        0        0      792 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/colorrgb.py
+-rw-rw-rw-   0        0        0      719 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/parameters/colorrgba.py
+-rw-rw-rw-   0        0        0      911 2022-02-17 16:47:54.000000 uplogic-1.9.5/uplogic/nodes/parameters/dictvalue.py
+-rw-rw-rw-   0        0        0      920 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/distance.py
+-rw-rw-rw-   0        0        0      910 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/parameters/euler.py
+-rw-rw-rw-   0        0        0      786 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/parameters/eulertomatrix.py
+-rw-rw-rw-   0        0        0     1284 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/formattedstring.py
+-rw-rw-rw-   0        0        0     2158 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/parameters/formula.py
+-rw-rw-rw-   0        0        0     1858 2023-07-07 11:36:29.000000 uplogic-1.9.5/uplogic/nodes/parameters/gamepadsticks.py
+-rw-rw-rw-   0        0        0     1563 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/gamepadtrigger.py
+-rw-rw-rw-   0        0        0     1097 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getactuatorvalue.py
+-rw-rw-rw-   0        0        0      612 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getcollection.py
+-rw-rw-rw-   0        0        0     1056 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getcollectionobjectnames.py
+-rw-rw-rw-   0        0        0     1047 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getcollectionobjects.py
+-rw-rw-rw-   0        0        0     1055 2022-01-10 11:25:35.000000 uplogic-1.9.5/uplogic/nodes/parameters/getcurvepoints.py
+-rw-rw-rw-   0        0        0      527 2023-03-02 19:33:55.000000 uplogic-1.9.5/uplogic/nodes/parameters/getfont.py
+-rw-rw-rw-   0        0        0      401 2023-06-07 19:15:13.000000 uplogic-1.9.5/uplogic/nodes/parameters/getfullscreen.py
+-rw-rw-rw-   0        0        0     1100 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getglobalvalue.py
+-rw-rw-rw-   0        0        0      432 2021-12-21 09:41:07.000000 uplogic-1.9.5/uplogic/nodes/parameters/getgravity.py
+-rw-rw-rw-   0        0        0      534 2022-01-10 11:08:34.000000 uplogic-1.9.5/uplogic/nodes/parameters/getimage.py
+-rw-rw-rw-   0        0        0      648 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getlightcolor.py
+-rw-rw-rw-   0        0        0      654 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getlightenergy.py
+-rw-rw-rw-   0        0        0     1420 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getnodeattribute.py
+-rw-rw-rw-   0        0        0     1294 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getnodesocket.py
+-rw-rw-rw-   0        0        0      762 2023-05-16 10:12:45.000000 uplogic-1.9.5/uplogic/nodes/parameters/getobject.py
+-rw-rw-rw-   0        0        0      442 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getowner.py
+-rw-rw-rw-   0        0        0      614 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getparent.py
+-rw-rw-rw-   0        0        0     1080 2023-05-14 16:12:28.000000 uplogic-1.9.5/uplogic/nodes/parameters/getproperty.py
+-rw-rw-rw-   0        0        0      715 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getpyinstanceattr.py
+-rw-rw-rw-   0        0        0      760 2022-01-12 11:11:52.000000 uplogic-1.9.5/uplogic/nodes/parameters/getresolution.py
+-rw-rw-rw-   0        0        0      384 2021-12-21 09:41:07.000000 uplogic-1.9.5/uplogic/nodes/parameters/getscene.py
+-rw-rw-rw-   0        0        0      954 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getsensorvalue.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/getsound.py
+-rw-rw-rw-   0        0        0      385 2021-12-21 09:41:07.000000 uplogic-1.9.5/uplogic/nodes/parameters/gettimescale.py
+-rw-rw-rw-   0        0        0     1070 2023-03-02 22:50:45.000000 uplogic-1.9.5/uplogic/nodes/parameters/getuiwidgetattr.py
+-rw-rw-rw-   0        0        0      381 2023-06-07 19:15:17.000000 uplogic-1.9.5/uplogic/nodes/parameters/getvsync.py
+-rw-rw-rw-   0        0        0      429 2022-01-12 11:37:03.000000 uplogic-1.9.5/uplogic/nodes/parameters/initemptydict.py
+-rw-rw-rw-   0        0        0      599 2022-01-26 18:13:15.000000 uplogic-1.9.5/uplogic/nodes/parameters/initemptylist.py
+-rw-rw-rw-   0        0        0      652 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/initnewdict.py
+-rw-rw-rw-   0        0        0      873 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/interpolate.py
+-rw-rw-rw-   0        0        0      620 2022-01-10 14:18:19.000000 uplogic-1.9.5/uplogic/nodes/parameters/invertvalue.py
+-rw-rw-rw-   0        0        0      316 2022-01-10 11:08:17.000000 uplogic-1.9.5/uplogic/nodes/parameters/keycode.py
+-rw-rw-rw-   0        0        0     1475 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/limitrange.py
+-rw-rw-rw-   0        0        0      620 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/listduplicate.py
+-rw-rw-rw-   0        0        0      823 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/listextend.py
+-rw-rw-rw-   0        0        0      697 2022-12-21 14:09:17.000000 uplogic-1.9.5/uplogic/nodes/parameters/listfromitems.py
+-rw-rw-rw-   0        0        0      827 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/listindex.py
+-rw-rw-rw-   0        0        0      835 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/listindexrandom.py
+-rw-rw-rw-   0        0        0     1951 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/loadvariable.py
+-rw-rw-rw-   0        0        0     1479 2023-02-14 10:12:26.000000 uplogic-1.9.5/uplogic/nodes/parameters/loadvariabledict.py
+-rw-rw-rw-   0        0        0     1432 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/materialgetattribute.py
+-rw-rw-rw-   0        0        0      799 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/materialgetnode.py
+-rw-rw-rw-   0        0        0     1300 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/materialgetsocket.py
+-rw-rw-rw-   0        0        0     2549 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/math.py
+-rw-rw-rw-   0        0        0      672 2022-01-30 10:48:51.000000 uplogic-1.9.5/uplogic/nodes/parameters/matrixtoxyz.py
+-rw-rw-rw-   0        0        0     1278 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/mousedata.py
+-rw-rw-rw-   0        0        0     1197 2023-07-07 13:57:45.000000 uplogic-1.9.5/uplogic/nodes/parameters/objectattr.py
+-rw-rw-rw-   0        0        0      601 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/objectdataname.py
+-rw-rw-rw-   0        0        0     1146 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/objectdatavertices.py
+-rw-rw-rw-   0        0        0     1222 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/randomfloat.py
+-rw-rw-rw-   0        0        0     1167 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/randomint.py
+-rw-rw-rw-   0        0        0      979 2022-01-16 18:24:15.000000 uplogic-1.9.5/uplogic/nodes/parameters/randomvect.py
+-rw-rw-rw-   0        0        0     1032 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/rangedthreshold.py
+-rw-rw-rw-   0        0        0      789 2023-06-13 19:51:24.000000 uplogic-1.9.5/uplogic/nodes/parameters/rebuilddata.py
+-rw-rw-rw-   0        0        0      871 2023-05-14 16:12:38.000000 uplogic-1.9.5/uplogic/nodes/parameters/screenposition.py
+-rw-rw-rw-   0        0        0      829 2023-05-16 09:25:56.000000 uplogic-1.9.5/uplogic/nodes/parameters/serializedata.py
+-rw-rw-rw-   0        0        0      417 2022-01-10 11:08:17.000000 uplogic-1.9.5/uplogic/nodes/parameters/simplevalue.py
+-rw-rw-rw-   0        0        0      775 2023-06-16 18:58:38.000000 uplogic-1.9.5/uplogic/nodes/parameters/storevalue.py
+-rw-rw-rw-   0        0        0     1102 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/threshold.py
+-rw-rw-rw-   0        0        0     1007 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/timedata.py
+-rw-rw-rw-   0        0        0      988 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/typecastvalue.py
+-rw-rw-rw-   0        0        0     4507 2023-05-14 09:01:49.000000 uplogic-1.9.5/uplogic/nodes/parameters/valueswitch.py
+-rw-rw-rw-   0        0        0      751 2023-05-14 16:12:43.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorabsolute.py
+-rw-rw-rw-   0        0        0      886 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorangle.py
+-rw-rw-rw-   0        0        0     1385 2023-05-14 09:01:59.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectoranglecheck.py
+-rw-rw-rw-   0        0        0      646 2023-05-14 16:12:48.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorlength.py
+-rw-rw-rw-   0        0        0     3763 2023-07-07 13:51:11.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectormath.py
+-rw-rw-rw-   0        0        0      717 2022-01-10 11:08:17.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorsplitxy.py
+-rw-rw-rw-   0        0        0     1032 2022-01-30 14:47:33.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorsplitxyz.py
+-rw-rw-rw-   0        0        0      691 2023-03-03 08:53:48.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorxy.py
+-rw-rw-rw-   0        0        0      818 2023-07-07 13:46:43.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorxyz.py
+-rw-rw-rw-   0        0        0      945 2022-01-10 11:08:17.000000 uplogic-1.9.5/uplogic/nodes/parameters/vectorxyzw.py
+-rw-rw-rw-   0        0        0     1378 2023-03-06 09:01:43.000000 uplogic-1.9.5/uplogic/nodes/parameters/vrcontrollervalues.py
+-rw-rw-rw-   0        0        0      583 2023-03-06 09:01:01.000000 uplogic-1.9.5/uplogic/nodes/parameters/vrheadsetvalues.py
+-rw-rw-rw-   0        0        0     1026 2023-05-14 09:01:09.000000 uplogic-1.9.5/uplogic/nodes/parameters/withinrange.py
+-rw-rw-rw-   0        0        0     1293 2023-05-14 16:12:52.000000 uplogic-1.9.5/uplogic/nodes/parameters/worldposition.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.429846 uplogic-1.9.5/uplogic/physics/
+-rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-1.9.5/uplogic/physics/__init__.py
+-rw-rw-rw-   0        0        0     4196 2023-05-14 08:28:32.000000 uplogic-1.9.5/uplogic/physics/buoyancy.py
+-rw-rw-rw-   0        0        0     4099 2023-07-05 14:13:35.000000 uplogic-1.9.5/uplogic/physics/character.py
+-rw-rw-rw-   0        0        0     3450 2023-05-14 08:29:19.000000 uplogic-1.9.5/uplogic/physics/collision.py
+-rw-rw-rw-   0        0        0     8370 2023-05-14 08:38:03.000000 uplogic-1.9.5/uplogic/physics/constraints.py
+-rw-rw-rw-   0        0        0    10072 2023-05-14 08:30:19.000000 uplogic-1.9.5/uplogic/physics/vehicle.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.431856 uplogic-1.9.5/uplogic/serialize/
+-rw-rw-rw-   0        0        0     2945 2023-05-16 08:33:09.000000 uplogic-1.9.5/uplogic/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.450850 uplogic-1.9.5/uplogic/shaders/
+-rw-rw-rw-   0        0        0      675 2023-04-01 06:53:28.000000 uplogic-1.9.5/uplogic/shaders/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-1.9.5/uplogic/shaders/adaptivetonemapping.py
+-rw-rw-rw-   0        0        0     1631 2023-04-01 06:53:32.000000 uplogic-1.9.5/uplogic/shaders/blur.py
+-rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/brightness.py
+-rw-rw-rw-   0        0        0     1050 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/chromaticaberration.py
+-rw-rw-rw-   0        0        0     8869 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/distort.py
+-rw-rw-rw-   0        0        0     9818 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/dof.py
+-rw-rw-rw-   0        0        0     9106 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/droplets.py
+-rw-rw-rw-   0        0        0    33424 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/fxaa.py
+-rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/grayscale.py
+-rw-rw-rw-   0        0        0     9683 2023-07-05 14:45:48.000000 uplogic-1.9.5/uplogic/shaders/hbao.py
+-rw-rw-rw-   0        0        0     1173 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/letterbox.py
+-rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/levels.py
+-rw-rw-rw-   0        0        0     4209 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/mist.py
+-rw-rw-rw-   0        0        0     5411 2023-04-01 07:02:38.000000 uplogic-1.9.5/uplogic/shaders/shader.py
+-rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/sharpen.py
+-rw-rw-rw-   0        0        0     5738 2023-06-20 15:34:55.000000 uplogic-1.9.5/uplogic/shaders/ssao.py
+-rw-rw-rw-   0        0        0     1190 2023-04-01 06:54:25.000000 uplogic-1.9.5/uplogic/shaders/vignette.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.459853 uplogic-1.9.5/uplogic/ui/
+-rw-rw-rw-   0        0        0      367 2023-06-20 17:11:49.000000 uplogic-1.9.5/uplogic/ui/__init__.py
+-rw-rw-rw-   0        0        0      579 2023-04-02 14:03:20.000000 uplogic-1.9.5/uplogic/ui/behaviors.py
+-rw-rw-rw-   0        0        0     5139 2023-06-05 09:06:00.000000 uplogic-1.9.5/uplogic/ui/button.py
+-rw-rw-rw-   0        0        0     1301 2023-06-05 09:06:00.000000 uplogic-1.9.5/uplogic/ui/canvas.py
+-rw-rw-rw-   0        0        0     2438 2023-04-26 12:34:19.000000 uplogic-1.9.5/uplogic/ui/cursor.py
+-rw-rw-rw-   0        0        0     4179 2023-06-26 10:59:15.000000 uplogic-1.9.5/uplogic/ui/image.py
+-rw-rw-rw-   0        0        0     6180 2023-06-05 09:06:00.000000 uplogic-1.9.5/uplogic/ui/label.py
+-rw-rw-rw-   0        0        0     6441 2023-06-14 10:42:03.000000 uplogic-1.9.5/uplogic/ui/layout.py
+-rw-rw-rw-   0        0        0    11258 2023-06-14 10:56:40.000000 uplogic-1.9.5/uplogic/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.472856 uplogic-1.9.5/uplogic/utils/
+-rw-rw-rw-   0        0        0     7036 2023-07-07 10:14:02.000000 uplogic-1.9.5/uplogic/utils/__init__.py
+-rw-rw-rw-   0        0        0     1429 2023-07-05 18:18:21.000000 uplogic-1.9.5/uplogic/utils/constants.py
+-rw-rw-rw-   0        0        0     1089 2023-06-20 14:44:01.000000 uplogic-1.9.5/uplogic/utils/engine.py
+-rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-1.9.5/uplogic/utils/errors.py
+-rw-rw-rw-   0        0        0     7571 2023-06-05 09:06:00.000000 uplogic-1.9.5/uplogic/utils/lights.py
+-rw-rw-rw-   0        0        0     7975 2023-07-05 15:28:25.000000 uplogic-1.9.5/uplogic/utils/math.py
+-rw-rw-rw-   0        0        0     4801 2022-08-22 17:00:51.000000 uplogic-1.9.5/uplogic/utils/nodetrees.py
+-rw-rw-rw-   0        0        0    11155 2023-07-07 11:02:08.000000 uplogic-1.9.5/uplogic/utils/objects.py
+-rw-rw-rw-   0        0        0     6193 2023-07-07 11:33:19.000000 uplogic-1.9.5/uplogic/utils/pooling.py
+-rw-rw-rw-   0        0        0    13346 2023-05-14 16:52:14.000000 uplogic-1.9.5/uplogic/utils/raycasting.py
+-rw-rw-rw-   0        0        0     5831 2022-10-05 11:16:36.000000 uplogic-1.9.5/uplogic/utils/scene.py
+-rw-rw-rw-   0        0        0     2037 2023-06-05 09:06:00.000000 uplogic-1.9.5/uplogic/utils/visuals.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:28.086239 uplogic-1.9.5/uplogic.egg-info/
+-rw-rw-rw-   0        0        0     1049 2023-07-07 13:58:27.000000 uplogic-1.9.5/uplogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13638 2023-07-07 13:58:27.000000 uplogic-1.9.5/uplogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:58:27.000000 uplogic-1.9.5/uplogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-07 13:58:27.000000 uplogic-1.9.5/uplogic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 13:58:27.000000 uplogic-1.9.5/uplogic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-1.9.5/uplogic.egg-info/zip-safe
```

### Comparing `uplogic-1.9.4/PKG-INFO` & `uplogic-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 1.9.4
+Version: 1.9.5
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.4.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.5.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-1.9.4/setup.py` & `uplogic-1.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = 'v1.9.4'
+version = 'v1.9.5'
 shortdesc = "Uplogic utility for UPBGE."
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.md',
     'LICENSE.md'
 ]])
 
 
@@ -27,15 +27,15 @@
         'Topic :: Multimedia :: Graphics',
         'Programming Language :: Python',
     ],
     keywords='Blender UPBGE logic',
     author='Leopold Auersperg-Castell',
     author_email='lauersperg@gmx.at',
     url='https://github.com/UPBGE/uplogic',
-    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.4.tar.gz',
+    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.5.tar.gz',
     license='GPLv2',
     packages=[
         'uplogic',
         'uplogic.animation',
         'uplogic.audio',
         'uplogic.data',
         'uplogic.decorators',
```

### Comparing `uplogic-1.9.4/uplogic/__init__.py` & `uplogic-1.9.5/uplogic/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/animation/action.py` & `uplogic-1.9.5/uplogic/animation/action.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/animation/actionsystem.py` & `uplogic-1.9.5/uplogic/animation/actionsystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/animation/sequence.py` & `uplogic-1.9.5/uplogic/animation/sequence.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/audio/__init__.py` & `uplogic-1.9.5/uplogic/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/audio/audiosystem.py` & `uplogic-1.9.5/uplogic/audio/audiosystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/audio/music.py` & `uplogic-1.9.5/uplogic/audio/music.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/audio/sound.py` & `uplogic-1.9.5/uplogic/audio/sound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/data/__init__.py` & `uplogic-1.9.5/uplogic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/data/file.py` & `uplogic-1.9.5/uplogic/data/file.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/data/globaldb.py` & `uplogic-1.9.5/uplogic/data/globaldb.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/data/serializers.py` & `uplogic-1.9.5/uplogic/data/serializers.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/decorators/__init__.py` & `uplogic-1.9.5/uplogic/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/events/__init__.py` & `uplogic-1.9.5/uplogic/events/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/input/__init__.py` & `uplogic-1.9.5/uplogic/input/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/input/gamepad.py` & `uplogic-1.9.5/uplogic/input/gamepad.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/input/keyboard.py` & `uplogic-1.9.5/uplogic/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/input/mouse.py` & `uplogic-1.9.5/uplogic/input/mouse.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/input/vr.py` & `uplogic-1.9.5/uplogic/input/vr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/logging/__init__.py` & `uplogic-1.9.5/uplogic/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/network/client.py` & `uplogic-1.9.5/uplogic/network/client.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/network/server.py` & `uplogic-1.9.5/uplogic/network/server.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/__init__.py` & `uplogic-1.9.5/uplogic/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/__init__.py` & `uplogic-1.9.5/uplogic/nodes/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/addfilter.py` & `uplogic-1.9.5/uplogic/nodes/actions/addfilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/addobject.py` & `uplogic-1.9.5/uplogic/nodes/actions/addobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/addphysicsconstraint.py` & `uplogic-1.9.5/uplogic/nodes/actions/addphysicsconstraint.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/adduiwidget.py` & `uplogic-1.9.5/uplogic/nodes/actions/adduiwidget.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/alignaxistovector.py` & `uplogic-1.9.5/uplogic/nodes/actions/alignaxistovector.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/appendlistitem.py` & `uplogic-1.9.5/uplogic/nodes/actions/appendlistitem.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/applyforce.py` & `uplogic-1.9.5/uplogic/nodes/actions/applyforce.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/applyimpulse.py` & `uplogic-1.9.5/uplogic/nodes/actions/applyimpulse.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/applymovement.py` & `uplogic-1.9.5/uplogic/nodes/actions/applymovement.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/applyrotation.py` & `uplogic-1.9.5/uplogic/nodes/actions/applyrotation.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/applytorque.py` & `uplogic-1.9.5/uplogic/nodes/actions/applytorque.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/cameraraycast.py` & `uplogic-1.9.5/uplogic/nodes/actions/cameraraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/characterjump.py` & `uplogic-1.9.5/uplogic/nodes/actions/characterjump.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/clampedmodifyproperty.py` & `uplogic-1.9.5/uplogic/nodes/actions/clampedmodifyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/clearvariables.py` & `uplogic-1.9.5/uplogic/nodes/actions/clearvariables.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/copyproperty.py` & `uplogic-1.9.5/uplogic/nodes/actions/copyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/createuibutton.py` & `uplogic-1.9.5/uplogic/nodes/actions/createuibutton.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/createuicanvas.py` & `uplogic-1.9.5/uplogic/nodes/actions/createuicanvas.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/createuiimage.py` & `uplogic-1.9.5/uplogic/nodes/actions/createuiimage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/createuilabel.py` & `uplogic-1.9.5/uplogic/nodes/actions/createuilabel.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/createuilayout.py` & `uplogic-1.9.5/uplogic/nodes/actions/createuilayout.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/createvehicle.py` & `uplogic-1.9.5/uplogic/nodes/actions/createvehicle.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/cursorbehavior.py` & `uplogic-1.9.5/uplogic/nodes/actions/cursorbehavior.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/cursorvisibility.py` & `uplogic-1.9.5/uplogic/nodes/actions/cursorvisibility.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/dispatchevent.py` & `uplogic-1.9.5/uplogic/nodes/actions/dispatchevent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/drawbox.py` & `uplogic-1.9.5/uplogic/nodes/actions/drawbox.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/drawcube.py` & `uplogic-1.9.5/uplogic/nodes/actions/drawcube.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/drawline.py` & `uplogic-1.9.5/uplogic/nodes/actions/drawline.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/editbone.py` & `uplogic-1.9.5/uplogic/nodes/actions/editbone.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/endgame.py` & `uplogic-1.9.5/uplogic/nodes/actions/endgame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/endobject.py` & `uplogic-1.9.5/uplogic/nodes/actions/endobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/executesubnetwork.py` & `uplogic-1.9.5/uplogic/nodes/actions/executesubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/followpath.py` & `uplogic-1.9.5/uplogic/nodes/actions/followpath.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/gamepadlook.py` & `uplogic-1.9.5/uplogic/nodes/actions/gamepadlook.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/gamepadvibration.py` & `uplogic-1.9.5/uplogic/nodes/actions/gamepadvibration.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/getperformanceprofile.py` & `uplogic-1.9.5/uplogic/nodes/actions/getperformanceprofile.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/installsubnetwork.py` & `uplogic-1.9.5/uplogic/nodes/actions/installsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/instream.py` & `uplogic-1.9.5/uplogic/nodes/actions/instream.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/listglobalvalues.py` & `uplogic-1.9.5/uplogic/nodes/actions/listglobalvalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/listvariables.py` & `uplogic-1.9.5/uplogic/nodes/actions/listvariables.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/loadblendfile.py` & `uplogic-1.9.5/uplogic/nodes/actions/loadblendfile.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/loadfilecontent.py` & `uplogic-1.9.5/uplogic/nodes/actions/loadfilecontent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/loadgame.py` & `uplogic-1.9.5/uplogic/nodes/actions/loadgame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/loadscene.py` & `uplogic-1.9.5/uplogic/nodes/actions/loadscene.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/localclient.py` & `uplogic-1.9.5/uplogic/nodes/actions/localclient.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/localserver.py` & `uplogic-1.9.5/uplogic/nodes/actions/localserver.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/makeuniquelight.py` & `uplogic-1.9.5/uplogic/nodes/actions/makeuniquelight.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/modifyproperty.py` & `uplogic-1.9.5/uplogic/nodes/actions/modifyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/mouselook.py` & `uplogic-1.9.5/uplogic/nodes/actions/mouselook.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/mouseraycast.py` & `uplogic-1.9.5/uplogic/nodes/actions/mouseraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/mousesetposition.py` & `uplogic-1.9.5/uplogic/nodes/actions/mousesetposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/moveto.py` & `uplogic-1.9.5/uplogic/nodes/actions/moveto.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/movetowithnavmesh.py` & `uplogic-1.9.5/uplogic/nodes/actions/movetowithnavmesh.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/pausesound.py` & `uplogic-1.9.5/uplogic/nodes/actions/pausesound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/playaction.py` & `uplogic-1.9.5/uplogic/nodes/actions/playaction.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/playsequence.py` & `uplogic-1.9.5/uplogic/nodes/actions/playsequence.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/popdictkey.py` & `uplogic-1.9.5/uplogic/nodes/actions/popdictkey.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/printvalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/printvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/projectileraycast.py` & `uplogic-1.9.5/uplogic/nodes/actions/projectileraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/raycast.py` & `uplogic-1.9.5/uplogic/nodes/actions/raycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removefilter.py` & `uplogic-1.9.5/uplogic/nodes/actions/removefilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removelistindex.py` & `uplogic-1.9.5/uplogic/nodes/actions/removelistindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removelistvalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/removelistvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removeoverlaycollection.py` & `uplogic-1.9.5/uplogic/nodes/actions/removeoverlaycollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removeparent.py` & `uplogic-1.9.5/uplogic/nodes/actions/removeparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removephysicsconstraint.py` & `uplogic-1.9.5/uplogic/nodes/actions/removephysicsconstraint.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/removevariable.py` & `uplogic-1.9.5/uplogic/nodes/actions/removevariable.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/replacemesh.py` & `uplogic-1.9.5/uplogic/nodes/actions/replacemesh.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/restartgame.py` & `uplogic-1.9.5/uplogic/nodes/actions/restartgame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/resumesound.py` & `uplogic-1.9.5/uplogic/nodes/actions/resumesound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/rotateto.py` & `uplogic-1.9.5/uplogic/nodes/actions/rotateto.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/runactuator.py` & `uplogic-1.9.5/uplogic/nodes/actions/runactuator.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/runpython.py` & `uplogic-1.9.5/uplogic/nodes/actions/runpython.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/savegame.py` & `uplogic-1.9.5/uplogic/nodes/actions/savegame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/savevariable.py` & `uplogic-1.9.5/uplogic/nodes/actions/savevariable.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/savevariabledict.py` & `uplogic-1.9.5/uplogic/nodes/actions/savevariabledict.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/sendmessage.py` & `uplogic-1.9.5/uplogic/nodes/actions/sendmessage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/sendnetworkmessage.py` & `uplogic-1.9.5/uplogic/nodes/actions/sendnetworkmessage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setactionframe.py` & `uplogic-1.9.5/uplogic/nodes/actions/setactionframe.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setactuatorvalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/setactuatorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setboneconstraintattr.py` & `uplogic-1.9.5/uplogic/nodes/actions/setboneconstraintattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setboneconstraintinfluence.py` & `uplogic-1.9.5/uplogic/nodes/actions/setboneconstraintinfluence.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setboneconstrainttarget.py` & `uplogic-1.9.5/uplogic/nodes/actions/setboneconstrainttarget.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setboneposition.py` & `uplogic-1.9.5/uplogic/nodes/actions/setboneposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcamera.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcamera.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcamerafov.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcamerafov.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcameraorthoscale.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcameraorthoscale.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcharactergravity.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcharactergravity.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcharacterjumpspeed.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcharacterjumpspeed.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcharactermaxjumps.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcharactermaxjumps.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcharactervelocity.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcharactervelocity.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcharacterwalkdir.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcharacterwalkdir.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcollisiongroup.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcollisiongroup.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcollisionmask.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcollisionmask.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcurvepoints.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcurvepoints.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setcustomcursor.py` & `uplogic-1.9.5/uplogic/nodes/actions/setcustomcursor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setdictkey.py` & `uplogic-1.9.5/uplogic/nodes/actions/setdictkey.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setdynamics.py` & `uplogic-1.9.5/uplogic/nodes/actions/setdynamics.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/seteeveeao.py` & `uplogic-1.9.5/uplogic/nodes/actions/seteeveeao.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/seteeveebloom.py` & `uplogic-1.9.5/uplogic/nodes/actions/seteeveebloom.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/seteeveesmaa.py` & `uplogic-1.9.5/uplogic/nodes/actions/seteeveesmaa.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/seteeveesmaaquality.py` & `uplogic-1.9.5/uplogic/nodes/actions/seteeveesmaaquality.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/seteeveessr.py` & `uplogic-1.9.5/uplogic/nodes/actions/seteeveessr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/seteeveevolumetrics.py` & `uplogic-1.9.5/uplogic/nodes/actions/seteeveevolumetrics.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setexposure.py` & `uplogic-1.9.5/uplogic/nodes/actions/setexposure.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setfilterstate.py` & `uplogic-1.9.5/uplogic/nodes/actions/setfilterstate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setfullscreen.py` & `uplogic-1.9.5/uplogic/nodes/actions/setfullscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setgameobjectattr.py` & `uplogic-1.9.5/uplogic/nodes/actions/setgameobjectattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setgamma.py` & `uplogic-1.9.5/uplogic/nodes/actions/setgamma.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setglobalvalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/setglobalvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setgravity.py` & `uplogic-1.9.5/uplogic/nodes/actions/setgravity.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setlightcolor.py` & `uplogic-1.9.5/uplogic/nodes/actions/setlightcolor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setlightenergy.py` & `uplogic-1.9.5/uplogic/nodes/actions/setlightenergy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setlightshadow.py` & `uplogic-1.9.5/uplogic/nodes/actions/setlightshadow.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setlistindex.py` & `uplogic-1.9.5/uplogic/nodes/actions/setlistindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setmaterial.py` & `uplogic-1.9.5/uplogic/nodes/actions/setmaterial.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setmatnodesocket.py` & `uplogic-1.9.5/uplogic/nodes/actions/setmatnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setmatnodevalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/setmatnodevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setnodesocket.py` & `uplogic-1.9.5/uplogic/nodes/actions/setnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setnodevalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/setnodevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setoverlaycollection.py` & `uplogic-1.9.5/uplogic/nodes/actions/setoverlaycollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setparent.py` & `uplogic-1.9.5/uplogic/nodes/actions/setparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setphysics.py` & `uplogic-1.9.5/uplogic/nodes/actions/setphysics.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setprofile.py` & `uplogic-1.9.5/uplogic/nodes/actions/setprofile.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setproperty.py` & `uplogic-1.9.5/uplogic/nodes/actions/setproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setpyinstanceattr.py` & `uplogic-1.9.5/uplogic/nodes/actions/setpyinstanceattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setresolution.py` & `uplogic-1.9.5/uplogic/nodes/actions/setresolution.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setrigidbody.py` & `uplogic-1.9.5/uplogic/nodes/actions/setrigidbody.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setscene.py` & `uplogic-1.9.5/uplogic/nodes/actions/setscene.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setsensorvalue.py` & `uplogic-1.9.5/uplogic/nodes/actions/setsensorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/settimescale.py` & `uplogic-1.9.5/uplogic/nodes/actions/settimescale.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setuiwidgetattr.py` & `uplogic-1.9.5/uplogic/nodes/actions/setuiwidgetattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setvisibility.py` & `uplogic-1.9.5/uplogic/nodes/actions/setvisibility.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/setvsync.py` & `uplogic-1.9.5/uplogic/nodes/actions/setvsync.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/showframerate.py` & `uplogic-1.9.5/uplogic/nodes/actions/showframerate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/slowfollow.py` & `uplogic-1.9.5/uplogic/nodes/actions/slowfollow.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/spawnpool.py` & `uplogic-1.9.5/uplogic/nodes/actions/spawnpool.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/startsound.py` & `uplogic-1.9.5/uplogic/nodes/actions/startsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/startsound3d.py` & `uplogic-1.9.5/uplogic/nodes/actions/startsound3d.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/startspeaker.py` & `uplogic-1.9.5/uplogic/nodes/actions/startspeaker.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/startsubnetwork.py` & `uplogic-1.9.5/uplogic/nodes/actions/startsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/stopaction.py` & `uplogic-1.9.5/uplogic/nodes/actions/stopaction.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/stopallsounds.py` & `uplogic-1.9.5/uplogic/nodes/actions/stopallsounds.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/stopsound.py` & `uplogic-1.9.5/uplogic/nodes/actions/stopsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/stopsubnetwork.py` & `uplogic-1.9.5/uplogic/nodes/actions/stopsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/togglefilter.py` & `uplogic-1.9.5/uplogic/nodes/actions/togglefilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/toggleproperty.py` & `uplogic-1.9.5/uplogic/nodes/actions/toggleproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/translate.py` & `uplogic-1.9.5/uplogic/nodes/actions/translate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/vehicleapplybraking.py` & `uplogic-1.9.5/uplogic/nodes/actions/vehicleapplybraking.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/vehicleapplyforce.py` & `uplogic-1.9.5/uplogic/nodes/actions/vehicleapplyforce.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/vehicleapplysteering.py` & `uplogic-1.9.5/uplogic/nodes/actions/vehicleapplysteering.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/actions/vehiclesetattributes.py` & `uplogic-1.9.5/uplogic/nodes/actions/vehiclesetattributes.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/__init__.py` & `uplogic-1.9.5/uplogic/nodes/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/barrier.py` & `uplogic-1.9.5/uplogic/nodes/conditions/barrier.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/checkdistance.py` & `uplogic-1.9.5/uplogic/nodes/conditions/checkdistance.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/collision.py` & `uplogic-1.9.5/uplogic/nodes/conditions/collision.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/compare.py` & `uplogic-1.9.5/uplogic/nodes/conditions/compare.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/comparevectors.py` & `uplogic-1.9.5/uplogic/nodes/conditions/comparevectors.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/controllerstatus.py` & `uplogic-1.9.5/uplogic/nodes/conditions/controllerstatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/evaluateproperty.py` & `uplogic-1.9.5/uplogic/nodes/conditions/evaluateproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/gamepadactive.py` & `uplogic-1.9.5/uplogic/nodes/conditions/gamepadactive.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/gamepadbutton.py` & `uplogic-1.9.5/uplogic/nodes/conditions/gamepadbutton.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/gamepadbuttonup.py` & `uplogic-1.9.5/uplogic/nodes/conditions/gamepadbuttonup.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/handleevent.py` & `uplogic-1.9.5/uplogic/nodes/conditions/handleevent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/hasproperty.py` & `uplogic-1.9.5/uplogic/nodes/conditions/hasproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/keypressed.py` & `uplogic-1.9.5/uplogic/nodes/conditions/keypressed.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/keyreleased.py` & `uplogic-1.9.5/uplogic/nodes/conditions/keyreleased.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/logicand.py` & `uplogic-1.9.5/uplogic/nodes/conditions/logicand.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/logicandnot.py` & `uplogic-1.9.5/uplogic/nodes/conditions/logicandnot.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/logicnot.py` & `uplogic-1.9.5/uplogic/nodes/conditions/logicnot.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/logicor.py` & `uplogic-1.9.5/uplogic/nodes/conditions/logicor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/logictreestatus.py` & `uplogic-1.9.5/uplogic/nodes/conditions/logictreestatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/mouseover.py` & `uplogic-1.9.5/uplogic/nodes/conditions/mouseover.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/mousepressed.py` & `uplogic-1.9.5/uplogic/nodes/conditions/mousepressed.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/mousepressedon.py` & `uplogic-1.9.5/uplogic/nodes/conditions/mousepressedon.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/mousereleased.py` & `uplogic-1.9.5/uplogic/nodes/conditions/mousereleased.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/mousescroll.py` & `uplogic-1.9.5/uplogic/nodes/conditions/mousescroll.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/once.py` & `uplogic-1.9.5/uplogic/nodes/conditions/once.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/onnexttick.py` & `uplogic-1.9.5/uplogic/nodes/conditions/onnexttick.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/onvaluechanged.py` & `uplogic-1.9.5/uplogic/nodes/conditions/onvaluechanged.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/onvaluechangedto.py` & `uplogic-1.9.5/uplogic/nodes/conditions/onvaluechangedto.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/pulsify.py` & `uplogic-1.9.5/uplogic/nodes/conditions/pulsify.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/sensorpositive.py` & `uplogic-1.9.5/uplogic/nodes/conditions/sensorpositive.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/timedelay.py` & `uplogic-1.9.5/uplogic/nodes/conditions/timedelay.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/timer.py` & `uplogic-1.9.5/uplogic/nodes/conditions/timer.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/conditions/truefalse.py` & `uplogic-1.9.5/uplogic/nodes/conditions/truefalse.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/logictree.py` & `uplogic-1.9.5/uplogic/nodes/logictree.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/__init__.py` & `uplogic-1.9.5/uplogic/nodes/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/absolutevalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/absolutevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/actionstatus.py` & `uplogic-1.9.5/uplogic/nodes/parameters/actionstatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/activecamera.py` & `uplogic-1.9.5/uplogic/nodes/parameters/activecamera.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/axisvector.py` & `uplogic-1.9.5/uplogic/nodes/parameters/axisvector.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/bonestatus.py` & `uplogic-1.9.5/uplogic/nodes/parameters/bonestatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/characterinfo.py` & `uplogic-1.9.5/uplogic/nodes/parameters/characterinfo.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/childbyindex.py` & `uplogic-1.9.5/uplogic/nodes/parameters/childbyindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/childbyname.py` & `uplogic-1.9.5/uplogic/nodes/parameters/childbyname.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/clamp.py` & `uplogic-1.9.5/uplogic/nodes/parameters/clamp.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/colorrgb.py` & `uplogic-1.9.5/uplogic/nodes/parameters/colorrgb.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/colorrgba.py` & `uplogic-1.9.5/uplogic/nodes/parameters/colorrgba.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/dictvalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/dictvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/distance.py` & `uplogic-1.9.5/uplogic/nodes/parameters/distance.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/euler.py` & `uplogic-1.9.5/uplogic/nodes/parameters/euler.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/eulertomatrix.py` & `uplogic-1.9.5/uplogic/nodes/parameters/eulertomatrix.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/formattedstring.py` & `uplogic-1.9.5/uplogic/nodes/parameters/formattedstring.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/formula.py` & `uplogic-1.9.5/uplogic/nodes/parameters/formula.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/gamepadsticks.py` & `uplogic-1.9.5/uplogic/nodes/parameters/gamepadsticks.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/gamepadtrigger.py` & `uplogic-1.9.5/uplogic/nodes/parameters/gamepadtrigger.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getactuatorvalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getactuatorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getcollection.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getcollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getcollectionobjectnames.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getcollectionobjectnames.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getcollectionobjects.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getcollectionobjects.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getcurvepoints.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getcurvepoints.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getfont.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getfont.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getglobalvalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getglobalvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getimage.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getimage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getlightcolor.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getlightcolor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getlightenergy.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getlightenergy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getnodeattribute.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getnodeattribute.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getnodesocket.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getobject.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getparent.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getproperty.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getpyinstanceattr.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getpyinstanceattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getresolution.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getresolution.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getsensorvalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getsensorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getsound.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/getuiwidgetattr.py` & `uplogic-1.9.5/uplogic/nodes/parameters/getuiwidgetattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/initemptylist.py` & `uplogic-1.9.5/uplogic/nodes/parameters/initemptylist.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/initnewdict.py` & `uplogic-1.9.5/uplogic/nodes/parameters/initnewdict.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/interpolate.py` & `uplogic-1.9.5/uplogic/nodes/parameters/interpolate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/invertvalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/invertvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/limitrange.py` & `uplogic-1.9.5/uplogic/nodes/parameters/limitrange.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/listduplicate.py` & `uplogic-1.9.5/uplogic/nodes/parameters/listduplicate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/listextend.py` & `uplogic-1.9.5/uplogic/nodes/parameters/listextend.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/listfromitems.py` & `uplogic-1.9.5/uplogic/nodes/parameters/listfromitems.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/listindex.py` & `uplogic-1.9.5/uplogic/nodes/parameters/listindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/listindexrandom.py` & `uplogic-1.9.5/uplogic/nodes/parameters/listindexrandom.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/loadvariable.py` & `uplogic-1.9.5/uplogic/nodes/parameters/loadvariable.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/loadvariabledict.py` & `uplogic-1.9.5/uplogic/nodes/parameters/loadvariabledict.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/materialgetattribute.py` & `uplogic-1.9.5/uplogic/nodes/parameters/materialgetattribute.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/materialgetnode.py` & `uplogic-1.9.5/uplogic/nodes/parameters/materialgetnode.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/materialgetsocket.py` & `uplogic-1.9.5/uplogic/nodes/parameters/materialgetsocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/math.py` & `uplogic-1.9.5/uplogic/nodes/parameters/math.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/matrixtoxyz.py` & `uplogic-1.9.5/uplogic/nodes/parameters/matrixtoxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/mousedata.py` & `uplogic-1.9.5/uplogic/nodes/parameters/mousedata.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/objectattr.py` & `uplogic-1.9.5/uplogic/nodes/parameters/objectattr.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class ULObjectAttribute(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
         self.attribute_name = None
+        self.OUT = ULOutSocket(self, self.get_done)
         self.VAL = ULOutSocket(self, self.get_done)
         self.VEC = ULOutSocket(self, self.get_done)
         self.BOOL = ULOutSocket(self, self.get_done)
 
     def get_done(self):
         game_object = self.get_input(self.game_object)
         attribute_name = self.get_input(self.attribute_name)
```

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/objectdataname.py` & `uplogic-1.9.5/uplogic/nodes/parameters/objectdataname.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/objectdatavertices.py` & `uplogic-1.9.5/uplogic/nodes/parameters/objectdatavertices.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/randomfloat.py` & `uplogic-1.9.5/uplogic/nodes/parameters/randomfloat.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/randomint.py` & `uplogic-1.9.5/uplogic/nodes/parameters/randomint.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/randomvect.py` & `uplogic-1.9.5/uplogic/nodes/parameters/randomvect.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/rangedthreshold.py` & `uplogic-1.9.5/uplogic/nodes/parameters/rangedthreshold.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/rebuilddata.py` & `uplogic-1.9.5/uplogic/nodes/parameters/rebuilddata.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/screenposition.py` & `uplogic-1.9.5/uplogic/nodes/parameters/screenposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/serializedata.py` & `uplogic-1.9.5/uplogic/nodes/parameters/serializedata.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/storevalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/storevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/threshold.py` & `uplogic-1.9.5/uplogic/nodes/parameters/threshold.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/timedata.py` & `uplogic-1.9.5/uplogic/nodes/parameters/timedata.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/typecastvalue.py` & `uplogic-1.9.5/uplogic/nodes/parameters/typecastvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/valueswitch.py` & `uplogic-1.9.5/uplogic/nodes/parameters/valueswitch.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorabsolute.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorabsolute.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorangle.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorangle.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectoranglecheck.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectoranglecheck.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorlength.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorlength.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectormath.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectormath.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             'multadd': self.get_multadd,
             'divide': self.get_divide,
             'multiply': self.get_multiply,
             'subtract': self.get_subtract,
             'add': self.get_add,
             'normalize': self.get_normalize,
             'lerp': self.get_lerp,
+            'slerp': self.get_slerp,
             'negate': self.get_negate,
         }
         if vector:
             vector = vector.copy()
         if vector_2:
             vector_2 = vector_2.copy()
         if vector_3:
@@ -108,10 +109,13 @@
 
     def get_normalize(self, vec, vec2, vec3, fac, scale):
         return vec.normalized()
 
     def get_lerp(self, vec, vec2, vec3, fac, scale):
         return vec.lerp(vec2, fac)
 
+    def get_slerp(self, vec, vec2, vec3, fac, scale):
+        return vec.slerp(vec2, fac, vec3)
+
     def get_negate(self, vec, vec2, vec3, fac, scale):
         vec.negate()
         return vec
```

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorsplitxy.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorsplitxy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorsplitxyz.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorsplitxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorxy.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorxy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorxyz.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vectorxyzw.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vectorxyzw.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vrcontrollervalues.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vrcontrollervalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/vrheadsetvalues.py` & `uplogic-1.9.5/uplogic/nodes/parameters/vrheadsetvalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/withinrange.py` & `uplogic-1.9.5/uplogic/nodes/parameters/withinrange.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/nodes/parameters/worldposition.py` & `uplogic-1.9.5/uplogic/nodes/parameters/worldposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/physics/__init__.py` & `uplogic-1.9.5/uplogic/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/physics/buoyancy.py` & `uplogic-1.9.5/uplogic/physics/buoyancy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/physics/character.py` & `uplogic-1.9.5/uplogic/physics/character.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/physics/collision.py` & `uplogic-1.9.5/uplogic/physics/collision.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/physics/constraints.py` & `uplogic-1.9.5/uplogic/physics/constraints.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/physics/vehicle.py` & `uplogic-1.9.5/uplogic/physics/vehicle.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/serialize/__init__.py` & `uplogic-1.9.5/uplogic/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/__init__.py` & `uplogic-1.9.5/uplogic/shaders/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/adaptivetonemapping.py` & `uplogic-1.9.5/uplogic/shaders/adaptivetonemapping.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/blur.py` & `uplogic-1.9.5/uplogic/shaders/blur.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/brightness.py` & `uplogic-1.9.5/uplogic/shaders/brightness.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/chromaticaberration.py` & `uplogic-1.9.5/uplogic/shaders/chromaticaberration.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/distort.py` & `uplogic-1.9.5/uplogic/shaders/distort.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/dof.py` & `uplogic-1.9.5/uplogic/shaders/dof.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/droplets.py` & `uplogic-1.9.5/uplogic/shaders/droplets.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/fxaa.py` & `uplogic-1.9.5/uplogic/shaders/fxaa.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/grayscale.py` & `uplogic-1.9.5/uplogic/shaders/grayscale.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/hbao.py` & `uplogic-1.9.5/uplogic/shaders/hbao.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/letterbox.py` & `uplogic-1.9.5/uplogic/shaders/letterbox.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/levels.py` & `uplogic-1.9.5/uplogic/shaders/levels.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/mist.py` & `uplogic-1.9.5/uplogic/shaders/mist.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/shader.py` & `uplogic-1.9.5/uplogic/shaders/shader.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/sharpen.py` & `uplogic-1.9.5/uplogic/shaders/sharpen.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/ssao.py` & `uplogic-1.9.5/uplogic/shaders/ssao.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/shaders/vignette.py` & `uplogic-1.9.5/uplogic/shaders/vignette.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/behaviors.py` & `uplogic-1.9.5/uplogic/ui/behaviors.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/button.py` & `uplogic-1.9.5/uplogic/ui/button.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/canvas.py` & `uplogic-1.9.5/uplogic/ui/canvas.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/cursor.py` & `uplogic-1.9.5/uplogic/ui/cursor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/image.py` & `uplogic-1.9.5/uplogic/ui/image.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/label.py` & `uplogic-1.9.5/uplogic/ui/label.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/layout.py` & `uplogic-1.9.5/uplogic/ui/layout.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/ui/widget.py` & `uplogic-1.9.5/uplogic/ui/widget.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/__init__.py` & `uplogic-1.9.5/uplogic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/constants.py` & `uplogic-1.9.5/uplogic/utils/constants.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/engine.py` & `uplogic-1.9.5/uplogic/utils/engine.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/errors.py` & `uplogic-1.9.5/uplogic/utils/errors.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/lights.py` & `uplogic-1.9.5/uplogic/utils/lights.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/math.py` & `uplogic-1.9.5/uplogic/utils/math.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/nodetrees.py` & `uplogic-1.9.5/uplogic/utils/nodetrees.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/objects.py` & `uplogic-1.9.5/uplogic/utils/objects.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/pooling.py` & `uplogic-1.9.5/uplogic/utils/pooling.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/raycasting.py` & `uplogic-1.9.5/uplogic/utils/raycasting.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/scene.py` & `uplogic-1.9.5/uplogic/utils/scene.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic/utils/visuals.py` & `uplogic-1.9.5/uplogic/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.9.4/uplogic.egg-info/PKG-INFO` & `uplogic-1.9.5/uplogic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 1.9.4
+Version: 1.9.5
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.4.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.5.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-1.9.4/uplogic.egg-info/SOURCES.txt` & `uplogic-1.9.5/uplogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

