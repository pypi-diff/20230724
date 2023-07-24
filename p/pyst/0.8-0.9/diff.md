# Comparing `tmp/pyst-0.8.tar.gz` & `tmp/pyst-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyst-0.8.tar", last modified: Fri Dec  4 10:42:33 2020, max compression
+gzip compressed data, was "pyst-0.9.tar", last modified: Mon Jul 24 09:21:45 2023, max compression
```

## Comparing `pyst-0.8.tar` & `pyst-0.9.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2020-12-04 10:42:33.000000 pyst-0.8/
--rw-r--r--   0 ralf      (1000) priv      (1011)    19728 2020-12-04 10:42:33.000000 pyst-0.8/README.html
--rw-r--r--   0 ralf      (1000) priv      (1011)      243 2014-04-17 17:52:07.000000 pyst-0.8/MANIFEST.in
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2020-12-04 10:42:33.000000 pyst-0.8/asterisk/
--rw-r--r--   0 ralf      (1000) priv      (1011)      459 2014-04-15 10:00:10.000000 pyst-0.8/asterisk/__init__.py
--rw-r--r--   0 ralf      (1000) priv      (1011)     4862 2014-04-19 13:51:58.000000 pyst-0.8/asterisk/astemu.py
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2020-12-04 10:42:33.000000 pyst-0.8/asterisk/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)    21109 2020-12-03 09:34:30.000000 pyst-0.8/asterisk/manager.py
--rw-r--r--   0 ralf      (1000) priv      (1011)    26143 2020-01-14 10:36:31.000000 pyst-0.8/asterisk/agi.py
--rw-r--r--   0 ralf      (1000) priv      (1011)     4907 2020-01-14 10:24:04.000000 pyst-0.8/asterisk/config.py
--rw-r--r--   0 ralf      (1000) priv      (1011)      641 2014-04-15 10:00:10.000000 pyst-0.8/asterisk/compat.py
--rw-r--r--   0 ralf      (1000) priv      (1011)     7921 2020-01-14 10:25:44.000000 pyst-0.8/asterisk/agitb.py
--rw-r--r--   0 ralf      (1000) priv      (1011)    12315 2020-12-04 10:41:33.000000 pyst-0.8/README.rst
--rw-r--r--   0 ralf      (1000) priv      (1011)     2735 2014-04-15 10:43:52.000000 pyst-0.8/ChangeLog
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2020-12-04 10:42:33.000000 pyst-0.8/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)    33780 2020-01-14 11:32:09.000000 pyst-0.8/test/test_base.py
--rw-r--r--   0 ralf      (1000) priv      (1011)    15755 2020-12-04 10:42:33.000000 pyst-0.8/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     1849 2014-04-17 17:53:34.000000 pyst-0.8/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:21:45.880954 pyst-0.9/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2735 2014-04-15 10:43:52.000000 pyst-0.9/ChangeLog
+-rw-r--r--   0 ralf      (1000) priv      (1011)    26341 2023-07-24 08:57:05.000000 pyst-0.9/LICENSE
+-rw-r--r--   0 ralf      (1000) priv      (1011)      243 2014-04-17 17:52:07.000000 pyst-0.9/MANIFEST.in
+-rw-r--r--   0 ralf      (1000) priv      (1011)    14504 2023-07-24 09:21:45.876954 pyst-0.9/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)    20406 2023-07-24 09:21:03.000000 pyst-0.9/README.html
+-rw-r--r--   0 ralf      (1000) priv      (1011)    12862 2023-07-24 09:13:42.000000 pyst-0.9/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:21:45.852954 pyst-0.9/asterisk/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-07-24 09:21:03.000000 pyst-0.9/asterisk/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)      459 2014-04-15 10:00:10.000000 pyst-0.9/asterisk/__init__.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)    26143 2020-01-14 10:36:31.000000 pyst-0.9/asterisk/agi.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7921 2020-01-14 10:25:44.000000 pyst-0.9/asterisk/agitb.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)     4862 2014-04-19 13:51:58.000000 pyst-0.9/asterisk/astemu.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)      641 2014-04-15 10:00:10.000000 pyst-0.9/asterisk/compat.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)     4907 2020-01-14 10:24:04.000000 pyst-0.9/asterisk/config.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)    21293 2023-02-13 17:49:57.000000 pyst-0.9/asterisk/manager.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1745 2023-07-24 09:14:40.000000 pyst-0.9/pyproject.toml
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:21:45.868954 pyst-0.9/pyst.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    14504 2023-07-24 09:21:45.000000 pyst-0.9/pyst.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      358 2023-07-24 09:21:45.000000 pyst-0.9/pyst.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-07-24 09:21:45.000000 pyst-0.9/pyst.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        9 2023-07-24 09:21:45.000000 pyst-0.9/pyst.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-07-24 09:21:45.880954 pyst-0.9/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1849 2014-04-17 17:53:34.000000 pyst-0.9/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:21:45.872954 pyst-0.9/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    33780 2020-01-14 11:32:09.000000 pyst-0.9/test/test_base.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyst-0.8/README.html` & `pyst-0.9/README.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8" ?>
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
 <head>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-<meta name="generator" content="Docutils 0.14: http://docutils.sourceforge.net/" />
