# Comparing `tmp/socid-extractor-0.0.8.tar.gz` & `tmp/socid-extractor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socid-extractor-0.0.8.tar", last modified: Wed Feb  3 18:52:42 2021, max compression
+gzip compressed data, was "socid-extractor-0.0.9.tar", last modified: Sat Feb  6 15:24:32 2021, max compression
```

## Comparing `socid-extractor-0.0.8.tar` & `socid-extractor-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-03 18:52:42.709587 socid-extractor-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      382 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       80 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3545 2021-02-03 18:52:42.709587 socid-extractor-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2688 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      106 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-03 18:52:42.709587 socid-extractor-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      648 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-03 18:52:42.709587 socid-extractor-0.0.8/socid_extractor/
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1038 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/activation.py
--rw-r--r--   0 runner    (1001) docker     (116)     3386 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     3622 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     1692 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/matching.py
--rw-r--r--   0 runner    (1001) docker     (116)    44340 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/schemes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/socid_extractor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-03 18:52:42.709587 socid-extractor-0.0.8/socid_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3545 2021-02-03 18:52:42.000000 socid-extractor-0.0.8/socid_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      535 2021-02-03 18:52:42.000000 socid-extractor-0.0.8/socid_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-03 18:52:42.000000 socid-extractor-0.0.8/socid_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2021-02-03 18:52:42.000000 socid-extractor-0.0.8/socid_extractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-03 18:52:42.000000 socid-extractor-0.0.8/socid_extractor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       22 2021-02-03 18:52:42.000000 socid-extractor-0.0.8/socid_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-03 18:52:42.709587 socid-extractor-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    27916 2021-02-03 18:52:32.000000 socid-extractor-0.0.8/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 15:24:32.063514 socid-extractor-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      467 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     3813 2021-02-06 15:24:32.063514 socid-extractor-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2900 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      106 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-06 15:24:32.067514 socid-extractor-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      648 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 15:24:32.063514 socid-extractor-0.0.9/socid_extractor/
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1038 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/activation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3386 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3822 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1692 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/matching.py
+-rw-r--r--   0 runner    (1001) docker     (116)    45997 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1135 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/socid_extractor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 15:24:32.063514 socid-extractor-0.0.9/socid_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3813 2021-02-06 15:24:31.000000 socid-extractor-0.0.9/socid_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      535 2021-02-06 15:24:31.000000 socid-extractor-0.0.9/socid_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-06 15:24:31.000000 socid-extractor-0.0.9/socid_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2021-02-06 15:24:31.000000 socid-extractor-0.0.9/socid_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-06 15:24:31.000000 socid-extractor-0.0.9/socid_extractor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2021-02-06 15:24:31.000000 socid-extractor-0.0.9/socid_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 15:24:32.063514 socid-extractor-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    28005 2021-02-06 15:24:20.000000 socid-extractor-0.0.9/tests/test_e2e.py
```

### Comparing `socid-extractor-0.0.8/LICENSE` & `socid-extractor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `socid-extractor-0.0.8/PKG-INFO` & `socid-extractor-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: socid-extractor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extract accounts' identifiers from personal pages on various platforms
 Home-page: https://github.com/soxoj/socid-extractor
 Author: Soxoj
 Author-email: soxoj@protonmail.com
 License: GPL-3.0
 Description: # socid_extractor
-        Extract accounts' identifiers and other info from personal pages on popular sites.
+        
+        Extract information about a user from profile webpages / API responses and save it in machine-readable format.
         
         ## When it may be useful
         
-        - Getting additional info by the username or/and account UID. Examples: [Week in OSINT - Getting a Grasp on GoogleID’s](https://medium.com/week-in-osint/getting-a-grasp-on-googleids-77a8ab707e43), [OSINTCurious - searching Instagram](https://osintcurio.us/2019/10/01/searching-instagram-part-2/)
+        - Getting all available info by the username or/and account UID. Examples: [Week in OSINT](https://medium.com/week-in-osint/getting-a-grasp-on-googleids-77a8ab707e43), [OSINTCurious](https://osintcurio.us/2019/10/01/searching-instagram-part-2/)
         - Searching by commonly used cross-service UIDs (GAIA ID, Facebook UID, Yandex Public ID, etc.)
           - DB leaks of forums and platforms in SQL format
           - Indexed links that contain target profile ID
         - Searching for tracking data by comparison with other IDs - [how it works](https://www.eff.org/wp/behind-the-one-way-mirror), [how can it be used](https://www.nytimes.com/interactive/2019/12/19/opinion/location-tracking-cell-phone.html).
         - Checking that the account was previously known (by ID) even if all public info has changed
         
         ## Tools using socid_extractor
         
         [Maigret](https://github.com/soxoj/maigret) - powerful namechecker, generate a report with all available info from accounts found. 
         
+        [YaSeeker](https://github.com/HowToFind-bot/YaSeeker) - tool to gather all available information about Yandex account by login/email.
+        
         ## Installation
         
             $ pip3 install socid-extractor
         
         The latest development version can be installed directly from GitHub:
         
             $ pip3 install -U git+https://github.com/soxoj/socid_extractor.git
@@ -40,15 +43,18 @@
         gender: female
         username: Muse1908
         website: www.patreon.com/musemercier
         links: ['https://www.facebook.com/musemercier', 'https://www.instagram.com/muse.mercier/', 'https://www.patreon.com/musemercier']
         tagline: Nothing worth having is easy...
         ```
         
