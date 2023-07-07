# Comparing `tmp/thorpy-2.0.4.tar.gz` & `tmp/thorpy-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thorpy-2.0.4.tar", last modified: Thu May  4 15:32:41 2023, max compression
+gzip compressed data, was "thorpy-2.0.5.tar", last modified: Fri Jul  7 13:58:46 2023, max compression
```

## Comparing `thorpy-2.0.4.tar` & `thorpy-2.0.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.676273 thorpy-2.0.4/
--rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.4/LICENSE
--rw-rw-rw-   0        0        0      378 2023-05-04 15:32:41.675273 thorpy-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2409 2023-05-04 15:31:08.000000 thorpy-2.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 15:32:41.676273 thorpy-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      596 2023-05-04 15:32:24.000000 thorpy-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.623261 thorpy-2.0.4/thorpy/
--rw-rw-rw-   0        0        0     3603 2023-05-04 15:29:32.000000 thorpy-2.0.4/thorpy/__init__.py
--rw-rw-rw-   0        0        0    53415 2023-05-04 15:29:59.000000 thorpy-2.0.4/thorpy/canonical.py
--rw-rw-rw-   0        0        0   124135 2023-04-24 16:05:18.000000 thorpy-2.0.4/thorpy/elements.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.674272 thorpy-2.0.4/thorpy/examples/
--rw-rw-rw-   0        0        0        0 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-04-24 16:24:03.000000 thorpy-2.0.4/thorpy/examples/_example_alert.py
--rw-rw-rw-   0        0        0     1243 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_anim_move.py
--rw-rw-rw-   0        0        0     1703 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_animatedgif.py
--rw-rw-rw-   0        0        0      992 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_box.py
--rw-rw-rw-   0        0        0      861 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_button_helloworld.py
--rw-rw-rw-   0        0        0      868 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_color_gradient.py
--rw-rw-rw-   0        0        0     1183 2023-04-24 16:05:29.000000 thorpy-2.0.4/thorpy/examples/_example_colorpicker.py
--rw-rw-rw-   0        0        0     2400 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_colorpicker2.py
--rw-rw-rw-   0        0        0     2402 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_colorpicker_fine_tuning.py
--rw-rw-rw-   0        0        0     3284 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_create_style.py
--rw-rw-rw-   0        0        0     3425 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_create_style2.py
--rw-rw-rw-   0        0        0     2249 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_custom_theme.py
--rw-rw-rw-   0        0        0     2063 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_dropdownlist.py
--rw-rw-rw-   0        0        0     1790 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_events.py
--rw-rw-rw-   0        0        0     1177 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_filebrowser.py
--rw-rw-rw-   0        0        0     2245 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_fx_light_emitting_image.py
--rw-rw-rw-   0        0        0     3235 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_fx_lights.py
--rw-rw-rw-   0        0        0     1984 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_get_value_from_elements.py
--rw-rw-rw-   0        0        0     1376 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_grouping.py
--rw-rw-rw-   0        0        0     1112 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_grouping_without_sorting.py
--rw-rw-rw-   0        0        0     2575 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_groups_of_groups.py
--rw-rw-rw-   0        0        0     3731 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_guess_the_number.py
--rw-rw-rw-   0        0        0     1573 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_helper.py
--rw-rw-rw-   0        0        0      982 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_heterogeneous_texts.py
--rw-rw-rw-   0        0        0      685 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_image_with_text.py
--rw-rw-rw-   0        0        0     1322 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_imagebutton.py
--rw-rw-rw-   0        0        0     1532 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_integration_in_existing_code.py
--rw-rw-rw-   0        0        0     1316 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_labels.py
--rw-rw-rw-   0        0        0     3028 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_launch.py
--rw-rw-rw-   0        0        0     1287 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_lifebar.py
--rw-rw-rw-   0        0        0     1305 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_look_tune.py
--rw-rw-rw-   0        0        0     2297 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_rich_text.py
--rw-rw-rw-   0        0        0     1307 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_set_default_font.py
--rw-rw-rw-   0        0        0     2128 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_shadows.py
--rw-rw-rw-   0        0        0     3051 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_showcase_themes.py
--rw-rw-rw-   0        0        0     3184 2023-04-24 16:00:12.000000 thorpy-2.0.4/thorpy/examples/_example_showcase_themes2.py
--rw-rw-rw-   0        0        0     2119 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_showcase_themes_buttons.py
--rw-rw-rw-   0        0        0     1500 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_showfps.py
--rw-rw-rw-   0        0        0     1660 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_slider.py
--rw-rw-rw-   0        0        0     2460 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_text_input.py
--rw-rw-rw-   0        0        0     2765 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_text_width.py
--rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_togglables_pool.py
--rw-rw-rw-   0        0        0     1105 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_user_choices.py
--rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_user_choices2.py
--rw-rw-rw-   0        0        0     2051 2023-04-24 16:01:46.000000 thorpy-2.0.4/thorpy/examples/_example_user_chooses_font.py
--rw-rw-rw-   0        0        0     2219 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/examples/_example_waiting_bar.py
--rw-rw-rw-   0        0        0     4520 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/gametools.py
--rw-rw-rw-   0        0        0    28781 2023-04-22 19:22:36.000000 thorpy-2.0.4/thorpy/graphics.py
--rw-rw-rw-   0        0        0     6068 2023-04-24 15:17:59.000000 thorpy-2.0.4/thorpy/loops.py
--rw-rw-rw-   0        0        0     2639 2023-04-22 15:23:24.000000 thorpy-2.0.4/thorpy/monitoring.py
--rw-rw-rw-   0        0        0      467 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/parameters.py
--rw-rw-rw-   0        0        0      625 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/setup.py
--rw-rw-rw-   0        0        0     3727 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/shadows.py
--rw-rw-rw-   0        0        0     2540 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/sorting.py
--rw-rw-rw-   0        0        0     2307 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/sound.py
--rw-rw-rw-   0        0        0    35577 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/styles.py
--rw-rw-rw-   0        0        0    32875 2023-04-21 16:56:57.000000 thorpy-2.0.4/thorpy/themes.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:32:41.635264 thorpy-2.0.4/thorpy.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 15:32:41.000000 thorpy-2.0.4/thorpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.786334 thorpy-2.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0      378 2023-07-07 13:58:46.785352 thorpy-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2768 2023-07-07 13:58:29.000000 thorpy-2.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:58:46.786334 thorpy-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-07-07 13:57:27.000000 thorpy-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.727809 thorpy-2.0.5/thorpy/
+-rw-rw-rw-   0        0        0     3603 2023-07-07 13:58:24.000000 thorpy-2.0.5/thorpy/__init__.py
+-rw-rw-rw-   0        0        0    53629 2023-07-07 13:25:05.000000 thorpy-2.0.5/thorpy/canonical.py
+-rw-rw-rw-   0        0        0   124246 2023-07-07 13:42:31.000000 thorpy-2.0.5/thorpy/elements.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.785352 thorpy-2.0.5/thorpy/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_alert.py
+-rw-rw-rw-   0        0        0     1243 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_anim_move.py
+-rw-rw-rw-   0        0        0     1703 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_animatedgif.py
+-rw-rw-rw-   0        0        0      992 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_box.py
+-rw-rw-rw-   0        0        0      861 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_button_helloworld.py
+-rw-rw-rw-   0        0        0      868 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_color_gradient.py
+-rw-rw-rw-   0        0        0     1183 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_colorpicker.py
+-rw-rw-rw-   0        0        0     2400 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_colorpicker2.py
+-rw-rw-rw-   0        0        0     2402 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_colorpicker_fine_tuning.py
+-rw-rw-rw-   0        0        0     3284 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_create_style.py
+-rw-rw-rw-   0        0        0     3425 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_create_style2.py
+-rw-rw-rw-   0        0        0     2249 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_custom_theme.py
+-rw-rw-rw-   0        0        0     2063 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_dropdownlist.py
+-rw-rw-rw-   0        0        0     1790 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_events.py
+-rw-rw-rw-   0        0        0     1177 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_filebrowser.py
+-rw-rw-rw-   0        0        0     2245 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_fx_light_emitting_image.py
+-rw-rw-rw-   0        0        0     3235 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_fx_lights.py
+-rw-rw-rw-   0        0        0     1984 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_get_value_from_elements.py
+-rw-rw-rw-   0        0        0     1376 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_grouping.py
+-rw-rw-rw-   0        0        0     1112 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_grouping_without_sorting.py
+-rw-rw-rw-   0        0        0     2575 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_groups_of_groups.py
+-rw-rw-rw-   0        0        0     3731 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_guess_the_number.py
+-rw-rw-rw-   0        0        0     1573 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_helper.py
+-rw-rw-rw-   0        0        0      982 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_heterogeneous_texts.py
+-rw-rw-rw-   0        0        0      685 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_image_with_text.py
+-rw-rw-rw-   0        0        0     1322 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_imagebutton.py
+-rw-rw-rw-   0        0        0     1532 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_integration_in_existing_code.py
+-rw-rw-rw-   0        0        0     1316 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_labels.py
+-rw-rw-rw-   0        0        0     3028 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_launch.py
+-rw-rw-rw-   0        0        0     1287 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_lifebar.py
+-rw-rw-rw-   0        0        0     1305 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_look_tune.py
+-rw-rw-rw-   0        0        0     2297 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_rich_text.py
+-rw-rw-rw-   0        0        0     1307 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_set_default_font.py
+-rw-rw-rw-   0        0        0     2128 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_shadows.py
+-rw-rw-rw-   0        0        0     3051 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showcase_themes.py
+-rw-rw-rw-   0        0        0     3184 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showcase_themes2.py
+-rw-rw-rw-   0        0        0     2119 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showcase_themes_buttons.py
+-rw-rw-rw-   0        0        0     1500 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_showfps.py
+-rw-rw-rw-   0        0        0     1660 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_slider.py
+-rw-rw-rw-   0        0        0     2460 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_text_input.py
+-rw-rw-rw-   0        0        0     2765 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_text_width.py
+-rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_togglables_pool.py
+-rw-rw-rw-   0        0        0     1105 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_user_choices.py
+-rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_user_choices2.py
+-rw-rw-rw-   0        0        0     2051 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_user_chooses_font.py
+-rw-rw-rw-   0        0        0     2219 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/examples/_example_waiting_bar.py
+-rw-rw-rw-   0        0        0     4520 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/gametools.py
+-rw-rw-rw-   0        0        0    32626 2023-07-07 13:18:26.000000 thorpy-2.0.5/thorpy/graphics.py
+-rw-rw-rw-   0        0        0     6068 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/loops.py
+-rw-rw-rw-   0        0        0     2257 2023-07-04 10:28:17.000000 thorpy-2.0.5/thorpy/monitoring.py
+-rw-rw-rw-   0        0        0      467 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/parameters.py
+-rw-rw-rw-   0        0        0      625 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/setup.py
+-rw-rw-rw-   0        0        0     3727 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/shadows.py
+-rw-rw-rw-   0        0        0     2540 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/sorting.py
+-rw-rw-rw-   0        0        0     2307 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/sound.py
+-rw-rw-rw-   0        0        0    35577 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/styles.py
+-rw-rw-rw-   0        0        0    32875 2023-05-11 18:30:45.000000 thorpy-2.0.5/thorpy/themes.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:58:46.738812 thorpy-2.0.5/thorpy.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 13:58:46.000000 thorpy-2.0.5/thorpy.egg-info/top_level.txt
```

### Comparing `thorpy-2.0.4/LICENSE` & `thorpy-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/README.md` & `thorpy-2.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # ThorpyWebsite (c) Yann Thorimbert 2023
 
 How to generate site :
 * Set the root for Thorpy in generate_website.py
