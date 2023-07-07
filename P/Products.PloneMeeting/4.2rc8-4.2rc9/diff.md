# Comparing `tmp/Products.PloneMeeting-4.2rc8.tar.gz` & `tmp/Products.PloneMeeting-4.2rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.PloneMeeting-4.2rc8.tar", last modified: Thu Feb  3 10:25:46 2022, max compression
+gzip compressed data, was "dist/Products.PloneMeeting-4.2rc9.tar", last modified: Fri Feb  4 08:36:18 2022, max compression
```

## Comparing `Products.PloneMeeting-4.2rc8.tar` & `Products.PloneMeeting-4.2rc9.tar`

### file list

```diff
@@ -1,694 +1,694 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   271060 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43066 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      894 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       62 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/README.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20188 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingGroup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17310 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/indexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10327 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/events.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28941 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      525 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiling.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5360 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/etags.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/exportimport/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43705 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/exportimport/content.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/exportimport/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    74540 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16093 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeetingpopups.js
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    34772 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.js
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/prevalidate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      296 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new_greyed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      212 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/gotoItem.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      585 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      824 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/refused.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/propose.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      373 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/takenOverByNobody.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      642 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/save.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingFileType.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemfrozen_from_returned_to_proposing_group.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      275 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/copy_icon.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      675 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/see_everything.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/documentviewer_convert.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      212 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/arrowLeftDouble.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      239 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/delete_small.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      459 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_public.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      185 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_inherited.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      826 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussNo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialYes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      911 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_disabled_big.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      635 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/questionMark.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemRed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/departure.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      191 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/late.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      671 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/oralQuestion.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      626 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      641 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_accepted.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel4_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_refused.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemCreated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      433 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/takenOverByCurrentUser.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      628 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_comments.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      435 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/reorder.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      372 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/eye.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      837 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_prevalidated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new_meetingadvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/PodTemplate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/rename_icon.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       90 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/refresh.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      520 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemGreen.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      484 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemYellow.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/meetingcategory.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      607 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/videoconference.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2898 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/drop_down.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel5.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel1_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      896 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      373 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new_multiple.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      626 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      496 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemAzur.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      836 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedNo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      958 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      604 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/yes.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1023 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/Meeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      431 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/annexToPrintYes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      158 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/changes.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/back_to.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      893 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/return_to_proposing_group.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToCreated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      285 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/duplicate_and_keep_link.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      681 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/cloned_and_decided.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1715 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/sprites.zip
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      484 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemPurple.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/postponed_next_meeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      501 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency_secret.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      461 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItem.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1881 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm-contenttypes-sprite.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemcreated_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      824 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/refuse.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/arrowSeveral.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      983 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/switch_not_allowed.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      306 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      374 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      195 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/errored_conversion.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      426 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/takenOverByOtherUser.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1185 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      558 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again_back_to_previous.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel5.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_prevalidated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      836 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itempublish.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel5.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemGrey.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new_from_greyed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/plus.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      550 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret_heading.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingGroup.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      763 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/help.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      170 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/night.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedYes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2141 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/save_and_exit.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingUser.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposed_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel4.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      691 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialNo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToAccepted.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3229 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wf_up.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accepted_but_modified.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingFile.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/blue_arrow.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemPublished.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from_prevalidated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      284 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/search_button_icon.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      345 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm_preferences.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      904 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_orange.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/marked_not_applicable.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_cautious.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      973 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/manage.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       85 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pixel.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      614 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/group_users.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      229 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/delay.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      588 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/more_less_details.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      212 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/arrowRightDouble.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1121 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/users.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      791 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_red.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      451 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/budgetRelatedNo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       66 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/checked.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      203 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      381 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new_from.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/arrowLeftSimple.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3211 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from_itemcreated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      921 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_green.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/mark_not_applicable.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_validated_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemPink.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      813 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel5.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      304 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_up_from.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      511 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/store_as_annex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      550 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel2_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm_home.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToPublished.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      480 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/ploneMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/delete_grey_icon.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      323 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingConfig.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      401 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      715 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      386 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/greyedMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      442 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemOrange.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      813 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel5.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/confirm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept_but_modify.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      350 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/annexToPrintNo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      264 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/removeSeveral.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      719 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/funnel.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      858 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_presented_from_returned_to_proposing_group.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      401 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_enable_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      746 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting_emergency.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItem.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      422 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_considered_not_given_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToPrevalidated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel4.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      896 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      526 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public_heading.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/validate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      822 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel4.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      858 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/linkOpaqueDisabled.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itempublished_from_returned_to_proposing_group.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      522 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1765 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_manage.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1145 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_not_given.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_down_from.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_proposed_from_returned_to_proposing_group_prevalidated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      206 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/present.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/postpone_next_meeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/collapseDescrs.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/switch.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      241 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/deadlineKo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      391 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/cloned_not_decided.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_asked.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToClosed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      837 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      558 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again_back_to_previous.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      868 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm_config.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      823 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      755 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      822 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel4.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      776 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      278 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_inherited_remove.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/delete_many.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      268 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/annexToPrintDisabled.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeetingEmergency.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/arrowRightSimple.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel5_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      892 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_reinit_delay.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/manage_annexes.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      526 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel4.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       76 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/leaving.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      367 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/select_items.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      422 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_considered_not_given_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pre_accept.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemFrozen.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/new_meetingadvicefinances.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      620 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_comments.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/cancel_edit.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pre_accepted.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/remove.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1003 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/sendMail.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToDecided.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      280 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemBlack.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4172 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/gotoItemInMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/ToolPloneMeeting.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/removed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel4.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      837 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_prevalidated_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3160 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wf_down.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      229 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/delayed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      525 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/meetingadvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      397 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_disable_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public_heading.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      229 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/presentSeveral.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      628 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussYes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      397 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_disable_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      506 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency_public.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from_proposed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      461 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_not_asked.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/entrance.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel5.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      522 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret_heading.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/budgetRelatedYes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      110 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/expandDescrs.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/acceptable_out_of_meeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      459 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_secret.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel3_from_waiting_advices.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      151 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/view.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      686 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/extraordinarySession.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      323 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/ToolPloneMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToPresented.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      941 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pb_close_small.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1145 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_not_given.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itemfreeze.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/gotoMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      214 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/to.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      401 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_enable_hidden_during_redaction.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_cautious.png
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4924 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/base_edit.cpt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6773 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/livesearch_reply.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3116 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_multiselect_cell.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/base_edit.cpt.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13065 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/versions_history_form.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      359 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/login_success.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      765 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/displayContentsTab.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1780 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_checkbox_cell.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7442 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_edit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    75572 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingconfig_view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    39581 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22614 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meeting_edit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12450 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/toolplonemeeting_view.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4016 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/overrides.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2604 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      428 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/adapters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3238 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      554 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      321 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4249 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/plugin.js
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/lang/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/lang/fr.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      293 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/lang/en.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      291 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/lang/et.js
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      288 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/rotate-right.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      295 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/rotate-left.png
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      525 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-right.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      527 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-left.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       86 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/README.md
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10518 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/monkey.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2095 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MIGRATE_TO_DX.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4100 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/maintenance.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26441 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    93405 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/adapters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   367051 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingConfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19282 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/columns.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3241 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/advice.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1272 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7701 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/meeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    98890 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/Meeting.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      172 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      674 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/organizations.csv
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17124 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/Import_contacts.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1074 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/persons.csv
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      581 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/decision.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11274 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/SignatureCadranel.jpg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      574 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/deliberation_signed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/deliberation_to_sign.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      910 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/person1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1394 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/heldpositions.csv
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9587 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/all_item.odt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    81373 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Agenda.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12815 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/styles2.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11290 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/styles1.odt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    26260 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Decisions.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11422 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Dashboard.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12170 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/organizations-export.ods
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    25537 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Item.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/PloneMeeting_testing_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      325 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23960 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/import_data.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      280 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1745 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10090 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1901 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/propertiestool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1748 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/viewlets.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meetingitem_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22920 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meetingitem_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meeting_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13299 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meeting_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_onestate_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3905 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_onestate_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6694 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_managers_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5839 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_managers_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meetingadvice_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5447 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meetingadvice_workflow/definition.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      289 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/factorytool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/PloneMeeting_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1409 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1148 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/skins.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      333 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ContentCategoryGroup.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      319 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/person.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      521 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/held_position.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      402 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/directory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2226 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/meetingcategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4095 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/annexDecision.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      507 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      258 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ContentCategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      264 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ContentSubcategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3653 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/Meeting.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2335 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/annex.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/organization.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2328 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingItemTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      238 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/Topic.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingConfig.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1900 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ToolPloneMeeting.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2977 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingItem.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2329 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingItemRecurring.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1080 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/DashboardPODTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2452 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ConfigurablePODTemplate.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2664 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/meetingadvice.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3935 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentSubcategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3963 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentCategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14365 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1175 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/portal_atct.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1723 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1208 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/portlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      379 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/repositorytool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6680 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/actions.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17802 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1074 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      242 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      734 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/controlpanel.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3219 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    41569 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2777 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/testing.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14141 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/advice.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2360 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16015 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/held_position.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2954 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/directory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1757 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/person.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15227 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/organization.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    99383 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/meeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1462 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/source.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8559 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/category.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18726 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingUser.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      807 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/LICENSE.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/documentgenerator/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      828 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/documentgenerator/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/documentgenerator/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1927 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/documentgenerator/condition.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2355 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/LICENSE.ZPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   365886 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingItem.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/filters/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1629 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/filters/remove_highlight.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      444 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/filters/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/filters/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30479 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    79226 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ToolPloneMeeting.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/behaviors/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      788 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/behaviors/overrides.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/behaviors/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   100250 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12974 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/validators.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    53382 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/adaptations.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      159 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/generate.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       33 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3050 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/generate.conf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    76464 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/PloneMeeting.zargo
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      672 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_selectreadonly.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_number_input.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      663 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_orderedselect.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1134 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_checkbox.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2658 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/orderedselect_hidden.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1649 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/datagridfield_display.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      962 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_orderedselect_display.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1338 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_selectreadonly_input.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2063 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_richtext_fastedit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      893 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_number.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5261 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_checkbox_input.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1725 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_textarea.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_checkbox_display.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4248 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_richtext.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2239 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_richtext_display.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    17100 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10054 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/vocabularies.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    67025 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12282 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/LICENSE.GPL
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/refresh.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      142 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   115684 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/vocabularies.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/Extensions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/Extensions/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24423 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/Extensions/imports.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12360 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingCategory.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1127 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/default_dashboard_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3878 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/default_dashboard_meetings_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      647 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_meeting_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4413 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_item_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1886 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_update_meeting_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1763 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_4104_add_item_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24435 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_add_item_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26106 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/default_dashboard_items_widgets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1344 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/README.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    40550 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testFaceted.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35265 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testVotes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   221573 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testAdvices.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11905 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeetingCategory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      974 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/events.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33584 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/PloneMeetingTestCase.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   123029 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testContacts.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4747 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_unconvertableFormat.eml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34521 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testChangeItemOrderView.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10823 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testUtils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1207 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/keywords.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      687 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/doc-fr.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/views.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16961 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testColumns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13542 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testSetup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/FILE.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    71364 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testToolPloneMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    50761 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testWorkflows.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9137 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_correct2.pdf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42599 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_errorDuringConversion.pdf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26396 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/helpers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      873 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/dot.gif
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)   430590 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeetingItem.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   130280 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testWFAdaptations.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       44 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/annex_not_to_index.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1257 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15612 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testValidators.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8855 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testPortlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    88619 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testAnnexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    41996 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testPerformances.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1074 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/test_robot.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   200722 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6851 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_correct.pdf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    68351 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testSearches.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   139589 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testViews.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   131654 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeetingConfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12487 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tool.gif
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3412 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3834 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemlisttype.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22862 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemvotes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4377 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itempolltype.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   119942 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    70688 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/overrides.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6759 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/portlet_todo.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    51019 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18825 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemassembly.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4664 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/advicecomment.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      353 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/macros.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1269 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/redirect.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14856 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/advicechangedelay.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7023 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itememergency.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4934 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/viewlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5423 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/adviceinheritance.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19003 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemchangeorder.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2963 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/jsvariables.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8555 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemtemplates.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21907 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/advices.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24159 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/async.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      450 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/notify.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10533 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/annexes.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1557 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_annexes.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5538 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/ramcache.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2601 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advicedelays.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1251 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemtemplates_tree_recurse.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3161 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/item_navigation_widget.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    57285 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/macros.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4985 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advices-icons.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2002 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemissigned.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      902 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/viewlet_held_position_back_refs.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      369 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_assembly_from_meeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2588 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemtemplates.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      635 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemcompleteness.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itememergency.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10936 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1842 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemnumber.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3171 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/generationlinks.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      955 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advice_version_preview.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9342 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meetingassemblyandsignatures.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3329 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/imgselectbox.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1221 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/actions_panel_deletewholemeeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34761 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advices-icons-infos.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2100 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemstaticinfos.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1646 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/term_searchmeetings.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1165 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemlisttype.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      550 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/actions_panel_config_viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2748 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/category_meetingitems.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5021 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meetingadvice.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5970 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemassemblyandsignatures.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2512 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/portlet_todo.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2785 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/portlet_plonemeeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_absents_from_meeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      944 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/header_item.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3661 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advicedelayshistory.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      337 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_signatures_from_meeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1496 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/plonemeeting_redirect_to_app_view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4280 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/categorized_annexes.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      802 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/header_meeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      708 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itempolltype.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2849 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itememergencyhistory.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1106 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_signatories.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1499 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/ajax.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_excused_from_meeting.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      884 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/actions_panel_config_linkedplonegroups.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2663 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_voters.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1026 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/sections.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1669 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemcompletenesschange.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1752 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_inserting_methods_help_msg.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      536 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_inherited_advice_item_infos.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      472 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meetingstaticinfos.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13001 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_attendees_edit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/pod_template_mailing_lists.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2858 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemcompletenesshistory.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      708 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_select_all_vote_value.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/grouped_configs.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1777 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/held_position_back_refs.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      670 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/viewlet_force_insert_normal.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1172 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_redefined_position.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1203 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/item_linked_items.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      872 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_not_present.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1520 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/category_meetings.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2591 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemmoreinfos.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3012 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemtodiscuss.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      120 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/header_advice.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2162 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/adviceconfidentiality.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2391 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_available_items_view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7638 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemsignatures.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28599 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/meeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2939 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/portlet_plonemeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6573 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/views_unrestricted.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3560 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/imgselectbox.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25682 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemattendee.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8557 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemduplicate.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5122 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemcompleteness.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4296 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1633 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/INSTALL.TXT
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7742 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/columns.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2532 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4102.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2264 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4108.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12103 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4101.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    55084 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4200.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2760 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4103.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3271 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4106.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3070 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4107.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    72042 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4_1.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1528 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4109.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1528 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4100.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8841 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4110.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6193 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4104.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26220 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6294 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4105.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1555 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/EXTEND_GUIDE.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/src/Products/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3317 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   271060 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1169 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   241815 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      379 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/README.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-03 10:25:45.000000 Products.PloneMeeting-4.2rc8/bin/
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      464 2022-02-03 10:25:44.000000 Products.PloneMeeting-4.2rc8/bin/svn_global.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2022-02-03 10:25:46.000000 Products.PloneMeeting-4.2rc8/setup.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   271255 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43066 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      894 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       62 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/README.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20188 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingGroup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17310 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/indexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10327 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/events.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28941 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      525 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiling.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5360 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/etags.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/exportimport/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43705 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/exportimport/content.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/exportimport/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    74540 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16093 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeetingpopups.js
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    34772 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.js
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/prevalidate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      296 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new_greyed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      212 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/gotoItem.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      585 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      824 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/refused.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/propose.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      373 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/takenOverByNobody.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      642 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/save.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingFileType.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemfrozen_from_returned_to_proposing_group.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      275 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/copy_icon.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      675 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/see_everything.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/documentviewer_convert.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      212 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/arrowLeftDouble.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      239 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/delete_small.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      459 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_public.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      185 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_inherited.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      826 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussNo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialYes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      911 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_disabled_big.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      635 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/questionMark.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemRed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/departure.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      191 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/late.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      671 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/oralQuestion.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      626 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      641 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_accepted.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel4_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_refused.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemCreated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      433 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/takenOverByCurrentUser.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      628 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_comments.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      435 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/reorder.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      372 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/eye.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      837 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_prevalidated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new_meetingadvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/PodTemplate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/rename_icon.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       90 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/refresh.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      520 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemGreen.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      484 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemYellow.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/meetingcategory.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      607 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/videoconference.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2898 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/drop_down.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel5.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel1_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      896 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      373 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new_multiple.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      626 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      496 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemAzur.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      836 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedNo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      958 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      604 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/yes.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1023 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/Meeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      431 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/annexToPrintYes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      158 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/changes.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/back_to.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      893 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/return_to_proposing_group.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToCreated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      285 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/duplicate_and_keep_link.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      681 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/cloned_and_decided.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1715 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/sprites.zip
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      484 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemPurple.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/postponed_next_meeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      501 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency_secret.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      461 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItem.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1881 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm-contenttypes-sprite.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemcreated_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      824 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/refuse.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/arrowSeveral.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      983 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/switch_not_allowed.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      306 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      374 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      195 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/errored_conversion.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      426 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/takenOverByOtherUser.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1185 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      558 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again_back_to_previous.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel5.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_prevalidated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      836 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itempublish.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel5.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemGrey.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new_from_greyed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/plus.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      550 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret_heading.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingGroup.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      763 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/help.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      170 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/night.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedYes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2141 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/save_and_exit.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingUser.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposed_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel4.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      691 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialNo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToAccepted.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3229 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wf_up.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accepted_but_modified.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingFile.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/blue_arrow.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemPublished.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from_prevalidated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      284 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/search_button_icon.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      345 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm_preferences.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      904 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_orange.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/marked_not_applicable.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_cautious.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      973 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/manage.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       85 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pixel.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      614 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/group_users.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      229 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/delay.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      588 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/more_less_details.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      212 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/arrowRightDouble.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1121 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/users.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      791 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_red.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      451 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/budgetRelatedNo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       66 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/checked.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      203 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      381 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new_from.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/arrowLeftSimple.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3211 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from_itemcreated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      921 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_green.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/mark_not_applicable.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_validated_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemPink.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      813 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel5.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      304 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_up_from.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      511 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/store_as_annex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      550 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel2_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm_home.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToPublished.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      480 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/ploneMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/delete_grey_icon.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      323 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingConfig.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      401 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      715 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      386 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/greyedMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      442 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemOrange.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      813 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel5.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/confirm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept_but_modify.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      350 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/annexToPrintNo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      264 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/removeSeveral.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      719 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/funnel.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      858 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_presented_from_returned_to_proposing_group.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      401 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_enable_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      746 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting_emergency.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItem.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      422 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_considered_not_given_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToPrevalidated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel4.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      896 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      526 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public_heading.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/validate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      822 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel4.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      858 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/linkOpaqueDisabled.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itempublished_from_returned_to_proposing_group.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      522 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1765 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_manage.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1145 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_not_given.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_down_from.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_proposed_from_returned_to_proposing_group_prevalidated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      206 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/present.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/postpone_next_meeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/collapseDescrs.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/switch.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      241 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/deadlineKo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      391 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/cloned_not_decided.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_asked.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToClosed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      837 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      558 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again_back_to_previous.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      868 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm_config.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      823 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      755 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      822 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel4.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      776 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      278 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_inherited_remove.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/delete_many.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      268 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/annexToPrintDisabled.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeetingEmergency.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/arrowRightSimple.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel5_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      892 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_reinit_delay.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/manage_annexes.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      526 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel4.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       76 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/leaving.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      367 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/select_items.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      422 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_considered_not_given_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pre_accept.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemFrozen.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/new_meetingadvicefinances.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      620 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_comments.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/cancel_edit.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pre_accepted.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/remove.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1003 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/sendMail.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToDecided.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      280 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemBlack.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4172 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/gotoItemInMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/ToolPloneMeeting.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/removed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel4.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      837 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_prevalidated_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3160 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wf_down.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      229 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/delayed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      525 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/meetingadvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      397 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_disable_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public_heading.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      229 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/presentSeveral.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      628 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussYes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      397 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_disable_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      506 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency_public.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wait_advices_from_proposed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      461 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_not_asked.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/entrance.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel5.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      522 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret_heading.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/budgetRelatedYes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      110 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/expandDescrs.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/acceptable_out_of_meeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      459 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_secret.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel3_from_waiting_advices.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      151 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/view.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      686 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/extraordinarySession.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      323 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/ToolPloneMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToPresented.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      941 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pb_close_small.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1145 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_not_given.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itemfreeze.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/gotoMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      214 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/to.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      401 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_enable_hidden_during_redaction.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_cautious.png
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4924 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/base_edit.cpt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6773 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/livesearch_reply.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3116 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_multiselect_cell.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/base_edit.cpt.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13065 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/versions_history_form.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      359 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/login_success.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      765 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/displayContentsTab.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1780 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_checkbox_cell.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7442 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_edit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    75572 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingconfig_view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    39581 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22614 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meeting_edit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12450 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/toolplonemeeting_view.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4016 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/overrides.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2604 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      428 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/adapters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3238 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      554 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      321 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4249 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/plugin.js
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/lang/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/lang/fr.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      293 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/lang/en.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      291 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/lang/et.js
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      288 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/rotate-right.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      295 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/rotate-left.png
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      525 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-right.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      527 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-left.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       86 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/README.md
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10518 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/monkey.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2095 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MIGRATE_TO_DX.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4100 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/maintenance.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26441 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    93405 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/adapters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   367051 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingConfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19282 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/columns.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3241 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/advice.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1272 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7701 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/meeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    98890 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/Meeting.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      172 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      674 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/organizations.csv
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17124 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/Import_contacts.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1074 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/persons.csv
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      581 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/decision.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11274 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/SignatureCadranel.jpg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      574 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/deliberation_signed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/deliberation_to_sign.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      910 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/person1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1394 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/heldpositions.csv
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9587 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/all_item.odt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    81373 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Agenda.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12815 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/styles2.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11290 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/styles1.odt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    26260 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Decisions.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11422 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Dashboard.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12170 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/organizations-export.ods
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    25537 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Item.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/PloneMeeting_testing_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      325 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23960 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/import_data.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      280 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1745 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10090 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1901 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/propertiestool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1748 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/viewlets.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meetingitem_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22920 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meetingitem_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meeting_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13299 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meeting_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_onestate_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3905 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_onestate_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6694 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_managers_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5839 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_managers_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meetingadvice_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5447 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meetingadvice_workflow/definition.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      289 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/factorytool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/PloneMeeting_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1409 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1148 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/skins.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      333 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ContentCategoryGroup.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      319 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/person.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      521 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/held_position.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      402 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/directory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2226 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/meetingcategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4095 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/annexDecision.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      507 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      258 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ContentCategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      264 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ContentSubcategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3653 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/Meeting.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2335 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/annex.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/organization.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2328 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingItemTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      238 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/Topic.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingConfig.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1900 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ToolPloneMeeting.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2977 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingItem.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2329 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingItemRecurring.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1080 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/DashboardPODTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2452 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ConfigurablePODTemplate.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2664 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/meetingadvice.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3935 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentSubcategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3963 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentCategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14365 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1175 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/portal_atct.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1723 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1208 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/portlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      379 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/repositorytool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6680 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/actions.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17802 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1074 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      242 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      734 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/controlpanel.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3219 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    41569 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2777 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/testing.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14141 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/advice.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2360 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16015 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/held_position.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2954 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/directory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1757 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/person.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15227 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/organization.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    99383 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/meeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1462 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/source.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8559 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/category.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18726 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingUser.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      807 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/LICENSE.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/documentgenerator/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      828 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/documentgenerator/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/documentgenerator/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1927 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/documentgenerator/condition.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2355 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/LICENSE.ZPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   365886 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingItem.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/filters/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1629 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/filters/remove_highlight.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      444 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/filters/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/filters/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30479 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    79226 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ToolPloneMeeting.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/behaviors/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      788 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/behaviors/overrides.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/behaviors/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   100250 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12974 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/validators.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    53382 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/adaptations.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      159 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/generate.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       33 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3050 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/generate.conf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    76464 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/PloneMeeting.zargo
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      672 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_selectreadonly.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_number_input.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      663 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_orderedselect.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1134 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_checkbox.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2658 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/orderedselect_hidden.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1649 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/datagridfield_display.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      962 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_orderedselect_display.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1338 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_selectreadonly_input.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2063 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_richtext_fastedit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      893 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_number.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5261 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_checkbox_input.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1725 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_textarea.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_checkbox_display.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4248 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_richtext.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2239 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_richtext_display.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/__init__.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    17100 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10054 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/vocabularies.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    67025 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12282 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/LICENSE.GPL
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/refresh.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      142 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/testing.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   115684 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/vocabularies.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/Extensions/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24423 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/Extensions/imports.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12360 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingCategory.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1127 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/default_dashboard_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3878 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/default_dashboard_meetings_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      647 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_meeting_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4413 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_item_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1886 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_update_meeting_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1763 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_4104_add_item_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24435 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_add_item_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26106 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/default_dashboard_items_widgets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1344 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/README.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    40550 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testFaceted.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35265 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testVotes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   221573 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testAdvices.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11905 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeetingCategory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      974 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/events.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33584 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/PloneMeetingTestCase.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   123029 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testContacts.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4747 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_unconvertableFormat.eml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34521 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10823 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testUtils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1207 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/keywords.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      687 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/doc-fr.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      593 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/views.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16961 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testColumns.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13542 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testSetup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/FILE.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    71364 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    50761 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testWorkflows.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9137 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_correct2.pdf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42599 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_errorDuringConversion.pdf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26396 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/helpers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      873 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/dot.gif
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)   430590 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeetingItem.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   130280 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testWFAdaptations.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       44 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/annex_not_to_index.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1257 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15612 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testValidators.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8855 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testPortlets.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    88619 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testAnnexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    41996 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testPerformances.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1074 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/test_robot.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   200722 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6851 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_correct.pdf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    68351 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testSearches.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   139589 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testViews.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   131654 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeetingConfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12487 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      339 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tool.gif
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3412 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3834 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemlisttype.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22862 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemvotes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4377 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itempolltype.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   119942 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    70889 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/overrides.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6759 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/portlet_todo.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    51019 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18825 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemassembly.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4664 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/advicecomment.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      353 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/macros.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1269 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/redirect.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14856 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/advicechangedelay.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7023 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itememergency.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4934 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/viewlets.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5423 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/adviceinheritance.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19003 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemchangeorder.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2963 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/jsvariables.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8555 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemtemplates.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21907 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/advices.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24159 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/async.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      450 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/notify.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10533 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/annexes.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1557 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_annexes.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5538 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/ramcache.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2601 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advicedelays.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1251 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemtemplates_tree_recurse.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3161 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/item_navigation_widget.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    57285 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/macros.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4985 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advices-icons.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2002 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemissigned.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      902 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/viewlet_held_position_back_refs.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      369 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_assembly_from_meeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2588 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemtemplates.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      635 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemcompleteness.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itememergency.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10936 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1842 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemnumber.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3171 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/generationlinks.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      955 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advice_version_preview.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9342 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meetingassemblyandsignatures.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3329 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/imgselectbox.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1221 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/actions_panel_deletewholemeeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34761 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advices-icons-infos.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2100 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemstaticinfos.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1646 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/term_searchmeetings.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1165 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemlisttype.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      550 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/actions_panel_config_viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2748 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/category_meetingitems.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5021 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meetingadvice.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5970 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemassemblyandsignatures.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2512 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/portlet_todo.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2785 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/portlet_plonemeeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_absents_from_meeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      944 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/header_item.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3661 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advicedelayshistory.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      337 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_signatures_from_meeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1496 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/plonemeeting_redirect_to_app_view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4280 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/categorized_annexes.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      802 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/header_meeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      708 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itempolltype.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2849 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itememergencyhistory.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1106 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_signatories.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1499 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/ajax.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_excused_from_meeting.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      884 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/actions_panel_config_linkedplonegroups.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2663 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_voters.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1026 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/sections.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1669 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemcompletenesschange.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1752 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_inserting_methods_help_msg.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      536 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_inherited_advice_item_infos.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      472 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meetingstaticinfos.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13001 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_attendees_edit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/pod_template_mailing_lists.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2858 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemcompletenesshistory.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      708 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_select_all_vote_value.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/grouped_configs.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1777 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/held_position_back_refs.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      670 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/viewlet_force_insert_normal.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1172 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_redefined_position.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1203 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/item_linked_items.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      872 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_not_present.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1520 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/category_meetings.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2591 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemmoreinfos.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3012 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemtodiscuss.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      120 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/header_advice.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2162 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/adviceconfidentiality.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2391 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_available_items_view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7638 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemsignatures.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28599 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/meeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2939 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/portlet_plonemeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6573 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/views_unrestricted.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3560 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/imgselectbox.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25682 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemattendee.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8557 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemduplicate.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5122 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemcompleteness.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4296 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1633 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/INSTALL.TXT
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7742 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/columns.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2532 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4102.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2264 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4108.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12103 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4101.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    55084 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4200.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2760 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4103.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3271 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4106.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3070 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4107.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    72042 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4_1.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1528 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4109.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1528 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4100.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8841 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4110.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6193 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4104.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26220 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6294 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4105.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1555 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/EXTEND_GUIDE.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/src/Products/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3317 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   271255 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1169 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   241962 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      379 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/README.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/bin/
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      464 2022-02-04 08:36:17.000000 Products.PloneMeeting-4.2rc9/bin/svn_global.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2022-02-04 08:36:18.000000 Products.PloneMeeting-4.2rc9/setup.cfg
```

### Comparing `Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/PKG-INFO` & `Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.PloneMeeting
-Version: 4.2rc8
+Version: 4.2rc9
 Summary: Official meetings management
 Home-page: https://www.imio.be/nos-applications/ia-delib
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: =====================
         Products.PloneMeeting
