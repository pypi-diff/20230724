# Comparing `tmp/shareddata-2.0.9.tar.gz` & `tmp/shareddata-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.0.9.tar", last modified: Tue May  9 14:25:32 2023, max compression
+gzip compressed data, was "shareddata-2.1.0.tar", last modified: Mon Jul 24 01:11:20 2023, max compression
```

## Comparing `shareddata-2.0.9.tar` & `shareddata-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.461357 shareddata-2.0.9/
--rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.9/LICENSE
--rw-rw-rw-   0        0        0     1100 2023-05-09 14:25:32.461357 shareddata-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-07 14:43:50.000000 shareddata-2.0.9/README.md
--rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-05-09 14:25:32.462356 shareddata-2.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.432356 shareddata-2.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.450356 shareddata-2.0.9/src/SharedData/
--rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.9/src/SharedData/Defaults.py
--rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.9/src/SharedData/Logger.py
--rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.9/src/SharedData/LoggerConsumerProcess.py
--rw-rw-rw-   0        0        0    11544 2023-05-07 12:00:04.000000 shareddata-2.0.9/src/SharedData/Metadata.py
--rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/MultiProc.py
--rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/SeriesLib.py
--rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.9/src/SharedData/SharedData.py
--rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.9/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-rw-   0        0        0     4586 2023-05-07 14:46:16.000000 shareddata-2.0.9/src/SharedData/SharedDataAWSS3.py
--rw-rw-rw-   0        0        0     6275 2023-05-04 17:59:07.000000 shareddata-2.0.9/src/SharedData/SharedDataFeeder.py
--rw-rw-rw-   0        0        0    11176 2023-05-07 14:43:48.000000 shareddata-2.0.9/src/SharedData/SharedDataFrame.py
--rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.9/src/SharedData/SharedDataPeriod.py
--rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/SharedDataRealTime.py
--rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-rw-   0        0        0    26032 2023-05-09 10:40:45.000000 shareddata-2.0.9/src/SharedData/SharedDataTable.py
--rw-rw-rw-   0        0        0    31268 2023-05-09 14:25:12.000000 shareddata-2.0.9/src/SharedData/SharedDataTableKeys.py
--rw-rw-rw-   0        0        0    17673 2023-05-07 14:43:48.000000 shareddata-2.0.9/src/SharedData/SharedDataTimeSeries.py
--rw-rw-rw-   0        0        0     7221 2023-05-09 14:12:01.000000 shareddata-2.0.9/src/SharedData/SharedNumpy.py
--rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.460358 shareddata-2.0.9/src/shareddata.egg-info/
--rw-rw-rw-   0        0        0     1100 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:11:20.155553 shareddata-2.1.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:11:20.155553 shareddata-2.1.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-24 01:11:20.159553 shareddata-2.1.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:11:20.155553 shareddata-2.1.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:11:20.155553 shareddata-2.1.0/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.0/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/SeriesLib.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.0/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.0/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/SharedDataAWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1822 2023-07-23 19:20:04.000000 shareddata-2.1.0/src/SharedData/SharedDataFeeder.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.0/src/SharedData/SharedDataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14997 2023-07-24 01:04:18.000000 shareddata-2.1.0/src/SharedData/SharedDataPeriod.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.0/src/SharedData/SharedDataRealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28691 2023-07-18 17:59:43.000000 shareddata-2.1.0/src/SharedData/SharedDataTable.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.0/src/SharedData/SharedDataTableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.0/src/SharedData/SharedDataTableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21457 2023-07-24 01:05:01.000000 shareddata-2.1.0/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.0/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.0/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.0/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-24 01:11:20.155553 shareddata-2.1.0/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-24 01:11:20.000000 shareddata-2.1.0/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-24 01:11:20.000000 shareddata-2.1.0/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-24 01:11:20.000000 shareddata-2.1.0/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-24 01:11:20.000000 shareddata-2.1.0/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-24 01:11:20.000000 shareddata-2.1.0/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.0.9/LICENSE` & `shareddata-2.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `shareddata-2.0.9/src/SharedData/Logger.py` & `shareddata-2.1.0/src/SharedData/Logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,119 @@
-import os,sys
-import logging
-import boto3
-from pathlib import Path
-from datetime import datetime, timedelta
-import glob
-import pandas as pd
-from pythonjsonlogger.jsonlogger import JsonFormatter
-import boto3
-
-from importlib.metadata import version
-
-import SharedData.Defaults as Defaults 
-from SharedData.SharedDataAWSKinesis import KinesisLogStreamHandler
-
-
-class Logger:
-
-    log = None
-    user = None
-
-    def __init__(self, source, user=None):
-        if Logger.log is None:                                
-            if 'SOURCE_FOLDER' in os.environ:
-                try:
-                    commompath = os.path.commonpath([source,os.environ['SOURCE_FOLDER']])
-                    source = source.replace(commompath,'')
-                except:
-                    pass
-            elif 'USERPROFILE' in os.environ:
-                try:
-                    commompath = os.path.commonpath([source,os.environ['USERPROFILE']])
-                    source = source.replace(commompath,'')
-                except:
-                    pass
-            
-            source = source.replace('venv\\lib\\site-packages\\','')
-            source = source.replace('Windows\\system32\\','')
-
-            if not user is None:                
-                Logger.user = user
-            else:
-                user = 'guest'
-                Logger.user = 'guest'
-            
-            
-            source = source.lstrip('src').lstrip('\\src')
-            source = source.lstrip('\\').lstrip('/')        
-            source = source.replace('.py','')
-            self.source = source
-
-            path = Path(os.environ['DATABASE_FOLDER'])
-            path = path / 'Logs'
-            path = path / datetime.now().strftime('%Y%m%d')
-            path = path / (os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'])        
-            path = path / (source+'.log')
-            if not path.parents[0].is_dir():
-                os.makedirs(path.parents[0])
-            os.environ['LOG_PATH'] = str(path)
-
-            if 'LOG_LEVEL' in os.environ:
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    loglevel = logging.DEBUG
-                elif os.environ['LOG_LEVEL']=='INFO':
-                    loglevel = logging.INFO   
-            else:
-                loglevel = logging.INFO
-
-            # Create Logger
-            self.log = logging.getLogger(source)
-            self.log.setLevel(logging.DEBUG)    
-            formatter = logging.Formatter(os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'] + 
-                ';%(asctime)s;%(name)s;%(levelname)s;%(message)s',\
-                datefmt='%Y-%m-%dT%H:%M:%S%z')
-            #log screen
-            handler = logging.StreamHandler()
-            handler.setLevel(loglevel)    
-            handler.setFormatter(formatter)
-            self.log.addHandler(handler)
-            #log file        
-            fhandler = logging.FileHandler(os.environ['LOG_PATH'], mode='a')
-            fhandler.setLevel(loglevel)    
-            fhandler.setFormatter(formatter)
-            self.log.addHandler(fhandler)
-            #log to aws kinesis
-            kinesishandler = KinesisLogStreamHandler(user=Logger.user)
-            kinesishandler.setLevel(logging.DEBUG)
-            jsonformatter = JsonFormatter(os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'] + 
-                ';%(asctime)s;%(name)s;%(levelname)s;%(message)s',\
-                datefmt='%Y-%m-%dT%H:%M:%S%z')
-            kinesishandler.setFormatter(jsonformatter)
-            self.log.addHandler(kinesishandler)
-            #assign static variable log to be used by modules
-            Logger.log = self.log
-            try:
-                Logger.log.debug('Logger initialized shareddata user %s version %s!' % \
-                    (Logger.user,version('SharedData')))
-            except:
-                Logger.log.debug('Logger initialized shareddata!')
-        
-    def readLogs(self):    
-        logsdir = Path(os.environ['LOG_PATH']).parents[0]
-        lenlogsdir = len(str(logsdir))
-        files = glob.glob(str(logsdir) + "/**/*.log", recursive = True)   
-        df = pd.DataFrame()
-        # f=files[0]
-        for f in files:
-            source = f[lenlogsdir+1:].replace('.log','.py')
-            try:
-                _df = pd.read_csv(f,header=None,sep=';',\
-                    engine='python',on_bad_lines='skip')
-                _df.columns = ['user','datetime','name','type','message']
-                _df['source'] = source
-                df = df.append(_df)
-            except Exception as e:
-                print('Read logs error:'+str(e))
-
-        return df
+import os,sys
+import logging
+import boto3
+from pathlib import Path
+from datetime import datetime, timedelta
+import glob
+import pandas as pd
+from pythonjsonlogger.jsonlogger import JsonFormatter
+import boto3
+
+from importlib.metadata import version
+
+import SharedData.Defaults as Defaults 
+from SharedData.SharedDataAWSKinesis import KinesisLogStreamHandler
+
+
+class Logger:
+
+    log = None
+    user = None
+
+    def __init__(self, source, user=None):
+        if Logger.log is None:                                
+            if 'SOURCE_FOLDER' in os.environ:
+                try:
+                    commompath = os.path.commonpath([source,os.environ['SOURCE_FOLDER']])
+                    source = source.replace(commompath,'')
+                except:
+                    pass
+            elif 'USERPROFILE' in os.environ:
+                try:
+                    commompath = os.path.commonpath([source,os.environ['USERPROFILE']])
+                    source = source.replace(commompath,'')
+                except:
+                    pass
+            
+            finds = 'site-packages'
+            if finds in source:
+                cutid = source.find(finds) + len(finds) + 1
+                source = source[cutid:]            
+            source = source.replace('Windows\\system32\\','')
+            source = source.lstrip('src').lstrip('\\src')
+            source = source.lstrip('\\').lstrip('/')        
+            source = source.replace('.py','')
+            self.source = source
+            
+            if not user is None:                
+                Logger.user = user
+            else:
+                user = 'guest'
+                Logger.user = 'guest'
+                        
+            path = Path(os.environ['DATABASE_FOLDER'])
+            path = path / 'Logs'
+            path = path / datetime.now().strftime('%Y%m%d')
+            path = path / (os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'])        
+            path = path / (source+'.log')
+            if not path.parents[0].is_dir():
+                os.makedirs(path.parents[0])
+            os.environ['LOG_PATH'] = str(path)
+
+            if 'LOG_LEVEL' in os.environ:
+                if os.environ['LOG_LEVEL']=='DEBUG':
+                    loglevel = logging.DEBUG
+                elif os.environ['LOG_LEVEL']=='INFO':
+                    loglevel = logging.INFO   
+            else:
+                loglevel = logging.INFO
+
+            # Create Logger
+            self.log = logging.getLogger(source)
+            self.log.setLevel(logging.DEBUG)    
+            formatter = logging.Formatter(os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'] + 
+                ';%(asctime)s;%(name)s;%(levelname)s;%(message)s',\
+                datefmt='%Y-%m-%dT%H:%M:%S%z')
+            #log screen
+            handler = logging.StreamHandler()
+            handler.setLevel(loglevel)    
+            handler.setFormatter(formatter)
+            self.log.addHandler(handler)
+            #log file        
+            fhandler = logging.FileHandler(os.environ['LOG_PATH'], mode='a')
+            fhandler.setLevel(loglevel)    
+            fhandler.setFormatter(formatter)
+            self.log.addHandler(fhandler)
+            #log to aws kinesis
+            kinesishandler = KinesisLogStreamHandler(user=Logger.user)
+            kinesishandler.setLevel(logging.DEBUG)
+            jsonformatter = JsonFormatter(os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'] + 
+                ';%(asctime)s;%(name)s;%(levelname)s;%(message)s',\
+                datefmt='%Y-%m-%dT%H:%M:%S%z')
+            kinesishandler.setFormatter(jsonformatter)
+            self.log.addHandler(kinesishandler)
+            #assign static variable log to be used by modules
+            Logger.log = self.log
+            try:
+                Logger.log.debug('Logger initialized shareddata user %s version %s!' % \
+                    (Logger.user,version('SharedData')))
+            except:
+                Logger.log.debug('Logger initialized shareddata!')
+        
+    def readLogs(self):    
+        logsdir = Path(os.environ['LOG_PATH']).parents[0]
+        lenlogsdir = len(str(logsdir))
+        files = glob.glob(str(logsdir) + "/**/*.log", recursive = True)   
+        df = pd.DataFrame()
+        # f=files[0]
+        for f in files:
+            source = f[lenlogsdir+1:].replace('.log','.py')
+            try:
+                _df = pd.read_csv(f,header=None,sep=';',\
+                    engine='python',on_bad_lines='skip')
+                _df.columns = ['user','datetime','name','type','message']
+                _df['source'] = source
+                df = df.append(_df)
+            except Exception as e:
+                print('Read logs error:'+str(e))
+
+        return df
```