+    (in general, I copy/paste all the code from site-packages/thorpy to ../Thorpy2)
+* Copy paste the actual thorpy folder to ./thorpy/
+    Attention /!\ : j'ai dû c/c aussi dans ./thorpy pour que ça marche...
 * Run generate_website.py
 
 How to update elements :
 * Nothing special to do for the doc description, it is automatic as long as you indicate things in docstrings
 * For the image, put an image with the same name as the class (but lowercase) in the doc folder
 
 Files to upload to server:
-* All things inside to_upload/
+* All things inside to_upload/ should be sent to ftp.thorpy.org/httpdocs/
 
 Upload on PyPi :
 1. Copy paste the actual thorpy folder (on my computer its 'Thorpy2') to ./thorpy/
 2. Change version number in both setup.py AND thorpy/__init__.py (and dont forget the actual thorpy git !)
 3. pip install twine setuptools wheel
 4. python setup.py sdist bdist_wheel
 5. twine upload dist/*
 Account : Thorpy
 Pwd : Don't worry
 
 
 ***TODO***
 
-pygame mailing list
+cursor resize marche pas
+Documentation pour les attributs de style (set_style("border_thickness", 1) n'est pas inné ! )
 
 
 # versions + tard: ####################################################################
 #TODOs
 #script de tutos auto basé sur les commentaires
 # detecter quels examples figurent pas dans les automatiquement proposes et faire un systeme de tags bijectifs
 #lifebar vertical
```

### Comparing `thorpy-2.0.4/setup.py` & `thorpy-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 setup(name='thorpy',
-      version='2.0.4',
+      version='2.0.5',
       description='GUI library for pygame',
       long_description='ThorPy is a non-intrusive, straightforward GUI kit for Pygame.',
       author='Yann Thorimbert',
       author_email='yann.thorimbert@gmail.com',
       url='http://www.thorpy.org/',
       keywords=['pygame', 'gui', 'menus', 'buttons', 'widgets', 'user interface', 'toolkit'],
       packages=find_packages(),
```

### Comparing `thorpy-2.0.4/thorpy/__init__.py` & `thorpy-2.0.5/thorpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #Import styling functions
 from .themes import theme_classic, theme_human, theme_round, theme_simple, theme_text, theme_game2
 from .themes import theme_round_gradient, theme_round2
 from .themes import theme_text_dark, theme_game1, set_style_attr, refresh_all_elements_style, get_theme_bck_color, get_theme_main_bck_color
 from .styles import get_default_font, set_default_font, get_text_size, get_text_height
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 def set_screen(screen):
     """Set the default surface display for all elements that will be created after this call."""
     parameters.screen = screen
 
 def get_screen():
     """Get the default surface display for elements that will be created after this call."""
```

### Comparing `thorpy-2.0.4/thorpy/canonical.py` & `thorpy-2.0.5/thorpy/canonical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1125,21 +1125,25 @@
 
 
     #convenience function for users
     def get_current_state(self):
         """Return the current state (string) of the element."""
         return self.state
     
-    def set_invisible(self, value):
+    def set_invisible(self, value, recursive=False):
         """Set the element as invisible.
-        <value> : if False, the element is visible, otherwise it is invisible."""
+        <value> : if False, the element is visible, otherwise it is invisible.
+        <recursive> : if True, recursively call this on the children elements."""
         if not value:
             self.state = "normal"
         else:
             self.state = "unactive"
+        if recursive:
+            for e in self.get_children():
+                e.set_invisible(value, recursive)
 
     def set_locked(self, value):
         """Set the current state from 'locked' to 'normal' or from 'normal' to 'locked'.
         <value> : (bool) if True, the new state will be 'locked', wheras if False, the new state
         will be 'normal'. Also adapt the children states.
         """
         if value:
```

### Comparing `thorpy-2.0.4/thorpy/elements.py` & `thorpy-2.0.5/thorpy/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -2671,18 +2671,19 @@
     def __init__(self, clock, pre="", post="", font_size=None, font_color=None,
                  style_normal=None, generate_surfaces=True, only_normal=True):
         self.pre = pre
         self.post = post
         self.clock = clock
         text = self.pre + str(60) + self.post
         super().__init__(text, font_size, font_color, style_normal, generate_surfaces, only_normal, None)
+        self.adapt_parent = False
 
     def update(self, mouse_delta):
         text = self.pre + str(round(self.clock.get_fps())) + self.post
-        self.set_text(text)
+        self.set_text(text, adapt_parent=self.adapt_parent)
         return super().update(mouse_delta)
 
 class TkDialog(Labelled):
     """Uses Tkinter to browse files on the user's machine.
     ***Mandatory arguments***
     <label> : a string defining the label of the element.
     <tk_dialog> : the tkinter dialog launch, e.g. askfolder, askfiles, etc.
@@ -2710,14 +2711,15 @@
             self.tk_dialog = fd.askopenfilename
         elif tk_dialog == "filenames":
             self.tk_dialog = fd.askopenfilenames
         elif tk_dialog == "save":
             self.tk_dialog = fd.asksaveasfilename
         if cls_text is None:
             cls_text = Text
+        self.initial_value = initial_value
         self.tk_dialog_value = cls_text(initial_value)
         self.tk_dialog_value.hand_cursor = True
         self.basename = basename
         self.extension = extension
         self.filetypes = filetypes
         self.initial_dir = initial_dir
         super().__init__(label, self.tk_dialog_value, cls_label)
```

### Comparing `thorpy-2.0.4/thorpy/examples/_example_alert.py` & `thorpy-2.0.5/thorpy/examples/_example_alert.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_anim_move.py` & `thorpy-2.0.5/thorpy/examples/_example_anim_move.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_animatedgif.py` & `thorpy-2.0.5/thorpy/examples/_example_animatedgif.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_box.py` & `thorpy-2.0.5/thorpy/examples/_example_box.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_button_helloworld.py` & `thorpy-2.0.5/thorpy/examples/_example_button_helloworld.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_color_gradient.py` & `thorpy-2.0.5/thorpy/examples/_example_color_gradient.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_colorpicker.py` & `thorpy-2.0.5/thorpy/examples/_example_colorpicker.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_colorpicker2.py` & `thorpy-2.0.5/thorpy/examples/_example_colorpicker2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_colorpicker_fine_tuning.py` & `thorpy-2.0.5/thorpy/examples/_example_colorpicker_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_create_style.py` & `thorpy-2.0.5/thorpy/examples/_example_create_style.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_create_style2.py` & `thorpy-2.0.5/thorpy/examples/_example_create_style2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_custom_theme.py` & `thorpy-2.0.5/thorpy/examples/_example_custom_theme.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_dropdownlist.py` & `thorpy-2.0.5/thorpy/examples/_example_dropdownlist.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_events.py` & `thorpy-2.0.5/thorpy/examples/_example_events.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_filebrowser.py` & `thorpy-2.0.5/thorpy/examples/_example_filebrowser.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_fx_light_emitting_image.py` & `thorpy-2.0.5/thorpy/examples/_example_fx_light_emitting_image.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_fx_lights.py` & `thorpy-2.0.5/thorpy/examples/_example_fx_lights.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_get_value_from_elements.py` & `thorpy-2.0.5/thorpy/examples/_example_get_value_from_elements.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_grouping.py` & `thorpy-2.0.5/thorpy/examples/_example_grouping.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_grouping_without_sorting.py` & `thorpy-2.0.5/thorpy/examples/_example_grouping_without_sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_groups_of_groups.py` & `thorpy-2.0.5/thorpy/examples/_example_groups_of_groups.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_guess_the_number.py` & `thorpy-2.0.5/thorpy/examples/_example_guess_the_number.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_helper.py` & `thorpy-2.0.5/thorpy/examples/_example_helper.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_heterogeneous_texts.py` & `thorpy-2.0.5/thorpy/examples/_example_heterogeneous_texts.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_image_with_text.py` & `thorpy-2.0.5/thorpy/examples/_example_image_with_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_imagebutton.py` & `thorpy-2.0.5/thorpy/examples/_example_imagebutton.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_integration_in_existing_code.py` & `thorpy-2.0.5/thorpy/examples/_example_integration_in_existing_code.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_labels.py` & `thorpy-2.0.5/thorpy/examples/_example_labels.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_launch.py` & `thorpy-2.0.5/thorpy/examples/_example_launch.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_lifebar.py` & `thorpy-2.0.5/thorpy/examples/_example_lifebar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_look_tune.py` & `thorpy-2.0.5/thorpy/examples/_example_look_tune.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_rich_text.py` & `thorpy-2.0.5/thorpy/examples/_example_rich_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_set_default_font.py` & `thorpy-2.0.5/thorpy/examples/_example_set_default_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_shadows.py` & `thorpy-2.0.5/thorpy/examples/_example_shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_showcase_themes.py` & `thorpy-2.0.5/thorpy/examples/_example_showcase_themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_showcase_themes2.py` & `thorpy-2.0.5/thorpy/examples/_example_showcase_themes2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_showcase_themes_buttons.py` & `thorpy-2.0.5/thorpy/examples/_example_showcase_themes_buttons.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_showfps.py` & `thorpy-2.0.5/thorpy/examples/_example_showfps.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_slider.py` & `thorpy-2.0.5/thorpy/examples/_example_slider.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_text_input.py` & `thorpy-2.0.5/thorpy/examples/_example_text_input.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_text_width.py` & `thorpy-2.0.5/thorpy/examples/_example_text_width.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_togglables_pool.py` & `thorpy-2.0.5/thorpy/examples/_example_togglables_pool.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_user_choices.py` & `thorpy-2.0.5/thorpy/examples/_example_user_choices.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_user_choices2.py` & `thorpy-2.0.5/thorpy/examples/_example_user_choices2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_user_chooses_font.py` & `thorpy-2.0.5/thorpy/examples/_example_user_chooses_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/examples/_example_waiting_bar.py` & `thorpy-2.0.5/thorpy/examples/_example_waiting_bar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/gametools.py` & `thorpy-2.0.5/thorpy/gametools.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/graphics.py` & `thorpy-2.0.5/thorpy/graphics.py`

 * *Files 7% similar despite different names*

```diff
@@ -247,19 +247,21 @@
     ***Mandatory arguments***
     <surf> : the image you want to blur (pygame.Surface).
     ***Optional arguments***
     <radius> : radius of the blurry zone.
     <color_format> : an accepted color format by PIL."""
     img = pygame_surf_to_pil_img(surf, color_format)
     img = img.filter(ImageFilter.GaussianBlur(radius))
+    img = pil_img_to_pygame_surf(img, color_format)
     return img
 
 def get_shadow(surf, radius=2, black=255, color_format="RGBA", alpha_factor=255,
                decay_mode="exponential", color=(0,0,0)):
-    """_prefer the Shadow class if possible"""
+    """_prefer the Shadow class if possible
+    <black> : gray value below which the pixel is considered as opaque."""
     img = get_black_white(surf, black, color_format)
     img = img.filter(ImageFilter.GaussianBlur(radius))
     img = pil_img_to_pygame_surf(img, color_format)
     img = set_alpha_from_intensity(img, alpha_factor, decay_mode, color)
     return img
 
 def set_alpha_from_intensity(surface, alpha_factor, decay_mode, color):
@@ -655,14 +657,104 @@
     surface.blit(s, (0,0))
     if orientation:
         scolor = color_gradient(all_colors, s.get_size(), orientation)
         surface.blit(scolor, (0,0), special_flags=pygame.BLEND_RGBA_MIN)
     return surface
 
 
+def draw_pixel_border_ip(surface, border_color, color_empty=None):
+    """This function is very slow and intended to be used once and for all before any loop,
+    most suitably on small sprites. The function uses the defined colorkey as <color_empty> by default."""
+    if not color_empty:
+        color_empty = surface.get_colorkey()
+    if not color_empty:
+        raise Exception("You must provide <color_empty> or a surface with non-None colorkey")
+    w,h = surface.get_size()
+    def draw_pix_if_needed(x,y):
+        color = surface.get_at((x,y))
+        if color != color_empty:
+            gfx.pixel(surface, x, y, border_color) #this or surface.set_at() ?
+            return True
+    for x in range(w): #columns from top to bottom
+        for y in range(h):
+            if draw_pix_if_needed(x,y):
+                break
+    for y in range(h): #lines 
+        for x in range(w): #from left to right
+            if draw_pix_if_needed(x,y):
+                break
+        for x in range(w-1, -1, -1): #from right to left
+            if draw_pix_if_needed(x,y):
+                break
+
+
+def illuminate_border_ip(surface, light_color, orientation, depth, intensity=0.5, color_empty=None):
+    """This function is very slow and intended to be used once and for all before any loop,
+    most suitably on small sprites. The function uses the defined colorkey as <color_empty> by default."""
+    if not color_empty:
+        color_empty = surface.get_colorkey()
+    if not color_empty:
+        raise Exception("You must provide <color_empty> or a surface with non-None colorkey")
+    intensity = 1. - intensity
+    w,h = surface.get_size()
+    def draw_pix_if_needed(x,y):
+        color = surface.get_at((x,y))
+        if color != color_empty:
+            border_color = interpolate_2colors(color[0:len(light_color)], light_color, intensity)
+            gfx.pixel(surface, x, y, border_color) #this or surface.set_at() ?
+            return True
+    if "top" in orientation:
+        for x in range(w): #columns from top to bottom
+            for y in range(h):
+                if draw_pix_if_needed(x,y):
+                    break
+    for y in range(h): #lines 
+        if "left" in orientation:
+            n = 0
+            for x in range(w): #from left to right
+                if draw_pix_if_needed(x,y):
+                    n += 1
+                    if n >= depth:
+                        break
+        if "right" in orientation:
+            n = 0
+            for x in range(w-1, -1, -1): #from right to left
+                if draw_pix_if_needed(x,y):
+                    n += 1
+                    if n >= depth:
+                        break
+
+def scale_image_with_constraint(img, w, h, mode, smooth=True):
+    """Return an image that is scaled so that it fits or fill, without deformation nor cropping,
+    inside a rect of a given size.
+    ***Mandatory arguments***
+    <img> : a Pygame Surface
+    <w>: final width
+    <h>: final height
+    ***Optional arguments***
+    <mode> : (str) either 'fill' or 'fit'.
+    <smooth> : (bool) if True, uses pygame's smoothscale, otherwise uses pygame's scale function."""
+    if smooth:
+        scale_func = pygame.transform.smoothscale
+    else:
+        scale_func = pygame.transform.scale
+    iw, ih = img.get_size()
+    scale_w = w/iw
+    scale_h = h/ih
+    if mode == "fill":
+        if scale_w < scale_h:
+            new_size = int(scale_h*iw), h
+        else:
+            new_size = w, int(scale_w*ih)
+    else:
+        if scale_w > scale_h:
+            new_size = int(scale_h*iw), h
+        else:
+            new_size = w, int(scale_w*ih)
+    return scale_func(img, new_size)
 
 # def draw_aa(color, func, rect, params):
 #     """_Generic function"""
 # ##    size = rect.size
 #     s = Surface(rect.size, pygame.SRCALPHA)
 #     n = 2
 # ##    bigs = pygame.Surface((size[0]*n,size[1]*n), pygame.SRCALPHA)
```

### Comparing `thorpy-2.0.4/thorpy/loops.py` & `thorpy-2.0.5/thorpy/loops.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/setup.py` & `thorpy-2.0.5/thorpy/setup.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/shadows.py` & `thorpy-2.0.5/thorpy/shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/sorting.py` & `thorpy-2.0.5/thorpy/sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/sound.py` & `thorpy-2.0.5/thorpy/sound.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/styles.py` & `thorpy-2.0.5/thorpy/styles.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy/themes.py` & `thorpy-2.0.5/thorpy/themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.4/thorpy.egg-info/SOURCES.txt` & `thorpy-2.0.5/thorpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