@@ -15,14 +15,20 @@
         .. image:: https://coveralls.io/repos/github/IMIO/Products.PloneMeeting/badge.svg?branch=master
             :target: https://coveralls.io/github/IMIO/Products.PloneMeeting?branch=master
         
         Changelog
         =========
         
         
+        4.2rc9 (2022-02-04)
+        -------------------
+        
+        - Fixed bug where a meeting was not correctly reloaded after transition from actions_panel.
+          [gbastien]
+        
         4.2rc8 (2022-02-03)
         -------------------
         
         - For security reason, do no more cache the `image_view_fullscreen` view.
           See https://github.com/plone/Products.CMFPlone/security/advisories/GHSA-8w54-22w9-3g8f.
           [gbastien]
         - Some fixes for meeting created using restapi:
```

### Comparing `Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/SOURCES.txt` & `Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products.PloneMeeting.egg-info/requires.txt` & `Products.PloneMeeting-4.2rc9/src/Products.PloneMeeting.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingGroup.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingGroup.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/indexes.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/indexes.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/events.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/setuphandlers.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiling.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiling.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/etags.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/etags.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/exportimport/content.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/exportimport/content.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.css.dtml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.css.dtml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeetingpopups.js` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeetingpopups.js`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.js` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_styles/plonemeeting.js`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/prevalidate.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/prevalidate.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/refused.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/refused.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/propose.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/propose.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/will_be_cloned_to_other_mc_emergency.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/save.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/save.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel2.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel2.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemfrozen_from_returned_to_proposing_group.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemfrozen_from_returned_to_proposing_group.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/see_everything.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/see_everything.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/documentviewer_convert.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/documentviewer_convert.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussNo.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussNo.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialYes.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialYes.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_disabled_big.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_disabled_big.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/questionMark.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/questionMark.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel3.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel3.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/oralQuestion.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/oralQuestion.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel3.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel3.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_accepted.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_accepted.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel4_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel4_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_refused.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_refused.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemCreated.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemCreated.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_comments.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_comments.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_prevalidated.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_prevalidated.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemGreen.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/MeetingItemGreen.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/videoconference.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/videoconference.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/drop_down.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/drop_down.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel5.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel5.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel1_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel1_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel3.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel3.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_negative.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_negative.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedNo.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedNo.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_nil.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_nil.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/yes.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/yes.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/Meeting.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/Meeting.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/back_to.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/back_to.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel2.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel2.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/return_to_proposing_group.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/return_to_proposing_group.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToCreated.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToCreated.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/cloned_and_decided.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/cloned_and_decided.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/sprites.zip` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/sprites.zip`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm-contenttypes-sprite.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm-contenttypes-sprite.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemcreated_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itemcreated_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel2.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel2.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/refuse.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/refuse.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/switch_not_allowed.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/switch_not_allowed.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/logo.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/logo.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again_back_to_previous.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again_back_to_previous.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel5.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel5.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_prevalidated.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_prevalidated.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itempublish.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itempublish.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel5.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel5.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret_heading.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret_heading.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/help.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/help.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedYes.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itemIsSignedYes.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/save_and_exit.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/save_and_exit.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposed_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposed_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel4.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel4.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialNo.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/isConfidentialNo.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToAccepted.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToAccepted.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wf_up.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wf_up.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accepted_but_modified.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accepted_but_modified.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel3.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposedToValidationLevel3.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/blue_arrow.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/blue_arrow.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemPublished.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemPublished.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_orange.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_orange.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_cautious.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_cautious.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/manage.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/manage.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/group_users.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/group_users.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/more_less_details.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/more_less_details.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/users.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/users.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_red.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_red.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_green.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay_big_green.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_validated_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_validated_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel5.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel5.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel3.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel3.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel2.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel2.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_secret.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel2_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel2_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm_home.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm_home.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToPublished.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToPublished.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_remarks.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_negative.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_negative.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel5.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel5.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/confirm.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/confirm.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept_but_modify.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept_but_modify.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/funnel.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/funnel.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_presented_from_returned_to_proposing_group.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_presented_from_returned_to_proposing_group.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeeting.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeeting.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting_emergency.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting_emergency.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_nil.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_nil.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposed.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposed.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposed.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposed.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToPrevalidated.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToPrevalidated.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel4.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_from_returned_to_proposing_group_proposedToValidationLevel4.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_asked_again.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public_heading.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public_heading.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/validate.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/validate.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel4.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel4.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/linkOpaqueDisabled.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/linkOpaqueDisabled.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itempublished_from_returned_to_proposing_group.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_itempublished_from_returned_to_proposing_group.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_manage.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_manage.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_not_given.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_not_given.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_proposed_from_returned_to_proposing_group_prevalidated.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_returned_to_proposing_group_proposed_from_returned_to_proposing_group_prevalidated.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_asked.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/emergency_asked.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToClosed.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToClosed.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel2.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposeToValidationLevel2.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again_back_to_previous.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_asked_again_back_to_previous.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposed.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToProposed.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pm_config.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pm_config.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel3.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel3.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_with_delay.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel4.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel4.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/accept_out_of_meeting.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeetingEmergency.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToValidatedFromAcceptedOutOfMeetingEmergency.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel5_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel5_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_reinit_delay.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_reinit_delay.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/manage_annexes.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/manage_annexes.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_public.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel4.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel4.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemFrozen.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToItemFrozen.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_comments.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_hands_positive_with_comments.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/cancel_edit.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/cancel_edit.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/remove.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/remove.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/sendMail.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/sendMail.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToDecided.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToDecided.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/gotoItemInMeeting.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/gotoItemInMeeting.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/removed.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/removed.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel4.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposedToValidationLevel4.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel2.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/goTo_returned_to_proposing_group_proposedToValidationLevel2.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_prevalidated_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_prevalidated_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/wf_down.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/wf_down.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/meetingadvice.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/meetingadvice.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public_heading.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_emergency_public_heading.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussYes.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/toDiscussYes.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel5.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/proposeToValidationLevel5.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret_heading.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/clone_to_other_mc_secret_heading.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/budgetRelatedYes.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/budgetRelatedYes.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/acceptable_out_of_meeting.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/acceptable_out_of_meeting.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel3_from_waiting_advices.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backTo_proposedToValidationLevel3_from_waiting_advices.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/extraordinarySession.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/extraordinarySession.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/backToPresented.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/backToPresented.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/pb_close_small.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/pb_close_small.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_not_given.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_not_given.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/itemfreeze.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/itemfreeze.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_remarks.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_positive_with_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_cautious.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_images/advice_standard_cautious.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/base_edit.cpt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/base_edit.cpt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/livesearch_reply.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/livesearch_reply.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_multiselect_cell.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_multiselect_cell.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/versions_history_form.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/versions_history_form.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/displayContentsTab.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/displayContentsTab.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_checkbox_cell.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_plone/datagrid_checkbox_cell.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_edit.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingconfig_view.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingconfig_view.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_view.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meetingitem_view.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/meeting_edit.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/meeting_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/skins/plonemeeting_templates/toolplonemeeting_view.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/skins/plonemeeting_templates/toolplonemeeting_view.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/overrides.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/vocabularies.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/vocabularies.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ftw_labels/overrides.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ftw_labels/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/plugin.js` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/plugin.js`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-right.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-right.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-left.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ckeditor/imagerotate/icons/hidpi/rotate-left.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/monkey.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/monkey.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MIGRATE_TO_DX.rst` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MIGRATE_TO_DX.rst`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/maintenance.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/maintenance.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/adapters.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/adapters.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingConfig.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/columns.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/columns.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/advice.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/advice.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/workflows/meeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/workflows/meeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/Meeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/Meeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/organizations.csv` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/organizations.csv`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/Import_contacts.ods` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/Import_contacts.ods`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/persons.csv` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/persons.csv`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/overheadAnalysis.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/positive.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/attach.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/cahier.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/budget.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/financialAnalysis.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/decision.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/decision.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/remarks.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/SignatureCadranel.jpg` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/SignatureCadranel.jpg`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/legalAdvice.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/negative.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/deliberation_signed.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/deliberation_signed.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/images/person1.png` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/images/person1.png`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/heldpositions.csv` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/heldpositions.csv`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/all_item.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/all_item.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Agenda.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Agenda.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/styles2.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/styles2.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/styles1.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/styles1.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Decisions.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Decisions.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Dashboard.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Dashboard.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/organizations-export.ods` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/organizations-export.ods`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/templates/Item.odt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/templates/Item.odt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/testing/import_data.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/metadata.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/registry.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/propertiestool.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/propertiestool.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/viewlets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/viewlets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meetingitem_workflow/definition.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meetingitem_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meeting_workflow/definition.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meeting_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_onestate_workflow/definition.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_onestate_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_workflow/definition.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_managers_workflow/definition.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/plonemeeting_activity_managers_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows/meetingadvice_workflow/definition.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows/meetingadvice_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/rolemap.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/skins.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/held_position.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/held_position.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/meetingcategory.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/meetingcategory.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/annexDecision.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/annexDecision.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/Meeting.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/Meeting.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/annex.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/annex.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingItemTemplate.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingItemTemplate.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingConfig.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingConfig.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ToolPloneMeeting.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ToolPloneMeeting.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingItem.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingItem.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/MeetingItemRecurring.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/MeetingItemRecurring.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/DashboardPODTemplate.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/DashboardPODTemplate.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ConfigurablePODTemplate.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ConfigurablePODTemplate.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/meetingadvice.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/meetingadvice.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentSubcategory.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentSubcategory.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentCategory.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types/ItemAnnexContentCategory.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/cssregistry.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/portal_atct.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/portal_atct.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/types.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/portlets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/portlets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/actions.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/jsregistry.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/import_steps.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/controlpanel.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/default/workflows.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles/__init__.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/testing.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/testing.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/advice.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/advice.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/held_position.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/held_position.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/directory.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/directory.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/person.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/person.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/organization.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/organization.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/meeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/meeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/source.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/source.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/content/category.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/content/category.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingUser.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingUser.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/LICENSE.txt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/documentgenerator/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/documentgenerator/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/documentgenerator/condition.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/documentgenerator/condition.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/LICENSE.ZPL` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/LICENSE.ZPL`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingItem.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/filters/remove_highlight.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/filters/remove_highlight.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/interfaces.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/ToolPloneMeeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/ToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/behaviors/overrides.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/behaviors/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/utils.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/utils.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/validators.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/validators.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/adaptations.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/adaptations.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/generate.conf` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/generate.conf`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/model/PloneMeeting.zargo` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/model/PloneMeeting.zargo`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_selectreadonly.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_selectreadonly.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_number_input.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_number_input.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_orderedselect.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_orderedselect.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_checkbox.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_checkbox.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/datagridfield_display.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/datagridfield_display.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_orderedselect_display.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_orderedselect_display.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_selectreadonly_input.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_selectreadonly_input.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_richtext_fastedit.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_richtext_fastedit.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_number.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_number.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_checkbox_input.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_textarea.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_textarea.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_checkbox_display.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_checkbox_display.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_richtext.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_richtext.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/widgets/pm_richtext_display.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/widgets/pm_richtext_display.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/config.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/config.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/vocabularies.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/events.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/events.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/LICENSE.GPL` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/vocabularies.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/vocabularies.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/Extensions/imports.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/Extensions/imports.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/MeetingCategory.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/MeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/default_dashboard_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/default_dashboard_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/default_dashboard_meetings_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/default_dashboard_meetings_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_meeting_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_meeting_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_item_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_add_item_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_update_meeting_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_update_meeting_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_4104_add_item_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_4104_add_item_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_add_item_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/upgrade_step_4200_add_item_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/faceted_conf/default_dashboard_items_widgets.xml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/faceted_conf/default_dashboard_items_widgets.xml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/README.txt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/README.txt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testFaceted.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testVotes.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testVotes.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testAdvices.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeetingCategory.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/events.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/PloneMeetingTestCase.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/PloneMeetingTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testContacts.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_unconvertableFormat.eml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_unconvertableFormat.eml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testChangeItemOrderView.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testUtils.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/keywords.robot` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/doc-fr.robot` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/doc-fr.robot`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/robot/views.robot` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/robot/views.robot`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testColumns.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testSetup.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testToolPloneMeeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testWorkflows.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_correct2.pdf` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_correct2.pdf`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_errorDuringConversion.pdf` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_errorDuringConversion.pdf`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/helpers.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/dot.gif` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/dot.gif`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeetingItem.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testWFAdaptations.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/events.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/events.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testValidators.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testPortlets.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testAnnexes.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testPerformances.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testPerformances.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/test_robot.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/file_correct.pdf` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/file_correct.pdf`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testSearches.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testViews.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/tests/testMeetingConfig.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/overrides.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/__init__.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemlisttype.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemlisttype.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemvotes.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemvotes.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itempolltype.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itempolltype.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/views.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/views.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/overrides.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/overrides.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,29 +833,33 @@
             showEdit=True,
             showOwnDelete=True,
             showActions=True,
             showAddContent=False,
             showHistory=False,
             showHistoryLastEventHasComments=True,
             showArrows=False,