### Comparing `shareddata-2.0.9/src/SharedData/MultiProc.py` & `shareddata-2.1.0/src/SharedData/MultiProc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,242 +1,280 @@
-00000000: 0d0a 2320 5375 7065 7246 6173 7450 7974  ..# SuperFastPyt
-00000010: 686f 6e2e 636f 6d0d 0a23 206c 6f61 6420  hon.com..# load 
-00000020: 6d61 6e79 2066 696c 6573 2063 6f6e 6375  many files concu
-00000030: 7272 656e 746c 7920 7769 7468 2070 726f  rrently with pro
-00000040: 6365 7373 6573 2061 6e64 2074 6872 6561  cesses and threa
-00000050: 6473 2069 6e20 6261 7463 680d 0a69 6d70  ds in batch..imp
-00000060: 6f72 7420 6d75 6c74 6970 726f 6365 7373  ort multiprocess
-00000070: 696e 670d 0a66 726f 6d20 636f 6e63 7572  ing..from concur
-00000080: 7265 6e74 2e66 7574 7572 6573 2069 6d70  rent.futures imp
-00000090: 6f72 7420 5072 6f63 6573 7350 6f6f 6c45  ort ProcessPoolE
-000000a0: 7865 6375 746f 720d 0a66 726f 6d20 636f  xecutor..from co
-000000b0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-000000c0: 2069 6d70 6f72 7420 5468 7265 6164 506f   import ThreadPo
-000000d0: 6f6c 4578 6563 7574 6f72 0d0a 0d0a 0d0a  olExecutor......
-000000e0: 2320 5553 4147 4520 4558 414d 504c 453a  # USAGE EXAMPLE:
-000000f0: 0d0a 2320 696f 5f62 6f75 6e64 2874 6872  ..# io_bound(thr
-00000100: 6561 645f 6675 6e63 2c20 6974 6572 6174  ead_func, iterat
-00000110: 6f72 2c20 6172 6773 290d 0a23 2074 6872  or, args)..# thr
-00000120: 6561 645f 6675 6e63 3a64 6566 696e 6520  ead_func:define 
-00000130: 7468 6520 7461 736b 2066 756e 6374 696f  the task functio
-00000140: 6e20 746f 2072 756e 2070 6172 616c 6c65  n to run paralle
-00000150: 6c2e 2049 653a 2072 6561 645f 6669 6c65  l. Ie: read_file
-00000160: 732c 6461 7973 5f74 7261 6469 6e67 5f66  s,days_trading_f
-00000170: 726f 6d5f 746f 0d0a 2320 6974 6572 6174  rom_to..# iterat
-00000180: 696f 6e3a 2073 696e 676c 6520 6974 6572  ion: single iter
-00000190: 6174 696f 6e20 6974 656d 7320 6f66 2070  ation items of p
-000001a0: 6172 616c 6c65 6c20 7461 736b 0d0a 2320  arallel task..# 
-000001b0: 6172 6773 3a20 636f 6d6d 6f6d 2074 6173  args: commom tas
-000001c0: 6b20 7661 7269 6162 6c65 7320 0d0a 0d0a  k variables ....
-000001d0: 2320 7468 7265 6164 5f66 756e 6320 4558  # thread_func EX
-000001e0: 414d 504c 4553 0d0a 0d0a 2320 494f 2042  AMPLES....# IO B
-000001f0: 4f55 4e44 2045 5841 4d50 4c45 0d0a 2320  OUND EXAMPLE..# 
-00000200: 6465 6620 7265 6164 5f66 696c 6573 2869  def read_files(i
-00000210: 7465 7261 7469 6f6e 2c20 6172 6773 293a  teration, args):
-00000220: 0d0a 2320 2020 2020 6669 6c65 6964 203d  ..#     fileid =
-00000230: 2069 7465 7261 7469 6f6e 5b30 5d20 2020   iteration[0]   
-00000240: 200d 0a23 2020 2020 2066 696c 655f 6c69   ..#     file_li
-00000250: 7374 203d 2061 7267 735b 305d 0d0a 2320  st = args[0]..# 
-00000260: 2020 2020 6670 6174 6820 3d20 6669 6c65      fpath = file
-00000270: 5f6c 6973 745b 6669 6c65 6964 5d0d 0a23  _list[fileid]..#
-00000280: 2020 2020 2064 6620 3d20 7064 2e72 6561       df = pd.rea
-00000290: 645f 6373 7628 6670 6174 6829 0d0a 2320  d_csv(fpath)..# 
-000002a0: 2020 2020 7265 7475 726e 205b 6466 5d0d      return [df].
-000002b0: 0a0d 0a23 2043 5055 2042 4f55 4e44 2045  ...# CPU BOUND E
-000002c0: 5841 4d50 4c45 0d0a 2320 6465 6620 6461  XAMPLE..# def da
-000002d0: 7973 5f74 7261 6469 6e67 5f66 726f 6d5f  ys_trading_from_
-000002e0: 746f 2869 7465 7261 7469 6f6e 2c20 6172  to(iteration, ar
-000002f0: 6773 293a 0d0a 2320 2020 2020 6361 6c20  gs):..#     cal 
-00000300: 3d20 6974 6572 6174 696f 6e5b 305d 0d0a  = iteration[0]..
-00000310: 2320 2020 2020 7374 6172 7420 3d20 6974  #     start = it
-00000320: 6572 6174 696f 6e5b 315d 0d0a 2320 2020  eration[1]..#   
-00000330: 2020 656e 6420 3d20 6974 6572 6174 696f    end = iteratio
-00000340: 6e5b 325d 0d0a 2320 2020 2020 6361 6c65  n[2]..#     cale
-00000350: 6e64 6172 7320 3d20 6172 6773 5b30 5d0d  ndars = args[0].
-00000360: 0a23 2020 2020 2069 6478 203d 2028 6361  .#     idx = (ca
-00000370: 6c65 6e64 6172 735b 6361 6c5d 3e3d 7374  lendars[cal]>=st
-00000380: 6172 7429 2026 2028 2863 616c 656e 6461  art) & ((calenda
-00000390: 7273 5b63 616c 5d3c 3d65 6e64 2929 0d0a  rs[cal]<=end))..
-000003a0: 2320 2020 2020 7265 7475 726e 205b 6e70  #     return [np
-000003b0: 2e63 6f75 6e74 5f6e 6f6e 7a65 726f 2869  .count_nonzero(i
-000003c0: 6478 295d 0d0a 0d0a 2320 7265 7475 726e  dx)]....# return
-000003d0: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
-000003e0: 206d 616e 7920 6669 6c65 730d 0a64 6566   many files..def
-000003f0: 2069 6f5f 626f 756e 645f 7072 6f63 6573   io_bound_proces
-00000400: 7328 7468 7265 6164 5f66 756e 632c 2070  s(thread_func, p
-00000410: 726f 635f 6974 6572 6174 6f72 2c20 6172  roc_iterator, ar
-00000420: 6773 293a 0d0a 2020 2020 7265 7375 6c74  gs):..    result
-00000430: 7320 3d20 5b5d 0d0a 2020 2020 2320 6372  s = []..    # cr
-00000440: 6561 7465 2061 2074 6872 6561 6420 706f  eate a thread po
-00000450: 6f6c 0d0a 2020 2020 6e70 726f 635f 6974  ol..    nproc_it
-00000460: 6572 6174 6f72 203d 206c 656e 2870 726f  erator = len(pro
-00000470: 635f 6974 6572 6174 6f72 290d 0a20 2020  c_iterator)..   
-00000480: 2069 6620 6e70 726f 635f 6974 6572 6174   if nproc_iterat
-00000490: 6f72 3e30 3a0d 0a20 2020 2020 2020 2077  or>0:..        w
-000004a0: 6974 6820 5468 7265 6164 506f 6f6c 4578  ith ThreadPoolEx
-000004b0: 6563 7574 6f72 286e 7072 6f63 5f69 7465  ecutor(nproc_ite
-000004c0: 7261 746f 7229 2061 7320 6578 653a 0d0a  rator) as exe:..
-000004d0: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-000004e0: 6164 2066 696c 6573 0d0a 2020 2020 2020  ad files..      
-000004f0: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
-00000500: 5b65 7865 2e73 7562 6d69 7428 7468 7265  [exe.submit(thre
-00000510: 6164 5f66 756e 632c 2069 7465 7261 7469  ad_func, iterati
-00000520: 6f6e 2c20 6172 6773 2920 666f 7220 6974  on, args) for it
-00000530: 6572 6174 696f 6e20 696e 2070 726f 635f  eration in proc_
-00000540: 6974 6572 6174 6f72 5d0d 0a20 2020 2020  iterator]..     
-00000550: 2020 2020 2020 2023 2063 6f6c 6c65 6374         # collect
-00000560: 2064 6174 610d 0a20 2020 2020 2020 2020   data..         
-00000570: 2020 2066 6f72 2066 7574 7572 6520 696e     for future in
-00000580: 2066 7574 7572 6573 3a0d 0a20 2020 2020   futures:..     
-00000590: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-000005a0: 2066 7574 7572 652e 7265 7375 6c74 2829   future.result()
-000005b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000005c0: 2020 7265 7375 6c74 7320 3d20 5b2a 7265    results = [*re
-000005d0: 7375 6c74 732c 202a 7265 735d 0d0a 2020  sults, *res]..  
-000005e0: 2020 2020 2020 0d0a 2020 2020 7265 7475        ..    retu
-000005f0: 726e 2072 6573 756c 7473 0d0a 200d 0a23  rn results.. ..#
-00000600: 206c 6f61 6420 616c 6c20 6669 6c65 7320   load all files 
-00000610: 696e 2061 2064 6972 6563 746f 7279 2069  in a directory i
-00000620: 6e74 6f20 6d65 6d6f 7279 0d0a 6465 6620  nto memory..def 
-00000630: 696f 5f62 6f75 6e64 2874 6872 6561 645f  io_bound(thread_
-00000640: 6675 6e63 2c20 6974 6572 6174 6f72 2c20  func, iterator, 
-00000650: 6172 6773 293a 0d0a 2020 2020 7265 7375  args):..    resu
-00000660: 6c74 7320 3d20 5b5d 0d0a 2020 2020 2320  lts = []..    # 
-00000670: 6465 7465 726d 696e 6520 6368 756e 6b73  determine chunks
-00000680: 697a 650d 0a20 2020 206e 6974 6572 6174  ize..    niterat
-00000690: 6f72 203d 206c 656e 2869 7465 7261 746f  or = len(iterato
-000006a0: 7229 0d0a 2020 2020 6966 206e 6974 6572  r)..    if niter
-000006b0: 6174 6f72 3e30 3a0d 0a20 2020 2020 2020  ator>0:..       
-000006c0: 206e 5f77 6f72 6b65 7273 203d 206d 756c   n_workers = mul
-000006d0: 7469 7072 6f63 6573 7369 6e67 2e63 7075  tiprocessing.cpu
-000006e0: 5f63 6f75 6e74 2829 202d 2032 2020 2020  _count() - 2    
-000006f0: 2020 0d0a 2020 2020 2020 2020 6e5f 776f    ..        n_wo
-00000700: 726b 6572 7320 3d20 6d69 6e28 6e5f 776f  rkers = min(n_wo
-00000710: 726b 6572 732c 6e69 7465 7261 746f 7229  rkers,niterator)
-00000720: 0d0a 2020 2020 2020 2020 6368 756e 6b73  ..        chunks
-00000730: 697a 6520 3d20 726f 756e 6428 6e69 7465  ize = round(nite
-00000740: 7261 746f 7220 2f20 6e5f 776f 726b 6572  rator / n_worker
-00000750: 7329 0d0a 2020 2020 2020 2020 2320 6372  s)..        # cr
-00000760: 6561 7465 2074 6865 2070 726f 6365 7373  eate the process
-00000770: 2070 6f6f 6c0d 0a20 2020 2020 2020 2077   pool..        w
-00000780: 6974 6820 5072 6f63 6573 7350 6f6f 6c45  ith ProcessPoolE
-00000790: 7865 6375 746f 7228 6e5f 776f 726b 6572  xecutor(n_worker
-000007a0: 7329 2061 7320 6578 6563 7574 6f72 3a20  s) as executor: 
-000007b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000007c0: 2020 2020 2066 7574 7572 6573 203d 206c       futures = l
-000007d0: 6973 7428 290d 0a20 2020 2020 2020 2020  ist()..         
-000007e0: 2020 2023 2073 706c 6974 2074 6865 206c     # split the l
-000007f0: 6f61 6420 6f70 6572 6174 696f 6e73 2069  oad operations i
-00000800: 6e74 6f20 6368 756e 6b73 0d0a 2020 2020  nto chunks..    
-00000810: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00000820: 2072 616e 6765 2830 2c20 6e69 7465 7261   range(0, nitera
-00000830: 746f 722c 2063 6875 6e6b 7369 7a65 293a  tor, chunksize):
-00000840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000850: 2020 2320 7365 6c65 6374 2061 2063 6875    # select a chu
-00000860: 6e6b 206f 6620 6669 6c65 6e61 6d65 730d  nk of filenames.
-00000870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000880: 2070 726f 635f 6974 6572 6174 6f72 203d   proc_iterator =
-00000890: 2069 7465 7261 746f 725b 693a 2869 202b   iterator[i:(i +
-000008a0: 2063 6875 6e6b 7369 7a65 295d 0d0a 2020   chunksize)]..  
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000008c0: 7375 626d 6974 2074 6865 2074 6173 6b0d  submit the task.
-000008d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000008e0: 2066 7574 7572 6520 3d20 6578 6563 7574   future = execut
-000008f0: 6f72 2e73 7562 6d69 7428 696f 5f62 6f75  or.submit(io_bou
-00000900: 6e64 5f70 726f 6365 7373 2c20 7468 7265  nd_process, thre
-00000910: 6164 5f66 756e 632c 2070 726f 635f 6974  ad_func, proc_it
-00000920: 6572 6174 6f72 2c20 6172 6773 290d 0a20  erator, args).. 
-00000930: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000940: 7574 7572 6573 2e61 7070 656e 6428 6675  utures.append(fu
-00000950: 7475 7265 290d 0a20 2020 2020 2020 2020  ture)..         
-00000960: 2020 2023 2070 726f 6365 7373 2061 6c6c     # process all
-00000970: 2072 6573 756c 7473 0d0a 2020 2020 2020   results..      
-00000980: 2020 2020 2020 666f 7220 6675 7475 7265        for future
-00000990: 2069 6e20 6675 7475 7265 733a 0d0a 2020   in futures:..  
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000009b0: 6f70 656e 2074 6865 2066 696c 6520 616e  open the file an
-000009c0: 6420 6c6f 6164 2074 6865 2064 6174 610d  d load the data.
-000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009e0: 2072 6573 203d 2066 7574 7572 652e 7265   res = future.re
-000009f0: 7375 6c74 2829 0d0a 2020 2020 2020 2020  sult()..        
-00000a00: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-00000a10: 3d20 5b2a 7265 7375 6c74 732c 202a 7265  = [*results, *re
-00000a20: 735d 0d0a 2020 2020 7265 7475 726e 2072  s]..    return r
-00000a30: 6573 756c 7473 0d0a 0d0a 0d0a 2320 7265  esults......# re
-00000a40: 7475 726e 2074 6865 2063 6f6e 7465 6e74  turn the content
-00000a50: 7320 6f66 206d 616e 7920 6669 6c65 730d  s of many files.
-00000a60: 0a64 6566 2063 7075 5f62 6f75 6e64 5f70  .def cpu_bound_p
-00000a70: 726f 6365 7373 2874 6872 6561 645f 6675  rocess(thread_fu
-00000a80: 6e63 2c20 7072 6f63 5f69 7465 7261 746f  nc, proc_iterato
-00000a90: 722c 2061 7267 7329 3a0d 0a20 2020 2072  r, args):..    r
-00000aa0: 6574 7572 6e20 5b74 6872 6561 645f 6675  eturn [thread_fu
-00000ab0: 6e63 2869 7465 7261 7469 6f6e 2c20 6172  nc(iteration, ar
-00000ac0: 6773 2920 666f 7220 6974 6572 6174 696f  gs) for iteratio
-00000ad0: 6e20 696e 2070 726f 635f 6974 6572 6174  n in proc_iterat
-00000ae0: 6f72 5d0d 0a0d 0a64 6566 2063 7075 5f62  or]....def cpu_b
-00000af0: 6f75 6e64 2874 6872 6561 645f 6675 6e63  ound(thread_func
-00000b00: 2c20 6974 6572 6174 6f72 2c20 6172 6773  , iterator, args
-00000b10: 293a 0d0a 2020 2020 7265 7375 6c74 7320  ):..    results 
-00000b20: 3d20 5b5d 0d0a 2020 2020 2320 6465 7465  = []..    # dete
-00000b30: 726d 696e 6520 6368 756e 6b73 697a 650d  rmine chunksize.
-00000b40: 0a20 2020 206e 6974 6572 6174 6f72 203d  .    niterator =
-00000b50: 206c 656e 2869 7465 7261 746f 7229 0d0a   len(iterator)..
-00000b60: 2020 2020 6966 206e 6974 6572 6174 6f72      if niterator
-00000b70: 3e30 3a0d 0a20 2020 2020 2020 206e 5f77  >0:..        n_w
-00000b80: 6f72 6b65 7273 203d 206d 756c 7469 7072  orkers = multipr
-00000b90: 6f63 6573 7369 6e67 2e63 7075 5f63 6f75  ocessing.cpu_cou
-00000ba0: 6e74 2829 202d 2032 2020 2020 0d0a 2020  nt() - 2    ..  
-00000bb0: 2020 2020 2020 6e5f 776f 726b 6572 7320        n_workers 
-00000bc0: 3d20 6d69 6e28 6e5f 776f 726b 6572 732c  = min(n_workers,
-00000bd0: 6e69 7465 7261 746f 7229 0d0a 2020 2020  niterator)..    
-00000be0: 2020 2020 6368 756e 6b73 697a 6520 3d20      chunksize = 
-00000bf0: 726f 756e 6428 6e69 7465 7261 746f 7220  round(niterator 
-00000c00: 2f20 6e5f 776f 726b 6572 7329 0d0a 2020  / n_workers)..  
-00000c10: 2020 2020 2020 2320 6372 6561 7465 2074        # create t
-00000c20: 6865 2070 726f 6365 7373 2070 6f6f 6c0d  he process pool.
-00000c30: 0a20 2020 2020 2020 2077 6974 6820 5072  .        with Pr
-00000c40: 6f63 6573 7350 6f6f 6c45 7865 6375 746f  ocessPoolExecuto
-00000c50: 7228 6e5f 776f 726b 6572 7329 2061 7320  r(n_workers) as 
-00000c60: 6578 6563 7574 6f72 3a20 2020 2020 2020  executor:       
-00000c70: 200d 0a20 2020 2020 2020 2020 2020 2066   ..            f
-00000c80: 7574 7572 6573 203d 206c 6973 7428 290d  utures = list().
-00000c90: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00000ca0: 706c 6974 2074 6865 206c 6f61 6420 6f70  plit the load op
-00000cb0: 6572 6174 696f 6e73 2069 6e74 6f20 6368  erations into ch
-00000cc0: 756e 6b73 0d0a 2020 2020 2020 2020 2020  unks..          
-00000cd0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00000ce0: 2830 2c20 6e69 7465 7261 746f 722c 2063  (0, niterator, c
-00000cf0: 6875 6e6b 7369 7a65 293a 0d0a 2020 2020  hunksize):..    
-00000d00: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00000d10: 6c65 6374 2061 2063 6875 6e6b 206f 6620  lect a chunk of 
-00000d20: 6669 6c65 6e61 6d65 730d 0a20 2020 2020  filenames..     
-00000d30: 2020 2020 2020 2020 2020 2070 726f 635f             proc_
-00000d40: 6974 6572 6174 6f72 203d 2069 7465 7261  iterator = itera
-00000d50: 746f 725b 693a 2869 202b 2063 6875 6e6b  tor[i:(i + chunk
-00000d60: 7369 7a65 295d 0d0a 2020 2020 2020 2020  size)]..        
-00000d70: 2020 2020 2020 2020 2320 7375 626d 6974          # submit
-00000d80: 2074 6865 2074 6173 6b0d 0a20 2020 2020   the task..     
-00000d90: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-00000da0: 6520 3d20 6578 6563 7574 6f72 2e73 7562  e = executor.sub
-00000db0: 6d69 7428 6370 755f 626f 756e 645f 7072  mit(cpu_bound_pr
-00000dc0: 6f63 6573 732c 2074 6872 6561 645f 6675  ocess, thread_fu
-00000dd0: 6e63 2c20 7072 6f63 5f69 7465 7261 746f  nc, proc_iterato
-00000de0: 722c 2061 7267 7329 0d0a 2020 2020 2020  r, args)..      
-00000df0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-00000e00: 732e 6170 7065 6e64 2866 7574 7572 6529  s.append(future)
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
-00000e40: 2070 726f 6365 7373 2061 6c6c 2072 6573   process all res
-00000e50: 756c 7473 0d0a 2020 2020 2020 2020 2020  ults..          
-00000e60: 2020 666f 7220 6675 7475 7265 2069 6e20    for future in 
-00000e70: 6675 7475 7265 733a 0d0a 2020 2020 2020  futures:..      
-00000e80: 2020 2020 2020 2020 2020 2320 6f70 656e            # open
-00000e90: 2074 6865 2066 696c 6520 616e 6420 6c6f   the file and lo
-00000ea0: 6164 2074 6865 2064 6174 610d 0a20 2020  ad the data..   
-00000eb0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00000ec0: 203d 2066 7574 7572 652e 7265 7375 6c74   = future.result
-00000ed0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00000ee0: 2020 2020 7265 7375 6c74 7320 3d20 5b2a      results = [*
-00000ef0: 7265 7375 6c74 732c 202a 7265 735d 0d0a  results, *res]..
-00000f00: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00000f10: 7473 0d0a 0d0a                           ts....
+00000000: 0a23 2053 7570 6572 4661 7374 5079 7468  .# SuperFastPyth
+00000010: 6f6e 2e63 6f6d 0a23 206c 6f61 6420 6d61  on.com.# load ma
+00000020: 6e79 2066 696c 6573 2063 6f6e 6375 7272  ny files concurr
+00000030: 656e 746c 7920 7769 7468 2070 726f 6365  ently with proce
+00000040: 7373 6573 2061 6e64 2074 6872 6561 6473  sses and threads
+00000050: 2069 6e20 6261 7463 680a 696d 706f 7274   in batch.import
+00000060: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+00000070: 0a66 726f 6d20 636f 6e63 7572 7265 6e74  .from concurrent
+00000080: 2e66 7574 7572 6573 2069 6d70 6f72 7420  .futures import 
+00000090: 5072 6f63 6573 7350 6f6f 6c45 7865 6375  ProcessPoolExecu
+000000a0: 746f 720a 6672 6f6d 2063 6f6e 6375 7272  tor.from concurr
+000000b0: 656e 742e 6675 7475 7265 7320 696d 706f  ent.futures impo
+000000c0: 7274 2054 6872 6561 6450 6f6f 6c45 7865  rt ThreadPoolExe
+000000d0: 6375 746f 720a 6672 6f6d 2063 6666 6920  cutor.from cffi 
+000000e0: 696d 706f 7274 2046 4649 0a66 726f 6d20  import FFI.from 
+000000f0: 7471 646d 2069 6d70 6f72 7420 7471 646d  tqdm import tqdm
+00000100: 0a69 6d70 6f72 7420 7469 6d65 0a66 726f  .import time.fro
+00000110: 6d20 7468 7265 6164 696e 6720 696d 706f  m threading impo
+00000120: 7274 2054 6872 6561 640a 0a23 2055 5341  rt Thread..# USA
+00000130: 4745 2045 5841 4d50 4c45 3a0a 2320 696f  GE EXAMPLE:.# io
+00000140: 5f62 6f75 6e64 2874 6872 6561 645f 6675  _bound(thread_fu
+00000150: 6e63 2c20 6974 6572 6174 6f72 2c20 6172  nc, iterator, ar
+00000160: 6773 290a 2320 7468 7265 6164 5f66 756e  gs).# thread_fun
+00000170: 633a 6465 6669 6e65 2074 6865 2074 6173  c:define the tas
+00000180: 6b20 6675 6e63 7469 6f6e 2074 6f20 7275  k function to ru
+00000190: 6e20 7061 7261 6c6c 656c 2e20 4965 3a20  n parallel. Ie: 
+000001a0: 7265 6164 5f66 696c 6573 2c64 6179 735f  read_files,days_
+000001b0: 7472 6164 696e 675f 6672 6f6d 5f74 6f0a  trading_from_to.
+000001c0: 2320 6974 6572 6174 696f 6e3a 2073 696e  # iteration: sin
+000001d0: 676c 6520 6974 6572 6174 696f 6e20 6974  gle iteration it
+000001e0: 656d 7320 6f66 2070 6172 616c 6c65 6c20  ems of parallel 
+000001f0: 7461 736b 0a23 2061 7267 733a 2063 6f6d  task.# args: com
+00000200: 6d6f 6d20 7461 736b 2076 6172 6961 626c  mom task variabl
+00000210: 6573 200a 0a23 2074 6872 6561 645f 6675  es ..# thread_fu
+00000220: 6e63 2045 5841 4d50 4c45 530a 0a23 2049  nc EXAMPLES..# I
+00000230: 4f20 424f 554e 4420 4558 414d 504c 450a  O BOUND EXAMPLE.
+00000240: 2320 6465 6620 7265 6164 5f66 696c 6573  # def read_files
+00000250: 2869 7465 7261 7469 6f6e 2c20 6172 6773  (iteration, args
+00000260: 293a 0a23 2020 2020 2066 696c 6569 6420  ):.#     fileid 
+00000270: 3d20 6974 6572 6174 696f 6e5b 305d 2020  = iteration[0]  
+00000280: 2020 0a23 2020 2020 2066 696c 655f 6c69    .#     file_li
+00000290: 7374 203d 2061 7267 735b 305d 0a23 2020  st = args[0].#  
+000002a0: 2020 2066 7061 7468 203d 2066 696c 655f     fpath = file_
+000002b0: 6c69 7374 5b66 696c 6569 645d 0a23 2020  list[fileid].#  
+000002c0: 2020 2064 6620 3d20 7064 2e72 6561 645f     df = pd.read_
+000002d0: 6373 7628 6670 6174 6829 0a23 2020 2020  csv(fpath).#    
+000002e0: 2072 6574 7572 6e20 5b64 665d 0a0a 2320   return [df]..# 
+000002f0: 4350 5520 424f 554e 4420 4558 414d 504c  CPU BOUND EXAMPL
+00000300: 450a 2320 6465 6620 6461 7973 5f74 7261  E.# def days_tra
+00000310: 6469 6e67 5f66 726f 6d5f 746f 2869 7465  ding_from_to(ite
+00000320: 7261 7469 6f6e 2c20 6172 6773 293a 0a23  ration, args):.#
+00000330: 2020 2020 2063 616c 203d 2069 7465 7261       cal = itera
+00000340: 7469 6f6e 5b30 5d0a 2320 2020 2020 7374  tion[0].#     st
+00000350: 6172 7420 3d20 6974 6572 6174 696f 6e5b  art = iteration[
+00000360: 315d 0a23 2020 2020 2065 6e64 203d 2069  1].#     end = i
+00000370: 7465 7261 7469 6f6e 5b32 5d0a 2320 2020  teration[2].#   
+00000380: 2020 6361 6c65 6e64 6172 7320 3d20 6172    calendars = ar
+00000390: 6773 5b30 5d0a 2320 2020 2020 6964 7820  gs[0].#     idx 
+000003a0: 3d20 2863 616c 656e 6461 7273 5b63 616c  = (calendars[cal
+000003b0: 5d3e 3d73 7461 7274 2920 2620 2828 6361  ]>=start) & ((ca
+000003c0: 6c65 6e64 6172 735b 6361 6c5d 3c3d 656e  lendars[cal]<=en
+000003d0: 6429 290a 2320 2020 2020 7265 7475 726e  d)).#     return
+000003e0: 205b 6e70 2e63 6f75 6e74 5f6e 6f6e 7a65   [np.count_nonze
+000003f0: 726f 2869 6478 295d 0a0a 0a23 206c 6f61  ro(idx)]...# loa
+00000400: 6420 616c 6c20 6669 6c65 7320 696e 2061  d all files in a
+00000410: 2064 6972 6563 746f 7279 2069 6e74 6f20   directory into 
+00000420: 6d65 6d6f 7279 0a64 6566 2069 6f5f 626f  memory.def io_bo
+00000430: 756e 6428 7468 7265 6164 5f66 756e 632c  und(thread_func,
+00000440: 2069 7465 7261 746f 722c 2061 7267 732c   iterator, args,
+00000450: 206d 6178 7072 6f63 3d4e 6f6e 652c 206d   maxproc=None, m
+00000460: 6178 7468 7265 6164 733d 3130 293a 0a20  axthreads=10):. 
+00000470: 2020 2072 6573 756c 7473 203d 205b 5d20     results = [] 
+00000480: 2020 200a 2020 2020 2320 6465 7465 726d     .    # determ
+00000490: 696e 6520 6368 756e 6b73 697a 650a 2020  ine chunksize.  
+000004a0: 2020 6e69 7465 7261 746f 7220 3d20 6c65    niterator = le
+000004b0: 6e28 6974 6572 6174 6f72 290a 2020 2020  n(iterator).    
+000004c0: 6966 206e 6974 6572 6174 6f72 3e30 3a0a  if niterator>0:.
+000004d0: 2020 2020 2020 2020 6e5f 776f 726b 6572          n_worker
+000004e0: 7320 3d20 6d75 6c74 6970 726f 6365 7373  s = multiprocess
+000004f0: 696e 672e 6370 755f 636f 756e 7428 2920  ing.cpu_count() 
+00000500: 2d20 320a 2020 2020 2020 2020 6e5f 776f  - 2.        n_wo
+00000510: 726b 6572 7320 3d20 6d69 6e28 6e5f 776f  rkers = min(n_wo
+00000520: 726b 6572 732c 6e69 7465 7261 746f 7229  rkers,niterator)
+00000530: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00000540: 6d61 7870 726f 6320 6973 204e 6f6e 653a  maxproc is None:
+00000550: 0a20 2020 2020 2020 2020 2020 206e 5f77  .            n_w
+00000560: 6f72 6b65 7273 203d 206d 696e 286e 5f77  orkers = min(n_w
+00000570: 6f72 6b65 7273 2c6d 6178 7072 6f63 290a  orkers,maxproc).
+00000580: 2020 2020 2020 2020 6368 756e 6b73 697a          chunksiz
+00000590: 6520 3d20 726f 756e 6428 6e69 7465 7261  e = round(nitera
+000005a0: 746f 7220 2f20 6e5f 776f 726b 6572 7329  tor / n_workers)
+000005b0: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
+000005c0: 6520 7468 6520 7072 6f63 6573 7320 706f  e the process po
+000005d0: 6f6c 0a20 2020 2020 2020 2077 6974 6820  ol.        with 
+000005e0: 5072 6f63 6573 7350 6f6f 6c45 7865 6375  ProcessPoolExecu
+000005f0: 746f 7228 6e5f 776f 726b 6572 7329 2061  tor(n_workers) a
+00000600: 7320 6578 6563 7574 6f72 3a20 2020 2020  s executor:     
+00000610: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+00000620: 6675 7475 7265 7320 3d20 6c69 7374 2829  futures = list()
+00000630: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00000640: 706c 6974 2074 6865 206c 6f61 6420 6f70  plit the load op
+00000650: 6572 6174 696f 6e73 2069 6e74 6f20 6368  erations into ch
+00000660: 756e 6b73 0a20 2020 2020 2020 2020 2020  unks.           
+00000670: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00000680: 302c 206e 6974 6572 6174 6f72 2c20 6368  0, niterator, ch
+00000690: 756e 6b73 697a 6529 3a0a 2020 2020 2020  unksize):.      
+000006a0: 2020 2020 2020 2020 2020 2320 7365 6c65            # sele
+000006b0: 6374 2061 2063 6875 6e6b 206f 6620 6669  ct a chunk of fi
+000006c0: 6c65 6e61 6d65 730a 2020 2020 2020 2020  lenames.        
+000006d0: 2020 2020 2020 2020 7072 6f63 5f69 7465          proc_ite
+000006e0: 7261 746f 7220 3d20 6974 6572 6174 6f72  rator = iterator
+000006f0: 5b69 3a28 6920 2b20 6368 756e 6b73 697a  [i:(i + chunksiz
+00000700: 6529 5d0a 2020 2020 2020 2020 2020 2020  e)].            
+00000710: 2020 2020 2320 7375 626d 6974 2074 6865      # submit the
+00000720: 2074 6173 6b0a 2020 2020 2020 2020 2020   task.          
+00000730: 2020 2020 2020 6675 7475 7265 203d 2065        future = e
+00000740: 7865 6375 746f 722e 7375 626d 6974 2869  xecutor.submit(i
+00000750: 6f5f 626f 756e 645f 7072 6f63 6573 732c  o_bound_process,
+00000760: 2074 6872 6561 645f 6675 6e63 2c20 7072   thread_func, pr
+00000770: 6f63 5f69 7465 7261 746f 722c 2061 7267  oc_iterator, arg
+00000780: 732c 206d 6178 7468 7265 6164 7329 0a20  s, maxthreads). 
+00000790: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000007a0: 7574 7572 6573 2e61 7070 656e 6428 6675  utures.append(fu
+000007b0: 7475 7265 290a 2020 2020 2020 2020 2020  ture).          
+000007c0: 2020 2320 7072 6f63 6573 7320 616c 6c20    # process all 
+000007d0: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
+000007e0: 2020 2020 666f 7220 6675 7475 7265 2069      for future i
+000007f0: 6e20 6675 7475 7265 733a 0a20 2020 2020  n futures:.     
+00000800: 2020 2020 2020 2020 2020 2023 206f 7065             # ope
+00000810: 6e20 7468 6520 6669 6c65 2061 6e64 206c  n the file and l
+00000820: 6f61 6420 7468 6520 6461 7461 0a20 2020  oad the data.   
+00000830: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00000840: 203d 2066 7574 7572 652e 7265 7375 6c74   = future.result
+00000850: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00000860: 2020 2072 6573 756c 7473 203d 205b 2a72     results = [*r
+00000870: 6573 756c 7473 2c20 2a72 6573 5d20 2020  esults, *res]   
+00000880: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00000890: 2020 7265 7475 726e 2072 6573 756c 7473    return results
+000008a0: 0a0a 2320 7265 7475 726e 2074 6865 2063  ..# return the c
+000008b0: 6f6e 7465 6e74 7320 6f66 206d 616e 7920  ontents of many 
+000008c0: 6669 6c65 730a 6465 6620 696f 5f62 6f75  files.def io_bou
+000008d0: 6e64 5f70 726f 6365 7373 2874 6872 6561  nd_process(threa
+000008e0: 645f 6675 6e63 2c20 7072 6f63 5f69 7465  d_func, proc_ite
+000008f0: 7261 746f 722c 2061 7267 732c 206d 6178  rator, args, max
+00000900: 7468 7265 6164 7329 3a0a 2020 2020 7265  threads):.    re
+00000910: 7375 6c74 7320 3d20 5b5d 0a20 2020 2023  sults = [].    #
+00000920: 2063 7265 6174 6520 6120 7468 7265 6164   create a thread
+00000930: 2070 6f6f 6c0a 2020 2020 6e74 6872 6561   pool.    nthrea
+00000940: 6473 203d 206c 656e 2870 726f 635f 6974  ds = len(proc_it
+00000950: 6572 6174 6f72 290a 2020 2020 6e74 6872  erator).    nthr
+00000960: 6561 6473 203d 206d 696e 286e 7468 7265  eads = min(nthre
+00000970: 6164 732c 6d61 7874 6872 6561 6473 290a  ads,maxthreads).
+00000980: 2020 2020 6966 206e 7468 7265 6164 733e      if nthreads>
+00000990: 303a 0a20 2020 2020 2020 2077 6974 6820  0:.        with 
+000009a0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+000009b0: 6f72 286e 7468 7265 6164 7329 2061 7320  or(nthreads) as 
+000009c0: 6578 653a 0a20 2020 2020 2020 2020 2020  exe:.           
+000009d0: 2023 206c 6f61 6420 6669 6c65 730a 2020   # load files.  
+000009e0: 2020 2020 2020 2020 2020 6675 7475 7265            future
+000009f0: 7320 3d20 5b65 7865 2e73 7562 6d69 7428  s = [exe.submit(
+00000a00: 7468 7265 6164 5f66 756e 632c 2069 7465  thread_func, ite
+00000a10: 7261 7469 6f6e 2c20 6172 6773 2920 666f  ration, args) fo
+00000a20: 7220 6974 6572 6174 696f 6e20 696e 2070  r iteration in p
+00000a30: 726f 635f 6974 6572 6174 6f72 5d0a 2020  roc_iterator].  
+00000a40: 2020 2020 2020 2020 2020 2320 636f 6c6c            # coll
+00000a50: 6563 7420 6461 7461 0a20 2020 2020 2020  ect data.       
+00000a60: 2020 2020 2066 6f72 2066 7574 7572 6520       for future 
+00000a70: 696e 2066 7574 7572 6573 3a0a 2020 2020  in futures:.    
+00000a80: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00000a90: 3d20 6675 7475 7265 2e72 6573 756c 7428  = future.result(
+00000aa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00000ab0: 2020 7265 7375 6c74 7320 3d20 5b2a 7265    results = [*re
+00000ac0: 7375 6c74 732c 202a 7265 735d 0a20 2020  sults, *res].   
+00000ad0: 2020 2020 200a 2020 2020 7265 7475 726e       .    return
+00000ae0: 2072 6573 756c 7473 0a20 0a0a 6465 6620   results. ..def 
+00000af0: 6370 755f 626f 756e 6428 7468 7265 6164  cpu_bound(thread
+00000b00: 5f66 756e 632c 2069 7465 7261 746f 722c  _func, iterator,
+00000b10: 2061 7267 732c 206d 6178 7072 6f63 203d   args, maxproc =
+00000b20: 204e 6f6e 6529 3a0a 2020 2020 7265 7375   None):.    resu
+00000b30: 6c74 7320 3d20 5b5d 2020 2020 0a20 2020  lts = []    .   
+00000b40: 2023 2064 6574 6572 6d69 6e65 2063 6875   # determine chu
+00000b50: 6e6b 7369 7a65 0a20 2020 206e 6974 6572  nksize.    niter
+00000b60: 6174 6f72 203d 206c 656e 2869 7465 7261  ator = len(itera
+00000b70: 746f 7229 0a20 2020 2069 6620 6e69 7465  tor).    if nite
+00000b80: 7261 746f 723e 303a 0a20 2020 2020 2020  rator>0:.       
+00000b90: 206e 5f77 6f72 6b65 7273 203d 206d 756c   n_workers = mul
+00000ba0: 7469 7072 6f63 6573 7369 6e67 2e63 7075  tiprocessing.cpu
+00000bb0: 5f63 6f75 6e74 2829 202d 2032 2020 2020  _count() - 2    
+00000bc0: 0a20 2020 2020 2020 206e 5f77 6f72 6b65  .        n_worke
+00000bd0: 7273 203d 206d 696e 286e 5f77 6f72 6b65  rs = min(n_worke
+00000be0: 7273 2c6e 6974 6572 6174 6f72 290a 2020  rs,niterator).  
+00000bf0: 2020 2020 2020 6966 206e 6f74 206d 6178        if not max
+00000c00: 7072 6f63 2069 7320 4e6f 6e65 3a0a 2020  proc is None:.  
+00000c10: 2020 2020 2020 2020 2020 6e5f 776f 726b            n_work
+00000c20: 6572 7320 3d20 6d69 6e28 6e5f 776f 726b  ers = min(n_work
+00000c30: 6572 732c 6d61 7870 726f 6329 0a20 2020  ers,maxproc).   
+00000c40: 2020 2020 2063 6875 6e6b 7369 7a65 203d       chunksize =
+00000c50: 2072 6f75 6e64 286e 6974 6572 6174 6f72   round(niterator
+00000c60: 202f 206e 5f77 6f72 6b65 7273 290a 2020   / n_workers).  
+00000c70: 2020 2020 2020 2320 6372 6561 7465 2074        # create t
+00000c80: 6865 2070 726f 6365 7373 2070 6f6f 6c0a  he process pool.
+00000c90: 2020 2020 2020 2020 7769 7468 2050 726f          with Pro
+00000ca0: 6365 7373 506f 6f6c 4578 6563 7574 6f72  cessPoolExecutor
+00000cb0: 286e 5f77 6f72 6b65 7273 2920 6173 2065  (n_workers) as e
+00000cc0: 7865 6375 746f 723a 2020 2020 2020 2020  xecutor:        
+00000cd0: 0a20 2020 2020 2020 2020 2020 2066 7574  .            fut
+00000ce0: 7572 6573 203d 206c 6973 7428 290a 2020  ures = list().  
+00000cf0: 2020 2020 2020 2020 2020 2320 7370 6c69            # spli
+00000d00: 7420 7468 6520 6c6f 6164 206f 7065 7261  t the load opera
+00000d10: 7469 6f6e 7320 696e 746f 2063 6875 6e6b  tions into chunk
+00000d20: 730a 2020 2020 2020 2020 2020 2020 666f  s.            fo
+00000d30: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
+00000d40: 6e69 7465 7261 746f 722c 2063 6875 6e6b  niterator, chunk
+00000d50: 7369 7a65 293a 0a20 2020 2020 2020 2020  size):.         
+00000d60: 2020 2020 2020 2023 2073 656c 6563 7420         # select 
+00000d70: 6120 6368 756e 6b20 6f66 2066 696c 656e  a chunk of filen
+00000d80: 616d 6573 0a20 2020 2020 2020 2020 2020  ames.           
+00000d90: 2020 2020 2070 726f 635f 6974 6572 6174       proc_iterat
+00000da0: 6f72 203d 2069 7465 7261 746f 725b 693a  or = iterator[i:
+00000db0: 2869 202b 2063 6875 6e6b 7369 7a65 295d  (i + chunksize)]
+00000dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000dd0: 2023 2073 7562 6d69 7420 7468 6520 7461   # submit the ta
+00000de0: 736b 0a20 2020 2020 2020 2020 2020 2020  sk.             
+00000df0: 2020 2066 7574 7572 6520 3d20 6578 6563     future = exec
+00000e00: 7574 6f72 2e73 7562 6d69 7428 6370 755f  utor.submit(cpu_
+00000e10: 626f 756e 645f 7072 6f63 6573 732c 2074  bound_process, t
+00000e20: 6872 6561 645f 6675 6e63 2c20 7072 6f63  hread_func, proc
+00000e30: 5f69 7465 7261 746f 722c 2061 7267 7329  _iterator, args)
+00000e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e50: 2066 7574 7572 6573 2e61 7070 656e 6428   futures.append(
+00000e60: 6675 7475 7265 2920 2020 2020 2020 2020  future)         
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000e90: 2020 2020 2023 2070 726f 6365 7373 2061       # process a
+00000ea0: 6c6c 2072 6573 756c 7473 0a20 2020 2020  ll results.     
+00000eb0: 2020 2020 2020 2066 6f72 2066 7574 7572         for futur
+00000ec0: 6520 696e 2066 7574 7572 6573 3a0a 2020  e in futures:.  
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00000ee0: 6f70 656e 2074 6865 2066 696c 6520 616e  open the file an
+00000ef0: 6420 6c6f 6164 2074 6865 2064 6174 610a  d load the data.
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 7265 7320 3d20 6675 7475 7265 2e72 6573  res = future.res
+00000f20: 756c 7428 290a 2020 2020 2020 2020 2020  ult().          
+00000f30: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
+00000f40: 5b2a 7265 7375 6c74 732c 202a 7265 735d  [*results, *res]
+00000f50: 2020 2020 0a20 2020 2072 6574 7572 6e20      .    return 
+00000f60: 7265 7375 6c74 730a 0a0a 2320 7265 7475  results...# retu
+00000f70: 726e 2074 6865 2063 6f6e 7465 6e74 7320  rn the contents 
+00000f80: 6f66 206d 616e 7920 6669 6c65 730a 6465  of many files.de
+00000f90: 6620 6370 755f 626f 756e 645f 7072 6f63  f cpu_bound_proc
+00000fa0: 6573 7328 7468 7265 6164 5f66 756e 632c  ess(thread_func,
+00000fb0: 2070 726f 635f 6974 6572 6174 6f72 2c20   proc_iterator, 
+00000fc0: 6172 6773 293a 0a20 2020 2072 6573 756c  args):.    resul
+00000fd0: 7473 203d 205b 5d0a 2020 2020 666f 7220  ts = [].    for 
+00000fe0: 6974 6572 6174 696f 6e20 696e 2070 726f  iteration in pro
+00000ff0: 635f 6974 6572 6174 6f72 3a0a 2020 2020  c_iterator:.    
+00001000: 2020 2020 7265 7320 3d20 7468 7265 6164      res = thread
+00001010: 5f66 756e 6328 6974 6572 6174 696f 6e2c  _func(iteration,
+00001020: 2061 7267 7329 0a20 2020 2020 2020 2072   args).        r
+00001030: 6573 756c 7473 203d 205b 2a72 6573 756c  esults = [*resul
+00001040: 7473 2c20 2a72 6573 5d20 2020 2020 2020  ts, *res]       
+00001050: 2020 2020 2020 200a 2020 2020 7265 7475         .    retu
+00001060: 726e 2072 6573 756c 7473 0a0a 6465 6620  rn results..def 
+00001070: 7072 6f67 7265 7373 6261 725f 7468 7265  progressbar_thre
+00001080: 6164 2870 726f 6772 6573 732c 6e69 7465  ad(progress,nite
+00001090: 7261 7469 6f6e 7329 3a0a 2020 2020 7062  rations):.    pb
+000010a0: 6172 203d 2074 7164 6d28 746f 7461 6c3d  ar = tqdm(total=
+000010b0: 6e69 7465 7261 7469 6f6e 732c 6465 7363  niterations,desc
+000010c0: 3d27 5275 6e6e 696e 6720 6d75 6c74 6920  ='Running multi 
+000010d0: 7072 6f63 2e2e 2e27 290a 2020 2020 7768  proc...').    wh
+000010e0: 696c 6520 5472 7565 3a20 2020 2020 2020  ile True:       
+000010f0: 200a 2020 2020 2020 2020 7062 6172 2e75   .        pbar.u
+00001100: 7064 6174 6528 7072 6f67 7265 7373 202d  pdate(progress -
+00001110: 2070 6261 722e 6e29 0a20 2020 2020 2020   pbar.n).       
+00001120: 2069 6620 7072 6f67 7265 7373 203e 3d20   if progress >= 
+00001130: 6e69 7465 7261 7469 6f6e 733a 0a20 2020  niterations:.   
+00001140: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00001150: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00001160: 7028 302e 3229 0a20 2020 2020 2020 200a  p(0.2).        .
+00001170: 2020 2020 2020 2020
```

### Comparing `shareddata-2.0.9/src/SharedData/SeriesLib.py` & `shareddata-2.1.0/src/SharedData/SeriesLib.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import pandas as pd
-import numpy as np
-from numba import njit, prange
-
-
-def unstack_series(values,symbols):
-    tmp = pd.DataFrame(values.unstack())
-    tmp['symbol']=symbols.unstack()    
-    tmp = tmp.reset_index()
-    tmp.columns=['serie','date','value','symbol']
-    tmp = tmp.pivot_table(values='value',index='date',columns='symbol')
-    return tmp
-
-
-@njit(parallel=True)
-def ffill_sequence(dt_ini_row,dt_end_row, mktdata_cols, sequence_chg, values):
-    nsymbols = values.shape[1]
-    for dt in range(dt_ini_row,dt_end_row+1):
-        for s in prange(nsymbols):        
-            mktdata_s = mktdata_cols[s]
-            if (~np.isnan(sequence_chg[dt,mktdata_s])):
-                last_s = int(s-sequence_chg[dt,s])
-                last_dt = int(dt-1)
-                if (np.isnan(values[dt,s])):
-                    values[dt,s] = values[last_dt,last_s]
-
-
-@njit(parallel=True)
-def shift_sequence(dt_ini_row,dt_end_row, mktdata_cols, sequence_chg, values):
-    nsymbols = values.shape[1]
-    for dt in range(dt_ini_row,dt_end_row+1):
-        for s in prange(nsymbols):        
-            mktdata_s = mktdata_cols[s]
-            if (~np.isnan(sequence_chg[dt,mktdata_s])):
-                last_s = int(s-sequence_chg[dt,mktdata_s])
-                last_dt = int(dt-1)
-                values[dt,s] = values[last_dt,last_s]
-
-
-@njit(parallel=True)
-def diff_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_diff):
-    nsymbols = values_diff.shape[1]
-    for dt in range(dt_ini_row,dt_end_row+1):        
-        for s in prange(nsymbols):        
-            mktdata_s = int(mktdata_cols[s])
-            if (~np.isnan(sequence_chg[dt,mktdata_s])):
-                last_s = int(s-sequence_chg[dt,mktdata_s])
-                last_dt = int(dt-1)
-                if (~np.isnan(values[dt,s])) & (~np.isnan(values[last_dt,last_s])):
-                    values_diff[dt,s] = values[dt,s] - values[last_dt,last_s]
-            else:
-                values_diff[dt,s] = values[dt,s]
-
-
-@njit(parallel=True)
-def mean_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_mean, alpha=0.06):
-    nsymbols = values_mean.shape[1]
-    for dt in range(dt_ini_row,dt_end_row+1):        
-        for s in prange(nsymbols):        
-            mktdata_s = int(mktdata_cols[s])
-            if (~np.isnan(sequence_chg[dt,mktdata_s])):
-                last_s = int(s-sequence_chg[dt,mktdata_s])
-                last_dt = int(dt-1)
-                if (~np.isnan(values[dt,s])):
-
-                    if (~np.isnan(values_mean[last_dt,last_s])):
-                        values_mean[dt,s] = values[dt,s]*alpha \
-                            + values_mean[last_dt,last_s]*(1-alpha)
-                    else:
-                        values_mean[dt,s] = values[dt,s]
-
-                elif (~np.isnan(values_mean[last_dt,s])):
-                    # forward fill mean sequence
-                    values_mean[dt,s] = values_mean[last_dt,last_s]
-            else:
-                # first value of sequence
-                values_mean[dt,s] = values[dt,s]
-
-@njit(parallel=True)
-def rollmax_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_rollmax):
-    nsymbols = values_rollmax.shape[1]
-    for dt in range(dt_ini_row,dt_end_row+1):
-        for s in prange(nsymbols):        
-            mktdata_s = int(mktdata_cols[s])
-            if (~np.isnan(sequence_chg[dt,mktdata_s])):                
-                last_s = int(s-sequence_chg[dt,mktdata_s])
-                last_dt = int(dt-1)
-                if (~np.isnan(values[dt,s])):
-
-                    if (~np.isnan(values_rollmax[last_dt,last_s])):
-                        values_rollmax[dt,s] = max(values_rollmax[last_dt,last_s],values[dt,s])
-                    else:
-                        values_rollmax[dt,s] = values[dt,s]
-
-                elif (~np.isnan(values_rollmax[last_dt,last_s])):
-                    values_rollmax[dt,s] = values_rollmax[last_dt,last_s]
-
-            elif (~np.isnan(values[dt,s])):
-                values_rollmax[dt,s] = values[dt,s]
-
-
-@njit(parallel=True)
-def rollmin_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_rollmin):
-    nsymbols = values_rollmin.shape[1]
-    for dt in range(dt_ini_row,dt_end_row+1):
-        for s in prange(nsymbols):        
-            mktdata_s = int(mktdata_cols[s])
-            if (~np.isnan(sequence_chg[dt,mktdata_s])):                
-                last_s = int(s-sequence_chg[dt,mktdata_s])
-                last_dt = int(dt-1)
-                if (~np.isnan(values[dt,s])):
-
-                    if (~np.isnan(values_rollmin[last_dt,last_s])):
-                        values_rollmin[dt,s] = min(values_rollmin[last_dt,last_s],values[dt,s])
-                    else:
-                        values_rollmin[dt,s] = values[dt,s]
-
-                elif (~np.isnan(values_rollmin[last_dt,last_s])):
-                    values_rollmin[dt,s] = values_rollmin[last_dt,last_s]
-
-            elif (~np.isnan(values[dt,s])):
+import pandas as pd
+import numpy as np
+from numba import njit, prange
+
+
+def unstack_series(values,symbols):
+    tmp = pd.DataFrame(values.unstack())
+    tmp['symbol']=symbols.unstack()    
+    tmp = tmp.reset_index()
+    tmp.columns=['serie','date','value','symbol']
+    tmp = tmp.pivot_table(values='value',index='date',columns='symbol')
+    return tmp
+
+
+@njit(parallel=True)
+def ffill_sequence(dt_ini_row,dt_end_row, mktdata_cols, sequence_chg, values):
+    nsymbols = values.shape[1]
+    for dt in range(dt_ini_row,dt_end_row+1):
+        for s in prange(nsymbols):        
+            mktdata_s = mktdata_cols[s]
+            if (~np.isnan(sequence_chg[dt,mktdata_s])):
+                last_s = int(s-sequence_chg[dt,s])
+                last_dt = int(dt-1)
+                if (np.isnan(values[dt,s])):
+                    values[dt,s] = values[last_dt,last_s]
+
+
+@njit(parallel=True)
+def shift_sequence(dt_ini_row,dt_end_row, mktdata_cols, sequence_chg, values):
+    nsymbols = values.shape[1]
+    for dt in range(dt_ini_row,dt_end_row+1):
+        for s in prange(nsymbols):        
+            mktdata_s = mktdata_cols[s]
+            if (~np.isnan(sequence_chg[dt,mktdata_s])):
+                last_s = int(s-sequence_chg[dt,mktdata_s])
+                last_dt = int(dt-1)
+                values[dt,s] = values[last_dt,last_s]
+
+
+@njit(parallel=True)
+def diff_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_diff):
+    nsymbols = values_diff.shape[1]
+    for dt in range(dt_ini_row,dt_end_row+1):        
+        for s in prange(nsymbols):        
+            mktdata_s = int(mktdata_cols[s])
+            if (~np.isnan(sequence_chg[dt,mktdata_s])):
+                last_s = int(s-sequence_chg[dt,mktdata_s])
+                last_dt = int(dt-1)
+                if (~np.isnan(values[dt,s])) & (~np.isnan(values[last_dt,last_s])):
+                    values_diff[dt,s] = values[dt,s] - values[last_dt,last_s]
+            else:
+                values_diff[dt,s] = values[dt,s]
+
+
+@njit(parallel=True)
+def mean_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_mean, alpha=0.06):
+    nsymbols = values_mean.shape[1]
+    for dt in range(dt_ini_row,dt_end_row+1):        
+        for s in prange(nsymbols):        
+            mktdata_s = int(mktdata_cols[s])
+            if (~np.isnan(sequence_chg[dt,mktdata_s])):
+                last_s = int(s-sequence_chg[dt,mktdata_s])
+                last_dt = int(dt-1)
+                if (~np.isnan(values[dt,s])):
+
+                    if (~np.isnan(values_mean[last_dt,last_s])):
+                        values_mean[dt,s] = values[dt,s]*alpha \
+                            + values_mean[last_dt,last_s]*(1-alpha)
+                    else:
+                        values_mean[dt,s] = values[dt,s]
+
+                elif (~np.isnan(values_mean[last_dt,s])):
+                    # forward fill mean sequence
+                    values_mean[dt,s] = values_mean[last_dt,last_s]
+            else:
+                # first value of sequence
+                values_mean[dt,s] = values[dt,s]
+
+@njit(parallel=True)
+def rollmax_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_rollmax):
+    nsymbols = values_rollmax.shape[1]
+    for dt in range(dt_ini_row,dt_end_row+1):
+        for s in prange(nsymbols):        
+            mktdata_s = int(mktdata_cols[s])
+            if (~np.isnan(sequence_chg[dt,mktdata_s])):                
+                last_s = int(s-sequence_chg[dt,mktdata_s])
+                last_dt = int(dt-1)
+                if (~np.isnan(values[dt,s])):
+
+                    if (~np.isnan(values_rollmax[last_dt,last_s])):
+                        values_rollmax[dt,s] = max(values_rollmax[last_dt,last_s],values[dt,s])
+                    else:
+                        values_rollmax[dt,s] = values[dt,s]
+
+                elif (~np.isnan(values_rollmax[last_dt,last_s])):
+                    values_rollmax[dt,s] = values_rollmax[last_dt,last_s]
+
+            elif (~np.isnan(values[dt,s])):
+                values_rollmax[dt,s] = values[dt,s]
+
+
+@njit(parallel=True)
+def rollmin_sequence(dt_ini_row, dt_end_row, mktdata_cols, sequence_chg, values, values_rollmin):
+    nsymbols = values_rollmin.shape[1]
+    for dt in range(dt_ini_row,dt_end_row+1):
+        for s in prange(nsymbols):        
+            mktdata_s = int(mktdata_cols[s])
+            if (~np.isnan(sequence_chg[dt,mktdata_s])):                
+                last_s = int(s-sequence_chg[dt,mktdata_s])
+                last_dt = int(dt-1)
+                if (~np.isnan(values[dt,s])):
+
+                    if (~np.isnan(values_rollmin[last_dt,last_s])):
+                        values_rollmin[dt,s] = min(values_rollmin[last_dt,last_s],values[dt,s])
+                    else:
+                        values_rollmin[dt,s] = values[dt,s]
+
+                elif (~np.isnan(values_rollmin[last_dt,last_s])):
+                    values_rollmin[dt,s] = values_rollmin[last_dt,last_s]
+
+            elif (~np.isnan(values[dt,s])):
                 values_rollmin[dt,s] = values[dt,s]
