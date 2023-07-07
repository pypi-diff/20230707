# Comparing `tmp/zc.recipe.cmmi-3.0.0.tar.gz` & `tmp/zc.recipe.cmmi-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zc.recipe.cmmi-3.0.0.tar", last modified: Sat Mar 30 08:10:48 2019, max compression
+gzip compressed data, was "zc.recipe.cmmi-4.0.tar", last modified: Fri Jul  7 06:29:23 2023, max compression
```

## Comparing `zc.recipe.cmmi-3.0.0.tar` & `zc.recipe.cmmi-4.0.tar`

### file list

```diff
@@ -1,38 +1,35 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/
--rw-r--r--   0 mac        (501) staff       (20)    22232 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      721 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/test_all_pythons.cfg
--rw-r--r--   0 mac        (501) staff       (20)       32 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (501) staff       (20)      103 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/buildout.cfg
--rw-r--r--   0 mac        (501) staff       (20)       12 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/to-do.txt
--rw-r--r--   0 mac        (501) staff       (20)      190 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      154 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/.coveragerc
--rw-r--r--   0 mac        (501) staff       (20)     3395 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/setup.py
--rw-r--r--   0 mac        (501) staff       (20)      131 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)      250 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/tox.ini
--rw-r--r--   0 mac        (501) staff       (20)       67 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1707 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/README.rst
--rw-r--r--   0 mac        (501) staff       (20)     2070 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     3896 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)      623 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/.travis.yml
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/
--rw-r--r--   0 mac        (501) staff       (20)       76 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/
--rw-r--r--   0 mac        (501) staff       (20)     6046 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/downloadcache.rst
--rw-r--r--   0 mac        (501) staff       (20)    10602 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/shared.rst
--rw-r--r--   0 mac        (501) staff       (20)     8772 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     2666 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/patching.rst
--rw-r--r--   0 mac        (501) staff       (20)     2764 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/misc.rst
--rw-r--r--   0 mac        (501) staff       (20)    10095 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/README.rst
--rw-r--r--   0 mac        (501) staff       (20)     5520 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/tests.py
--rw-r--r--   0 mac        (501) staff       (20)       76 2019-03-30 08:10:47.000000 zc.recipe.cmmi-3.0.0/src/zc/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    22232 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        1 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/zip-safe
--rw-r--r--   0 mac        (501) staff       (20)       13 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)      769 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)       47 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       74 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        3 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2019-03-30 08:10:48.000000 zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/dependency_links.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-07 06:29:23.784245 zc.recipe.cmmi-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      514 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/.coveragerc
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4017 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      808 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      248 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17287 2023-07-07 06:29:23.784314 zc.recipe.cmmi-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1707 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      103 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      454 2023-07-07 06:29:23.784574 zc.recipe.cmmi-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3331 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-07 06:29:23.780008 zc.recipe.cmmi-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-07 06:29:23.781776 zc.recipe.cmmi-4.0/src/zc/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-07 06:29:23.783109 zc.recipe.cmmi-4.0/src/zc/recipe/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-07 06:29:23.784085 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10106 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8774 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6046 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/downloadcache.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2764 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/misc.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2666 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/patching.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10602 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/shared.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5208 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-07 06:29:23.782948 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17287 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      731 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       13 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        3 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1142 2023-07-07 06:29:23.000000 zc.recipe.cmmi-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zc.recipe.cmmi-3.0.0/PKG-INFO` & `zc.recipe.cmmi-4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,654 +1,661 @@
 Metadata-Version: 2.1
 Name: zc.recipe.cmmi
-Version: 3.0.0
+Version: 4.0
 Summary: ZC Buildout recipe for configure/make/make install
 Home-page: http://github.com/zopefoundation/zc.recipe.cmmi
 Author: Jim Fulton
 Author-email: jim@zope.com
 License: ZPL 2.1
