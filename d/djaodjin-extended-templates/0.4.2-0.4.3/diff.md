# Comparing `tmp/djaodjin-extended-templates-0.4.2.tar.gz` & `tmp/djaodjin-extended-templates-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-extended-templates-0.4.2.tar", last modified: Fri Feb 24 18:51:51 2023, max compression
+gzip compressed data, was "djaodjin-extended-templates-0.4.3.tar", last modified: Fri Jul  7 15:33:51 2023, max compression
```

## Comparing `djaodjin-extended-templates-0.4.2.tar` & `djaodjin-extended-templates-0.4.3.tar`

### file list

```diff
@@ -1,132 +1,83 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.785978 djaodjin-extended-templates-0.4.2/
--rw-r--r--   0 smirolo    (501) staff       (20)       72 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/.gitignore
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     6112 2022-09-11 19:36:31.000000 djaodjin-extended-templates-0.4.2/Makefile
--rw-r--r--   0 smirolo    (501) staff       (20)     2339 2023-02-24 18:51:51.786053 djaodjin-extended-templates-0.4.2/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1944 2023-02-24 18:41:05.000000 djaodjin-extended-templates-0.4.2/README.md
--rw-r--r--   0 smirolo    (501) staff       (20)     1445 2023-02-24 18:40:57.000000 djaodjin-extended-templates-0.4.2/changelog
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.767613 djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     2339 2023-02-24 18:51:51.000000 djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     3806 2023-02-24 18:51:51.000000 djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-02-24 18:51:51.000000 djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      225 2023-02-24 18:51:51.000000 djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       19 2023-02-24 18:51:51.000000 djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/top_level.txt
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.770342 djaodjin-extended-templates-0.4.2/extended_templates/
--rw-r--r--   0 smirolo    (501) staff       (20)     1447 2023-02-24 18:39:07.000000 djaodjin-extended-templates-0.4.2/extended_templates/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.772040 djaodjin-extended-templates-0.4.2/extended_templates/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4265 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/less_variables.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3582 2023-02-24 18:30:59.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1976 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/sitecss.py
--rw-r--r--   0 smirolo    (501) staff       (20)    19365 2023-02-17 19:40:33.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/sources.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5034 2023-02-03 04:47:19.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9953 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/api/upload_media.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.773012 djaodjin-extended-templates-0.4.2/extended_templates/backends/
--rw-r--r--   0 smirolo    (501) staff       (20)     3261 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/backends/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9333 2023-02-08 21:30:05.000000 djaodjin-extended-templates-0.4.2/extended_templates/backends/eml.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9459 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/backends/pdf.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1721 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/backends/s3.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7332 2023-02-07 21:34:10.000000 djaodjin-extended-templates-0.4.2/extended_templates/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2934 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/decorators.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3188 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3058 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/extras.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3152 2023-02-08 00:52:56.000000 djaodjin-extended-templates-0.4.2/extended_templates/helpers.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.773250 djaodjin-extended-templates-0.4.2/extended_templates/management/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/management/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.773673 djaodjin-extended-templates-0.4.2/extended_templates/management/commands/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/management/commands/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2696 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/management/commands/install_theme.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3398 2023-02-13 23:22:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/management/commands/list_css_classes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6691 2023-02-07 20:38:57.000000 djaodjin-extended-templates-0.4.2/extended_templates/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3581 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10334 2022-08-23 21:36:15.000000 djaodjin-extended-templates-0.4.2/extended_templates/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1471 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.764409 djaodjin-extended-templates-0.4.2/extended_templates/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.774277 djaodjin-extended-templates-0.4.2/extended_templates/static/css/
--rw-r--r--   0 smirolo    (501) staff       (20)     2031 2023-02-09 18:32:15.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/css/djaodjin-editor.css
--rw-r--r--   0 smirolo    (501) staff       (20)     5797 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/css/djaodjin-sidebar-gallery.css
--rw-r--r--   0 smirolo    (501) staff       (20)       42 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/css/djaodjin-style-editor.css
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.776666 djaodjin-extended-templates-0.4.2/extended_templates/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)     8818 2023-02-07 18:55:03.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-code-editor.js
--rw-r--r--   0 smirolo    (501) staff       (20)    22871 2022-07-27 19:54:45.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-editor.js
--rw-r--r--   0 smirolo    (501) staff       (20)    50544 2023-02-24 18:05:33.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (501) staff       (20)    27061 2022-07-27 20:10:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-sidebar-gallery.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12248 2022-07-27 19:55:29.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-style-editor.js
--rw-r--r--   0 smirolo    (501) staff       (20)     1149 2022-09-01 18:19:11.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-themes-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)    14671 2022-07-27 20:39:43.000000 djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-upload.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.764622 djaodjin-extended-templates-0.4.2/extended_templates/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.777063 djaodjin-extended-templates-0.4.2/extended_templates/templates/django/
--rw-r--r--   0 smirolo    (501) staff       (20)     2890 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/django/_field.html
--rw-r--r--   0 smirolo    (501) staff       (20)      560 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/django/_form.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.778203 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/
--rw-r--r--   0 smirolo    (501) staff       (20)     1933 2022-07-29 20:52:36.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/_body_bottom.html
--rw-r--r--   0 smirolo    (501) staff       (20)      105 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/_body_bottom_edit_tools.html
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/_body_top.html
--rw-r--r--   0 smirolo    (501) staff       (20)    12462 2022-07-29 20:55:46.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/_edit_tools.html
--rw-r--r--   0 smirolo    (501) staff       (20)      682 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/edit.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1646 2022-07-29 21:12:01.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/theme.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.778602 djaodjin-extended-templates-0.4.2/extended_templates/templates/jinja2/
--rw-r--r--   0 smirolo    (501) staff       (20)      363 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/jinja2/_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)     5700 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templates/jinja2/_form_fields.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.778868 djaodjin-extended-templates-0.4.2/extended_templates/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)      650 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/templatetags/extended_templates_tags.py
--rw-r--r--   0 smirolo    (501) staff       (20)    16499 2023-02-24 17:54:24.000000 djaodjin-extended-templates-0.4.2/extended_templates/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4370 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/thread_locals.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2845 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/uploadhandler.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.779018 djaodjin-extended-templates-0.4.2/extended_templates/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1525 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.779730 djaodjin-extended-templates-0.4.2/extended_templates/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1772 2022-08-10 04:49:00.000000 djaodjin-extended-templates-0.4.2/extended_templates/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2178 2023-01-07 00:10:20.000000 djaodjin-extended-templates-0.4.2/extended_templates/urls/api/assets.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1997 2023-01-07 00:09:49.000000 djaodjin-extended-templates-0.4.2/extended_templates/urls/api/templates.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.780201 djaodjin-extended-templates-0.4.2/extended_templates/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1478 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1683 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/urls/views/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7957 2022-07-27 20:24:14.000000 djaodjin-extended-templates-0.4.2/extended_templates/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.780974 djaodjin-extended-templates-0.4.2/extended_templates/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-07-29 19:32:33.000000 djaodjin-extended-templates-0.4.2/extended_templates/views/pages.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4929 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/extended_templates/views/static.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4602 2023-02-07 22:05:52.000000 djaodjin-extended-templates-0.4.2/extended_templates/views/themes.py
--rw-r--r--   0 smirolo    (501) staff       (20)      251 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/manage.py
--rw-r--r--   0 smirolo    (501) staff       (20)      225 2023-02-24 18:31:37.000000 djaodjin-extended-templates-0.4.2/requirements.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-02-24 18:51:51.786264 djaodjin-extended-templates-0.4.2/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     2766 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.782837 djaodjin-extended-templates-0.4.2/testsite/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.783153 djaodjin-extended-templates-0.4.2/testsite/etc/
--rw-r--r--   0 smirolo    (501) staff       (20)       97 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/etc/credentials
--rw-r--r--   0 smirolo    (501) staff       (20)      706 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/etc/gunicorn.conf
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.783298 djaodjin-extended-templates-0.4.2/testsite/fixtures/
--rw-r--r--   0 smirolo    (501) staff       (20)      466 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/fixtures/default-db.json
--rw-r--r--   0 smirolo    (501) staff       (20)     2468 2022-07-29 21:35:50.000000 djaodjin-extended-templates-0.4.2/testsite/jinja2.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.783439 djaodjin-extended-templates-0.4.2/testsite/management/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/management/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.783628 djaodjin-extended-templates-0.4.2/testsite/management/commands/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/management/commands/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2160 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/management/commands/sendtestemail.py
--rw-r--r--   0 smirolo    (501) staff       (20)      659 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/package.json
--rw-r--r--   0 smirolo    (501) staff       (20)      472 2023-02-24 18:33:19.000000 djaodjin-extended-templates-0.4.2/testsite/requirements-legacy.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      537 2023-02-24 18:33:54.000000 djaodjin-extended-templates-0.4.2/testsite/requirements.txt
--rw-r--r--   0 smirolo    (501) staff       (20)     7082 2022-08-23 20:57:01.000000 djaodjin-extended-templates-0.4.2/testsite/settings.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.765335 djaodjin-extended-templates-0.4.2/testsite/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.784669 djaodjin-extended-templates-0.4.2/testsite/static/vendor/
--rw-r--r--   0 smirolo    (501) staff       (20)    35247 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/static/vendor/jquery-ui.css
--rw-r--r--   0 smirolo    (501) staff       (20)   470596 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/static/vendor/jquery-ui.js
--rw-r--r--   0 smirolo    (501) staff       (20)    10254 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/static/vendor/jquery.ba-throttle-debounce.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.785311 djaodjin-extended-templates-0.4.2/testsite/templates/
--rw-r--r--   0 smirolo    (501) staff       (20)      628 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/templates/base.eml
--rw-r--r--   0 smirolo    (501) staff       (20)     2905 2022-07-29 20:45:11.000000 djaodjin-extended-templates-0.4.2/testsite/templates/base.html
--rw-r--r--   0 smirolo    (501) staff       (20)     4394 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/templates/index.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.785442 djaodjin-extended-templates-0.4.2/testsite/templates/registration/
--rw-r--r--   0 smirolo    (501) staff       (20)      297 2022-07-29 21:07:28.000000 djaodjin-extended-templates-0.4.2/testsite/templates/registration/login.html
--rw-r--r--   0 smirolo    (501) staff       (20)      342 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/templates/testemail.eml
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-02-24 18:51:51.785755 djaodjin-extended-templates-0.4.2/testsite/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1914 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/templatetags/testsite_tags.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2754 2022-08-23 05:50:58.000000 djaodjin-extended-templates-0.4.2/testsite/urls.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2070 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/views.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1224 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.2/testsite/wsgi.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.315857 djaodjin-extended-templates-0.4.3/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     2687 2023-07-07 15:33:51.315922 djaodjin-extended-templates-0.4.3/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1868 2023-07-07 15:32:14.000000 djaodjin-extended-templates-0.4.3/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.301870 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2687 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2641 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      227 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       19 2023-07-07 15:33:51.000000 djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/top_level.txt
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.305028 djaodjin-extended-templates-0.4.3/extended_templates/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1447 2023-07-07 15:32:44.000000 djaodjin-extended-templates-0.4.3/extended_templates/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.306845 djaodjin-extended-templates-0.4.3/extended_templates/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4265 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/less_variables.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3582 2023-02-24 18:30:59.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1976 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/sitecss.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    19365 2023-02-17 19:40:33.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/sources.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5034 2023-02-03 04:47:19.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9953 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/api/upload_media.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.307776 djaodjin-extended-templates-0.4.3/extended_templates/backends/
+-rw-r--r--   0 smirolo    (501) staff       (20)     3261 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9469 2023-04-05 21:35:22.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/eml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9459 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/pdf.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1721 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/backends/s3.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7332 2023-02-07 21:34:10.000000 djaodjin-extended-templates-0.4.3/extended_templates/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2934 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/decorators.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3188 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3058 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/extras.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3152 2023-02-08 00:52:56.000000 djaodjin-extended-templates-0.4.3/extended_templates/helpers.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.307937 djaodjin-extended-templates-0.4.3/extended_templates/management/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.308330 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2696 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/install_theme.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3398 2023-02-13 23:22:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/management/commands/list_css_classes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6691 2023-02-07 20:38:57.000000 djaodjin-extended-templates-0.4.3/extended_templates/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3581 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10334 2022-08-23 21:36:15.000000 djaodjin-extended-templates-0.4.3/extended_templates/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1471 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.299581 djaodjin-extended-templates-0.4.3/extended_templates/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.311159 djaodjin-extended-templates-0.4.3/extended_templates/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)     8818 2023-02-07 18:55:03.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-code-editor.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    22871 2023-04-27 17:26:14.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-editor.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:05.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    27061 2022-07-27 20:10:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-sidebar-gallery.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12248 2022-07-27 19:55:29.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-style-editor.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     1149 2022-09-01 18:19:11.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-themes-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    14671 2022-07-27 20:39:43.000000 djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-upload.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.299699 djaodjin-extended-templates-0.4.3/extended_templates/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.312259 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1933 2022-07-29 20:52:36.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_bottom.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      105 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_bottom_edit_tools.html
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_top.html
+-rw-r--r--   0 smirolo    (501) staff       (20)    12462 2022-07-29 20:55:46.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_edit_tools.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      682 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/edit.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1646 2022-07-29 21:12:01.000000 djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/theme.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.312592 djaodjin-extended-templates-0.4.3/extended_templates/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      650 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/templatetags/extended_templates_tags.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    16499 2023-02-24 17:54:24.000000 djaodjin-extended-templates-0.4.3/extended_templates/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4370 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/thread_locals.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2845 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/uploadhandler.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.312725 djaodjin-extended-templates-0.4.3/extended_templates/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1525 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.313374 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1772 2022-08-10 04:49:00.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2178 2023-01-07 00:10:20.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/assets.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1997 2023-01-07 00:09:49.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/api/templates.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.314214 djaodjin-extended-templates-0.4.3/extended_templates/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1478 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1683 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/urls/views/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8083 2023-03-03 21:48:25.000000 djaodjin-extended-templates-0.4.3/extended_templates/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:33:51.315636 djaodjin-extended-templates-0.4.3/extended_templates/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-07-29 19:32:33.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/pages.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4929 2022-07-26 19:09:34.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/static.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4602 2023-02-07 22:05:52.000000 djaodjin-extended-templates-0.4.3/extended_templates/views/themes.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1578 2023-07-07 13:42:34.000000 djaodjin-extended-templates-0.4.3/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-07-07 15:33:51.316130 djaodjin-extended-templates-0.4.3/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-07-07 13:42:54.000000 djaodjin-extended-templates-0.4.3/setup.py
```

### Comparing `djaodjin-extended-templates-0.4.2/LICENSE.txt` & `djaodjin-extended-templates-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/PKG-INFO` & `djaodjin-extended-templates-0.4.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-Metadata-Version: 2.1
-Name: djaodjin-extended-templates
-Version: 0.4.2
-Summary: DjaoDjin's Template wrappers for HTML email and PDF templates
-Home-page: https://github.com/djaodjin/djaodjin-extended-templates/
-Download-URL: https://github.com/djaodjin/djaodjin-extended-templates/tarball/0.4.2
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
-License-File: LICENSE.txt
-
 djaodjin-extended-templates is a Django application that adds missing features
 for managing Django templates.
 
 Major Features:
 
 - Live editing of HTML templates
 - Build .css from .scss on page load
 - HTML email templates
 - PDF templates
 - Media assets gallery
 - Upload theme packages
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.1 (latest), **Django Rest Framework:** 3.12
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 
 Development
 ===========
 
 After cloning the repository, create a virtualenv environment, install
 the prerequisites, create the database then run the testsite webapp.
 