```

### Comparing `shareddata-2.0.9/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.1.0/src/SharedData/SharedDataAWSKinesis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,349 +1,350 @@
-import os
-import logging
-import subprocess
-import boto3
-from pathlib import Path
-import pandas as pd
-from datetime import datetime,timedelta
-import time
-import pytz
-import json
-
-from botocore.exceptions import ClientError
-
-# LOGS
-class KinesisLogStreamHandler(logging.StreamHandler):
-    #reference: https://docs.python.org/3/library/logging.html#logging.LogRecord
-    def __init__(self,user='guest'):
-        # By default, logging.StreamHandler uses sys.stderr if stream parameter is not specified
-        logging.StreamHandler.__init__(self)
-        
-        self.user = user
-        self.datastream = None
-        self.stream_buffer = []
-
-        try:
-            session = boto3.Session(profile_name=os.environ['LOG_AWS_PROFILE'])
-            if 'KINESIS_ENDPOINT_URL' in os.environ:
-                self.datastream = session.client('kinesis',\
-                    endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
-            else:
-                self.datastream = session.client('kinesis')
-        except Exception:
-            print('Kinesis client initialization failed.')
-
-        self.stream_name = os.environ['LOG_STREAMNAME']
-        try:
-            self.datastream.create_stream(
-                StreamName=self.stream_name,
-                ShardCount=1,
-                StreamModeDetails={
-                    'StreamMode': 'PROVISIONED'
-                }
-                )
-            time.sleep(10)
-        except Exception as e:
-            pass        
-        
-    def emit(self, record):
-        try:
-            #msg = self.format(record)
-            user = os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME']
-            timezone = pytz.timezone("UTC")
-            dt = datetime.utcfromtimestamp(record.created)
-            dt= timezone.localize(dt)
-            asctime = dt.strftime('%Y-%m-%dT%H:%M:%S%z')
-            msg = {
-                    'user_name': user,
-                    'asctime': asctime,
-                    'logger_name': record.name,
-                    'level': record.levelname,
-                    'message': str(record.msg).replace('\'','\"'),
-                    #'function_name': record.funcName,
-                    #'file_name': record.filename,                
-                }   
-            msg = json.dumps(msg)
-            if self.datastream:
-                self.stream_buffer.append({
-                    'Data': str(msg).encode(encoding="UTF-8", errors="strict"),
-                    'PartitionKey' : user,
-                })
-            else:
-                stream = self.stream
-                stream.write(msg)
-                stream.write(self.terminator)
-
-            self.flush()
-        except Exception:
-            self.handleError(record)
-
-    def flush(self):
-        self.acquire()
-        try:
-            if self.datastream and self.stream_buffer:
-                self.datastream.put_records(
-                    StreamName=self.stream_name,
-                    Records=self.stream_buffer                   
-                )
-
-                self.stream_buffer.clear()
-        except Exception as e:
-            print("An error occurred during flush operation.")
-            print(f"Exception: {e}")
-            print(f"Stream buffer: {self.stream_buffer}")
-        finally:
-            if self.stream and hasattr(self.stream, "flush"):
-                self.stream.flush()
-            self.release()
-
-class KinesisLogStreamConsumer():
-    def __init__(self,user='guest'):
-        self.user = user
-
-    def readLogs(self):
-        self.logfilepath = Path(os.environ['DATABASE_FOLDER']) / 'Logs'
-        self.logfilepath = self.logfilepath / (datetime.utcnow().strftime('%Y%m%d')+'.log')
-
-        self.lastlogfilepath = Path(os.environ['DATABASE_FOLDER']) / 'Logs'
-        self.lastlogfilepath = self.lastlogfilepath / ((datetime.utcnow() + timedelta(days=-1)).strftime('%Y%m%d')+'.log')
-
-        self.dflogs = pd.DataFrame([])
-        if self.logfilepath.is_file():
-            try:
-                self.dflogs = pd.read_csv(self.logfilepath,header=None,sep=';',\
-                    engine='python',on_bad_lines='skip')
-                self.dflogs.columns = ['shardid','sequence_number','user_name','asctime','logger_name','level','message']
-            except:
-                pass
-        
-        if self.lastlogfilepath.is_file():
-            try:
-                _dflogs = pd.read_csv(self.lastlogfilepath,header=None,sep=';',\
-                    engine='python',on_bad_lines='skip')
-                _dflogs.columns = ['shardid','sequence_number','user_name','asctime','logger_name','level','message']
-                self.dflogs = pd.concat([_dflogs,self.dflogs],axis=0)
-            except:
-                pass
-
-        return self.dflogs
-    
-    def connect(self):
-        try:
-            session = boto3.Session(profile_name=os.environ['LOG_AWS_PROFILE'])        
-            if 'KINESIS_ENDPOINT_URL' in os.environ:
-                self.client = session.client('kinesis',\
-                    endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
-            else:
-                self.client = session.client('kinesis')
-        except:
-            print('Could not connect to AWS!')
-            return False
-
-        try:
-            print("Trying to create stream %s..." % (os.environ['LOG_STREAMNAME']))
-            self.client.create_stream(
-                StreamName=os.environ['LOG_STREAMNAME'],
-                ShardCount=1,
-                StreamModeDetails={
-                    'StreamMode': 'PROVISIONED'
-                    }
-                )
-            time.sleep(10)
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'ResourceInUseException':                                
-                print("Stream already exists")                
-            else:
-                print("Trying to create stream unexpected error: %s" % e)
-                pass        
-
-        try:            
-            self.stream = self.client.describe_stream(StreamName=os.environ['LOG_STREAMNAME'])            
-        except:
-            print('Could not describe stream!')
-            return False
-        
-        if self.stream and 'StreamDescription' in self.stream:
-            self.stream = self.stream['StreamDescription']
-            for i in range(len(self.stream['Shards'])):
-                readfromstart = True
-                shardid = self.stream['Shards'][i]['ShardId']
-                if not self.dflogs.empty and (shardid in self.dflogs['shardid'].values):
-                    readfromstart = False
-                    seqnum = self.dflogs[self.dflogs['shardid']==shardid].iloc[-1]['sequence_number']
-                    try:
-                        shard_iterator = self.client.get_shard_iterator(
-                            StreamName=self.stream['StreamName'],
-                            ShardId=self.stream['Shards'][i]['ShardId'],
-                            ShardIteratorType='AFTER_SEQUENCE_NUMBER',
-                            StartingSequenceNumber=seqnum
-                            )
-                    except:
-                        print('Failed retrieving shard iterator, reading from start...')
-                        readfromstart=True
-                
-                if readfromstart:
-                    shard_iterator = self.client.get_shard_iterator(
-                        StreamName=self.stream['StreamName'],
-                        ShardId=self.stream['Shards'][i]['ShardId'],
-                        ShardIteratorType='TRIM_HORIZON'
-                        )
-
-                self.stream['Shards'][i]['ShardIterator'] = shard_iterator['ShardIterator']
-        else:
-            print('Failed connecting StreamDescriptor not found!')
-            return False
-        
-        
-        return True
-
-    def consume(self):        
-        try:
-            for i in range(len(self.stream['Shards'])):                
-                response = self.client.get_records(\
-                    ShardIterator = self.stream['Shards'][i]['ShardIterator'],\
-                    Limit = 100)
-                self.stream['Shards'][i]['ShardIterator'] = response['NextShardIterator']
-                if len(response['Records'])> 0:
-                    for r in response['Records']:
-                        try:
-                            rec = r['Data'].decode(encoding="UTF-8", errors="strict")
-                            rec = json.loads(rec.replace("\'", "\"").replace(';',','))
-
-                            line = '%s;%s;%s;%s;%s;%s;%s' % (self.stream['Shards'][i]['ShardId'],\
-                                r['SequenceNumber'],rec['user_name'],rec['asctime'],\
-                                rec['logger_name'],rec['level'],rec['message'])
-
-                            dt = datetime.strptime(rec['asctime'][:-5], '%Y-%m-%dT%H:%M:%S')
-
-                            logfilepath = Path(os.environ['DATABASE_FOLDER']) / 'Logs'
-                            logfilepath = logfilepath / (dt.strftime('%Y%m%d')+'.log')
-                            if not logfilepath.parents[0].is_dir():
-                                os.makedirs(logfilepath.parents[0])
-
-                            with open(logfilepath,'a+',encoding = 'utf-8') as f:
-                                f.write(line.replace('\n',' ').replace('\r',' ')+'\n')
-                                f.flush()
-
-                        except Exception as e:
-                            print('Invalid record:%s\nerror:%s' % (str(rec),str(e)) )
-            return True
-        except:            
-            return False        
-        
-# REAL TIME
-class KinesisStreamProducer():
-    def __init__(self,stream_name):
-        self.stream_name = stream_name        
-        self.datastream = None
-        self.stream_buffer = []
-        try:
-            session = boto3.Session(profile_name=os.environ['STREAM_AWS_PROFILE'])
-            if 'KINESIS_ENDPOINT_URL' in os.environ:
-                self.datastream = session.client('kinesis',\
-                    endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
-            else:
-                self.datastream = session.client('kinesis')
-        except Exception:
-            print('Kinesis client initialization failed.')
-        
-        try:
-            self.datastream.create_stream(
-                StreamName=stream_name,
-                ShardCount=1,
-                StreamModeDetails={
-                    'StreamMode': 'PROVISIONED'
-                }
-                )
-            time.sleep(10)
-        except Exception as e:
-            pass        
-
-    def produce(self, record, partitionkey):    
-        _rec = json.dumps(record)            
-        self.stream_buffer.append({
-            'Data': str(_rec).encode(encoding="UTF-8", errors="strict"),
-            'PartitionKey' : partitionkey,
-        })
-        self.datastream.put_records(
-                    StreamName=self.stream_name,
-                    Records=self.stream_buffer                   
-                )
-        self.stream_buffer = []
-
-class KinesisStreamConsumer():
-    def __init__(self,stream_name):
-        self.stream_name = stream_name
-        self.stream_buffer = []
-        self.last_sequence_number = None
-        self.get_stream()
-
-    def get_stream(self):
-        print('Initializing stream...')
-        session = boto3.Session()
-        if 'KINESIS_ENDPOINT_URL' in os.environ:
-            self.client = session.client('kinesis',endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
-        else:
-            self.client = session.client('kinesis')
-        
-        try:
-            self.client.create_stream(
-                StreamName=self.stream_name,
-                ShardCount=1,
-                StreamModeDetails={
-                    'StreamMode': 'PROVISIONED'
-                }
-                )
-            time.sleep(10)
-        except Exception as e:
-            pass        
-
-        self.stream = self.client.describe_stream(StreamName=self.stream_name)
-        if self.stream and 'StreamDescription' in self.stream:
-            self.stream = self.stream['StreamDescription']
-            i=0    
-            for i in range(len(self.stream['Shards'])):        
-                shardid = self.stream['Shards'][i]['ShardId']
-                if self.last_sequence_number is None:
-                    shard_iterator = self.client.get_shard_iterator(
-                        StreamName=self.stream['StreamName'],
-                        ShardId=shardid,                
-                        ShardIteratorType='LATEST'
-                        )
-                else:
-                    shard_iterator = self.client.get_shard_iterator(
-                        StreamName=self.stream['StreamName'],
-                        ShardId=shardid,
-                        ShardIteratorType='AFTER_SEQUENCE_NUMBER',
-                        StartingSequenceNumber=self.last_sequence_number
-                        )
-                self.stream['Shards'][i]['ShardIterator'] = shard_iterator['ShardIterator']
-                
-        if self.stream['StreamStatus'] != 'ACTIVE':
-            raise Exception('Stream status %s' % (self.stream['StreamStatus']))
-        print('Initializing stream DONE!')
-                
-    def consume(self):
-        success=False
-
-        for i in range(len(self.stream['Shards'])):
-            try:
-                response = self.client.get_records(\
-                    ShardIterator = self.stream['Shards'][i]['ShardIterator'],\
-                    Limit = 100)
-                success = True
-                self.stream['Shards'][i]['ShardIterator'] = response['NextShardIterator']
-                if len(response['Records'])> 0:
-                    for r in response['Records']:
-                        try:
-                            rec = json.loads(r['Data'])
-                            self.last_sequence_number = r['SequenceNumber']
-                            self.stream_buffer.append(rec)
-                        except Exception as e:
-                            print('Invalid record:'+str(r['Data']))
-                            print('Invalid record:'+str(e))
-                
-            except Exception as e:
-                print('Kinesis consume exception:%s' % (e))
-                break
-
+import os
+import logging
+import subprocess
+import boto3
+from pathlib import Path
+import pandas as pd
+from datetime import datetime,timedelta
+import time
+import pytz
+import json
+
+from botocore.exceptions import ClientError
+
+# LOGS
+class KinesisLogStreamHandler(logging.StreamHandler):
+    #reference: https://docs.python.org/3/library/logging.html#logging.LogRecord
+    def __init__(self,user='guest'):
+        # By default, logging.StreamHandler uses sys.stderr if stream parameter is not specified
+        logging.StreamHandler.__init__(self)
+        
+        self.user = user
+        self.datastream = None
+        self.stream_buffer = []
+
+        try:
+            session = boto3.Session(profile_name=os.environ['LOG_AWS_PROFILE'])
+            if 'KINESIS_ENDPOINT_URL' in os.environ:
+                self.datastream = session.client('kinesis',\
+                    endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
+            else:
+                self.datastream = session.client('kinesis')
+        except Exception:
+            print('Kinesis client initialization failed.')
+
+        self.stream_name = os.environ['LOG_STREAMNAME']
+        try:
+            self.datastream.create_stream(
+                StreamName=self.stream_name,
+                ShardCount=1,
+                StreamModeDetails={
+                    'StreamMode': 'PROVISIONED'
+                }
+                )
+            time.sleep(10)
+        except Exception as e:
+            pass        
+        
+    def emit(self, record):
+        try:
+            #msg = self.format(record)
+            user = os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME']
+            timezone = pytz.timezone("UTC")
+            dt = datetime.utcfromtimestamp(record.created)
+            dt= timezone.localize(dt)
+            asctime = dt.strftime('%Y-%m-%dT%H:%M:%S%z')
+            msg = {
+                    'user_name': user,
+                    'asctime': asctime,
+                    'logger_name': record.name,
+                    'level': record.levelname,
+                    'message': str(record.msg).replace('\'','\"'),
+                    #'function_name': record.funcName,
+                    #'file_name': record.filename,                
+                }   
+            msg = json.dumps(msg)
+            if self.datastream:
+                self.stream_buffer.append({
+                    'Data': str(msg).encode(encoding="UTF-8", errors="strict"),
+                    'PartitionKey' : user,
+                })
+            else:
+                stream = self.stream
+                stream.write(msg)
+                stream.write(self.terminator)
+
+            self.flush()
+        except Exception:
+            self.handleError(record)
+
+    def flush(self):
+        self.acquire()
+        try:
+            if self.datastream and self.stream_buffer:
+                self.datastream.put_records(
+                    StreamName=self.stream_name,
+                    Records=self.stream_buffer                   
+                )
+
+                self.stream_buffer.clear()
+        except Exception as e:
+            print("An error occurred during flush operation.")
+            print(f"Exception: {e}")
+            print(f"Stream buffer: {self.stream_buffer}")
+            raise Exception('Logging failed check aws credentials!')
+        finally:
+            if self.stream and hasattr(self.stream, "flush"):
+                self.stream.flush()
+            self.release()
+
+class KinesisLogStreamConsumer():
+    def __init__(self,user='guest'):
+        self.user = user
+
+    def readLogs(self):
+        self.logfilepath = Path(os.environ['DATABASE_FOLDER']) / 'Logs'
+        self.logfilepath = self.logfilepath / (datetime.utcnow().strftime('%Y%m%d')+'.log')
+
+        self.lastlogfilepath = Path(os.environ['DATABASE_FOLDER']) / 'Logs'
+        self.lastlogfilepath = self.lastlogfilepath / ((datetime.utcnow() + timedelta(days=-1)).strftime('%Y%m%d')+'.log')
+
+        self.dflogs = pd.DataFrame([])
+        if self.logfilepath.is_file():
+            try:
+                self.dflogs = pd.read_csv(self.logfilepath,header=None,sep=';',\
+                    engine='python',on_bad_lines='skip')
+                self.dflogs.columns = ['shardid','sequence_number','user_name','asctime','logger_name','level','message']
+            except:
+                pass
+        
+        if self.lastlogfilepath.is_file():
+            try:
+                _dflogs = pd.read_csv(self.lastlogfilepath,header=None,sep=';',\
+                    engine='python',on_bad_lines='skip')
+                _dflogs.columns = ['shardid','sequence_number','user_name','asctime','logger_name','level','message']
+                self.dflogs = pd.concat([_dflogs,self.dflogs],axis=0)
+            except:
+                pass
+
+        return self.dflogs
+    
+    def connect(self):
+        try:
+            session = boto3.Session(profile_name=os.environ['LOG_AWS_PROFILE'])        
+            if 'KINESIS_ENDPOINT_URL' in os.environ:
+                self.client = session.client('kinesis',\
+                    endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
+            else:
+                self.client = session.client('kinesis')
+        except:
+            print('Could not connect to AWS!')
+            return False
+
+        try:
+            print("Trying to create stream %s..." % (os.environ['LOG_STREAMNAME']))
+            self.client.create_stream(
+                StreamName=os.environ['LOG_STREAMNAME'],
+                ShardCount=1,
+                StreamModeDetails={
+                    'StreamMode': 'PROVISIONED'
+                    }
+                )
+            time.sleep(10)
+        except ClientError as e:
+            if e.response['Error']['Code'] == 'ResourceInUseException':                                
+                print("Stream already exists")                
+            else:
+                print("Trying to create stream unexpected error: %s" % e)
+                pass        
+
+        try:            
+            self.stream = self.client.describe_stream(StreamName=os.environ['LOG_STREAMNAME'])            
+        except:
+            print('Could not describe stream!')
+            return False
+        
+        if self.stream and 'StreamDescription' in self.stream:
+            self.stream = self.stream['StreamDescription']
+            for i in range(len(self.stream['Shards'])):
+                readfromstart = True
+                shardid = self.stream['Shards'][i]['ShardId']
+                if not self.dflogs.empty and (shardid in self.dflogs['shardid'].values):
+                    readfromstart = False
+                    seqnum = self.dflogs[self.dflogs['shardid']==shardid].iloc[-1]['sequence_number']
+                    try:
+                        shard_iterator = self.client.get_shard_iterator(
+                            StreamName=self.stream['StreamName'],
+                            ShardId=self.stream['Shards'][i]['ShardId'],
+                            ShardIteratorType='AFTER_SEQUENCE_NUMBER',
+                            StartingSequenceNumber=seqnum
+                            )
+                    except:
+                        print('Failed retrieving shard iterator, reading from start...')
+                        readfromstart=True
+                
+                if readfromstart:
+                    shard_iterator = self.client.get_shard_iterator(
+                        StreamName=self.stream['StreamName'],
+                        ShardId=self.stream['Shards'][i]['ShardId'],
+                        ShardIteratorType='TRIM_HORIZON'
+                        )
+
+                self.stream['Shards'][i]['ShardIterator'] = shard_iterator['ShardIterator']
+        else:
+            print('Failed connecting StreamDescriptor not found!')
+            return False
+        
+        
+        return True
+
+    def consume(self):        
+        try:
+            for i in range(len(self.stream['Shards'])):                
+                response = self.client.get_records(\
+                    ShardIterator = self.stream['Shards'][i]['ShardIterator'],\
+                    Limit = 100)
+                self.stream['Shards'][i]['ShardIterator'] = response['NextShardIterator']
+                if len(response['Records'])> 0:
+                    for r in response['Records']:
+                        try:
+                            rec = r['Data'].decode(encoding="UTF-8", errors="strict")
+                            rec = json.loads(rec.replace("\'", "\"").replace(';',','))
+
+                            line = '%s;%s;%s;%s;%s;%s;%s' % (self.stream['Shards'][i]['ShardId'],\
+                                r['SequenceNumber'],rec['user_name'],rec['asctime'],\
+                                rec['logger_name'],rec['level'],rec['message'])
+
+                            dt = datetime.strptime(rec['asctime'][:-5], '%Y-%m-%dT%H:%M:%S')
+
+                            logfilepath = Path(os.environ['DATABASE_FOLDER']) / 'Logs'
+                            logfilepath = logfilepath / (dt.strftime('%Y%m%d')+'.log')
+                            if not logfilepath.parents[0].is_dir():
+                                os.makedirs(logfilepath.parents[0])
+
+                            with open(logfilepath,'a+',encoding = 'utf-8') as f:
+                                f.write(line.replace('\n',' ').replace('\r',' ')+'\n')
+                                f.flush()
+
+                        except Exception as e:
+                            print('Invalid record:%s\nerror:%s' % (str(rec),str(e)) )
+            return True
+        except:            
+            return False        
+        
+# REAL TIME
+class KinesisStreamProducer():
+    def __init__(self,stream_name):
+        self.stream_name = stream_name        
+        self.datastream = None
+        self.stream_buffer = []
+        try:
+            session = boto3.Session(profile_name=os.environ['STREAM_AWS_PROFILE'])
+            if 'KINESIS_ENDPOINT_URL' in os.environ:
+                self.datastream = session.client('kinesis',\
+                    endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
+            else:
+                self.datastream = session.client('kinesis')
+        except Exception:
+            print('Kinesis client initialization failed.')
+        
+        try:
+            self.datastream.create_stream(
+                StreamName=stream_name,
+                ShardCount=1,
+                StreamModeDetails={
+                    'StreamMode': 'PROVISIONED'
+                }
+                )
+            time.sleep(10)
+        except Exception as e:
+            pass        
+
+    def produce(self, record, partitionkey):    
+        _rec = json.dumps(record)            
+        self.stream_buffer.append({
+            'Data': str(_rec).encode(encoding="UTF-8", errors="strict"),
+            'PartitionKey' : partitionkey,
+        })
+        self.datastream.put_records(
+                    StreamName=self.stream_name,
+                    Records=self.stream_buffer                   
+                )
+        self.stream_buffer = []
+
+class KinesisStreamConsumer():
+    def __init__(self,stream_name):
+        self.stream_name = stream_name
+        self.stream_buffer = []
+        self.last_sequence_number = None
+        self.get_stream()
+
+    def get_stream(self):
+        print('Initializing stream...')
+        session = boto3.Session()
+        if 'KINESIS_ENDPOINT_URL' in os.environ:
+            self.client = session.client('kinesis',endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
+        else:
+            self.client = session.client('kinesis')
+        
+        try:
+            self.client.create_stream(
+                StreamName=self.stream_name,
+                ShardCount=1,
+                StreamModeDetails={
+                    'StreamMode': 'PROVISIONED'
+                }
+                )
+            time.sleep(10)
+        except Exception as e:
+            pass        
+
+        self.stream = self.client.describe_stream(StreamName=self.stream_name)
+        if self.stream and 'StreamDescription' in self.stream:
+            self.stream = self.stream['StreamDescription']
+            i=0    
+            for i in range(len(self.stream['Shards'])):        
+                shardid = self.stream['Shards'][i]['ShardId']
+                if self.last_sequence_number is None:
+                    shard_iterator = self.client.get_shard_iterator(
+                        StreamName=self.stream['StreamName'],
+                        ShardId=shardid,                
+                        ShardIteratorType='LATEST'
+                        )
+                else:
+                    shard_iterator = self.client.get_shard_iterator(
+                        StreamName=self.stream['StreamName'],
+                        ShardId=shardid,
+                        ShardIteratorType='AFTER_SEQUENCE_NUMBER',
+                        StartingSequenceNumber=self.last_sequence_number
+                        )
+                self.stream['Shards'][i]['ShardIterator'] = shard_iterator['ShardIterator']
+                
+        if self.stream['StreamStatus'] != 'ACTIVE':
+            raise Exception('Stream status %s' % (self.stream['StreamStatus']))
+        print('Initializing stream DONE!')
+                
+    def consume(self):
+        success=False
+
+        for i in range(len(self.stream['Shards'])):
+            try:
+                response = self.client.get_records(\
+                    ShardIterator = self.stream['Shards'][i]['ShardIterator'],\
+                    Limit = 100)
+                success = True
+                self.stream['Shards'][i]['ShardIterator'] = response['NextShardIterator']
+                if len(response['Records'])> 0:
+                    for r in response['Records']:
+                        try:
+                            rec = json.loads(r['Data'])
+                            self.last_sequence_number = r['SequenceNumber']
+                            self.stream_buffer.append(rec)
+                        except Exception as e:
+                            print('Invalid record:'+str(r['Data']))
+                            print('Invalid record:'+str(e))
+                
+            except Exception as e:
+                print('Kinesis consume exception:%s' % (e))
+                break
+
         return success
```

### Comparing `shareddata-2.0.9/src/SharedData/SharedDataFrame.py` & `shareddata-2.1.0/src/SharedData/SharedDataFrame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,297 +1,296 @@
-# THIRD PARTY LIBS
-import os,sys
-import pandas as pd
-import numpy as np
-import json
-import time
-import io,gzip, hashlib, shutil
-from threading import Thread
-
-from pandas.tseries.offsets import BDay
-from pathlib import Path
-from multiprocessing import shared_memory
-from datetime import datetime, timedelta
-
-
-from SharedData.Logger import Logger
-from SharedData.SharedDataAWSS3 import S3Download,S3Upload,UpdateModTime
-from SharedData.SharedDataRealTime import SharedDataRealTime
-
-
-class SharedDataFrame:
-
-    def __init__(self, sharedDataPeriod, tag, df=None):        
-        self.sharedDataPeriod = sharedDataPeriod
-        self.tag = tag
-        self.tagstr = self.tag.strftime('%Y%m%d%H%M')
-        
-        
-        self.sharedDataFeeder = sharedDataPeriod.sharedDataFeeder
-        self.feeder = sharedDataPeriod.sharedDataFeeder.feeder
-        self.sharedData = sharedDataPeriod.sharedDataFeeder.sharedData        
-        self.database = self.sharedData.database
-
-        self.period = sharedDataPeriod.period
-        self.periodSeconds = sharedDataPeriod.periodSeconds  
-        
-        self.init_time = time.time()             
-        
-        # Time series dataframe
-        self.data = pd.DataFrame()
-
-        self.create_map = 'na'
-        if df is None: #Read dataset tag
-            #allocate memory
-            ismapped = self.Malloc()
-            if not ismapped:
-                # Read
-                df = self.Read()
-                if not df.empty:
-                    self.Malloc(df)
-            
-        else: # map existing dataframe   
-            #drop non number fields   
-            df = df._get_numeric_data().astype(np.float64)
-            #allocate memory
-            self.Malloc(df)
-        
-        self.init_time = time.time() - self.init_time
-
-    #GETTERS AND SETTERS
-    def getDataPath(self,iswrite=False):        
-        shm_name = self.sharedData.user
-        shm_name = shm_name + '/' + self.sharedData.database
-        shm_name = shm_name + '/' + self.sharedDataFeeder.feeder
-        shm_name = shm_name + '/' + self.period + '/' + self.tagstr
-        if os.name=='posix':
-            shm_name = shm_name.replace('/','\\')
-        
-        path = Path(os.environ['DATABASE_FOLDER'])
-        path = path / self.sharedData.user
-        path = path / self.sharedData.database
-        path = path / self.sharedDataFeeder.feeder
-        path = path / self.period
-        path = Path(str(path).replace('\\','/'))
-        if self.sharedData.save_local:
-            if not os.path.isdir(path):
-                os.makedirs(path)
-
-        return path, shm_name
-
-    # C R U D
-    def Malloc(self, df=None):
-        tini=time.time()
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            Logger.log.debug('Malloc %s/%s/%s/%s ...%.2f%% ' % \
-                (self.database,self.feeder,self.period,self.tagstr,0.0))      
-
-        #Create write ndarray
-        path, shm_name = self.getDataPath()
-        if not df is None:
-            # try create memory file
-            try: 
-                r = len(df.index)
-                c = len(df.columns)
-                            
-                idx_b = str.encode(','.join(df.index.values),\
-                    encoding='UTF-8',errors='ignore')
-                colscsv_b = str.encode(','.join(df.columns.values),\
-                    encoding='UTF-8',errors='ignore')
-                nb_idx = len(idx_b)
-                nb_cols = len(colscsv_b)
-                nb_data = int(r*c*8)
-                header_b = np.array([r,c,nb_idx,nb_cols,nb_data]).astype(np.int64).tobytes()
-                nb_header = len(header_b)
-                
-                nb_buf = nb_header+nb_idx+nb_cols+nb_data
-                nb_offset = nb_header+nb_idx+nb_cols
-
-                self.shm = shared_memory.SharedMemory(\
-                    name = shm_name,create=True, size=nb_buf)
-
-                i=0
-                self.shm.buf[i:nb_header] = header_b
-                i = i + nb_header
-                self.shm.buf[i:i+nb_idx] = idx_b
-                i = i + nb_idx
-                self.shm.buf[i:i+nb_cols] = colscsv_b
-
-                self.shmarr = np.ndarray((r,c),\
-                    dtype=np.float64, buffer=self.shm.buf, offset=nb_offset)
-
-                self.shmarr[:] = df.values.copy()
-
-                self.data = pd.DataFrame(self.shmarr,\
-                            index=df.index,\
-                            columns=df.columns,\
-                            copy=False)                
-
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    Logger.log.debug('Malloc create %s ...%.2f%% %.2f sec! ' % \
-                        (shm_name,100,time.time()-tini))            
-                self.create_map = 'create'
-                return True
-            except Exception as e:
-                return False
-        else: # df is None
-            # try map dataframe
-            try:
-                self.shm = shared_memory.SharedMemory(\
-                    name = shm_name,create=False)
-                i=0
-                nb_header=40
-                header = np.frombuffer(self.shm.buf[i:nb_header],dtype=np.int64)
-                i = i + nb_header
-                nb_idx = header[2]
-                idx_b = bytes(self.shm.buf[i:i+nb_idx])
-                index = idx_b.decode(encoding='UTF-8',errors='ignore').split(',')
-                i = i + nb_idx
-                nb_cols = header[3]
-                cols_b = bytes(self.shm.buf[i:i+nb_cols])
-                columns = cols_b.decode(encoding='UTF-8',errors='ignore').split(',')
-
-                r = header[0]
-                c = header[1]        
-                nb_data = header[4]
-                nb_offset = nb_header+nb_idx+nb_cols                
-                
-                self.shmarr = np.ndarray((r,c), dtype=np.float64,\
-                    buffer=self.shm.buf, offset=nb_offset)
-
-                self.data = pd.DataFrame(self.shmarr,\
-                            index=index,\
-                            columns=columns,\
-                            copy=False)
-
-                if not df is None:
-                    iidx = df.index.intersection(self.data.index)
-                    icol = df.columns.intersection(self.data.columns)
-                    self.data.loc[iidx, icol] = df.loc[iidx, icol]
-
-                self.create_map = 'map'
-                return True
-            except:
-                pass
-    
-        return False
-   
-    # READ
-    def Read(self):
-        return self.ReadDataFrame()
-
-    def ReadDataFrame(self):
-        tini = time.time()
-        path, shm_name = self.getDataPath()
-        local_path = str(path/(self.tagstr+'.bin'))
-        remote_path = local_path+'.gzip'
-        df_io = None
-        if self.sharedData.s3read:
-            #Synchronize S3
-            force_download= (not self.sharedData.save_local)
-            [df_io_gzip, df_local_mtime, df_remote_mtime] = \
-                S3Download(local_path,remote_path,force_download)
-            if not df_io_gzip is None:
-                df_io = io.BytesIO()
-                df_io_gzip.seek(0)
-                with gzip.GzipFile(fileobj=df_io_gzip, mode='rb') as gz:
-                    shutil.copyfileobj(gz,df_io)                
-                if self.sharedData.save_local:
-                    SharedDataFrame.write_file(df_io,local_path,df_remote_mtime)
-                    UpdateModTime(local_path,df_remote_mtime)
-
-        if (df_io is None) & (self.sharedData.save_local):
-            # read local
-            if os.path.isfile(str(local_path)):
-                df_io = open(str(local_path),'rb')
-
-        if not df_io is None:
-            return SharedDataFrame.read_data(df_io,local_path)
-                
-        return pd.DataFrame([])
-
-    def read_data(df_io,local_path):
-        df_io.seek(0)
-        _header = np.frombuffer(df_io.read(40),dtype=np.int64) 
-        _idx_b = df_io.read(int(_header[2]))
-        _idxcsv = _idx_b.decode(encoding='UTF-8',errors='ignore')   
-        _idx = _idxcsv.split(',')
-        _colscsv_b = df_io.read(int(_header[3]))
-        _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
-        _cols = _colscsv.split(',')
-        _data = np.frombuffer(df_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))        
-        #calculate hash
-        _m = hashlib.md5(_idx_b)
-        _m.update(_colscsv_b)
-        _m.update(_data)
-        _md5hash_b = _m.digest()
-        __md5hash_b = df_io.read(16)
-        if not _md5hash_b==__md5hash_b:
-            raise Exception('DataFrame file corrupted!\n%s' % (local_path))
-        df = pd.DataFrame(_data,index=_idx,columns=_cols)
-        df_io.close()
-        return df
-
-    # WRITE
-    def Write(self):     
-        path, shm_name = self.getDataPath(iswrite=True)
-        local_path = str(path/(self.tagstr+'.bin'))
-        remote_path = local_path+'.gzip'
-        df_io = SharedDataFrame.create_dataframe_io(self.data)
-        mtime = datetime.now().timestamp()
-        threads=[]
-        if self.sharedData.s3write:
-            df_io.seek(0)
-            gzip_io = io.BytesIO()
-            with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
-                shutil.copyfileobj(df_io, gz)
-            threads = [*threads , \
-                Thread(target=S3Upload,args=(gzip_io, remote_path, mtime) )]
-
-        if self.sharedData.save_local:
-            threads = [*threads , \
-                Thread(target=SharedDataFrame.write_file, args=(df_io, local_path, mtime) )]
-                            
-        for i in range(len(threads)):
-            threads[i].start()
-
-        for i in range(len(threads)):
-            threads[i].join()
-
-    def create_dataframe_io(df):        
-        r, c = df.shape
-        idx_b = str.encode(','.join(df.index.values),\
-            encoding='UTF-8',errors='ignore')
-        colscsv_b = str.encode(','.join(df.columns.values),\
-            encoding='UTF-8',errors='ignore')
-        nbidx = len(idx_b)
-        nbcols = len(colscsv_b)
-        data = np.ascontiguousarray(df.values.astype(np.float64))
-        header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
-        #calculate hash
-        m = hashlib.md5(idx_b)
-        m.update(colscsv_b)
-        m.update(data)
-        md5hash_b = m.digest()
-        # allocate memory
-        io_obj = io.BytesIO()
-        io_obj.write(header)
-        io_obj.write(idx_b)
-        io_obj.write(colscsv_b)
-        io_obj.write(data)
-        io_obj.write(md5hash_b)        
-        return io_obj
-
-    def write_file(io_obj,path,mtime):
-        with open(path, 'wb') as f:
-            f.write(io_obj.getbuffer())
-            f.flush()
-        os.utime(path, (mtime, mtime))
-     
-    # MESSAGES
-    def Broadcast(self,idx,col):
-        SharedDataRealTime.Broadcast(
-            self.sharedData,
-            self.feeder,
-            self.period,
-            self.tag,
+# THIRD PARTY LIBS
+import os,sys
+import pandas as pd
+import numpy as np
+import json
+import time
+import io,gzip, hashlib, shutil
+from threading import Thread
+
+from pandas.tseries.offsets import BDay
+from pathlib import Path
+from multiprocessing import shared_memory
+from datetime import datetime, timedelta
+
+
+from SharedData.Logger import Logger
+from SharedData.SharedDataAWSS3 import S3Download,S3Upload,UpdateModTime
+from SharedData.SharedDataRealTime import SharedDataRealTime
+
+
+class SharedDataFrame:
+
+    def __init__(self, sharedDataPeriod, tag, df=None):        
+        self.sharedDataPeriod = sharedDataPeriod
+        self.tag = tag
+        self.tagstr = self.tag.strftime('%Y%m%d%H%M')
+        
+        
+        self.sharedDataFeeder = sharedDataPeriod.sharedDataFeeder
+        self.feeder = sharedDataPeriod.sharedDataFeeder.feeder
+        self.sharedData = sharedDataPeriod.sharedDataFeeder.sharedData        
+        self.database = self.sharedData.database
+
+        self.period = sharedDataPeriod.period
+        self.periodSeconds = sharedDataPeriod.periodSeconds  
+        
+        self.init_time = time.time()             
+        
+        # Time series dataframe
+        self.data = pd.DataFrame()
+
+        self.create_map = 'na'
+        if df is None: #Read dataset tag
+            #allocate memory
+            ismapped = self.Malloc()
+            if not ismapped:
+                # Read
+                df = self.Read()
+                if not df.empty:
+                    self.Malloc(df)
+            
+        else: # map existing dataframe   
+            #drop non number fields   
+            df = df._get_numeric_data().astype(np.float64)
+            #allocate memory
+            self.Malloc(df)
+        
+        self.init_time = time.time() - self.init_time
+
+    #GETTERS AND SETTERS
+    def getDataPath(self,iswrite=False):        
+        shm_name = self.sharedData.user
+        shm_name = shm_name + '/' + self.sharedData.database
+        shm_name = shm_name + '/' + self.sharedDataFeeder.feeder
+        shm_name = shm_name + '/' + self.period + '/' + self.tagstr
+        if os.name=='posix':
+            shm_name = shm_name.replace('/','\\')
+        
+        path = Path(os.environ['DATABASE_FOLDER'])
+        path = path / self.sharedData.user
+        path = path / self.sharedData.database
+        path = path / self.sharedDataFeeder.feeder
+        path = path / self.period
+        path = Path(str(path).replace('\\','/'))
+        if self.sharedData.save_local:
+            if not os.path.isdir(path):
+                os.makedirs(path)
+
+        return path, shm_name
+
+    # C R U D
+    def Malloc(self, df=None):
+        tini=time.time()
+        if os.environ['LOG_LEVEL']=='DEBUG':
+            Logger.log.debug('Malloc %s/%s/%s/%s ...%.2f%% ' % \
+                (self.database,self.feeder,self.period,self.tagstr,0.0))      
+
+        #Create write ndarray
+        path, shm_name = self.getDataPath()
+        if not df is None:
+            # try create memory file
+            try: 
+                r = len(df.index)
+                c = len(df.columns)
+                            
+                idx_b = str.encode(','.join(df.index.values),\
+                    encoding='UTF-8',errors='ignore')
+                colscsv_b = str.encode(','.join(df.columns.values),\
+                    encoding='UTF-8',errors='ignore')
+                nb_idx = len(idx_b)
+                nb_cols = len(colscsv_b)
+                nb_data = int(r*c*8)
+                header_b = np.array([r,c,nb_idx,nb_cols,nb_data]).astype(np.int64).tobytes()
+                nb_header = len(header_b)
+                
+                nb_buf = nb_header+nb_idx+nb_cols+nb_data
+                nb_offset = nb_header+nb_idx+nb_cols
+
+                [self.shm, ismalloc] = self.sharedData.malloc(shm_name,create=True,size=nb_buf)
+                
+                i=0
+                self.shm.buf[i:nb_header] = header_b
+                i = i + nb_header
+                self.shm.buf[i:i+nb_idx] = idx_b
+                i = i + nb_idx
+                self.shm.buf[i:i+nb_cols] = colscsv_b
+
+                self.shmarr = np.ndarray((r,c),\
+                    dtype=np.float64, buffer=self.shm.buf, offset=nb_offset)
+
+                self.shmarr[:] = df.values.copy()
+
+                self.data = pd.DataFrame(self.shmarr,\
+                            index=df.index,\
+                            columns=df.columns,\
+                            copy=False)                
+
+                if os.environ['LOG_LEVEL']=='DEBUG':
+                    Logger.log.debug('Malloc create %s ...%.2f%% %.2f sec! ' % \
+                        (shm_name,100,time.time()-tini))            
+                self.create_map = 'create'
+                return True
+            except Exception as e:
+                return False
+        else: # df is None
+            # try map dataframe
+            try:
+                [self.shm, ismalloc] = self.sharedData.malloc(shm_name)
+                
+                i=0
+                nb_header=40
+                header = np.frombuffer(self.shm.buf[i:nb_header],dtype=np.int64)
+                i = i + nb_header
+                nb_idx = header[2]
+                idx_b = bytes(self.shm.buf[i:i+nb_idx])
+                index = idx_b.decode(encoding='UTF-8',errors='ignore').split(',')
+                i = i + nb_idx
+                nb_cols = header[3]
+                cols_b = bytes(self.shm.buf[i:i+nb_cols])
+                columns = cols_b.decode(encoding='UTF-8',errors='ignore').split(',')
+
+                r = header[0]
+                c = header[1]        
+                nb_data = header[4]
+                nb_offset = nb_header+nb_idx+nb_cols                
+                
+                self.shmarr = np.ndarray((r,c), dtype=np.float64,\
+                    buffer=self.shm.buf, offset=nb_offset)
+
+                self.data = pd.DataFrame(self.shmarr,\
+                            index=index,\
+                            columns=columns,\
+                            copy=False)
+
+                if not df is None:
+                    iidx = df.index.intersection(self.data.index)
+                    icol = df.columns.intersection(self.data.columns)
+                    self.data.loc[iidx, icol] = df.loc[iidx, icol]
+
+                self.create_map = 'map'
+                return True
+            except:
+                pass
+    
+        return False
+   
+    # READ
+    def Read(self):
+        return self.ReadDataFrame()
+
+    def ReadDataFrame(self):
+        tini = time.time()
+        path, shm_name = self.getDataPath()
+        local_path = str(path/(self.tagstr+'.bin'))
+        remote_path = local_path+'.gzip'
+        df_io = None
+        if self.sharedData.s3read:
+            #Synchronize S3
+            force_download= (not self.sharedData.save_local)
+            [df_io_gzip, df_local_mtime, df_remote_mtime] = \
+                S3Download(local_path,remote_path,force_download)
+            if not df_io_gzip is None:
+                df_io = io.BytesIO()
+                df_io_gzip.seek(0)
+                with gzip.GzipFile(fileobj=df_io_gzip, mode='rb') as gz:
+                    shutil.copyfileobj(gz,df_io)                
+                if self.sharedData.save_local:
+                    SharedDataFrame.write_file(df_io,local_path,df_remote_mtime)
+                    UpdateModTime(local_path,df_remote_mtime)
+
+        if (df_io is None) & (self.sharedData.save_local):
+            # read local
+            if os.path.isfile(str(local_path)):
+                df_io = open(str(local_path),'rb')
+
+        if not df_io is None:
+            return SharedDataFrame.read_data(df_io,local_path)
+                
+        return pd.DataFrame([])
+
+    def read_data(df_io,local_path):
+        df_io.seek(0)
+        _header = np.frombuffer(df_io.read(40),dtype=np.int64) 
+        _idx_b = df_io.read(int(_header[2]))
+        _idxcsv = _idx_b.decode(encoding='UTF-8',errors='ignore')   
+        _idx = _idxcsv.split(',')
+        _colscsv_b = df_io.read(int(_header[3]))
+        _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
+        _cols = _colscsv.split(',')
+        _data = np.frombuffer(df_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))        
+        #calculate hash
+        _m = hashlib.md5(_idx_b)
+        _m.update(_colscsv_b)
+        _m.update(_data)
+        _md5hash_b = _m.digest()
+        __md5hash_b = df_io.read(16)
+        if not _md5hash_b==__md5hash_b:
+            raise Exception('DataFrame file corrupted!\n%s' % (local_path))
+        df = pd.DataFrame(_data,index=_idx,columns=_cols)
+        df_io.close()
+        return df
+
+    # WRITE
+    def Write(self):     
+        path, shm_name = self.getDataPath(iswrite=True)
+        local_path = str(path/(self.tagstr+'.bin'))
+        remote_path = local_path+'.gzip'
+        df_io = SharedDataFrame.create_dataframe_io(self.data)
+        mtime = datetime.now().timestamp()
+        threads=[]
+        if self.sharedData.s3write:
+            df_io.seek(0)
+            gzip_io = io.BytesIO()
+            with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
+                shutil.copyfileobj(df_io, gz)
+            threads = [*threads , \
+                Thread(target=S3Upload,args=(gzip_io, remote_path, mtime) )]
+
+        if self.sharedData.save_local:
+            threads = [*threads , \
+                Thread(target=SharedDataFrame.write_file, args=(df_io, local_path, mtime) )]
+                            
+        for i in range(len(threads)):
+            threads[i].start()
+
+        for i in range(len(threads)):
+            threads[i].join()
+
+    def create_dataframe_io(df):        
+        r, c = df.shape
+        idx_b = str.encode(','.join(df.index.values),\
+            encoding='UTF-8',errors='ignore')
+        colscsv_b = str.encode(','.join(df.columns.values),\
+            encoding='UTF-8',errors='ignore')
+        nbidx = len(idx_b)
+        nbcols = len(colscsv_b)
+        data = np.ascontiguousarray(df.values.astype(np.float64))
+        header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
+        #calculate hash
+        m = hashlib.md5(idx_b)
+        m.update(colscsv_b)
+        m.update(data)
+        md5hash_b = m.digest()
+        # allocate memory
+        io_obj = io.BytesIO()
+        io_obj.write(header)
+        io_obj.write(idx_b)
+        io_obj.write(colscsv_b)
+        io_obj.write(data)
+        io_obj.write(md5hash_b)        
+        return io_obj
+
+    def write_file(io_obj,path,mtime):
+        with open(path, 'wb') as f:
+            f.write(io_obj.getbuffer())
+            f.flush()
+        os.utime(path, (mtime, mtime))
+     
+    # MESSAGES
+    def Broadcast(self,idx,col):
+        SharedDataRealTime.Broadcast(
+            self.sharedData,
+            self.feeder,
+            self.period,
+            self.tag,
             idx,col)
```

### Comparing `shareddata-2.0.9/src/SharedData/SharedDataRealTime.py` & `shareddata-2.1.0/src/SharedData/SharedDataRealTime.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,93 @@
-
-import os,boto3,time,subprocess,sys
-import pandas as pd
-import numpy as np
-
-from SharedData.Logger import Logger
-from SharedData.SharedDataAWSKinesis import KinesisStreamProducer
-
-class SharedDataRealTime:
-
-    # producer dictionary
-    producer = {}
-
-    def Broadcast(shdata,feeder,period,tag,idx,col):        
-        producer = SharedDataRealTime.getProducer(shdata)
-        data = shdata[feeder][period][tag].loc[idx,col].values
-        
-        if isinstance(tag,pd.Timestamp):
-            msg = {
-                'sender' : os.environ['USER_COMPUTER'],
-                'msgtype' : 'df',
-                'feeder' : feeder,
-                'period' : period,
-                'tag' : str(tag),
-                'idx' : idx,
-                'col' : col,
-                'data' : data.tolist()
-            }            
-        else:
-            msg = {
-                'sender' : os.environ['USER_COMPUTER'],
-                'msgtype' : 'ts',
-                'feeder' : feeder,
-                'period' : period,
-                'tag' : tag,
-                'idx' : idx.astype('int64').tolist(),
-                'col' : col,
-                'data' : data.tolist()
-            }            
-                
-        producer.produce(msg, partitionkey=feeder)
-
-    def getProducer(shdata):
-        if not shdata.database in SharedDataRealTime.producer.keys():
-            streamname = os.environ['BASE_STREAM_NAME']+'-'+shdata.database.lower()
-            session = boto3.Session(profile_name=os.environ['STREAM_AWS_PROFILE'])
-            client = session.client('kinesis')
-            #create stream
-            try:
-                response = client.create_stream(
-                    StreamName=streamname,
-                    ShardCount=1,
-                    StreamModeDetails={
-                        'StreamMode': 'PROVISIONED'
-                    }
-                )
-                if response['ResponseMetadata']['HTTPStatusCode']==200:
-                    Logger.log.info('Kinesis Stream %s created!' % (streamname))
-                    time.sleep(10) #wait stream to be created
-            except Exception as e:
-                pass
-            
-            SharedDataRealTime.producer[shdata.database] =\
-                KinesisStreamProducer(stream_name=streamname)
-        return SharedDataRealTime.producer[shdata.database]
-    
-    def Subscribe(shdata):
-        today = pd.Timestamp(pd.Timestamp.now().date())
-        wd = shdata['WATCHDOG']['D1']
-        dfwatchdog = wd[today]
-        if dfwatchdog.empty:
-            df = pd.DataFrame(
-                0,
-                index = [shdata.database],
-                columns = ['watchdog']
-            )
-            dfwatchdog = df
-        
-        # start subprocess if 
-        if time.time() - dfwatchdog.loc[shdata.database,'watchdog'] > 15:
-            Logger.log.debug('Starting new real time consumer process for %s' % (shdata.database))
-            proc = subprocess.Popen(['python','-m',\
-                'SharedData.SharedDataRealTimeProcess',\
-                shdata.database],
-                stdout=subprocess.PIPE, stderr=subprocess.PIPE,\
-                universal_newlines=True, shell=True)
-            rc = proc.poll()
-            return (rc is None)
-        else:
-            Logger.log.debug('Real time consumer process for %s already exists' % (shdata.database))
-        
-        #success
-        return True
-
-        # C:\Users\TRADEBOT04\src\SharedData\venv\Scripts\python.exe
-        # C:\Users\TRADEBOT04\src\SharedData\venv\Lib\site-packages\SharedData\SharedDataRealTimeProcess.py
+
+import os,boto3,time,subprocess,sys
+import pandas as pd
+import numpy as np
+
+from SharedData.Logger import Logger
+from SharedData.SharedDataAWSKinesis import KinesisStreamProducer
+
+class SharedDataRealTime:
+
+    # producer dictionary
+    producer = {}
+
+    def broadcast(shdata,feeder,period,tag,idx,col):        
+        producer = SharedDataRealTime.getProducer(shdata)
+        data = shdata[feeder][period][tag].loc[idx,col].values
+        
+        if isinstance(tag,pd.Timestamp):
+            msg = {
+                'sender' : os.environ['USER_COMPUTER'],
+                'msgtype' : 'df',
+                'feeder' : feeder,
+                'period' : period,
+                'tag' : str(tag),
+                'idx' : idx,
+                'col' : col,
+                'data' : data.tolist()
+            }            
+        else:
+            msg = {
+                'sender' : os.environ['USER_COMPUTER'],
+                'msgtype' : 'ts',
+                'feeder' : feeder,
+                'period' : period,
+                'tag' : tag,
+                'idx' : idx.astype('int64').tolist(),
+                'col' : col,
+                'data' : data.tolist()
+            }            
+                
+        producer.produce(msg, partitionkey=feeder)
+
+    def getProducer(shdata):
+        if not shdata.database in SharedDataRealTime.producer.keys():
+            streamname = os.environ['BASE_STREAM_NAME']+'-'+shdata.database.lower()
+            session = boto3.Session(profile_name=os.environ['STREAM_AWS_PROFILE'])
+            client = session.client('kinesis')
+            #create stream
+            try:
+                response = client.create_stream(
+                    StreamName=streamname,
+                    ShardCount=1,
+                    StreamModeDetails={
+                        'StreamMode': 'PROVISIONED'
+                    }
+                )
+                if response['ResponseMetadata']['HTTPStatusCode']==200:
+                    Logger.log.info('Kinesis Stream %s created!' % (streamname))
+                    time.sleep(10) #wait stream to be created
+            except Exception as e:
+                pass
+            
+            SharedDataRealTime.producer[shdata.database] =\
+                KinesisStreamProducer(stream_name=streamname)
+        return SharedDataRealTime.producer[shdata.database]
+    
+    def subscribe(shdata):
+        today = pd.Timestamp(pd.Timestamp.now().date())
+        wd = shdata['WATCHDOG']['D1']
+        dfwatchdog = wd[today]
+        if dfwatchdog.empty:
+            df = pd.DataFrame(
+                0,
+                index = [shdata.database],
+                columns = ['watchdog']
+            )
+            dfwatchdog = df
+        
+        # start subprocess if 
+        if time.time() - dfwatchdog.loc[shdata.database,'watchdog'] > 15:
+            Logger.log.debug('Starting new real time consumer process for %s' % (shdata.database))
+            proc = subprocess.Popen(['python','-m',\
+                'SharedData.SharedDataRealTimeProcess',\
+                shdata.database],
+                stdout=subprocess.PIPE, stderr=subprocess.PIPE,\
+                universal_newlines=True, shell=True)
+            rc = proc.poll()
+            return (rc is None)
+        else:
+            Logger.log.debug('Real time consumer process for %s already exists' % (shdata.database))
+        
+        #success
+        return True
```

### Comparing `shareddata-2.0.9/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.1.0/src/SharedData/SharedDataRealTimeProcess.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import os,time,sys
-import pandas as pd
-import numpy as np
-from pathlib import Path
-
-from SharedData.Logger import Logger
-logger = Logger(__file__)
-from SharedData.SharedData import SharedData
-from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer
-
-
-try:
-    if len(sys.argv)>=2:
-        DATABASE = str(sys.argv[1])
-    else:
-        DATABASE = 'MarketData'
-
-    if len(sys.argv)>=3:
-        SLEEP_TIME = int(sys.argv[2])
-    else:
-        SLEEP_TIME = 5
-
-    if len(sys.argv)>=4:
-        PLOT_MESSAGES = bool(sys.argv[3])
-    else:
-        PLOT_MESSAGES = False
-
-
-    streamname = os.environ['BASE_STREAM_NAME']+'-'+DATABASE.lower()    
-    user = os.environ['USER_COMPUTER']
-
-    Logger.log.info('Starting SharedData real time'+\
-        ' subscription database:%s' % (DATABASE))
-
-    consumer = KinesisStreamConsumer(streamname)
-    shdata = SharedData(DATABASE)
-
-    Logger.log.info('SharedData real time'+\
-        ' subscription database:%s STARTED!' % (DATABASE))
-
-    today = pd.Timestamp(pd.Timestamp.now().date())
-    lastdate = today
-    while True:
-        today = pd.Timestamp(pd.Timestamp.now().date())
-        wd = shdata['WATCHDOG']['D1']
-        dfwatchdog = wd[today]
-        if dfwatchdog.empty:
-            df = pd.DataFrame(
-                time.time(),
-                index = [shdata.database],
-                columns = ['watchdog']
-            )
-            wd[today] = df        
-        
-        dfwatchdog.loc[DATABASE,'watchdog'] = time.time()
-
-        consumer.consume()
-        for msg in consumer.stream_buffer:
-            if PLOT_MESSAGES:
-               print(str(msg))
-               
-            if msg['sender'] != user:
-                if msg['msgtype']=='df':
-                    tag = pd.Timestamp(msg['tag'])
-                    data = np.array(msg['data'])
-                    df = shdata[msg['feeder']][msg['period']][tag]
-                    df.loc[msg['idx'],msg['col']] = data
-                elif msg['msgtype']=='ts':
-                    data = np.array(msg['data'])
-                    idx = pd.to_datetime(msg['idx'])
-                    df = shdata[msg['feeder']][msg['period']][msg['tag']]
-                    df.loc[idx,msg['col']] = data
-
-        consumer.stream_buffer = []        
-        time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
-except Exception as e:        
-    Logger.log.error('SharedData real time'+\
+import os,time,sys
+import pandas as pd
+import numpy as np
+from pathlib import Path
+
+from SharedData.Logger import Logger
+logger = Logger(__file__)
+from SharedData.SharedData import SharedData
+from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer
+
+
+try:
+    if len(sys.argv)>=2:
+        DATABASE = str(sys.argv[1])
+    else:
+        DATABASE = 'MarketData'
+
+    if len(sys.argv)>=3:
+        SLEEP_TIME = int(sys.argv[2])
+    else:
+        SLEEP_TIME = 5
+
+    if len(sys.argv)>=4:
+        PLOT_MESSAGES = bool(sys.argv[3])
+    else:
+        PLOT_MESSAGES = False
+
+
+    streamname = os.environ['BASE_STREAM_NAME']+'-'+DATABASE.lower()    
+    user = os.environ['USER_COMPUTER']
+
+    Logger.log.info('Starting SharedData real time'+\
+        ' subscription database:%s' % (DATABASE))
+
+    consumer = KinesisStreamConsumer(streamname)
+    shdata = SharedData(DATABASE)
+
+    Logger.log.info('SharedData real time'+\
+        ' subscription database:%s STARTED!' % (DATABASE))
+
+    today = pd.Timestamp(pd.Timestamp.now().date())
+    lastdate = today
+    while True:
+        today = pd.Timestamp(pd.Timestamp.now().date())
+        wd = shdata['WATCHDOG']['D1']
+        dfwatchdog = wd[today]
+        if dfwatchdog.empty:
+            df = pd.DataFrame(
+                time.time(),
+                index = [shdata.database],
+                columns = ['watchdog']
+            )
+            wd[today] = df        
+        
+        dfwatchdog.loc[DATABASE,'watchdog'] = time.time()
+
+        consumer.consume()
+        for msg in consumer.stream_buffer:
+            if PLOT_MESSAGES:
+               print(str(msg))
+               
+            if msg['sender'] != user:
+                if msg['msgtype']=='df':
+                    tag = pd.Timestamp(msg['tag'])
+                    data = np.array(msg['data'])
+                    df = shdata[msg['feeder']][msg['period']][tag]
+                    df.loc[msg['idx'],msg['col']] = data
+                elif msg['msgtype']=='ts':
+                    data = np.array(msg['data'])
+                    idx = pd.to_datetime(msg['idx'])
+                    df = shdata[msg['feeder']][msg['period']][msg['tag']]
+                    df.loc[idx,msg['col']] = data
+
+        consumer.stream_buffer = []        
+        time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
+except Exception as e:        
+    Logger.log.error('SharedData real time'+\
         ' subscription database:%s ERROR: %s!' % (DATABASE,str(e)))
```

### Comparing `shareddata-2.0.9/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.1.0/src/shareddata.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 src/SharedData/SharedDataAWSS3.py
 src/SharedData/SharedDataFeeder.py
 src/SharedData/SharedDataFrame.py
 src/SharedData/SharedDataPeriod.py
 src/SharedData/SharedDataRealTime.py
 src/SharedData/SharedDataRealTimeProcess.py
 src/SharedData/SharedDataTable.py
-src/SharedData/SharedDataTableKeys.py
+src/SharedData/SharedDataTableIndex.py
+src/SharedData/SharedDataTableIndexJit.py
 src/SharedData/SharedDataTimeSeries.py
 src/SharedData/SharedNumpy.py
+src/SharedData/Utils.py
 src/SharedData/__init__.py
 src/shareddata.egg-info/PKG-INFO
 src/shareddata.egg-info/SOURCES.txt
 src/shareddata.egg-info/dependency_links.txt
 src/shareddata.egg-info/requires.txt
 src/shareddata.egg-info/top_level.txt
```