-        Or simply `./run.py --url https://vimeo.com/alexaimephotography`
+        Without installing: 
+        ```
+        $ ./run.py --url https://www.deviantart.com/muse1908
+        ```
         
         As a Python library:
         ```
         >>> import socid_extractor, requests
         >>> r = requests.get('https://www.patreon.com/annetlovart')
         >>> socid_extractor.extract(r.text)
         {'patreon_id': '33913189', 'patreon_username': 'annetlovart', 'fullname': 'Annet Lovart', 'links': "['https://www.facebook.com/322598031832479', 'https://www.instagram.com/annet_lovart', 'https://twitter.com/annet_lovart', 'https://youtube.com/channel/UClDg4ntlOW_1j73zqSJxHHQ']"}
@@ -59,19 +65,20 @@
         - Google (all documents pages, maps contributions), cookies required
         - Yandex (disk, albums, znatoki, music, realty, collections), cookies required to prevent captcha blocks
         - Facebook (user & group pages)
         - Instagram
         - Reddit
         - Medium
         - Flickr
+        - Tumblr
         - TikTok
         - GitHub
         - VK (user page)
         - OK (user page)
         - Mail.ru (my.mail.ru user mainpage, photo, video, games, communities)
         
         ...and many others.
         
-        Check [tests file](./tests/test_e2e.py) for extracted data examples.
+        Check [tests file](./tests/test_e2e.py) for extracted data examples, [schemes file](./socid_extractor/schemes.py) to check all supported sites.
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socid-extractor-0.0.8/README.md` & `socid-extractor-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # socid_extractor
-Extract accounts' identifiers and other info from personal pages on popular sites.
+
+Extract information about a user from profile webpages / API responses and save it in machine-readable format.
 
 ## When it may be useful
 
-- Getting additional info by the username or/and account UID. Examples: [Week in OSINT - Getting a Grasp on GoogleID’s](https://medium.com/week-in-osint/getting-a-grasp-on-googleids-77a8ab707e43), [OSINTCurious - searching Instagram](https://osintcurio.us/2019/10/01/searching-instagram-part-2/)
+- Getting all available info by the username or/and account UID. Examples: [Week in OSINT](https://medium.com/week-in-osint/getting-a-grasp-on-googleids-77a8ab707e43), [OSINTCurious](https://osintcurio.us/2019/10/01/searching-instagram-part-2/)
 - Searching by commonly used cross-service UIDs (GAIA ID, Facebook UID, Yandex Public ID, etc.)
   - DB leaks of forums and platforms in SQL format
   - Indexed links that contain target profile ID
 - Searching for tracking data by comparison with other IDs - [how it works](https://www.eff.org/wp/behind-the-one-way-mirror), [how can it be used](https://www.nytimes.com/interactive/2019/12/19/opinion/location-tracking-cell-phone.html).
 - Checking that the account was previously known (by ID) even if all public info has changed
 
 ## Tools using socid_extractor
 
 [Maigret](https://github.com/soxoj/maigret) - powerful namechecker, generate a report with all available info from accounts found. 
 
+[YaSeeker](https://github.com/HowToFind-bot/YaSeeker) - tool to gather all available information about Yandex account by login/email.
+
 ## Installation
 
     $ pip3 install socid-extractor
 
 The latest development version can be installed directly from GitHub:
 
     $ pip3 install -U git+https://github.com/soxoj/socid_extractor.git
@@ -32,15 +35,18 @@
 gender: female
 username: Muse1908
 website: www.patreon.com/musemercier
 links: ['https://www.facebook.com/musemercier', 'https://www.instagram.com/muse.mercier/', 'https://www.patreon.com/musemercier']
 tagline: Nothing worth having is easy...
 ```
 