@@ -70,14 +53,20 @@
 Note that you will need to link ``podofo-flatform.cc`` with [podofo](http://podofo.sourceforge.net/)
 version 0.9.3. Version 0.9.1 as shipped with many RedHat systems will link
 with no error but the outputed PDF will be blank.
 
 Release Notes
 =============
 
-0.4.2
+Tested with
 
-  * shows TemplateSyntax errors when uploading theme
-  * removes unused dependency on bleach
-  * removes dependency on vue-infinite-loading for pagination
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
+- **Python:** 3.10, **Django:** 4.2 (latest)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.4.3
+
+  * sends raw text e-mail if premail resources cannot be found
+  * compatibles with django-storages==1.13
+  * installs using pyproject.toml
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-extended-templates-0.4.2/README.md` & `djaodjin-extended-templates-0.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,38 @@
+Metadata-Version: 2.1
+Name: djaodjin-extended-templates
+Version: 0.4.3
+Summary: DjaoDjin's Template wrappers for HTML email and PDF templates
+Author-email: The DjaoDjin Team <help@djaodjin.com>
+Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
+License: BSD-2-Clause
+Project-URL: repository, https://github.com/djaodjin/djaodjin-extended-templates
+Project-URL: documentation, https://djaodjin-extended-templates.readthedocs.io/
+Project-URL: changelog, https://github.com/djaodjin/djaodjin-extended-templates/changelog
+Keywords: django,templates,email,pdf
+Classifier: Framework :: Django
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 djaodjin-extended-templates is a Django application that adds missing features
 for managing Django templates.
 
 Major Features:
 
 - Live editing of HTML templates
 - Build .css from .scss on page load
 - HTML email templates
 - PDF templates
 - Media assets gallery
 - Upload theme packages
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.1 (latest), **Django Rest Framework:** 3.12
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 
 Development
 ===========
 
 After cloning the repository, create a virtualenv environment, install
 the prerequisites, create the database then run the testsite webapp.
 
@@ -59,14 +72,20 @@
 Note that you will need to link ``podofo-flatform.cc`` with [podofo](http://podofo.sourceforge.net/)
 version 0.9.3. Version 0.9.1 as shipped with many RedHat systems will link
 with no error but the outputed PDF will be blank.
 
 Release Notes
 =============
 
-0.4.2
+Tested with
 
-  * shows TemplateSyntax errors when uploading theme
-  * removes unused dependency on bleach
-  * removes dependency on vue-infinite-loading for pagination
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
+- **Python:** 3.10, **Django:** 4.2 (latest)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.4.3
+
+  * sends raw text e-mail if premail resources cannot be found
+  * compatibles with django-storages==1.13
+  * installs using pyproject.toml
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-extended-templates-0.4.2/djaodjin_extended_templates.egg-info/PKG-INFO` & `djaodjin-extended-templates-0.4.3/djaodjin_extended_templates.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: djaodjin-extended-templates
-Version: 0.4.2
+Version: 0.4.3
 Summary: DjaoDjin's Template wrappers for HTML email and PDF templates
-Home-page: https://github.com/djaodjin/djaodjin-extended-templates/
-Download-URL: https://github.com/djaodjin/djaodjin-extended-templates/tarball/0.4.2
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
+Author-email: The DjaoDjin Team <help@djaodjin.com>
+Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
+License: BSD-2-Clause
+Project-URL: repository, https://github.com/djaodjin/djaodjin-extended-templates
+Project-URL: documentation, https://djaodjin-extended-templates.readthedocs.io/
+Project-URL: changelog, https://github.com/djaodjin/djaodjin-extended-templates/changelog
+Keywords: django,templates,email,pdf
+Classifier: Framework :: Django
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 djaodjin-extended-templates is a Django application that adds missing features
 for managing Django templates.
 
 Major Features:
 
 - Live editing of HTML templates
 - Build .css from .scss on page load
 - HTML email templates
 - PDF templates
 - Media assets gallery
 - Upload theme packages
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.1 (latest), **Django Rest Framework:** 3.12
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 
 Development
 ===========
 
 After cloning the repository, create a virtualenv environment, install
 the prerequisites, create the database then run the testsite webapp.
 
@@ -70,14 +72,20 @@
 Note that you will need to link ``podofo-flatform.cc`` with [podofo](http://podofo.sourceforge.net/)
 version 0.9.3. Version 0.9.1 as shipped with many RedHat systems will link
 with no error but the outputed PDF will be blank.
 
 Release Notes
 =============
 
-0.4.2
+Tested with
 
-  * shows TemplateSyntax errors when uploading theme
-  * removes unused dependency on bleach
-  * removes dependency on vue-infinite-loading for pagination
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
+- **Python:** 3.10, **Django:** 4.2 (latest)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.4.3
+
+  * sends raw text e-mail if premail resources cannot be found
+  * compatibles with django-storages==1.13
+  * installs using pyproject.toml
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/__init__.py` & `djaodjin-extended-templates-0.4.3/extended_templates/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the extended_templates django app.
 """
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
```

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/api/less_variables.py` & `djaodjin-extended-templates-0.4.3/extended_templates/api/less_variables.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/api/serializers.py` & `djaodjin-extended-templates-0.4.3/extended_templates/api/serializers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/api/sitecss.py` & `djaodjin-extended-templates-0.4.3/extended_templates/api/sitecss.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/api/sources.py` & `djaodjin-extended-templates-0.4.3/extended_templates/api/sources.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/api/themes.py` & `djaodjin-extended-templates-0.4.3/extended_templates/api/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/api/upload_media.py` & `djaodjin-extended-templates-0.4.3/extended_templates/api/upload_media.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/backends/__init__.py` & `djaodjin-extended-templates-0.4.3/extended_templates/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/backends/eml.py` & `djaodjin-extended-templates-0.4.3/extended_templates/backends/eml.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,20 @@
               connection=None, fail_silently=False):
         #pylint: disable=too-many-locals
         subject = None
         plain_content = None
         headers = {'Reply-To': reply_to} if reply_to else None
         request = getattr(context, 'request', context.get('request', None))
 
-        html_content = Premailer(
-            self.render(context=context, request=request),
-            include_star_selectors=True).transform()
+        try:
+            html_content = Premailer(
+                self.render(context=context, request=request),
+                include_star_selectors=True).transform()
+        except ExternalNotFoundError:
+            html_content = self.render(context=context, request=request)
 
         if not plain_content:
             # Defaults to content stripped of html tags
             if not html_content:
                 raise EmlTemplateError(
                     "Template %s does not contain PLAIN nor HTML content."
                     % self.origin.name)
```

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/backends/pdf.py` & `djaodjin-extended-templates-0.4.3/extended_templates/backends/pdf.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/backends/s3.py` & `djaodjin-extended-templates-0.4.3/extended_templates/backends/s3.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/compat.py` & `djaodjin-extended-templates-0.4.3/extended_templates/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/decorators.py` & `djaodjin-extended-templates-0.4.3/extended_templates/decorators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/docs.py` & `djaodjin-extended-templates-0.4.3/extended_templates/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/extras.py` & `djaodjin-extended-templates-0.4.3/extended_templates/extras.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/helpers.py` & `djaodjin-extended-templates-0.4.3/extended_templates/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/management/commands/install_theme.py` & `djaodjin-extended-templates-0.4.3/extended_templates/management/commands/install_theme.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/management/commands/list_css_classes.py` & `djaodjin-extended-templates-0.4.3/extended_templates/management/commands/list_css_classes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/mixins.py` & `djaodjin-extended-templates-0.4.3/extended_templates/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/models.py` & `djaodjin-extended-templates-0.4.3/extended_templates/models.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/settings.py` & `djaodjin-extended-templates-0.4.3/extended_templates/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/signals.py` & `djaodjin-extended-templates-0.4.3/extended_templates/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-code-editor.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-code-editor.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-editor.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-editor.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-resources-vue.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources-vue.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -154,44 +154,27 @@
                 }
                 vm.showMessages(messages, "error");
             },
         }
     };
 
 
-    /** compute outdated based on params.
+    /** compute outdated based on `params`.
+
+        `params = {start_at, ends_at}` must exist in either the `props` or `data`
+        of the component.
 
         A subclass of this mixin must define either the function `autoReload`
         or `reload` in order to make updates as a user is typing in input fields
         or when a button is pressed respectively.
      */
     var paramsMixin = {
         data: function() {
             var data = {
                 lastGetParams: {},
-                params: {
-                    // The following dates will be stored as `String` objects
-                    // as oppossed to `moment` or `Date` objects because this
-                    // is how form fields input="date" will update them.
-                    start_at: null,
-                    ends_at: null,
-                    // The timezone for both start_at and ends_at.
-                    timezone: 'local'
-                }
-            }
-            if (this.$dateRange) {
-                if (this.$dateRange.start_at) {
-                    data.params['start_at'] = this.$dateRange.start_at;
-                }
-                if (this.$dateRange.ends_at) {
-                    data.params['ends_at'] = this.$dateRange.ends_at;
-                }
-                if (this.$dateRange.timezone) {
-                    data.params['timezone'] = this.$dateRange.timezone;
-                }
             }
             return data;
         },
         methods: {
             asDateInputField: function(dateISOString) {
                 const dateValue = moment(dateISOString);
                 return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
@@ -209,14 +192,31 @@
                     if (vm.params.hasOwnProperty(key) && vm.params[key]) {
                         if (excludes && key in excludes) continue;
                         params[key] = vm.params[key];
                     }
                 }
                 return params;
             },
+            getQueryString: function(excludes) {
+                var vm = this;
+                var sep = "";
+                var result = "";
+                var params = vm.getParams(excludes);
+                for (var key in params) {
+                    if (params.hasOwnProperty(key)) {
+                        result += sep + key + '=' + encodeURIComponent(
+                            params[key].toString());
+                        sep = "&";
+                    }
+                }
+                if (result) {
+                    result = '?' + result;
+                }
+                return result;
+            },
         },
         computed: {
             _start_at: {
                 get: function() {
                     return this.asDateInputField(this.params.start_at);
                 },
                 set: function(newVal) {
@@ -277,15 +277,15 @@
             // _.debounce is a function provided by lodash to limit how
             // often a particularly expensive operation can be run.
             if (typeof _ != 'undefined' && typeof _.debounce != 'undefined') {
                 this.debouncedAutoReload = _.debounce(this.autoReload, 500);
             } else {
                 this.debouncedAutoReload = this.autoReload;
             }
-        },
+        }
     };
 
 
     /** A wrapper around jQuery ajax functions that adds authentication
         parameters as necessary.
 
         requires `jQuery`
@@ -342,41 +342,41 @@
                 }
                 return "";
             },
 
             _safeUrl: function(base, path) {
                 if (!path) return base;
 
-                if (base && base[base.length - 1] == '/') {
-                    if (path && path[0] == '/') {
-                        return base + path.substring(1);
+                const parts = [base].concat(
+                    (typeof path === 'string') ? [path] : path);
+                var cleanParts = [];
+                var start, end;
+                for (var idx = 0; idx < parts.length; ++idx) {
+                    const part = parts[idx];
+                    for (start = 0; start < part.length; ++start) {
+                        if (part[start] !== '/') {
+                            break;
+                        }
                     }
-                    return base + path;
-                }
-                if (path && path[0] == '/') {
-                    return base + path;
-                }
-                return base + '/' + path;
-            },
-
-            getQueryString: function(excludes) {
-                var vm = this;
-                var sep = "";
-                var result = "";
-                var params = vm.getParams(excludes);
-                for (var key in params) {
-                    if (params.hasOwnProperty(key)) {
-                        result += sep + key + '=' + params[key].toString();
-                        sep = "&";
+                    for (end = part.length - 1; end >= 0; --end) {
+                        if (part[end] !== '/') {
+                            break;
+                        }
+                    }
+                    if (start < end) {
+                        cleanParts.push(part.slice(start, end + 1));
+                    } else {
+                        cleanParts.push(part);
                     }
                 }
-                if (result) {
-                    result = '?' + result;
+                var cleanUrl = cleanParts[0];
+                for (idx = 1; idx < cleanParts.length; ++idx) {
+                    cleanUrl += '/' + cleanParts[idx];
                 }
-                return result;
+                return cleanUrl.startsWith('http') ? cleanUrl[0] : '/' + cleanUrl;
             },
 
             /** This method generates a GET HTTP request to `url` with a query
                 string built of a `queryParams` dictionnary.
 
                 It supports the following prototypes:
 
@@ -827,38 +827,37 @@
                 if (!successCallback) {
                     successCallback = function() {};
                 }
                 if (!failureCallback) {
                     failureCallback = vm.showErrorMessages;
                 }
                 for (var idx = 0; idx < queryArray.length; ++idx) {
-                    ajaxCalls.push(function() {
-                        return $.ajax({
-                            method: queryArray[idx].method,
-                            url: queryArray[idx].url,
-                            data: JSON.stringify(queryArray[idx].data),
-                            beforeSend: function(xhr, settings) {
-                                var authToken = vm._getAuthToken();
-                                if (authToken) {
-                                    xhr.setRequestHeader("Authorization",
-                                        "Bearer " + authToken);
-                                } else {
-                                    if (!vm._csrfSafeMethod(settings.type)) {
-                                        var csrfToken = vm._getCSRFToken();
-                                        if (csrfToken) {
-                                            xhr.setRequestHeader("X-CSRFToken", csrfToken);
-                                        }
+                    ajaxCalls.push($.ajax({
+                        method: queryArray[idx].method,
+                        url: queryArray[idx].url,
+                        data: JSON.stringify(queryArray[idx].data),
+                        beforeSend: function(xhr, settings) {
+                            var authToken = vm._getAuthToken();
+                            if (authToken) {
+                                xhr.setRequestHeader("Authorization",
+                                    "Bearer " + authToken);
+                            } else {
+                                if (!vm._csrfSafeMethod(settings.type)) {
+                                    var csrfToken = vm._getCSRFToken();
+                                    if (csrfToken) {
+                                        xhr.setRequestHeader("X-CSRFToken", csrfToken);
                                     }
                                 }
-                            },
-                            contentType: 'application/json',
-                        });
-                    }());
+                            }
+                        },
+                        contentType: 'application/json',
+                    }));
                 }
-                jQuery.when(ajaxCalls).done(successCallback).fail(failureCallback);
+                jQuery.when.apply(jQuery, ajaxCalls).done(successCallback).fail(
+                    failureCallback);
             },
         }
     }
 
 
     var itemMixin = {
         mixins: [
@@ -1132,23 +1131,43 @@
         data: function() {
             return this.getInitData();
         },
         methods: {
             getInitData: function() {
                 var data = {
                     url: null,
+                    params: {
+                        // The following dates will be stored as `String` objects
+                        // as oppossed to `moment` or `Date` objects because this
+                        // is how form fields input="date" will update them.
+                        start_at: null,
+                        ends_at: null,
+                        // The timezone for both start_at and ends_at.
+                        timezone: 'local',
+                        q: '',
+                    },
                     itemsLoaded: false,
                     items: {
                         results: [],
                         count: 0
                     },
+                    mergeResults: false,
                     getCb: null,
+                    getCompleteCb: null,
                     getBeforeCb: null,
-                    params: {
-                        q: '',
+                }
+                if (this.$dateRange) {
+                    if (this.$dateRange.start_at) {
+                        data.params['start_at'] = this.$dateRange.start_at;
+                    }
+                    if (this.$dateRange.ends_at) {
+                        data.params['ends_at'] = this.$dateRange.ends_at;
+                    }
+                    if (this.$dateRange.timezone) {
+                        data.params['timezone'] = this.$dateRange.timezone;
                     }
                 }
                 return data;
             },
             get: function() {
                 var vm = this;
                 if (!vm.url) {
@@ -1185,29 +1204,33 @@
                             vm[vm.getCompleteCb]();
                         }
                     }
                 }
                 if (vm[vm.getBeforeCb]) {
                     vm[vm.getBeforeCb]();
                 }
+                vm.fetch(cb);
+            },
+            fetch: function(cb) {
+                let vm = this;
                 vm.lastGetParams = vm.getParams();
                 vm.reqGet(vm.url, vm.lastGetParams, cb);
             },
             reload: function() {
                 let vm = this;
                 for (let idx = 0; idx < vm.preReload.length; ++idx) {
                     vm[vm.preReload[idx]]();
                 }
                 vm.get();
             },
         },
     };
 
 
-    var TypeAhead = Vue.extend({
+    var typeAheadMixin = {
         mixins: [
             httpRequestMixin
         ],
         data: function data() {
             return {
                 url: null,
                 items: [],
@@ -1245,15 +1268,15 @@
                 var vm = this;
                 if (vm.current !== -1) {
                     vm.onHit(vm.items[vm.current]);
                 }
             },
 
             onHit: function onHit() {
-                Vue.util.warn('You need to implement the `onHit` method', this);
+                console.warn('You need to implement the `onHit` method', this);
             },
 
             reset: function() {
                 var vm = this;
                 vm.clear();
                 vm.query = '';
             },
@@ -1315,20 +1338,22 @@
                 return !this.query;
             },
             isDirty: function isDirty() {
                 return !!this.query;
             }
         },
         mounted: function() {
-            // do nothing.
+            if (this.$el.dataset && this.$el.dataset.url) {
+                this.url = this.$el.dataset.url;
+            }
         }
-    });
+    };
 
     // attach properties to the exports object to define
     // the exported module properties.
     exports.httpRequestMixin = httpRequestMixin;
     exports.itemListMixin = itemListMixin;
     exports.itemMixin = itemMixin;
     exports.messagesMixin = messagesMixin;
     exports.paramsMixin = paramsMixin;
-    exports.TypeAhead = TypeAhead;
+    exports.typeAheadMixin = typeAheadMixin;
 }));
```

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-resources.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-resources.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-sidebar-gallery.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-sidebar-gallery.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-style-editor.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-style-editor.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-themes-vue.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-themes-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/static/js/djaodjin-upload.js` & `djaodjin-extended-templates-0.4.3/extended_templates/static/js/djaodjin-upload.js`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/_body_bottom.html` & `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_body_bottom.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/_edit_tools.html` & `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/_edit_tools.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/edit.html` & `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/edit.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/templates/extended_templates/theme.html` & `djaodjin-extended-templates-0.4.3/extended_templates/templates/extended_templates/theme.html`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/templatetags/extended_templates_tags.py` & `djaodjin-extended-templates-0.4.3/extended_templates/templatetags/extended_templates_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/themes.py` & `djaodjin-extended-templates-0.4.3/extended_templates/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/thread_locals.py` & `djaodjin-extended-templates-0.4.3/extended_templates/thread_locals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/uploadhandler.py` & `djaodjin-extended-templates-0.4.3/extended_templates/uploadhandler.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/urls/__init__.py` & `djaodjin-extended-templates-0.4.3/extended_templates/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/urls/api/__init__.py` & `djaodjin-extended-templates-0.4.3/extended_templates/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/urls/api/assets.py` & `djaodjin-extended-templates-0.4.3/extended_templates/urls/api/assets.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/urls/api/templates.py` & `djaodjin-extended-templates-0.4.3/extended_templates/urls/api/templates.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/urls/views/__init__.py` & `djaodjin-extended-templates-0.4.3/extended_templates/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/urls/views/themes.py` & `djaodjin-extended-templates-0.4.3/extended_templates/urls/views/themes.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/utils.py` & `djaodjin-extended-templates-0.4.3/extended_templates/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,25 +153,28 @@
     # default implementation
     storage_class = get_storage_class()
     if 's3boto' in storage_class.__name__.lower():
         storage_kwargs = {}
         storage_kwargs.update(**kwargs)
         if public:
             storage_kwargs.update({'default_acl': 'public-read'})
-        for key in ['access_key', 'secret_key', 'security_token']:
+        for key in ['access_key', 'secret_key']:
             if key in request.session:
                 storage_kwargs[key] = request.session[key]
         bucket_name = _get_bucket_name(account)
         location = _get_media_prefix(account)
         LOGGER.debug("create %s(bucket_name='%s', location='%s', %s)",
             storage_class.__name__, bucket_name, location, storage_kwargs)
-        return storage_class(bucket_name=bucket_name, location=location,
+        storage = storage_class(bucket_name=bucket_name, location=location,
             **storage_kwargs)
-    LOGGER.debug("``%s`` does not contain a ``bucket_name``"\
-        " field, default to FileSystemStorage.", storage_class)
+        if 'security_token' in request.session:
+            storage.security_token = request.session['security_token']
+        return storage
+    LOGGER.debug("``%s`` does not contain ``s3boto`` in its name,"\
+        " default to FileSystemStorage.", storage_class)
     return _get_file_system_storage(account)
 
 
 def _get_bucket_name(account=None):
     if account:
         for bucket_field in settings.BUCKET_NAME_FROM_FIELDS:
             try:
```

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/views/pages.py` & `djaodjin-extended-templates-0.4.3/extended_templates/views/pages.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/views/static.py` & `djaodjin-extended-templates-0.4.3/extended_templates/views/static.py`

 * *Files identical despite different names*

### Comparing `djaodjin-extended-templates-0.4.2/extended_templates/views/themes.py` & `djaodjin-extended-templates-0.4.3/extended_templates/views/themes.py`

 * *Files identical despite different names*