-Description: ==============================================================
-         Recipe installing a download via configure/make/make install
-        ==============================================================
-        
-        The configure-make-make-install recipe automates installation of
-        configure-based source distribution into buildouts.
-        
-        .. contents::
-        
-        
-        Options
-        =======
-        
-        url
-           The URL of a source archive to download
-        
-        configure-command
-           The name of the configure script.
-        
-           The option defaults to ``./configure``.
-        
-        configure-options
-           Basic configure options.
-        
-           Defaults to a ``--prefix`` option that points to the part directory.
-        
-        extra_options
-           A string of extra options to pass to configure in *addition to* the
-           base options.
-        
-        environment
-           Optional environment variable settings of the forme NAME=VALUE.
-        
-           Newlines are ignored. Spaces may be included in environment values
-           as long as they can't be mistaken for environment settings.  So::
-        
-              environment = FOO=bar
-                            baz
-        
-           Sets the environment variable FOO, but::
-        
-              environment = FOO=bar xxx=baz
-        
-           Sets 2 environment values, FOO and xxx.
-        
-        patch
-           The name of an optional patch file to apply to the distribution.
-        
-        patch_options
-           Options to supply to the patch command (if a patch file is used).
-        
-           This defaults to ``-p0``
-        
-        shared
-           Share the build accross buildouts.
-        
-        autogen
-           The name of a script to run to generate a configure script.
-        
-        source-directory-contains
-           The name of a file in the distribution's source directory.
-        
-           This is used by the recipe to determine if it has found the source
-           directory. It defaults top "configure".
-        
-        
-        .. note::
-        
-            This recipe is not expected to work in a Microsoft Windows environment.
-        
-        =================
-         Release History
-        =================
-        
-        3.0.0 (2019-03-30)
-        ==================
-        
-        - Drop support for Python 3.4.
-        
-        - Add support for Python 3.7 and 3.8a2.
-        
-        - Flake8 the code.
-        
-        
-        2.0.0 (2017-06-21)
-        ==================
-        
-        - Add support for Python 3.4, 3.5, 3.6 and PyPy.
-        
-        - Automated testing is enabled on Travis CI.
-        
-        1.3.6 (2014-04-14)
-        ==================
-        
-        - Fixed: Strings were incorrectly compared using "is not ''" rather than !=
-        
-        - Fixed: Spaces weren't allowed in the installation location.
-        
-        1.3.5 (2011-08-06)
-        ==================
-        
-        - Fixed: Spaces weren't allowed in environment variables.
-        
-        - Fixed: Added missing option reference documentation.
-        
-        
-        1.3.4 (2011-01-18)
-        ==================
-        
-        - Fixed a bug in location book-keeping that caused shared builds to be deleted
-          from disk when a part didn't need them anymore. (#695977)
-        
-        - Made tests pass with both zc.buildout 1.4 and 1.5, lifted the upper version
-          bound on zc.buildout. (#695732)
-        
-        1.3.3 (2010-11-10)
-        ==================
-        
-        - Remove the temporary build directory when cmmi succeeds.
-        
-        - Specify that the zc.buildout version be <1.5.0b1, as the recipe is
-          currently not compatible with zc.buildout 1.5.
-        
-        1.3.2 (2010-08-09)
-        ==================
-        
-        - Remove the build directory for a shared build when the source cannot be
-          downloaded.
-        
-        - Declared a test dependency on zope.testing.
-        
-        
-        1.3.1 (2009-09-10)
-        ==================
-        
-        - Declare dependency on zc.buildout 1.4 or later. This dependency was introduced
-          in version 1.3.
-        
-        
-        1.3 (2009-09-03)
-        ================
-        
-        - Use zc.buildout's download API. As this allows MD5 checking, added the
-          md5sum and patch-md5sum options.
-        
-        - Added options for changing the name of the configure script and
-          overriding the ``--prefix`` parameter.
-        
-        - Moved the core "configure; make; make install" command sequence to a
-          method that can be overridden in other recipes, to support packages
-          whose installation process is slightly different.
-        
-        1.2.1 (2009-08-12)
-        ==================
-        
-        Bug fix: keep track of reused shared builds.
-        
-        
-        1.2.0 (2009-05-18)
-        ==================
-        
-        Enabled using a shared directory for completed builds.
-        
-        1.1.6 (2009-03-17)
-        ==================
-        
-        Moved 'zc' package from root of checkout into 'src', to prevent testrunner
-        from finding eggs installed locally by buildout.
-        
-        Removed deprecations under Python 2.6.
-        
-        1.1.5 (2008-11-07)
-        ==================
-        
-        - Added to the README.txt file a link to the SVN repository, so that Setuptools
-          can automatically find the development version when asked to install the
-          "-dev" version of zc.recipe.cmmi.
-        
-        - Applied fix for bug #261367 i.e. changed open() of file being downloaded to
-          binary, so that errors like the following no longer occur under Windows.
-        
-          uncompress = self.decompress.decompress(buf)
-          error: Error -3 while decompressing: invalid distance too far back
-        
-        1.1.4 (2008-06-25)
-        ==================
-        
-        Add support to autogen configure files.
-        
-        1.1.3 (2008-06-03)
-        ==================
-        
-        Add support for updating the environment.
-        
-        1.1.2 (2008-02-28)
-        ==================
-        
-        - Check if the ``location`` folder exists before creating it.
-        
-        After 1.1.0
-        ===========
-        
-        Added support for patches to be downloaded from a url rather than only using
-        patches on the filesystem
-        
-        1.1.0
-        =====
-        
-        Added support for:
-        
-         - download-cache: downloaded files are cached in the 'cmmi' subdirectory of
-           the cache cache keys are hashes of the url that the file was downloaded from
-           cache information recorded in the cache.ini file within each directory
-        
-         - offline mode: cmmi will not go online if the package is not in the cache
-        
-         - variable location: build files other than in the parts directory if required
-        
-         - additional logging/output
-        
-        1.0.2 (2007-06-03)
-        ==================
-        
-        - Added support for patches.
-        
-        - Tests fixed (buildout's output changed)
-        
-        1.0.1 (2006-11-22)
-        ==================
-        
-        - Added missing zip_safe flag.
-        
-        1.0 (2006-11-22)
-        ================
-        
-        Initial release.
-        
-        ======================
-        Detailed Documentation
-        ======================
-        
-        We have an archive with a demo foo tar ball and publish it by http in order
-        to see  offline effects:
-        
-            >>> ls(distros)
-            -  bar.tgz
-            -  baz.tgz
-            -  foo.tgz
-        
-            >>> distros_url = start_server(distros)
-        
-        Let's update a sample buildout to installs it:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... """ % distros_url)
-        
-        We used the url option to specify the location of the archive.
-        
-        If we run the buildout, the configure script in the archive is run.
-        It creates a make file which is also run:
-        
-            >>> print(system('bin/buildout').strip())
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample-buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        The recipe also creates the parts directory:
-        
-            >>> import os.path
-            >>> os.path.isdir(join(sample_buildout, "parts", "foo"))
-            True
-        
-        If we run the buildout again, the update method will be called, which
-        does nothing:
-        
-            >>> print(system('bin/buildout').strip())
-            Updating foo.
-        
-        You can supply extra configure options:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... extra_options = -a -b c
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample-buildout/parts/foo -a -b c
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        The recipe sets the location option, which can be read by other
-        recipes, to the location where the part is installed:
-        
-            >>> cat('.installed.cfg')
-            [buildout]
-            installed_develop_eggs =
-            parts = foo
-            <BLANKLINE>
-            [foo]
-        	...
-            location = /sample_buildout/parts/foo
-        	...
-        
-        It may be necessary to set some environment variables when running configure
-        or make. This can be done by adding an environment statement:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... environment =
-            ...   CFLAGS=-I/usr/lib/postgresql7.4/include
-            ... """ % distros_url)
-        
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            foo: Updating environment: CFLAGS=-I/usr/lib/postgresql7.4/include
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        Sometimes it's necessary to patch the sources before building a package.
-        You can specify the name of the patch to apply and (optional) patch options:
-        
-        First of all let's write a patchfile:
-        
-            >>> import sys
-            >>> mkdir('patches')
-            >>> write('patches/config.patch',
-            ... """--- configure
-            ... +++ /dev/null
-            ... @@ -1,13 +1,13 @@
-            ...  #!%s
-            ...  import sys
-            ... -print("configuring foo " + ' '.join(sys.argv[1:]))
-            ... +print("configuring foo patched " + ' '.join(sys.argv[1:]))
-            ...
-            ...  Makefile_template = '''
-            ...  all:
-            ... -\techo building foo
-            ... +\techo building foo patched
-            ...
-            ...  install:
-            ... -\techo installing foo
-            ... +\techo installing foo patched
-            ...  '''
-            ...
-            ...  with open('Makefile', 'w') as f:
-            ...      _ = f.write(Makefile_template)
-            ...
-            ... """ % sys.executable)
-        
-        Now let's create a buildout.cfg file. Note: If no patch option is beeing
-        passed, -p0 is appended by default.
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... patch_options = -p0
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            patching file configure
-            ...
-            configuring foo patched --prefix=/sample_buildout/parts/foo
-            echo building foo patched
-            building foo patched
-            echo installing foo patched
-            installing foo patched
-        
-        It is possible to autogenerate the configure files:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %s/bar.tgz
-            ... autogen = autogen.sh
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost//bar.tgz
-            foo: Unpacking and configuring
-            foo: auto generating configure files
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        It is also possible to support configure commands other than "./configure":
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %s/baz.tgz
-            ... source-directory-contains = configure.py
-            ... configure-command = ./configure.py
-            ... configure-options =
-            ...     --bindir=bin
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost//baz.tgz
-            foo: Unpacking and configuring
-            configuring foo --bindir=bin
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        When downloading a source archive or a patch, we can optionally make sure of
-        its authenticity by supplying an MD5 checksum that must be matched. If it
-        matches, we'll not be bothered with the check by buildout's output:
-        
-            >>> from hashlib import md5
-            >>> with open(join(distros, 'foo.tgz'), 'rb') as f:
-            ...     foo_md5sum = md5(f.read()).hexdigest()
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... md5sum = %s
-            ... """ % (distros_url, foo_md5sum))
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        But if the archive doesn't match the checksum, the recipe refuses to install:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sbar.tgz
-            ... md5sum = %s
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... """ % (distros_url, foo_md5sum))
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost:20617/bar.tgz
-            While:
-              Installing foo.
-            Error: MD5 checksum mismatch downloading 'http://localhost/bar.tgz'
-        
-        Similarly, a checksum mismatch for the patch will cause the buildout run to be
-        aborted:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... patch-md5sum = %s
-            ... """ % (distros_url, foo_md5sum))
-        
-            >>> print(system('bin/buildout').strip())
-            Installing foo.
-            foo: Downloading http://localhost:21669/foo.tgz
-            foo: Unpacking and configuring
-            While:
-              Installing foo.
-            Error: MD5 checksum mismatch for local resource at '/.../sample-buildout/patches/config.patch'.
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... """ % (distros_url))
-        
-        If the build fails, the temporary directory where the tarball was unpacked
-        is logged to stdout, and left intact for debugging purposes.
-        
-            >>> write('patches/config.patch', "dgdgdfgdfg")
-        
-            >>> res =  system('bin/buildout')
-            >>> print(res)
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            patch unexpectedly ends in middle of line
-            foo: cmmi failed: /.../...buildout-foo
-            patch: **** Only garbage was found in the patch input.
-            While:
-              Installing foo.
-            <BLANKLINE>
-            An internal error occurred due to a bug in either zc.buildout or in a
-            recipe being used:
-            ...
-            CalledProcessError: Command 'patch -p0 < ...' returned non-zero exit status ...
-            <BLANKLINE>
-        
-            >>> import re
-            >>> import os.path
-            >>> import shutil
-            >>> path = re.search('foo: cmmi failed: (.*)', res).group(1)
-            >>> os.path.exists(path)
-            True
-            >>> shutil.rmtree(path)
-        
-        After a successful build, such temporary directories are removed.
-        
-            >>> import glob
-            >>> import tempfile
-        
-            >>> old_tempdir = tempfile.gettempdir()
-            >>> tempdir = tempfile.tempdir = tempfile.mkdtemp(suffix='.buildout.build')
-            >>> dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... """ % (distros_url,))
-        
-            >>> print(system("bin/buildout"))
-            Installing foo.
-            foo: Downloading http://localhost:21445/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-            <BLANKLINE>
-        
-            >>> new_dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
-            >>> len(dirs) == len(new_dirs) == 0
-            True
-            >>> tempfile.tempdir = old_tempdir
-        
-        ==============
-        Download Cache
-        ==============
-        The recipe supports use of a download cache in the same way
-        as zc.buildout. See downloadcache.txt for details
-        
-        
 Keywords: zc.buildout buildout recipe cmmi configure make install
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Framework :: Buildout
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Software Distribution
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE.txt
+
+==============================================================
+ Recipe installing a download via configure/make/make install
+==============================================================
+
+The configure-make-make-install recipe automates installation of
+configure-based source distribution into buildouts.
+
+.. contents::
+
+
+Options
+=======
+
+url
+   The URL of a source archive to download
+
+configure-command
+   The name of the configure script.
+
+   The option defaults to ``./configure``.
+
+configure-options
+   Basic configure options.
+
+   Defaults to a ``--prefix`` option that points to the part directory.
+
+extra_options
+   A string of extra options to pass to configure in *addition to* the
+   base options.
+
+environment
+   Optional environment variable settings of the forme NAME=VALUE.
+
+   Newlines are ignored. Spaces may be included in environment values
+   as long as they can't be mistaken for environment settings.  So::
+
+      environment = FOO=bar
+                    baz
+
+   Sets the environment variable FOO, but::
+
+      environment = FOO=bar xxx=baz
+
+   Sets 2 environment values, FOO and xxx.
+
+patch
+   The name of an optional patch file to apply to the distribution.
+
+patch_options
+   Options to supply to the patch command (if a patch file is used).
+
+   This defaults to ``-p0``
+
+shared
+   Share the build accross buildouts.
+
+autogen
+   The name of a script to run to generate a configure script.
+
+source-directory-contains
+   The name of a file in the distribution's source directory.
+
+   This is used by the recipe to determine if it has found the source
+   directory. It defaults top "configure".
+
+
+.. note::
+
+    This recipe is not expected to work in a Microsoft Windows environment.
+
+=================
+ Release History
+=================
+
+4.0 (2023-07-07)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
+3.0.0 (2019-03-30)
+==================
+
+- Drop support for Python 3.4.
+
+- Add support for Python 3.7 and 3.8a2.
+
+- Flake8 the code.
+
+
+2.0.0 (2017-06-21)
+==================
+
+- Add support for Python 3.4, 3.5, 3.6 and PyPy.
+
+- Automated testing is enabled on Travis CI.
+
+1.3.6 (2014-04-14)
+==================
+
+- Fixed: Strings were incorrectly compared using "is not ''" rather than !=
+
+- Fixed: Spaces weren't allowed in the installation location.
+
+1.3.5 (2011-08-06)
+==================
+
+- Fixed: Spaces weren't allowed in environment variables.
+
+- Fixed: Added missing option reference documentation.
+
+
+1.3.4 (2011-01-18)
+==================
+
+- Fixed a bug in location book-keeping that caused shared builds to be deleted
+  from disk when a part didn't need them anymore. (#695977)
+
+- Made tests pass with both zc.buildout 1.4 and 1.5, lifted the upper version
+  bound on zc.buildout. (#695732)
+
+1.3.3 (2010-11-10)
+==================
+
+- Remove the temporary build directory when cmmi succeeds.
+
+- Specify that the zc.buildout version be <1.5.0b1, as the recipe is
+  currently not compatible with zc.buildout 1.5.
+
+1.3.2 (2010-08-09)
+==================
+
+- Remove the build directory for a shared build when the source cannot be
+  downloaded.
+
+- Declared a test dependency on zope.testing.
+
+
+1.3.1 (2009-09-10)
+==================
+
+- Declare dependency on zc.buildout 1.4 or later. This dependency was introduced
+  in version 1.3.
+
+
+1.3 (2009-09-03)
+================
+
+- Use zc.buildout's download API. As this allows MD5 checking, added the
+  md5sum and patch-md5sum options.
+
+- Added options for changing the name of the configure script and
+  overriding the ``--prefix`` parameter.
+
+- Moved the core "configure; make; make install" command sequence to a
+  method that can be overridden in other recipes, to support packages
+  whose installation process is slightly different.
+
+1.2.1 (2009-08-12)
+==================
+
+Bug fix: keep track of reused shared builds.
+
+
+1.2.0 (2009-05-18)
+==================
+
+Enabled using a shared directory for completed builds.
+
+1.1.6 (2009-03-17)
+==================
+
+Moved 'zc' package from root of checkout into 'src', to prevent testrunner
+from finding eggs installed locally by buildout.
+
+Removed deprecations under Python 2.6.
+
+1.1.5 (2008-11-07)
+==================
+
+- Added to the README.txt file a link to the SVN repository, so that Setuptools
+  can automatically find the development version when asked to install the
+  "-dev" version of zc.recipe.cmmi.
+
+- Applied fix for bug #261367 i.e. changed open() of file being downloaded to
+  binary, so that errors like the following no longer occur under Windows.
+
+  uncompress = self.decompress.decompress(buf)
+  error: Error -3 while decompressing: invalid distance too far back
+
+1.1.4 (2008-06-25)
+==================
+
+Add support to autogen configure files.
+
+1.1.3 (2008-06-03)
+==================
+
+Add support for updating the environment.
+
+1.1.2 (2008-02-28)
+==================
+
+- Check if the ``location`` folder exists before creating it.
+
+After 1.1.0
+===========
+
+Added support for patches to be downloaded from a url rather than only using
+patches on the filesystem
+
+1.1.0
+=====
+
+Added support for:
+
+ - download-cache: downloaded files are cached in the 'cmmi' subdirectory of
+   the cache cache keys are hashes of the url that the file was downloaded from
+   cache information recorded in the cache.ini file within each directory
+
+ - offline mode: cmmi will not go online if the package is not in the cache
+
+ - variable location: build files other than in the parts directory if required
+
+ - additional logging/output
+
+1.0.2 (2007-06-03)
+==================
+
+- Added support for patches.
+
+- Tests fixed (buildout's output changed)
+
+1.0.1 (2006-11-22)
+==================
+
+- Added missing zip_safe flag.
+
+1.0 (2006-11-22)
+================
+
+Initial release.
+
+======================
+Detailed Documentation
+======================
+
+We have an archive with a demo foo tar ball and publish it by http in order
+to see  offline effects:
+
+    >>> ls(distros)
+    -  bar.tgz
+    -  baz.tgz
+    -  foo.tgz
+
+    >>> distros_url = start_server(distros)
+
+Let's update a sample buildout to installs it:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... """ % distros_url)
+
+We used the url option to specify the location of the archive.
+
+If we run the buildout, the configure script in the archive is run.
+It creates a make file which is also run:
+
+    >>> print(system('bin/buildout').strip())
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample-buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+The recipe also creates the parts directory:
+
+    >>> import os.path
+    >>> os.path.isdir(join(sample_buildout, "parts", "foo"))
+    True
+
+If we run the buildout again, the update method will be called, which
+does nothing:
+
+    >>> print(system('bin/buildout').strip())
+    Updating foo.
+
+You can supply extra configure options:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... extra_options = -a -b c
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample-buildout/parts/foo -a -b c
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+The recipe sets the location option, which can be read by other
+recipes, to the location where the part is installed:
+
+    >>> cat('.installed.cfg')
+    [buildout]
+    installed_develop_eggs =
+    parts = foo
+    <BLANKLINE>
+    [foo]
+	...
+    location = /sample_buildout/parts/foo
+	...
+
+It may be necessary to set some environment variables when running configure
+or make. This can be done by adding an environment statement:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... environment =
+    ...   CFLAGS=-I/usr/lib/postgresql7.4/include
+    ... """ % distros_url)
+
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    foo: Updating environment: CFLAGS=-I/usr/lib/postgresql7.4/include
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+Sometimes it's necessary to patch the sources before building a package.
+You can specify the name of the patch to apply and (optional) patch options:
+
+First of all let's write a patchfile:
+
+    >>> import sys
+    >>> mkdir('patches')
+    >>> write('patches/config.patch',
+    ... """--- configure
+    ... +++ /dev/null
+    ... @@ -1,13 +1,13 @@
+    ...  #!%s
+    ...  import sys
+    ... -print("configuring foo " + ' '.join(sys.argv[1:]))
+    ... +print("configuring foo patched " + ' '.join(sys.argv[1:]))
+    ...
+    ...  Makefile_template = '''
+    ...  all:
+    ... -\techo building foo
+    ... +\techo building foo patched
+    ...
+    ...  install:
+    ... -\techo installing foo
+    ... +\techo installing foo patched
+    ...  '''
+    ...
+    ...  with open('Makefile', 'w') as f:
+    ...      _ = f.write(Makefile_template)
+    ...
+    ... """ % sys.executable)
+
+Now let's create a buildout.cfg file. Note: If no patch option is beeing
+passed, -p0 is appended by default.
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... patch_options = -p0
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    patching file configure
+    ...
+    configuring foo patched --prefix=/sample_buildout/parts/foo
+    echo building foo patched
+    building foo patched
+    echo installing foo patched
+    installing foo patched
+
+It is possible to autogenerate the configure files:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %s/bar.tgz
+    ... autogen = autogen.sh
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost//bar.tgz
+    foo: Unpacking and configuring
+    foo: auto generating configure files
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+It is also possible to support configure commands other than "./configure":
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %s/baz.tgz
+    ... source-directory-contains = configure.py
+    ... configure-command = ./configure.py
+    ... configure-options =
+    ...     --bindir=bin
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost//baz.tgz
+    foo: Unpacking and configuring
+    configuring foo --bindir=bin
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+When downloading a source archive or a patch, we can optionally make sure of
+its authenticity by supplying an MD5 checksum that must be matched. If it
+matches, we'll not be bothered with the check by buildout's output:
+
+    >>> from hashlib import md5
+    >>> with open(join(distros, 'foo.tgz'), 'rb') as f:
+    ...     foo_md5sum = md5(f.read()).hexdigest()
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... md5sum = %s
+    ... """ % (distros_url, foo_md5sum))
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+But if the archive doesn't match the checksum, the recipe refuses to install:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sbar.tgz
+    ... md5sum = %s
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... """ % (distros_url, foo_md5sum))
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost:20617/bar.tgz
+    While:
+      Installing foo.
+    Error: MD5 checksum mismatch downloading 'http://localhost/bar.tgz'
+
+Similarly, a checksum mismatch for the patch will cause the buildout run to be
+aborted:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... patch-md5sum = %s
+    ... """ % (distros_url, foo_md5sum))
+
+    >>> print(system('bin/buildout').strip())
+    Installing foo.
+    foo: Downloading http://localhost:21669/foo.tgz
+    foo: Unpacking and configuring
+    While:
+      Installing foo.
+    Error: MD5 checksum mismatch for local resource at '/.../sample-buildout/patches/config.patch'.
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... """ % (distros_url))
+
+If the build fails, the temporary directory where the tarball was unpacked
+is logged to stdout, and left intact for debugging purposes.
+
+    >>> write('patches/config.patch', "dgdgdfgdfg")
+
+    >>> res =  system('bin/buildout')
+    >>> print(res)
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    patch unexpectedly ends in middle of line
+    foo: cmmi failed: /.../...buildout-foo
+    patch: **** Only garbage was found in the patch input.
+    While:
+      Installing foo.
+    <BLANKLINE>
+    An internal error occurred due to a bug in either zc.buildout or in a
+    recipe being used:
+    ...
+    subprocess.CalledProcessError: Command 'patch -p0 < ...' returned non-zero exit status ...
+    <BLANKLINE>
+
+    >>> import re
+    >>> import os.path
+    >>> import shutil
+    >>> path = re.search('foo: cmmi failed: (.*)', res).group(1)
+    >>> os.path.exists(path)
+    True
+    >>> shutil.rmtree(path)
+
+After a successful build, such temporary directories are removed.
+
+    >>> import glob
+    >>> import tempfile
+
+    >>> old_tempdir = tempfile.gettempdir()
+    >>> tempdir = tempfile.tempdir = tempfile.mkdtemp(suffix='.buildout.build')
+    >>> dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... """ % (distros_url,))
+
+    >>> print(system("bin/buildout"))
+    Installing foo.
+    foo: Downloading http://localhost:21445/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+    <BLANKLINE>
+
+    >>> new_dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
+    >>> len(dirs) == len(new_dirs) == 0
+    True
+    >>> tempfile.tempdir = old_tempdir
+
+==============
+Download Cache
+==============
+The recipe supports use of a download cache in the same way
+as zc.buildout. See downloadcache.txt for details
+
```

### Comparing `zc.recipe.cmmi-3.0.0/setup.py` & `zc.recipe.cmmi-4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,47 +9,48 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
 name = "zc.recipe.cmmi"
 
 setup(
     name=name,
-    version='3.0.0',
+    version='4.0',
     author="Jim Fulton",
     author_email="jim@zope.com",
     description="ZC Buildout recipe for configure/make/make install",
     license="ZPL 2.1",
     keywords="zc.buildout buildout recipe cmmi configure make install",
     classifiers=[
-        "Environment :: Plugins",
-        "Framework :: Buildout",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Zope Public License",
-        "Topic :: Software Development :: Build Tools",
-        "Topic :: System :: Software Distribution",
+        'Environment :: Plugins',
+        'Framework :: Buildout',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Zope Public License',
+        'Topic :: Software Development :: Build Tools',
+        'Topic :: System :: Software Distribution',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
     ],
     url='http://github.com/zopefoundation/' + name,
     long_description=(
@@ -70,15 +71,15 @@
         'as zc.buildout. See downloadcache.txt for details\n'
         + '\n'
     ),
     package_dir={'': 'src'},
     packages=find_packages('src'),
     include_package_data=True,
     namespace_packages=['zc', 'zc.recipe'],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+    python_requires='>=3.7',
     install_requires=[
         'zc.buildout >= 2.9.4',
         'setuptools'],
     extras_require={
         'test': [
             # we import zc.buildout's 'test' package. It does have a
             # 'test' extra, but we really don't want all the things
```

### Comparing `zc.recipe.cmmi-3.0.0/README.rst` & `zc.recipe.cmmi-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `zc.recipe.cmmi-3.0.0/LICENSE.txt` & `zc.recipe.cmmi-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zc.recipe.cmmi-3.0.0/CHANGES.rst` & `zc.recipe.cmmi-4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =================
  Release History
 =================
 
+4.0 (2023-07-07)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
 3.0.0 (2019-03-30)
 ==================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.7 and 3.8a2.
```

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/downloadcache.rst` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/downloadcache.rst`

 * *Files identical despite different names*

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/shared.rst` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/shared.rst`

 * *Files identical despite different names*

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/__init__.py` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 
-from hashlib import sha1
 import logging
 import os
 import os.path
 import re
-import subprocess
-import setuptools.archive_util
 import shutil
+import subprocess
 import tempfile
+from hashlib import sha1
+
+import setuptools.archive_util
 import zc.buildout
 import zc.buildout.download
 
+
 almost_environment_setting = re.compile(r'\w+=').match
 not_starting_with_digit = re.compile(r'\D').match
 
 
 def system(c):
     subprocess.check_call(c, shell=True)
 
 
-class Recipe(object):
+class Recipe:
 
     def __init__(self, buildout, name, options):
         self.buildout, self.name, self.options = buildout, name, options
         directory = buildout['buildout']['directory']
         download_cache = buildout['buildout'].get('download-cache')
 
         self.url = self.options['url']
@@ -100,15 +102,15 @@
         options['location'] = location
 
     def _state_hash(self):
         # hash of our configuration state, so that e.g. different
         # ./configure options will get a different build directory.
         # Be sure to sort to keep a consistent order, since dictionary
         # iteration order is never guaranteed.
-        env = ''.join(['%s%s' % (key, value) for key, value
+        env = ''.join(['{}{}'.format(key, value) for key, value
                        in sorted(self.environ.items())])
         state = [self.url, self.extra_options, self.autogen,
                  self.patch, self.patch_options, env]
         data = ''.join(state)
         if not isinstance(data, bytes):
             data = data.encode('utf-8')
         return sha1(data).hexdigest()
@@ -217,10 +219,10 @@
         command sequence is different.
         """
         options = self.configure_options
         if options is None:
             options = '--prefix="%s"' % dest
         if self.extra_options:
             options += ' %s' % self.extra_options
-        system("%s %s" % (self.configure_cmd, options))
+        system("{} {}".format(self.configure_cmd, options))
         system("make")
         system("make install")
```

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/patching.rst` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/patching.rst`

 * *Files identical despite different names*

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/misc.rst` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/misc.rst`

 * *Files identical despite different names*

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/README.rst` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
     patch: **** Only garbage was found in the patch input.
     While:
       Installing foo.
     <BLANKLINE>
     An internal error occurred due to a bug in either zc.buildout or in a
     recipe being used:
     ...
-    CalledProcessError: Command 'patch -p0 < ...' returned non-zero exit status ...
+    subprocess.CalledProcessError: Command 'patch -p0 < ...' returned non-zero exit status ...
     <BLANKLINE>
 
     >>> import re
     >>> import os.path
     >>> import shutil
     >>> path = re.search('foo: cmmi failed: (.*)', res).group(1)
     >>> os.path.exists(path)
```

### Comparing `zc.recipe.cmmi-3.0.0/src/zc/recipe/cmmi/tests.py` & `zc.recipe.cmmi-4.0/src/zc/recipe/cmmi/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
+import doctest
 import os
 import re
-from io import BytesIO as _BytesIO
 import sys
 import tarfile
-import zc.buildout.testing
-
 import unittest
-import doctest
-from zope.testing import renormalizing
+from io import BytesIO as _BytesIO
+
+import zc.buildout.testing
 from zc.buildout.tests import normalize_bang
+from zope.testing import renormalizing
 
 
 def _as_bytes(s):
     return s.encode('utf-8') if not isinstance(s, bytes) else s
 
 
 def BytesIO(s):
@@ -109,22 +109,17 @@
                 (re.compile('occured'), 'occurred'),
                 # Buildout or setuptools has a bug not closing .egg-link files,
                 # leading to issues being reported by PyPy, which naturally
                 # mess up doctests.
                 (re.compile(
                     'Exception IOError: IOError.*finalizer of <closed file.*'),
                  ''),
-                # IGNORE_EXCEPTION_MODULE_IN_PYTHON2 fails because the output
-                # doesn't always look like a traceback.
-                (re.compile('subprocess.CalledProcessError'),
-                 'CalledProcessError'),
             ]),
             optionflags=(doctest.ELLIPSIS
-                         | doctest.NORMALIZE_WHITESPACE
-                         | renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2)
+                         | doctest.NORMALIZE_WHITESPACE)
         ),
         doctest.DocFileSuite(
             'downloadcache.rst',
             'patching.rst',
             'shared.rst',
             setUp=setUp,
             tearDown=tearDown,
```

### Comparing `zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/PKG-INFO` & `zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,654 +1,661 @@
 Metadata-Version: 2.1
 Name: zc.recipe.cmmi
-Version: 3.0.0
+Version: 4.0
 Summary: ZC Buildout recipe for configure/make/make install
 Home-page: http://github.com/zopefoundation/zc.recipe.cmmi
 Author: Jim Fulton
 Author-email: jim@zope.com
 License: ZPL 2.1
-Description: ==============================================================
-         Recipe installing a download via configure/make/make install
-        ==============================================================
-        
-        The configure-make-make-install recipe automates installation of
-        configure-based source distribution into buildouts.
-        
-        .. contents::
-        
-        
-        Options
-        =======
-        
-        url
-           The URL of a source archive to download
-        
-        configure-command
-           The name of the configure script.
-        
-           The option defaults to ``./configure``.
-        
-        configure-options
-           Basic configure options.
-        
-           Defaults to a ``--prefix`` option that points to the part directory.
-        
-        extra_options
-           A string of extra options to pass to configure in *addition to* the
-           base options.
-        
-        environment
-           Optional environment variable settings of the forme NAME=VALUE.
-        
-           Newlines are ignored. Spaces may be included in environment values
-           as long as they can't be mistaken for environment settings.  So::
-        
-              environment = FOO=bar
-                            baz
-        
-           Sets the environment variable FOO, but::
-        
-              environment = FOO=bar xxx=baz
-        
-           Sets 2 environment values, FOO and xxx.
-        
-        patch
-           The name of an optional patch file to apply to the distribution.
-        
-        patch_options
-           Options to supply to the patch command (if a patch file is used).
-        
-           This defaults to ``-p0``
-        
-        shared
-           Share the build accross buildouts.
-        
-        autogen
-           The name of a script to run to generate a configure script.
-        
-        source-directory-contains
-           The name of a file in the distribution's source directory.
-        
-           This is used by the recipe to determine if it has found the source
-           directory. It defaults top "configure".
-        
-        
-        .. note::
-        
-            This recipe is not expected to work in a Microsoft Windows environment.
-        
-        =================
-         Release History
-        =================
-        
-        3.0.0 (2019-03-30)
-        ==================
-        
-        - Drop support for Python 3.4.
-        
-        - Add support for Python 3.7 and 3.8a2.
-        
-        - Flake8 the code.
-        
-        
-        2.0.0 (2017-06-21)
-        ==================
-        
-        - Add support for Python 3.4, 3.5, 3.6 and PyPy.
-        
-        - Automated testing is enabled on Travis CI.
-        
-        1.3.6 (2014-04-14)
-        ==================
-        
-        - Fixed: Strings were incorrectly compared using "is not ''" rather than !=
-        
-        - Fixed: Spaces weren't allowed in the installation location.
-        
-        1.3.5 (2011-08-06)
-        ==================
-        
-        - Fixed: Spaces weren't allowed in environment variables.
-        
-        - Fixed: Added missing option reference documentation.
-        
-        
-        1.3.4 (2011-01-18)
-        ==================
-        
-        - Fixed a bug in location book-keeping that caused shared builds to be deleted
-          from disk when a part didn't need them anymore. (#695977)
-        
-        - Made tests pass with both zc.buildout 1.4 and 1.5, lifted the upper version
-          bound on zc.buildout. (#695732)
-        
-        1.3.3 (2010-11-10)
-        ==================
-        
-        - Remove the temporary build directory when cmmi succeeds.
-        
-        - Specify that the zc.buildout version be <1.5.0b1, as the recipe is
-          currently not compatible with zc.buildout 1.5.
-        
-        1.3.2 (2010-08-09)
-        ==================
-        
-        - Remove the build directory for a shared build when the source cannot be
-          downloaded.
-        
-        - Declared a test dependency on zope.testing.
-        
-        
-        1.3.1 (2009-09-10)
-        ==================
-        
-        - Declare dependency on zc.buildout 1.4 or later. This dependency was introduced
-          in version 1.3.
-        
-        
-        1.3 (2009-09-03)
-        ================
-        
-        - Use zc.buildout's download API. As this allows MD5 checking, added the
-          md5sum and patch-md5sum options.
-        
-        - Added options for changing the name of the configure script and
-          overriding the ``--prefix`` parameter.
-        
-        - Moved the core "configure; make; make install" command sequence to a
-          method that can be overridden in other recipes, to support packages
-          whose installation process is slightly different.
-        
-        1.2.1 (2009-08-12)
-        ==================
-        
-        Bug fix: keep track of reused shared builds.
-        
-        
-        1.2.0 (2009-05-18)
-        ==================
-        
-        Enabled using a shared directory for completed builds.
-        
-        1.1.6 (2009-03-17)
-        ==================
-        
-        Moved 'zc' package from root of checkout into 'src', to prevent testrunner
-        from finding eggs installed locally by buildout.
-        
-        Removed deprecations under Python 2.6.
-        
-        1.1.5 (2008-11-07)
-        ==================
-        
-        - Added to the README.txt file a link to the SVN repository, so that Setuptools
-          can automatically find the development version when asked to install the
-          "-dev" version of zc.recipe.cmmi.
-        
-        - Applied fix for bug #261367 i.e. changed open() of file being downloaded to
-          binary, so that errors like the following no longer occur under Windows.
-        
-          uncompress = self.decompress.decompress(buf)
-          error: Error -3 while decompressing: invalid distance too far back
-        
-        1.1.4 (2008-06-25)
-        ==================
-        
-        Add support to autogen configure files.
-        
-        1.1.3 (2008-06-03)
-        ==================
-        
-        Add support for updating the environment.
-        
-        1.1.2 (2008-02-28)
-        ==================
-        
-        - Check if the ``location`` folder exists before creating it.
-        
-        After 1.1.0
-        ===========
-        
-        Added support for patches to be downloaded from a url rather than only using
-        patches on the filesystem
-        
-        1.1.0
-        =====
-        
-        Added support for:
-        
-         - download-cache: downloaded files are cached in the 'cmmi' subdirectory of
-           the cache cache keys are hashes of the url that the file was downloaded from
-           cache information recorded in the cache.ini file within each directory
-        
-         - offline mode: cmmi will not go online if the package is not in the cache
-        
-         - variable location: build files other than in the parts directory if required
-        
-         - additional logging/output
-        
-        1.0.2 (2007-06-03)
-        ==================
-        
-        - Added support for patches.
-        
-        - Tests fixed (buildout's output changed)
-        
-        1.0.1 (2006-11-22)
-        ==================
-        
-        - Added missing zip_safe flag.
-        
-        1.0 (2006-11-22)
-        ================
-        
-        Initial release.
-        
-        ======================
-        Detailed Documentation
-        ======================
-        
-        We have an archive with a demo foo tar ball and publish it by http in order
-        to see  offline effects:
-        
-            >>> ls(distros)
-            -  bar.tgz
-            -  baz.tgz
-            -  foo.tgz
-        
-            >>> distros_url = start_server(distros)
-        
-        Let's update a sample buildout to installs it:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... """ % distros_url)
-        
-        We used the url option to specify the location of the archive.
-        
-        If we run the buildout, the configure script in the archive is run.
-        It creates a make file which is also run:
-        
-            >>> print(system('bin/buildout').strip())
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample-buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        The recipe also creates the parts directory:
-        
-            >>> import os.path
-            >>> os.path.isdir(join(sample_buildout, "parts", "foo"))
-            True
-        
-        If we run the buildout again, the update method will be called, which
-        does nothing:
-        
-            >>> print(system('bin/buildout').strip())
-            Updating foo.
-        
-        You can supply extra configure options:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... extra_options = -a -b c
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample-buildout/parts/foo -a -b c
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        The recipe sets the location option, which can be read by other
-        recipes, to the location where the part is installed:
-        
-            >>> cat('.installed.cfg')
-            [buildout]
-            installed_develop_eggs =
-            parts = foo
-            <BLANKLINE>
-            [foo]
-        	...
-            location = /sample_buildout/parts/foo
-        	...
-        
-        It may be necessary to set some environment variables when running configure
-        or make. This can be done by adding an environment statement:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... environment =
-            ...   CFLAGS=-I/usr/lib/postgresql7.4/include
-            ... """ % distros_url)
-        
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            foo: Updating environment: CFLAGS=-I/usr/lib/postgresql7.4/include
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        Sometimes it's necessary to patch the sources before building a package.
-        You can specify the name of the patch to apply and (optional) patch options:
-        
-        First of all let's write a patchfile:
-        
-            >>> import sys
-            >>> mkdir('patches')
-            >>> write('patches/config.patch',
-            ... """--- configure
-            ... +++ /dev/null
-            ... @@ -1,13 +1,13 @@
-            ...  #!%s
-            ...  import sys
-            ... -print("configuring foo " + ' '.join(sys.argv[1:]))
-            ... +print("configuring foo patched " + ' '.join(sys.argv[1:]))
-            ...
-            ...  Makefile_template = '''
-            ...  all:
-            ... -\techo building foo
-            ... +\techo building foo patched
-            ...
-            ...  install:
-            ... -\techo installing foo
-            ... +\techo installing foo patched
-            ...  '''
-            ...
-            ...  with open('Makefile', 'w') as f:
-            ...      _ = f.write(Makefile_template)
-            ...
-            ... """ % sys.executable)
-        
-        Now let's create a buildout.cfg file. Note: If no patch option is beeing
-        passed, -p0 is appended by default.
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... patch_options = -p0
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            patching file configure
-            ...
-            configuring foo patched --prefix=/sample_buildout/parts/foo
-            echo building foo patched
-            building foo patched
-            echo installing foo patched
-            installing foo patched
-        
-        It is possible to autogenerate the configure files:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %s/bar.tgz
-            ... autogen = autogen.sh
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost//bar.tgz
-            foo: Unpacking and configuring
-            foo: auto generating configure files
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        It is also possible to support configure commands other than "./configure":
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %s/baz.tgz
-            ... source-directory-contains = configure.py
-            ... configure-command = ./configure.py
-            ... configure-options =
-            ...     --bindir=bin
-            ... """ % distros_url)
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost//baz.tgz
-            foo: Unpacking and configuring
-            configuring foo --bindir=bin
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        When downloading a source archive or a patch, we can optionally make sure of
-        its authenticity by supplying an MD5 checksum that must be matched. If it
-        matches, we'll not be bothered with the check by buildout's output:
-        
-            >>> from hashlib import md5
-            >>> with open(join(distros, 'foo.tgz'), 'rb') as f:
-            ...     foo_md5sum = md5(f.read()).hexdigest()
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... md5sum = %s
-            ... """ % (distros_url, foo_md5sum))
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-        
-        But if the archive doesn't match the checksum, the recipe refuses to install:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sbar.tgz
-            ... md5sum = %s
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... """ % (distros_url, foo_md5sum))
-        
-            >>> print(system('bin/buildout').strip())
-            Uninstalling foo.
-            Installing foo.
-            foo: Downloading http://localhost:20617/bar.tgz
-            While:
-              Installing foo.
-            Error: MD5 checksum mismatch downloading 'http://localhost/bar.tgz'
-        
-        Similarly, a checksum mismatch for the patch will cause the buildout run to be
-        aborted:
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... patch-md5sum = %s
-            ... """ % (distros_url, foo_md5sum))
-        
-            >>> print(system('bin/buildout').strip())
-            Installing foo.
-            foo: Downloading http://localhost:21669/foo.tgz
-            foo: Unpacking and configuring
-            While:
-              Installing foo.
-            Error: MD5 checksum mismatch for local resource at '/.../sample-buildout/patches/config.patch'.
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... patch = ${buildout:directory}/patches/config.patch
-            ... """ % (distros_url))
-        
-        If the build fails, the temporary directory where the tarball was unpacked
-        is logged to stdout, and left intact for debugging purposes.
-        
-            >>> write('patches/config.patch', "dgdgdfgdfg")
-        
-            >>> res =  system('bin/buildout')
-            >>> print(res)
-            Installing foo.
-            foo: Downloading http://localhost/foo.tgz
-            foo: Unpacking and configuring
-            patch unexpectedly ends in middle of line
-            foo: cmmi failed: /.../...buildout-foo
-            patch: **** Only garbage was found in the patch input.
-            While:
-              Installing foo.
-            <BLANKLINE>
-            An internal error occurred due to a bug in either zc.buildout or in a
-            recipe being used:
-            ...
-            CalledProcessError: Command 'patch -p0 < ...' returned non-zero exit status ...
-            <BLANKLINE>
-        
-            >>> import re
-            >>> import os.path
-            >>> import shutil
-            >>> path = re.search('foo: cmmi failed: (.*)', res).group(1)
-            >>> os.path.exists(path)
-            True
-            >>> shutil.rmtree(path)
-        
-        After a successful build, such temporary directories are removed.
-        
-            >>> import glob
-            >>> import tempfile
-        
-            >>> old_tempdir = tempfile.gettempdir()
-            >>> tempdir = tempfile.tempdir = tempfile.mkdtemp(suffix='.buildout.build')
-            >>> dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
-        
-            >>> write('buildout.cfg',
-            ... """
-            ... [buildout]
-            ... parts = foo
-            ...
-            ... [foo]
-            ... recipe = zc.recipe.cmmi
-            ... url = %sfoo.tgz
-            ... """ % (distros_url,))
-        
-            >>> print(system("bin/buildout"))
-            Installing foo.
-            foo: Downloading http://localhost:21445/foo.tgz
-            foo: Unpacking and configuring
-            configuring foo --prefix=/sample_buildout/parts/foo
-            echo building foo
-            building foo
-            echo installing foo
-            installing foo
-            <BLANKLINE>
-        
-            >>> new_dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
-            >>> len(dirs) == len(new_dirs) == 0
-            True
-            >>> tempfile.tempdir = old_tempdir
-        
-        ==============
-        Download Cache
-        ==============
-        The recipe supports use of a download cache in the same way
-        as zc.buildout. See downloadcache.txt for details
-        
-        
 Keywords: zc.buildout buildout recipe cmmi configure make install
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Framework :: Buildout
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Software Distribution
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE.txt
+
+==============================================================
+ Recipe installing a download via configure/make/make install
+==============================================================
+
+The configure-make-make-install recipe automates installation of
+configure-based source distribution into buildouts.
+
+.. contents::
+
+
+Options
+=======
+
+url
+   The URL of a source archive to download
+
+configure-command
+   The name of the configure script.
+
+   The option defaults to ``./configure``.
+
+configure-options
+   Basic configure options.
+
+   Defaults to a ``--prefix`` option that points to the part directory.
+
+extra_options
+   A string of extra options to pass to configure in *addition to* the
+   base options.
+
+environment
+   Optional environment variable settings of the forme NAME=VALUE.
+
+   Newlines are ignored. Spaces may be included in environment values
+   as long as they can't be mistaken for environment settings.  So::
+
+      environment = FOO=bar
+                    baz
+
+   Sets the environment variable FOO, but::
+
+      environment = FOO=bar xxx=baz
+
+   Sets 2 environment values, FOO and xxx.
+
+patch
+   The name of an optional patch file to apply to the distribution.
+
+patch_options
+   Options to supply to the patch command (if a patch file is used).
+
+   This defaults to ``-p0``
+
+shared
+   Share the build accross buildouts.
+
+autogen
+   The name of a script to run to generate a configure script.
+
+source-directory-contains
+   The name of a file in the distribution's source directory.
+
+   This is used by the recipe to determine if it has found the source
+   directory. It defaults top "configure".
+
+
+.. note::
+
+    This recipe is not expected to work in a Microsoft Windows environment.
+
+=================
+ Release History
+=================
+
+4.0 (2023-07-07)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
+3.0.0 (2019-03-30)
+==================
+
+- Drop support for Python 3.4.
+
+- Add support for Python 3.7 and 3.8a2.
+
+- Flake8 the code.
+
+
+2.0.0 (2017-06-21)
+==================
+
+- Add support for Python 3.4, 3.5, 3.6 and PyPy.
+
+- Automated testing is enabled on Travis CI.
+
+1.3.6 (2014-04-14)
+==================
+
+- Fixed: Strings were incorrectly compared using "is not ''" rather than !=
+
+- Fixed: Spaces weren't allowed in the installation location.
+
+1.3.5 (2011-08-06)
+==================
+
+- Fixed: Spaces weren't allowed in environment variables.
+
+- Fixed: Added missing option reference documentation.
+
+
+1.3.4 (2011-01-18)
+==================
+
+- Fixed a bug in location book-keeping that caused shared builds to be deleted
+  from disk when a part didn't need them anymore. (#695977)
+
+- Made tests pass with both zc.buildout 1.4 and 1.5, lifted the upper version
+  bound on zc.buildout. (#695732)
+
+1.3.3 (2010-11-10)
+==================
+
+- Remove the temporary build directory when cmmi succeeds.
+
+- Specify that the zc.buildout version be <1.5.0b1, as the recipe is
+  currently not compatible with zc.buildout 1.5.
+
+1.3.2 (2010-08-09)
+==================
+
+- Remove the build directory for a shared build when the source cannot be
+  downloaded.
+
+- Declared a test dependency on zope.testing.
+
+
+1.3.1 (2009-09-10)
+==================
+
+- Declare dependency on zc.buildout 1.4 or later. This dependency was introduced
+  in version 1.3.
+
+
+1.3 (2009-09-03)
+================
+
+- Use zc.buildout's download API. As this allows MD5 checking, added the
+  md5sum and patch-md5sum options.
+
+- Added options for changing the name of the configure script and
+  overriding the ``--prefix`` parameter.
+
+- Moved the core "configure; make; make install" command sequence to a
+  method that can be overridden in other recipes, to support packages
+  whose installation process is slightly different.
+
+1.2.1 (2009-08-12)
+==================
+
+Bug fix: keep track of reused shared builds.
+
+
+1.2.0 (2009-05-18)
+==================
+
+Enabled using a shared directory for completed builds.
+
+1.1.6 (2009-03-17)
+==================
+
+Moved 'zc' package from root of checkout into 'src', to prevent testrunner
+from finding eggs installed locally by buildout.
+
+Removed deprecations under Python 2.6.
+
+1.1.5 (2008-11-07)
+==================
+
+- Added to the README.txt file a link to the SVN repository, so that Setuptools
+  can automatically find the development version when asked to install the
+  "-dev" version of zc.recipe.cmmi.
+
+- Applied fix for bug #261367 i.e. changed open() of file being downloaded to
+  binary, so that errors like the following no longer occur under Windows.
+
+  uncompress = self.decompress.decompress(buf)
+  error: Error -3 while decompressing: invalid distance too far back
+
+1.1.4 (2008-06-25)
+==================
+
+Add support to autogen configure files.
+
+1.1.3 (2008-06-03)
+==================
+
+Add support for updating the environment.
+
+1.1.2 (2008-02-28)
+==================
+
+- Check if the ``location`` folder exists before creating it.
+
+After 1.1.0
+===========
+
+Added support for patches to be downloaded from a url rather than only using
+patches on the filesystem
+
+1.1.0
+=====
+
+Added support for:
+
+ - download-cache: downloaded files are cached in the 'cmmi' subdirectory of
+   the cache cache keys are hashes of the url that the file was downloaded from
+   cache information recorded in the cache.ini file within each directory
+
+ - offline mode: cmmi will not go online if the package is not in the cache
+
+ - variable location: build files other than in the parts directory if required
+
+ - additional logging/output
+
+1.0.2 (2007-06-03)
+==================
+
+- Added support for patches.
+
+- Tests fixed (buildout's output changed)
+
+1.0.1 (2006-11-22)
+==================
+
+- Added missing zip_safe flag.
+
+1.0 (2006-11-22)
+================
+
+Initial release.
+
+======================
+Detailed Documentation
+======================
+
+We have an archive with a demo foo tar ball and publish it by http in order
+to see  offline effects:
+
+    >>> ls(distros)
+    -  bar.tgz
+    -  baz.tgz
+    -  foo.tgz
+
+    >>> distros_url = start_server(distros)
+
+Let's update a sample buildout to installs it:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... """ % distros_url)
+
+We used the url option to specify the location of the archive.
+
+If we run the buildout, the configure script in the archive is run.
+It creates a make file which is also run:
+
+    >>> print(system('bin/buildout').strip())
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample-buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+The recipe also creates the parts directory:
+
+    >>> import os.path
+    >>> os.path.isdir(join(sample_buildout, "parts", "foo"))
+    True
+
+If we run the buildout again, the update method will be called, which
+does nothing:
+
+    >>> print(system('bin/buildout').strip())
+    Updating foo.
+
+You can supply extra configure options:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... extra_options = -a -b c
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample-buildout/parts/foo -a -b c
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+The recipe sets the location option, which can be read by other
+recipes, to the location where the part is installed:
+
+    >>> cat('.installed.cfg')
+    [buildout]
+    installed_develop_eggs =
+    parts = foo
+    <BLANKLINE>
+    [foo]
+	...
+    location = /sample_buildout/parts/foo
+	...
+
+It may be necessary to set some environment variables when running configure
+or make. This can be done by adding an environment statement:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... environment =
+    ...   CFLAGS=-I/usr/lib/postgresql7.4/include
+    ... """ % distros_url)
+
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    foo: Updating environment: CFLAGS=-I/usr/lib/postgresql7.4/include
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+Sometimes it's necessary to patch the sources before building a package.
+You can specify the name of the patch to apply and (optional) patch options:
+
+First of all let's write a patchfile:
+
+    >>> import sys
+    >>> mkdir('patches')
+    >>> write('patches/config.patch',
+    ... """--- configure
+    ... +++ /dev/null
+    ... @@ -1,13 +1,13 @@
+    ...  #!%s
+    ...  import sys
+    ... -print("configuring foo " + ' '.join(sys.argv[1:]))
+    ... +print("configuring foo patched " + ' '.join(sys.argv[1:]))
+    ...
+    ...  Makefile_template = '''
+    ...  all:
+    ... -\techo building foo
+    ... +\techo building foo patched
+    ...
+    ...  install:
+    ... -\techo installing foo
+    ... +\techo installing foo patched
+    ...  '''
+    ...
+    ...  with open('Makefile', 'w') as f:
+    ...      _ = f.write(Makefile_template)
+    ...
+    ... """ % sys.executable)
+
+Now let's create a buildout.cfg file. Note: If no patch option is beeing
+passed, -p0 is appended by default.
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... patch_options = -p0
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    patching file configure
+    ...
+    configuring foo patched --prefix=/sample_buildout/parts/foo
+    echo building foo patched
+    building foo patched
+    echo installing foo patched
+    installing foo patched
+
+It is possible to autogenerate the configure files:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %s/bar.tgz
+    ... autogen = autogen.sh
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost//bar.tgz
+    foo: Unpacking and configuring
+    foo: auto generating configure files
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+It is also possible to support configure commands other than "./configure":
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %s/baz.tgz
+    ... source-directory-contains = configure.py
+    ... configure-command = ./configure.py
+    ... configure-options =
+    ...     --bindir=bin
+    ... """ % distros_url)
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost//baz.tgz
+    foo: Unpacking and configuring
+    configuring foo --bindir=bin
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+When downloading a source archive or a patch, we can optionally make sure of
+its authenticity by supplying an MD5 checksum that must be matched. If it
+matches, we'll not be bothered with the check by buildout's output:
+
+    >>> from hashlib import md5
+    >>> with open(join(distros, 'foo.tgz'), 'rb') as f:
+    ...     foo_md5sum = md5(f.read()).hexdigest()
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... md5sum = %s
+    ... """ % (distros_url, foo_md5sum))
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+
+But if the archive doesn't match the checksum, the recipe refuses to install:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sbar.tgz
+    ... md5sum = %s
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... """ % (distros_url, foo_md5sum))
+
+    >>> print(system('bin/buildout').strip())
+    Uninstalling foo.
+    Installing foo.
+    foo: Downloading http://localhost:20617/bar.tgz
+    While:
+      Installing foo.
+    Error: MD5 checksum mismatch downloading 'http://localhost/bar.tgz'
+
+Similarly, a checksum mismatch for the patch will cause the buildout run to be
+aborted:
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... patch-md5sum = %s
+    ... """ % (distros_url, foo_md5sum))
+
+    >>> print(system('bin/buildout').strip())
+    Installing foo.
+    foo: Downloading http://localhost:21669/foo.tgz
+    foo: Unpacking and configuring
+    While:
+      Installing foo.
+    Error: MD5 checksum mismatch for local resource at '/.../sample-buildout/patches/config.patch'.
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... patch = ${buildout:directory}/patches/config.patch
+    ... """ % (distros_url))
+
+If the build fails, the temporary directory where the tarball was unpacked
+is logged to stdout, and left intact for debugging purposes.
+
+    >>> write('patches/config.patch', "dgdgdfgdfg")
+
+    >>> res =  system('bin/buildout')
+    >>> print(res)
+    Installing foo.
+    foo: Downloading http://localhost/foo.tgz
+    foo: Unpacking and configuring
+    patch unexpectedly ends in middle of line
+    foo: cmmi failed: /.../...buildout-foo
+    patch: **** Only garbage was found in the patch input.
+    While:
+      Installing foo.
+    <BLANKLINE>
+    An internal error occurred due to a bug in either zc.buildout or in a
+    recipe being used:
+    ...
+    subprocess.CalledProcessError: Command 'patch -p0 < ...' returned non-zero exit status ...
+    <BLANKLINE>
+
+    >>> import re
+    >>> import os.path
+    >>> import shutil
+    >>> path = re.search('foo: cmmi failed: (.*)', res).group(1)
+    >>> os.path.exists(path)
+    True
+    >>> shutil.rmtree(path)
+
+After a successful build, such temporary directories are removed.
+
+    >>> import glob
+    >>> import tempfile
+
+    >>> old_tempdir = tempfile.gettempdir()
+    >>> tempdir = tempfile.tempdir = tempfile.mkdtemp(suffix='.buildout.build')
+    >>> dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
+
+    >>> write('buildout.cfg',
+    ... """
+    ... [buildout]
+    ... parts = foo
+    ...
+    ... [foo]
+    ... recipe = zc.recipe.cmmi
+    ... url = %sfoo.tgz
+    ... """ % (distros_url,))
+
+    >>> print(system("bin/buildout"))
+    Installing foo.
+    foo: Downloading http://localhost:21445/foo.tgz
+    foo: Unpacking and configuring
+    configuring foo --prefix=/sample_buildout/parts/foo
+    echo building foo
+    building foo
+    echo installing foo
+    installing foo
+    <BLANKLINE>
+
+    >>> new_dirs = glob.glob(os.path.join(tempdir, '*buildout-foo'))
+    >>> len(dirs) == len(new_dirs) == 0
+    True
+    >>> tempfile.tempdir = old_tempdir
+
+==============
+Download Cache
+==============
+The recipe supports use of a download cache in the same way
+as zc.buildout. See downloadcache.txt for details
+
```

### Comparing `zc.recipe.cmmi-3.0.0/src/zc.recipe.cmmi.egg-info/SOURCES.txt` & `zc.recipe.cmmi-4.0/src/zc.recipe.cmmi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 .coveragerc
-.gitignore
-.travis.yml
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 setup.cfg
 setup.py
-test_all_pythons.cfg
-to-do.txt
 tox.ini
 src/zc/__init__.py
 src/zc.recipe.cmmi.egg-info/PKG-INFO
 src/zc.recipe.cmmi.egg-info/SOURCES.txt
 src/zc.recipe.cmmi.egg-info/dependency_links.txt
 src/zc.recipe.cmmi.egg-info/entry_points.txt
 src/zc.recipe.cmmi.egg-info/namespace_packages.txt
```