-Or simply `./run.py --url https://vimeo.com/alexaimephotography`
+Without installing: 
+```
+$ ./run.py --url https://www.deviantart.com/muse1908
+```
 
 As a Python library:
 ```
 >>> import socid_extractor, requests
 >>> r = requests.get('https://www.patreon.com/annetlovart')
 >>> socid_extractor.extract(r.text)
 {'patreon_id': '33913189', 'patreon_username': 'annetlovart', 'fullname': 'Annet Lovart', 'links': "['https://www.facebook.com/322598031832479', 'https://www.instagram.com/annet_lovart', 'https://twitter.com/annet_lovart', 'https://youtube.com/channel/UClDg4ntlOW_1j73zqSJxHHQ']"}
@@ -51,16 +57,17 @@
 - Google (all documents pages, maps contributions), cookies required
 - Yandex (disk, albums, znatoki, music, realty, collections), cookies required to prevent captcha blocks
 - Facebook (user & group pages)
 - Instagram
 - Reddit
 - Medium
 - Flickr
+- Tumblr
 - TikTok
 - GitHub
 - VK (user page)
 - OK (user page)
 - Mail.ru (my.mail.ru user mainpage, photo, video, games, communities)
 
 ...and many others.
 
-Check [tests file](./tests/test_e2e.py) for extracted data examples.
+Check [tests file](./tests/test_e2e.py) for extracted data examples, [schemes file](./socid_extractor/schemes.py) to check all supported sites.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socid-extractor-0.0.8/setup.py` & `socid-extractor-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 )
 
 
 with open('README.md') as fh:
     long_description = fh.read()
 
 setup(name='socid-extractor',
-      version='0.0.8',
+      version='0.0.9',
       description='Extract accounts\' identifiers from personal pages on various platforms',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/soxoj/socid-extractor',
       entry_points={'console_scripts': ['socid_extractor = socid_extractor.cli:run']},
       packages=find_packages(),
       author='Soxoj',
```

### Comparing `socid-extractor-0.0.8/socid_extractor/activation.py` & `socid-extractor-0.0.9/socid_extractor/activation.py`

 * *Files identical despite different names*

### Comparing `socid-extractor-0.0.8/socid_extractor/cli.py` & `socid-extractor-0.0.9/socid_extractor/cli.py`

 * *Files identical despite different names*

### Comparing `socid-extractor-0.0.8/socid_extractor/main.py` & `socid-extractor-0.0.9/socid_extractor/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
                 transforms = scheme_data.get('transforms', [])
                 if transforms:
                     for t in transforms:
                         logging.debug(t)
                         try:
                             extracted = t(extracted)
-                        except KeyError as e:
+                        except (AttributeError, KeyError) as e:
                             logging.debug(f'Transform error: {e}')
                             extracted = {}
                         logging.debug(extracted)
 
                 json_data = json.loads(extracted)
 
                 if json_data == {}:
@@ -81,25 +81,28 @@
 
                 logging.debug(loaded_json_str)
                 if logging.root.level == logging.DEBUG:
                     with open('debug_extracted.json', 'w') as f:
                         f.write(loaded_json_str)
 
                 for name, get_field in scheme_data['fields'].items():
-                    value = get_field(json_data)
-                    values[name] = str(value) if value != None else ''
+                    try:
+                        value = get_field(json_data)
+                        values[name] = str(value) if value != None else ''
+                    except (AttributeError, KeyError) as e:
+                        logging.debug(f'Unable to extact field {name}: {e}')
             else:
                 values = regexp_group.groupdict()
 
         if use_html_parser:
             soup = bs(page, 'html.parser')
             for name, get_field in scheme_data['fields'].items():
                 try:
                     value = get_field(soup)
                     values[name] = str(value) if value != None else ''
-                except AttributeError as e:
+                except (AttributeError, KeyError) as e:
                     logging.debug(f'BS extract error: {e}')
 
         return {a: b for a, b in values.items() if b or type(b) == bool}
 
     # all schemes have been checked
     return {}
```

### Comparing `socid-extractor-0.0.8/socid_extractor/matching.py` & `socid-extractor-0.0.9/socid_extractor/matching.py`

 * *Files identical despite different names*

### Comparing `socid-extractor-0.0.8/socid_extractor/schemes.py` & `socid-extractor-0.0.9/socid_extractor/schemes.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,40 @@
                 'uid': a['userid'],
                 'username': a['username'],
                 'profile_id': a['profile_id']
             } for a in x.get('social')],
             'links': lambda x: list(itertools.chain(*[l.get('addresses') for l in x.get('social', [])])),
         },
     },
+    'Yandex Music API': {
+        'flags': ['invocationInfo', 'req-id"'],
+        'regex': r'^(.+)$',
+        'extract_json': True,
+        'transforms': [
+            json.loads,
+            lambda x: x.get('result', {}),
+            json.dumps,
+        ],
+        'fields': {
+            'username': lambda x: x.get('login'),
+            'yandex_uid': lambda x: x.get('uid'),
+            'yandex_public_id': lambda x: x.get('publicId'),
+            'fullname': lambda x: x.get('fullName'),
+            'links': lambda x: x.get('socialProfiles'),
+            'is_verified': lambda x: x.get('verified'),
+            'has_tracks': lambda x: x.get('statistics', {}).get('hasTracks'),
+            'liked_users': lambda x: x.get('statistics', {}).get('likedUsers'),
+            'liked_by_users': lambda x: x.get('statistics', {}).get('likedByUsers'),
+            'liked_artists': lambda x: x.get('statistics', {}).get('likedArtists'),
+            'liked_albums': lambda x: x.get('statistics', {}).get('likedAlbums'),
+            'ugc_tracks_count': lambda x: x.get('statistics', {}).get('ugcTracks'),
+            'is_private_statistics': lambda x: x.get('statistics') == 'private',
+            'is_private_social_profiles': lambda x: x.get('socialProfiles') == 'private',
+        },
+    },
     'Yandex Realty offer': {
         'flags': ['realty.yandex.ru/offer'],
         'regex': r'({"routing":{"locationBeforeTransitions.+?});',
         'extract_json': True,
         'fields': {
             'your_yuid': lambda x: x['user']['yuid'],
             'your_uid': lambda x: x['user']['uid'],
@@ -886,9 +912,17 @@
         'flags': ['https://assets.tumblr.com'],
         'bs': True,
         'fields': {
             'fullname': lambda x: x.find('h1', {'class': 'blog-title'}).find('a').text,
             'title': lambda x: x.find('div', {'class': 'title-group'}).find('span', {'class': 'description'}).text.strip(),
             'links': lambda x: [enrich_link(a.find('a').get('href')) for a in x.find('div', {'class': 'nav-wrapper'}).find_all('li', {'class': 'nav-item nav-item--page'})],
         }
+    },
+    '1x.com': {
+        'flags': ['content="https://www.1x.com/'],
+        'bs': True,
+        'fields': {
+            'fullname': lambda x: x.find('div', {'class': 'coveroverlay'}).find('td', {'valign': 'bottom'}).find('div').contents[0],
+            'image': lambda x:  'https://1x.com/' + x.find('img', {'class': 'member_profilepic'}).get('src', ''),
+        }
     }
 }
