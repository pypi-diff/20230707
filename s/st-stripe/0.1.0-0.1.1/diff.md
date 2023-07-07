# Comparing `tmp/st-stripe-0.1.0.tar.gz` & `tmp/st-stripe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-stripe-0.1.0.tar", last modified: Fri Jul  7 01:42:07 2023, max compression
+gzip compressed data, was "st-stripe-0.1.1.tar", last modified: Fri Jul  7 02:14:03 2023, max compression
```

## Comparing `st-stripe-0.1.0.tar` & `st-stripe-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 01:42:07.439068 st-stripe-0.1.0/
--rw-r--r--   0 trichards   (501) staff       (20)      237 2023-07-07 01:42:07.438879 st-stripe-0.1.0/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     4413 2023-07-04 16:49:26.000000 st-stripe-0.1.0/README.md
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-07 01:42:07.439131 st-stripe-0.1.0/setup.cfg
--rw-r--r--   0 trichards   (501) staff       (20)      441 2023-07-07 01:38:59.000000 st-stripe-0.1.0/setup.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 01:42:07.438544 st-stripe-0.1.0/st_stripe.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)      237 2023-07-07 01:42:07.000000 st-stripe-0.1.0/st_stripe.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      182 2023-07-07 01:42:07.000000 st-stripe-0.1.0/st_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 01:42:07.000000 st-stripe-0.1.0/st_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       35 2023-07-07 01:42:07.000000 st-stripe-0.1.0/st_stripe.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 01:42:07.000000 st-stripe-0.1.0/st_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 02:14:03.277280 st-stripe-0.1.1/
+-rw-r--r--   0 trichards   (501) staff       (20)      237 2023-07-07 02:14:03.276666 st-stripe-0.1.1/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     5205 2023-07-07 02:13:03.000000 st-stripe-0.1.1/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-07 02:14:03.277340 st-stripe-0.1.1/setup.cfg
+-rw-r--r--   0 trichards   (501) staff       (20)      441 2023-07-07 02:09:11.000000 st-stripe-0.1.1/setup.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 02:14:03.275493 st-stripe-0.1.1/st_stripe.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)      237 2023-07-07 02:14:03.000000 st-stripe-0.1.1/st_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      182 2023-07-07 02:14:03.000000 st-stripe-0.1.1/st_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 02:14:03.000000 st-stripe-0.1.1/st_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       35 2023-07-07 02:14:03.000000 st-stripe-0.1.1/st_stripe.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 02:14:03.000000 st-stripe-0.1.1/st_stripe.egg-info/top_level.txt
```

### Comparing `st-stripe-0.1.0/README.md` & `st-stripe-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -56,7 +56,25 @@
 ```toml
 client_id = '1234.....googleusercontent.com'
 client_secret = 'GOC...'
 redirect_url = 'http://localhost.com:8501'
 ```
 
 The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it!
+
+### Testing Mode
+
+You can also test this package out by going into 'testing mode', which will look for different credentials in your secrets.toml file. To activate test mode, go ahead and the following to the top of your secrets file.
+
+```toml
+testing_mode = true
+```
+
+After this, add test urls, api keys, and links to your secrets like so.
+
+```toml
+redirect_url_test = "your_google_test_client_id"
+stripe_api_key_test = "your_stripe_test_api_key"
+stripe_link_test = "your_stripe_test_link"
+```
+
+With testing mode enabled, you can safely test your Streamlit app's authentication and subscription functionality without affecting real user data or transactions. When you're ready to deploy your app, simply set testing_mode to false in your secrets.toml file to use the production credentials.
```