+            forceRedirectAfterTransition=False,
             **kwargs):
         """
           Redefined to add ram.cache...
         """
+        if not useIcons:
+            forceRedirectAfterTransition = True
         return super(MeetingActionsPanelView, self).\
             __call__(useIcons=useIcons,
                      showTransitions=showTransitions,
                      appendTypeNameToTransitionLabel=appendTypeNameToTransitionLabel,
                      showEdit=showEdit,
                      showOwnDelete=showOwnDelete,
                      showActions=showActions,
                      showAddContent=showAddContent,
                      showHistory=showHistory,
                      showHistoryLastEventHasComments=showHistoryLastEventHasComments,
                      showArrows=showArrows,
+                     forceRedirectAfterTransition=forceRedirectAfterTransition,
                      **kwargs)
 
     # do ram.cache have a different key name
     __call__ = MeetingActionsPanelView__call__
 
     def renderDeleteWholeMeeting(self):
         """
```

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/portlet_todo.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/portlet_todo.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/configure.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemassembly.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemassembly.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/advicecomment.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/advicecomment.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/redirect.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/redirect.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/advicechangedelay.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/advicechangedelay.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itememergency.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itememergency.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/viewlets.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/adviceinheritance.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/adviceinheritance.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemchangeorder.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemchangeorder.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/jsvariables.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/jsvariables.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemtemplates.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemtemplates.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/advices.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/advices.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/async.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/async.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/annexes.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/annexes.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_annexes.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_annexes.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/ramcache.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/ramcache.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advicedelays.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advicedelays.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemtemplates_tree_recurse.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemtemplates_tree_recurse.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/item_navigation_widget.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/item_navigation_widget.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/macros.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advices-icons.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advices-icons.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemissigned.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemissigned.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/viewlet_held_position_back_refs.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/viewlet_held_position_back_refs.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemtemplates.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemtemplates.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemcompleteness.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemcompleteness.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itememergency.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itememergency.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_view.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_view.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemnumber.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemnumber.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/generationlinks.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/generationlinks.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advice_version_preview.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advice_version_preview.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meetingassemblyandsignatures.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meetingassemblyandsignatures.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/imgselectbox.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/imgselectbox.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/actions_panel_deletewholemeeting.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/actions_panel_deletewholemeeting.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advices-icons-infos.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advices-icons-infos.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemstaticinfos.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemstaticinfos.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/term_searchmeetings.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/term_searchmeetings.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemlisttype.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemlisttype.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/actions_panel_config_viewlet.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/actions_panel_config_viewlet.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/category_meetingitems.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/category_meetingitems.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meetingadvice.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meetingadvice.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemassemblyandsignatures.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemassemblyandsignatures.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/portlet_todo.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/portlet_todo.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/portlet_plonemeeting.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/portlet_plonemeeting.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/header_item.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/header_item.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/advicedelayshistory.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/advicedelayshistory.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/plonemeeting_redirect_to_app_view.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/plonemeeting_redirect_to_app_view.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/categorized_annexes.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/categorized_annexes.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/header_meeting.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/header_meeting.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itempolltype.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itempolltype.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itememergencyhistory.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itememergencyhistory.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_signatories.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_signatories.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/ajax.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/ajax.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/actions_panel_config_linkedplonegroups.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/actions_panel_config_linkedplonegroups.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_voters.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_voters.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/sections.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/sections.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemcompletenesschange.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemcompletenesschange.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_inserting_methods_help_msg.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_inserting_methods_help_msg.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_inherited_advice_item_infos.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_inherited_advice_item_infos.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_attendees_edit.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_attendees_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/pod_template_mailing_lists.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/pod_template_mailing_lists.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemcompletenesshistory.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemcompletenesshistory.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/display_select_all_vote_value.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/display_select_all_vote_value.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/grouped_configs.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/grouped_configs.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/held_position_back_refs.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/held_position_back_refs.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/viewlet_force_insert_normal.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/viewlet_force_insert_normal.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_redefined_position.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_redefined_position.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/item_linked_items.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/item_linked_items.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_item_not_present.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_item_not_present.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/category_meetings.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/category_meetings.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemmoreinfos.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemmoreinfos.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/itemtodiscuss.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/itemtodiscuss.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/adviceconfidentiality.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/adviceconfidentiality.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/templates/meeting_available_items_view.pt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/templates/meeting_available_items_view.pt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemsignatures.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemsignatures.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/meeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/meeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/portlet_plonemeeting.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/portlet_plonemeeting.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/views_unrestricted.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/views_unrestricted.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/imgselectbox.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/imgselectbox.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemattendee.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemattendee.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemduplicate.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemduplicate.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/browser/itemcompleteness.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/browser/itemcompleteness.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/profiles.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/INSTALL.TXT` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/INSTALL.TXT`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/columns.zcml` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/columns.zcml`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4102.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4102.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4108.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4108.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4101.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4101.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4200.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4103.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4103.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4106.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4106.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4107.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4107.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4_1.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4109.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4109.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4100.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4100.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4110.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4110.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4104.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4104.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/__init__.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/migrations/migrate_to_4105.py` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/migrations/migrate_to_4105.py`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/src/Products/PloneMeeting/EXTEND_GUIDE.txt` & `Products.PloneMeeting-4.2rc9/src/Products/PloneMeeting/EXTEND_GUIDE.txt`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/docs/LICENSE.GPL` & `Products.PloneMeeting-4.2rc9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/setup.py` & `Products.PloneMeeting-4.2rc9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '4.2rc8'
+version = '4.2rc9'
 
 setup(name='Products.PloneMeeting',
       version=version,
       description="Official meetings management",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       # Get more strings from https://pypi.python.org/pypi?%3Aaction=list_classifiers
       classifiers=[
```

### Comparing `Products.PloneMeeting-4.2rc8/PKG-INFO` & `Products.PloneMeeting-4.2rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.PloneMeeting
-Version: 4.2rc8
+Version: 4.2rc9
 Summary: Official meetings management
 Home-page: https://www.imio.be/nos-applications/ia-delib
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: =====================
         Products.PloneMeeting
@@ -15,14 +15,20 @@
         .. image:: https://coveralls.io/repos/github/IMIO/Products.PloneMeeting/badge.svg?branch=master
             :target: https://coveralls.io/github/IMIO/Products.PloneMeeting?branch=master
         
         Changelog
         =========
         
         
+        4.2rc9 (2022-02-04)
+        -------------------
+        
+        - Fixed bug where a meeting was not correctly reloaded after transition from actions_panel.
+          [gbastien]
+        
         4.2rc8 (2022-02-03)
         -------------------
         
         - For security reason, do no more cache the `image_view_fullscreen` view.
           See https://github.com/plone/Products.CMFPlone/security/advisories/GHSA-8w54-22w9-3g8f.
           [gbastien]
         - Some fixes for meeting created using restapi:
```

### Comparing `Products.PloneMeeting-4.2rc8/MANIFEST.in` & `Products.PloneMeeting-4.2rc9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.PloneMeeting-4.2rc8/CHANGES.rst` & `Products.PloneMeeting-4.2rc9/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+4.2rc9 (2022-02-04)
+-------------------
+
+- Fixed bug where a meeting was not correctly reloaded after transition from actions_panel.
+  [gbastien]
+
 4.2rc8 (2022-02-03)
 -------------------
 
 - For security reason, do no more cache the `image_view_fullscreen` view.
   See https://github.com/plone/Products.CMFPlone/security/advisories/GHSA-8w54-22w9-3g8f.
   [gbastien]
 - Some fixes for meeting created using restapi:
```