```

### Comparing `socid-extractor-0.0.8/socid_extractor/utils.py` & `socid-extractor-0.0.9/socid_extractor/utils.py`

 * *Files identical despite different names*

### Comparing `socid-extractor-0.0.8/socid_extractor.egg-info/PKG-INFO` & `socid-extractor-0.0.9/socid_extractor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: socid-extractor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extract accounts' identifiers from personal pages on various platforms
 Home-page: https://github.com/soxoj/socid-extractor
 Author: Soxoj
 Author-email: soxoj@protonmail.com
 License: GPL-3.0
 Description: # socid_extractor
-        Extract accounts' identifiers and other info from personal pages on popular sites.
+        
+        Extract information about a user from profile webpages / API responses and save it in machine-readable format.
         
         ## When it may be useful
         
-        - Getting additional info by the username or/and account UID. Examples: [Week in OSINT - Getting a Grasp on GoogleID’s](https://medium.com/week-in-osint/getting-a-grasp-on-googleids-77a8ab707e43), [OSINTCurious - searching Instagram](https://osintcurio.us/2019/10/01/searching-instagram-part-2/)
+        - Getting all available info by the username or/and account UID. Examples: [Week in OSINT](https://medium.com/week-in-osint/getting-a-grasp-on-googleids-77a8ab707e43), [OSINTCurious](https://osintcurio.us/2019/10/01/searching-instagram-part-2/)
         - Searching by commonly used cross-service UIDs (GAIA ID, Facebook UID, Yandex Public ID, etc.)
           - DB leaks of forums and platforms in SQL format
           - Indexed links that contain target profile ID
         - Searching for tracking data by comparison with other IDs - [how it works](https://www.eff.org/wp/behind-the-one-way-mirror), [how can it be used](https://www.nytimes.com/interactive/2019/12/19/opinion/location-tracking-cell-phone.html).
         - Checking that the account was previously known (by ID) even if all public info has changed
         
         ## Tools using socid_extractor
         
         [Maigret](https://github.com/soxoj/maigret) - powerful namechecker, generate a report with all available info from accounts found. 
         
+        [YaSeeker](https://github.com/HowToFind-bot/YaSeeker) - tool to gather all available information about Yandex account by login/email.
+        
         ## Installation
         
             $ pip3 install socid-extractor
         
         The latest development version can be installed directly from GitHub:
         
             $ pip3 install -U git+https://github.com/soxoj/socid_extractor.git
@@ -40,15 +43,18 @@
         gender: female
         username: Muse1908
         website: www.patreon.com/musemercier
         links: ['https://www.facebook.com/musemercier', 'https://www.instagram.com/muse.mercier/', 'https://www.patreon.com/musemercier']
         tagline: Nothing worth having is easy...
         ```
         
-        Or simply `./run.py --url https://vimeo.com/alexaimephotography`
+        Without installing: 
+        ```
+        $ ./run.py --url https://www.deviantart.com/muse1908
+        ```
         
         As a Python library:
         ```
         >>> import socid_extractor, requests
         >>> r = requests.get('https://www.patreon.com/annetlovart')
         >>> socid_extractor.extract(r.text)
         {'patreon_id': '33913189', 'patreon_username': 'annetlovart', 'fullname': 'Annet Lovart', 'links': "['https://www.facebook.com/322598031832479', 'https://www.instagram.com/annet_lovart', 'https://twitter.com/annet_lovart', 'https://youtube.com/channel/UClDg4ntlOW_1j73zqSJxHHQ']"}
@@ -59,19 +65,20 @@
         - Google (all documents pages, maps contributions), cookies required
         - Yandex (disk, albums, znatoki, music, realty, collections), cookies required to prevent captcha blocks
         - Facebook (user & group pages)
         - Instagram
         - Reddit
         - Medium
         - Flickr
+        - Tumblr
         - TikTok
         - GitHub
         - VK (user page)
         - OK (user page)
         - Mail.ru (my.mail.ru user mainpage, photo, video, games, communities)
         
         ...and many others.
         
-        Check [tests file](./tests/test_e2e.py) for extracted data examples.
+        Check [tests file](./tests/test_e2e.py) for extracted data examples, [schemes file](./socid_extractor/schemes.py) to check all supported sites.
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socid-extractor-0.0.8/socid_extractor.egg-info/SOURCES.txt` & `socid-extractor-0.0.9/socid_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socid-extractor-0.0.8/tests/test_e2e.py` & `socid-extractor-0.0.9/tests/test_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import pytest
 
 from socid_extractor.activation import get_twitter_headers
-from socid_extractor.main import parse, extract
+from socid_extractor.main import parse, extract, HEADERS
 
 
 def test_vk_user_profile_full():
     info = extract(parse('https://vk.com/idsvyatoslavs')[0])
 
     assert info.get('vk_id') == '134173165'
     assert info.get('vk_username') == 'idsvyatoslavs'
@@ -51,15 +51,15 @@
     assert info.get('reviews_count') == '1'
     assert info.get('following_count') == '0'
     assert info.get('follower_count') == '0'
 
 
 @pytest.mark.skip(reason="failed from github CI infra IPs")
 def test_instagram():
-    info = extract(parse('https://www.instagram.com/alexaimephotography/')[0])
+    info = extract(parse('https://www.instagram.com/alexaimephotography/', headers=HEADERS)[0])
 
     assert info.get('uid') == '6828488620'
     assert info.get('username') == 'alexaimephotography'
     assert info.get('fullname') == 'Alexaimephotography'
     assert info.get('biography') == """🇮🇹 🇲🇫 🇩🇪
 Amateur photographer
 Follow me @street.reality.photography
@@ -224,14 +224,15 @@
     assert info.get('auId') == '6667000454247668890'
     assert info.get('email') == 'zubovo@mail.ru'
     assert info.get('isVip') == 'False'
     assert info.get('isCommunity') == 'False'
     assert info.get('isVideoChannel') == 'False'
 
 
+@pytest.mark.skip(reason="captcha")
 def test_yandex_music_user_profile():
     headers = {'referer': 'https://music.yandex.ru/users/pritisk/playlists'}
     info = extract(parse('https://music.yandex.ru/handlers/library.jsx?owner=pritisk', headers=headers)[0])
 
     assert info.get('yandex_uid') == '16480689'
     assert info.get('username') == 'pritisk'
     assert info.get('name') == 'Юрий Притиск'
@@ -313,14 +314,15 @@
 
     assert info.get('uid') == '39065909'
     assert info.get('username') == 'Skyratov'
     assert info.get('last_name') == 'Skuratov'
     assert info.get('first_name') == 'Vasiliy'
 
 
+@pytest.mark.github_failed
 def test_500px():
     info = extract(parse('https://api.500px.com/graphql?operationName=ProfileRendererQuery&variables=%7B%22username%22%3A%22the-maksimov%22%7D&extensions=%7B%22persistedQuery%22%3A%7B%22version%22%3A1%2C%22sha256Hash%22%3A%22105058632482dd2786fd5775745908dc928f537b28e28356b076522757d65c19%22%7D%7D')[0])
 
     assert info.get('uid') == 'dXJpOm5vZGU6VXNlcjoyMzg5Ng=='
     assert info.get('legacy_id') == '23896'
     assert info.get('username') == 'The-Maksimov'
     assert info.get('name') == 'Maxim Maximov'
```