+<meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <title>pyst: A Python Interface to Asterisk</title>
 <style type="text/css">
 
 /*
 :Author: David Goodger
 :Contact: goodger@users.sourceforge.net
 :Date: $Date: 2007-12-21 16:51:22 +0100 (Fri, 21 Dec 2007) $
@@ -351,14 +351,21 @@
 <tt class="docutils literal">setup.py</tt>. This means, the manager part of the package will probably
 run on any platform. The agi scripts on the other hand are called
 directly on the host where Asterisk is running in which case they are
 limited to the platforms asterisk is running on. Alternatively, you can
 use the <em>fastagi</em> mechanism of asterisk which calls the agi scripts on a
 remote host. In the latter case this host can be any platform where
 python runs.</p>
+<div class="section" id="tests">
+<h1>Tests</h1>
+<p>The tests are standard pytest-compatible tests. Run with:</p>
+<pre class="literal-block">
+python3 -m pytest test
+</pre>
+</div>
 <div class="section" id="credits">
 <h1>Credits</h1>
 <p>Thanks to Karl Putland for writing the original package.
 Thanks to Matthew Nicholson for maintaining the package for some years
 and for handing over maintenance when he was no longer interested.</p>
 <p>Thanks also to the people in the sourceforge project and those who just
 report bugs:
@@ -447,14 +454,24 @@
 (monotone is a free distributed version control system). This repository
 has also been incorporated into the GIT repository.</p>
 <p>prior to that the sources are in the CVS repository on sourceforge which
 has also been incorporated into the GIT repository.</p>
 </div>
 <div class="section" id="changes">
 <h1>Changes</h1>
+<p>Version 0.9: Add LICENSE, pyproject.toml, remove old test harness</p>
+<ul class="simple">
+<li>Added LICENSE, the software always was dual-licensed, no LGPL update
+clause (&quot;2.0 or later&quot;) was specified at the time. The license should
+still be GPL/LGPL 3.0 compatible due to the dual-licensing with the
+python software foundation license.</li>
+<li>New section in README.rst for running the tests after removing old
+test harness</li>
+<li>Add patch to allow connecting using IPv6</li>
+</ul>
 <p>Version 0.8: Fix README.rst</p>
 <p>Cleanup of README before releasing 0.8 on pypi.</p>
 <p>Version 0.7: Update tests, Compatibility</p>
 <p>Now a test for AGI exists (in addition the the existing AMI test).
 Asterisk in newer versions yields output of AMI commands prefixed with
 <tt class="docutils literal">Output:</tt>. This was already correctly parsed into the <tt class="docutils literal">multiheaders</tt>
 variable where Lines with a repeated header are kept. For
```

### Comparing `pyst-0.8/asterisk/astemu.py` & `pyst-0.9/asterisk/astemu.py`

 * *Files identical despite different names*

### Comparing `pyst-0.8/asterisk/manager.py` & `pyst-0.9/asterisk/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,16 +441,20 @@
         # make sure host is a string
         assert isinstance (host, string_types)
 
         port = int(port)  # make sure port is an int
 
         # create our socket and connect
         try:
-            _sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            _sock.connect((host,port))
+            if host.find(":") >= 0:
+                _sock = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
+                _sock.connect((host,port,0,0))
+            else:
+                _sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                _sock.connect((host,port))
             self._sock = _sock.makefile(mode='rwb')
             _sock.close()
         except socket.error as err:
             errno, reason = err
             raise ManagerSocketException(errno, reason)
 
         # we are connected and running
```

### Comparing `pyst-0.8/asterisk/agi.py` & `pyst-0.9/asterisk/agi.py`

 * *Files identical despite different names*

### Comparing `pyst-0.8/asterisk/config.py` & `pyst-0.9/asterisk/config.py`

 * *Files identical despite different names*

### Comparing `pyst-0.8/asterisk/compat.py` & `pyst-0.9/asterisk/compat.py`

 * *Files identical despite different names*

### Comparing `pyst-0.8/asterisk/agitb.py` & `pyst-0.9/asterisk/agitb.py`

 * *Files identical despite different names*

### Comparing `pyst-0.8/README.rst` & `pyst-0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,21 @@
 run on any platform. The agi scripts on the other hand are called
 directly on the host where Asterisk is running in which case they are
 limited to the platforms asterisk is running on. Alternatively, you can
 use the *fastagi* mechanism of asterisk which calls the agi scripts on a
 remote host. In the latter case this host can be any platform where
 python runs.
 
+Tests
+-----
+
+The tests are standard pytest-compatible tests. Run with::
+
+    python3 -m pytest test
+
 Credits
 -------
 
 Thanks to Karl Putland for writing the original package.
 Thanks to Matthew Nicholson for maintaining the package for some years
 and for handing over maintenance when he was no longer interested.
 
@@ -199,14 +206,24 @@
 prior to that the sources are in the CVS repository on sourceforge which
 has also been incorporated into the GIT repository.
 
 
 Changes
 -------
 
+Version 0.9: Add LICENSE, pyproject.toml, remove old test harness
+
+- Added LICENSE, the software always was dual-licensed, no LGPL update
+  clause ("2.0 or later") was specified at the time. The license should
+  still be GPL/LGPL 3.0 compatible due to the dual-licensing with the
+  python software foundation license.
+- New section in README.rst for running the tests after removing old
+  test harness
+- Add patch to allow connecting using IPv6
+
 Version 0.8: Fix README.rst
 
 Cleanup of README before releasing 0.8 on pypi.
 
 Version 0.7: Update tests, Compatibility
 
 Now a test for AGI exists (in addition the the existing AMI test).
```

### Comparing `pyst-0.8/ChangeLog` & `pyst-0.9/ChangeLog`

 * *Files identical despite different names*

### Comparing `pyst-0.8/test/test_base.py` & `pyst-0.9/test/test_base.py`

 * *Files identical despite different names*

### Comparing `pyst-0.8/PKG-INFO` & `pyst-0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,301 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyst
-Version: 0.8
+Version: 0.9
 Summary: A Python Interface to Asterisk
 Home-page: http://www.sourceforge.net/projects/pyst/
-Author: Ralf Schlatterbeck
-Author-email: rsc@runtux.com
-License: Python Software Foundation License, GNU Library or Lesser General Public License (LGPL)
-Download-URL: http://downloads.sourceforge.net/project/pyst/pyst/0.8/pyst-0.8.tar.gz
-Description: 
-        Pyst consists of a set of interfaces and libraries to allow programming of
-        Asterisk from python. The library currently supports AGI, AMI, and the parsing
-        of Asterisk configuration files. The library also includes debugging facilities
-        for AGI.
-        
-        News 2020: Updated to Python3 including Py7 which includes a new 'async'
-        keyword that was used in the code. Note that there is a pyst2 project
-        also on github which is a fork from an earlier version of pyst.
-        Unfortunately the fork was made from the old Subversion repository and
-        therefore the two repos do not share a common root in git which makes it
-        hard to merge changes. Also I've introduced a regression test since then
-        which afaik is not included in pyst2. The maintainers seem to have tried
-        to contact me via Sourceforge but this may not have worked at the time
-        due to problems forwarding mails by SF. This should no longer happen as
-        in GIT every commit from me contains my correct email address now.
-        
-        So far I've tried to be compatible with the mentioned change of the
-        async keyword so that the API will not diverge too much. Note that there
-        is one ad-hoc patch in pyst2 that breaks the old API:
-        
-        Newer versions of Asterisk now send the output of AMI commands prefixed
-        with ``Output:``.  With my version this fits nicely into the
-        already-implemented ``multiheaders`` variable where Lines with a
-        repeated header are kept.  So all the ``Output:`` lines already were
-        correctly parsed and put into ``self.multiheaders ['Output']``. The only
-        thing I had to fix was to put all these lines into the old ``data``
-        variable, too. So if you were using ``data`` with old versions of
-        asterisk your code continues to work with pyst. Conversely pyst2 has a
-        patch that will return ``data`` prefixed with ``Output:`` (untested,
-        this is how I read the code).
-        
-        When I have time I intend to graft the pyst2 repo onto my working copy
-        (probably using reposurgeon_) and look through the changes that are
-        interesting. Drop me a note if you find something in pyst2 that you
-        think should be in pyst.
-        
-        Github repo can be cloned with::
-        
-         git clone https://github.com/schlatterbeck/pyst.git
-        
-        
-        Old News: The source code is now in a GIT repository on Sourceforge.
-        To check out anonymously into the local directory ``pyst``, use::
-        
-         git clone git://git.code.sf.net/p/pyst/code pyst
-        
-        Update 2020: I will continue to push to the sourceforge repository, too.
-        
-        Thanks to Eric S. Raymond's `reposurgeon`_, it was possible to unite the
-        old CVS repository, the monotone repository used until 0.2 (and a little
-        beyond 0.2) and the recent subversion repository into one git repository
-        that contains the whole history and cleans up some artefacts.
-        
-        .. _reposurgeon: http://www.catb.org/esr/reposurgeon/
-        
-        A note on maintenance and forks:
-        The current maintainer is Ralf Schlatterbeck. I've contacted maintainers
-        of forks to try to join forces. For any questions, please contact me via
-        rsc@runtux.com or my sourceforge user.
-        
-        Download from `Sourceforge project page`_.
-        
-        .. _`Sourceforge project page`: http://sourceforge.net/projects/pyst/
-        
-        Installation is the standard python install::
-        
-         tar xvf pyst.tar.gz
-         cd pyst
-         python setup.py install --prefix=/usr/local
-        
-        Documentation is currently only in python docstrings, you can use
-        pythons built-in help facility::
-        
-         import asterisk
-         help (asterisk)
-         import asterisk.agi
-         help (asterisk.agi)
-         import asterisk.manager
-         help (asterisk.manager)
-         import asterisk.config
-         help (asterisk.config)
-        
-        Some notes on platforms: We now specify "platforms = 'Any'" in
-        ``setup.py``. This means, the manager part of the package will probably
-        run on any platform. The agi scripts on the other hand are called
-        directly on the host where Asterisk is running in which case they are
-        limited to the platforms asterisk is running on. Alternatively, you can
-        use the *fastagi* mechanism of asterisk which calls the agi scripts on a
-        remote host. In the latter case this host can be any platform where
-        python runs.
-        
-        Credits
-        -------
-        
-        Thanks to Karl Putland for writing the original package.
-        Thanks to Matthew Nicholson for maintaining the package for some years
-        and for handing over maintenance when he was no longer interested.
-        
-        Thanks also to the people in the sourceforge project and those who just
-        report bugs:
-        Antoine Brenner,
-        Max Nesterov,
-        Sven Uebelacker
-        To Matthias Urlichs for maintaining the debian package (at least for
-        some time).
-        
-        ... and to unnamed contributors to earlier releases.
-        
-        Things to do for pyst
-        ---------------------
-        
-        This is the original changelog merged into the readme file. I'm not so
-        sure I really want to change all these things (in particular the
-        threaded implementation looks good to me). I will maintain a section
-        summarizing the changes in this README, the ChangeLog won't be
-        maintained any longer. Detailed changes will be available in the version
-        control tool.
-        
-        * ChangeLog:
-          The ChangeLog needs to be updated from the monotone logs.
-        
-        * Documentation:
-          All of pyst's inline documentation needs to be updated.
-        
-        * manager.py:
-          This should be converted to be single threaded.  Also there is a race
-          condition when a user calls manager.logoff() followed by
-          manager.close().  The close() function may still call logoff again if
-          the socket thread has not yet cleared the _connected flag.
-        
-          A class should be made for each manager action rather than having a
-          function in a manager class.  The manager class should be adapted to
-          have a send method that know the general format of the classes.
-        
-        Matthew Nicholson writes on the mailinglist (note that I'm not sure I'll do
-        this, I'm currently satisfied with the threaded implementation):
-        
-            For pyst 0.3 I am planning to clean up the manager.py.  There are
-            several know issues with the code.  No one has actually reported these
-            as problems, but I have personally had trouble with these.  Currently
-            manager.py runs in several threads, the main program thread, a thread to
-            read from the network, and an event distribution thread.  This causes
-            problems with non thread safe code such as the MySQLdb libraries.  This
-            design also causes problems when an event handler throws an exception
-            that causes the event processing thread to terminate.
-        
-            The second problem is with the way actions are sent.  Each action has a
-            specific function associated with it in the manager object that takes
-            all possible arguments that may ever be passed to that action.  This
-            makes the api somewhat rigid and the Manager object cluttered.
-        
-            To solve these problems I am basically going to copy the design of my
-            Astxx manager library (written in c++) and make it more python like.
-            Each action will be a different object with certain methods to handle
-            various tasks, with one function in the actual Manager class to send the
-            action.  This will make the Manager class much smaller and much more
-            flexible.  The current code will be consolidated into a single threaded
-            design with hooks to have the library process events and such.  These
-            hooks will be called from the host application's main loop.
-        
-        
-        Source Code Repository Access
-        -----------------------------
-        
-        The current versions are kept in a GIT repository on Github.
-        You can check out the trunk with::
-        
-         git clone https://github.com/schlatterbeck/pyst.git
-        
-        I will continue to push to the Sourceforge version although Bug-Reports
-        etc. are easier with Github. Check out from Sourceforge with::
-        
-            git clone git://git.code.sf.net/p/pyst/code pyst
-        
-        There is a monotone-after-0.2 branch which contains unreleased changes
-        after 0.2 which were committed to the monotone repository after the
-        Release of Version 0.2 (which have been merged into trunk *after*
-        changing how manager commands to asterisk are parsed).
-        
-        Released versions are tagged, see the tags in the web-interface on
-        Sourceforge (or use local git commands to find out)
-        
-            https://sourceforge.net/p/pyst/code/ci/master/tree/
-        
-        For versions up to 0.6 the code was kept in a Subversion repository in
-        Sourceforge. This has been incorporated into the current GIT repository
-        (after cleaning up some subversion artefacts).
-        
-        For versions prior to the 0.2 release when Matthew Nicholson was
-        maintaining pyst, the changes were kept in a `monotone`_ repository
-        (monotone is a free distributed version control system). This repository
-        has also been incorporated into the GIT repository.
-        
-        .. _`monotone`: http://monotone.ca/
-        
-        prior to that the sources are in the CVS repository on sourceforge which
-        has also been incorporated into the GIT repository.
-        
-        
-        Changes
-        -------
-        
-        Version 0.8: Fix README.rst
-        
-        Cleanup of README before releasing 0.8 on pypi.
-        
-        Version 0.7: Update tests, Compatibility
-        
-        Now a test for AGI exists (in addition the the existing AMI test).
-        Asterisk in newer versions yields output of AMI commands prefixed with
-        ``Output:``. This was already correctly parsed into the ``multiheaders``
-        variable where Lines with a repeated header are kept. For
-        backwards-compatibility all these lines are also put into the old
-        ``data`` variable, too. So if you were using ``data`` with old versions
-        of asterisk your code continues to work with pyst.
-        Python 3.7 has introduced a new keyword ``async``. Unfortunately we were
-        using this keyword as a parameter of the AMI ``originate`` call. I've
-        changed this to ``run_async`` (to be compatible with pyst2, I would have
-        named it simpy ``asynchronous``, see the commit history).
-        
-        Version 0.6: Minor feature enhancements
-        
-        The asterisk management interface emulator asterisk/astemu now can be
-        used for unit-tests of applications using asterisk.manager. We're using
-        this in the regression test (see test directory). But this way it is
-        usable by others.
-        
-        - Factor asterisk emulator from regression test into own module
-        
-        Version 0.5: Small install change
-        
-        Fix setup.py to include download_url. This makes it installable using
-        intall tools like pip.
-        
-        - Add download_url to setup.py
-        - Fix svn url after SourceForge upgrade
-        
-        Version 0.4: Minor feature enhancements
-        
-        Small feature extensions to AGI and Manager modules. Add a regression
-        test which now covers some aspects of the manager API.
-        
-        - Handle events with several fields with the same name (e.g. 'Variable'
-          in the 'AgentCalled' event. Thanks to Max Nesterov for the
-          suggestion, implementation differs from the suggestion in SF patch
-          3290869. For a use-case see the give SF patch and the regression test
-          case test_agent_event.
-        - Allow to use AGI module in FastAGI way via TCP connection.
-          This change allows you to specify the socket streams instead
-          sys.stdin/sys.stdout streams. Thanks to Max Nesterov for the patch.
-          Applies SF patch 3047290.
-        - Add regression test framework and some test cases for manager API.
-        - The generated ActionID for the manager interface now includes the
-          process-ID, this allows several concurrent processes using the
-          manager API.
-        
-        Version 0.3: Minor feature enhancements
-        
-        New maintainer Ralf Schlatterbeck, this is my first release, please
-        report any problems via the Sourceforge Bug-Tracker or email me
-        directly. Thanks to Karl Putland for writing the original package.
-        Thanks to Matthew Nicholson for maintaining the package for some years
-        and for handing over maintenance when he was no longer interested.
-        The parsing of answers from asterisk was completely rewritten. This
-        should fix problems people were having with commands returning embedded
-        '/' or empty lines. Some new manager commands added.
-        
-        - Add playdtmf manager command
-        - add sippeers and sipshowpeer manager commands
-        - rewritten manager communication
-        - should no longer choke on '/' in answers returned from a manager
-          command (fixes SF Bug 2947866)
-        - should now correctly parse multi-line output with embedded empty
-          lines, e.g. ``mgr.command('dialplan show')``
-        - Bug-fix for list manipulation in ``event_dispatch``, thanks to Jan
-          Mueller, see mailinglist comment from 2008-04-18
-        - Merge unreleased changes from repository of Matthew Nicholson
-          in particular a typo in ``agi.py`` for ``set_autohangup``, and change
-          of ``get_header`` methods (see Upgrading instructions). The fixed
-          ``manager.command`` support is already in (with a different
-          solution). The unreleased changes are also on the 0.2 branch in the
-          subversion repository in case somebody is interested.
-        
-        
+Download-URL: http://downloads.sourceforge.net/project/pyst/pyst/None/pyst-None.tar.gz
+Author: Karl Putland
+Author-email: Karl Putland <kputland@users.sourceforge.net>, Matthew Nicholson <matt@matt-land.com>, Ralf Schlatterbeck <rsc@runtux.com>
+Maintainer: Ralf Schlatterbeck
+Maintainer-email: Ralf Schlatterbeck <rsc@runtux.com>
+License: Python Software Foundation License, GNU Library or Lesser General Public License (LGPL) version 2
+Project-URL: Homepage, https://github.com/schlatterbeck/pyst
+Project-URL: Bug Tracker, https://github.com/schlatterbeck/pyst/issues
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -304,7 +23,314 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Communications :: Internet Phone
 Classifier: Topic :: Communications :: Telephony
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+pyst: A Python Interface to Asterisk
+====================================
+
+Pyst consists of a set of interfaces and libraries to allow programming of
+Asterisk from python. The library currently supports AGI, AMI, and the parsing
+of Asterisk configuration files. The library also includes debugging facilities
+for AGI.
+
+News 2020: Updated to Python3 including Py7 which includes a new 'async'
+keyword that was used in the code. Note that there is a pyst2 project
+also on github which is a fork from an earlier version of pyst.
+Unfortunately the fork was made from the old Subversion repository and
+therefore the two repos do not share a common root in git which makes it
+hard to merge changes. Also I've introduced a regression test since then
+which afaik is not included in pyst2. The maintainers seem to have tried
+to contact me via Sourceforge but this may not have worked at the time
+due to problems forwarding mails by SF. This should no longer happen as
+in GIT every commit from me contains my correct email address now.
+
+So far I've tried to be compatible with the mentioned change of the
+async keyword so that the API will not diverge too much. Note that there
+is one ad-hoc patch in pyst2 that breaks the old API:
+
+Newer versions of Asterisk now send the output of AMI commands prefixed
+with ``Output:``.  With my version this fits nicely into the
+already-implemented ``multiheaders`` variable where Lines with a
+repeated header are kept.  So all the ``Output:`` lines already were
+correctly parsed and put into ``self.multiheaders ['Output']``. The only
+thing I had to fix was to put all these lines into the old ``data``
+variable, too. So if you were using ``data`` with old versions of
+asterisk your code continues to work with pyst. Conversely pyst2 has a
+patch that will return ``data`` prefixed with ``Output:`` (untested,
+this is how I read the code).
+
+When I have time I intend to graft the pyst2 repo onto my working copy
+(probably using reposurgeon_) and look through the changes that are
+interesting. Drop me a note if you find something in pyst2 that you
+think should be in pyst.
+
+Github repo can be cloned with::
+
+ git clone https://github.com/schlatterbeck/pyst.git
+
+
+Old News: The source code is now in a GIT repository on Sourceforge.
+To check out anonymously into the local directory ``pyst``, use::
+
+ git clone git://git.code.sf.net/p/pyst/code pyst
+
+Update 2020: I will continue to push to the sourceforge repository, too.
+
+Thanks to Eric S. Raymond's `reposurgeon`_, it was possible to unite the
+old CVS repository, the monotone repository used until 0.2 (and a little
+beyond 0.2) and the recent subversion repository into one git repository
+that contains the whole history and cleans up some artefacts.
+
+.. _reposurgeon: http://www.catb.org/esr/reposurgeon/
+
+A note on maintenance and forks:
+The current maintainer is Ralf Schlatterbeck. I've contacted maintainers
+of forks to try to join forces. For any questions, please contact me via
+rsc@runtux.com or my sourceforge user.
+
+Download from `Sourceforge project page`_.
+
+.. _`Sourceforge project page`: http://sourceforge.net/projects/pyst/
+
+Installation is the standard python install::
+
+ tar xvf pyst.tar.gz
+ cd pyst
+ python setup.py install --prefix=/usr/local
+
+Documentation is currently only in python docstrings, you can use
+pythons built-in help facility::
+
+ import asterisk
+ help (asterisk)
+ import asterisk.agi
+ help (asterisk.agi)
+ import asterisk.manager
+ help (asterisk.manager)
+ import asterisk.config
+ help (asterisk.config)
+
+Some notes on platforms: We now specify "platforms = 'Any'" in
+``setup.py``. This means, the manager part of the package will probably
+run on any platform. The agi scripts on the other hand are called
+directly on the host where Asterisk is running in which case they are
+limited to the platforms asterisk is running on. Alternatively, you can
+use the *fastagi* mechanism of asterisk which calls the agi scripts on a
+remote host. In the latter case this host can be any platform where
+python runs.
+
+Tests
+-----
+
+The tests are standard pytest-compatible tests. Run with::
+
+    python3 -m pytest test
+
+Credits
+-------
+
+Thanks to Karl Putland for writing the original package.
+Thanks to Matthew Nicholson for maintaining the package for some years
+and for handing over maintenance when he was no longer interested.
+
+Thanks also to the people in the sourceforge project and those who just
+report bugs:
+Antoine Brenner,
+Max Nesterov,
+Sven Uebelacker
+To Matthias Urlichs for maintaining the debian package (at least for
+some time).
+
+... and to unnamed contributors to earlier releases.
+
+Things to do for pyst
+---------------------
+
+This is the original changelog merged into the readme file. I'm not so
+sure I really want to change all these things (in particular the
+threaded implementation looks good to me). I will maintain a section
+summarizing the changes in this README, the ChangeLog won't be
+maintained any longer. Detailed changes will be available in the version
+control tool.
+
+* ChangeLog:
+  The ChangeLog needs to be updated from the monotone logs.
+
+* Documentation:
+  All of pyst's inline documentation needs to be updated.
+
+* manager.py:
+  This should be converted to be single threaded.  Also there is a race
+  condition when a user calls manager.logoff() followed by
+  manager.close().  The close() function may still call logoff again if
+  the socket thread has not yet cleared the _connected flag.
+
+  A class should be made for each manager action rather than having a
+  function in a manager class.  The manager class should be adapted to
+  have a send method that know the general format of the classes.
+
+Matthew Nicholson writes on the mailinglist (note that I'm not sure I'll do
+this, I'm currently satisfied with the threaded implementation):
+
+    For pyst 0.3 I am planning to clean up the manager.py.  There are
+    several know issues with the code.  No one has actually reported these
+    as problems, but I have personally had trouble with these.  Currently
+    manager.py runs in several threads, the main program thread, a thread to
+    read from the network, and an event distribution thread.  This causes
+    problems with non thread safe code such as the MySQLdb libraries.  This
+    design also causes problems when an event handler throws an exception
+    that causes the event processing thread to terminate.
+
+    The second problem is with the way actions are sent.  Each action has a
+    specific function associated with it in the manager object that takes
+    all possible arguments that may ever be passed to that action.  This
+    makes the api somewhat rigid and the Manager object cluttered.
+
+    To solve these problems I am basically going to copy the design of my
+    Astxx manager library (written in c++) and make it more python like.
+    Each action will be a different object with certain methods to handle
+    various tasks, with one function in the actual Manager class to send the
+    action.  This will make the Manager class much smaller and much more
+    flexible.  The current code will be consolidated into a single threaded
+    design with hooks to have the library process events and such.  These
+    hooks will be called from the host application's main loop.
+
+
+Source Code Repository Access
+-----------------------------
+
+The current versions are kept in a GIT repository on Github.
+You can check out the trunk with::
+
+ git clone https://github.com/schlatterbeck/pyst.git
+
+I will continue to push to the Sourceforge version although Bug-Reports
+etc. are easier with Github. Check out from Sourceforge with::
+
+    git clone git://git.code.sf.net/p/pyst/code pyst
+
+There is a monotone-after-0.2 branch which contains unreleased changes
+after 0.2 which were committed to the monotone repository after the
+Release of Version 0.2 (which have been merged into trunk *after*
+changing how manager commands to asterisk are parsed).
+
+Released versions are tagged, see the tags in the web-interface on
+Sourceforge (or use local git commands to find out)
+
+    https://sourceforge.net/p/pyst/code/ci/master/tree/
+
+For versions up to 0.6 the code was kept in a Subversion repository in
+Sourceforge. This has been incorporated into the current GIT repository
+(after cleaning up some subversion artefacts).
+
+For versions prior to the 0.2 release when Matthew Nicholson was
+maintaining pyst, the changes were kept in a `monotone`_ repository
+(monotone is a free distributed version control system). This repository
+has also been incorporated into the GIT repository.
+
+.. _`monotone`: http://monotone.ca/
+
+prior to that the sources are in the CVS repository on sourceforge which
+has also been incorporated into the GIT repository.
+
+
+Changes
+-------
+
+Version 0.9: Add LICENSE, pyproject.toml, remove old test harness
+
+- Added LICENSE, the software always was dual-licensed, no LGPL update
+  clause ("2.0 or later") was specified at the time. The license should
+  still be GPL/LGPL 3.0 compatible due to the dual-licensing with the
+  python software foundation license.
+- New section in README.rst for running the tests after removing old
+  test harness
+- Add patch to allow connecting using IPv6
+
+Version 0.8: Fix README.rst
+
+Cleanup of README before releasing 0.8 on pypi.
+
+Version 0.7: Update tests, Compatibility
+
+Now a test for AGI exists (in addition the the existing AMI test).
+Asterisk in newer versions yields output of AMI commands prefixed with
+``Output:``. This was already correctly parsed into the ``multiheaders``
+variable where Lines with a repeated header are kept. For
+backwards-compatibility all these lines are also put into the old
+``data`` variable, too. So if you were using ``data`` with old versions
+of asterisk your code continues to work with pyst.
+Python 3.7 has introduced a new keyword ``async``. Unfortunately we were
+using this keyword as a parameter of the AMI ``originate`` call. I've
+changed this to ``run_async`` (to be compatible with pyst2, I would have
+named it simpy ``asynchronous``, see the commit history).
+
+Version 0.6: Minor feature enhancements
+
+The asterisk management interface emulator asterisk/astemu now can be
+used for unit-tests of applications using asterisk.manager. We're using
+this in the regression test (see test directory). But this way it is
+usable by others.
+
+- Factor asterisk emulator from regression test into own module
+
+Version 0.5: Small install change
+
+Fix setup.py to include download_url. This makes it installable using
+intall tools like pip.
+
+- Add download_url to setup.py
+- Fix svn url after SourceForge upgrade
+
+Version 0.4: Minor feature enhancements
+
+Small feature extensions to AGI and Manager modules. Add a regression
+test which now covers some aspects of the manager API.
+
+- Handle events with several fields with the same name (e.g. 'Variable'
+  in the 'AgentCalled' event. Thanks to Max Nesterov for the
+  suggestion, implementation differs from the suggestion in SF patch
+  3290869. For a use-case see the give SF patch and the regression test
+  case test_agent_event.
+- Allow to use AGI module in FastAGI way via TCP connection.
+  This change allows you to specify the socket streams instead
+  sys.stdin/sys.stdout streams. Thanks to Max Nesterov for the patch.
+  Applies SF patch 3047290.
+- Add regression test framework and some test cases for manager API.
+- The generated ActionID for the manager interface now includes the
+  process-ID, this allows several concurrent processes using the
+  manager API.
+
+Version 0.3: Minor feature enhancements
+
+New maintainer Ralf Schlatterbeck, this is my first release, please
+report any problems via the Sourceforge Bug-Tracker or email me
+directly. Thanks to Karl Putland for writing the original package.
+Thanks to Matthew Nicholson for maintaining the package for some years
+and for handing over maintenance when he was no longer interested.
+The parsing of answers from asterisk was completely rewritten. This
+should fix problems people were having with commands returning embedded
+'/' or empty lines. Some new manager commands added.
+
+- Add playdtmf manager command
+- add sippeers and sipshowpeer manager commands
+- rewritten manager communication
+- should no longer choke on '/' in answers returned from a manager
+  command (fixes SF Bug 2947866)
+- should now correctly parse multi-line output with embedded empty
+  lines, e.g. ``mgr.command('dialplan show')``
+- Bug-fix for list manipulation in ``event_dispatch``, thanks to Jan
+  Mueller, see mailinglist comment from 2008-04-18
+- Merge unreleased changes from repository of Matthew Nicholson
+  in particular a typo in ``agi.py`` for ``set_autohangup``, and change
+  of ``get_header`` methods (see Upgrading instructions). The fixed
+  ``manager.command`` support is already in (with a different
+  solution). The unreleased changes are also on the 0.2 branch in the
+  subversion repository in case somebody is interested.
+
```

### Comparing `pyst-0.8/setup.py` & `pyst-0.9/setup.py`

 * *Files identical despite different names*

