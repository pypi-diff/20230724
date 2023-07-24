# Comparing `tmp/merge-downloader-0.0.2.tar.gz` & `tmp/merge-downloader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merge-downloader-0.0.2.tar", last modified: Wed Jun 28 18:22:06 2023, max compression
+gzip compressed data, was "merge-downloader-0.0.3.tar", last modified: Mon Jul 24 18:18:30 2023, max compression
```

## Comparing `merge-downloader-0.0.2.tar` & `merge-downloader-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 cordmaur   (501) staff       (20)        0 2023-06-28 18:22:06.277032 merge-downloader-0.0.2/
--rw-r--r--   0 cordmaur   (501) staff       (20)    35149 2023-06-22 16:56:44.000000 merge-downloader-0.0.2/LICENSE
--rw-r--r--   0 cordmaur   (501) staff       (20)      226 2023-06-28 18:22:06.276909 merge-downloader-0.0.2/PKG-INFO
--rw-r--r--   0 cordmaur   (501) staff       (20)     8393 2023-06-26 14:55:55.000000 merge-downloader-0.0.2/README.md
-drwxr-xr-x   0 cordmaur   (501) staff       (20)        0 2023-06-28 18:22:06.275292 merge-downloader-0.0.2/merge_downloader.egg-info/
--rw-r--r--   0 cordmaur   (501) staff       (20)      226 2023-06-28 18:22:06.000000 merge-downloader-0.0.2/merge_downloader.egg-info/PKG-INFO
--rw-r--r--   0 cordmaur   (501) staff       (20)      455 2023-06-28 18:22:06.000000 merge-downloader-0.0.2/merge_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 cordmaur   (501) staff       (20)        1 2023-06-28 18:22:06.000000 merge-downloader-0.0.2/merge_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 cordmaur   (501) staff       (20)       62 2023-06-28 18:22:06.000000 merge-downloader-0.0.2/merge_downloader.egg-info/entry_points.txt
--rw-r--r--   0 cordmaur   (501) staff       (20)       79 2023-06-28 18:22:06.000000 merge-downloader-0.0.2/merge_downloader.egg-info/requires.txt
--rw-r--r--   0 cordmaur   (501) staff       (20)       16 2023-06-28 18:22:06.000000 merge-downloader-0.0.2/merge_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 cordmaur   (501) staff       (20)        0 2023-06-28 18:22:06.276570 merge-downloader-0.0.2/mergedownloader/
--rw-r--r--   0 cordmaur   (501) staff       (20)       55 2023-06-28 18:20:15.000000 merge-downloader-0.0.2/mergedownloader/__init__.py
--rw-r--r--   0 cordmaur   (501) staff       (20)     8285 2023-06-23 16:49:55.000000 merge-downloader-0.0.2/mergedownloader/cli.py
--rw-r--r--   0 cordmaur   (501) staff       (20)    15581 2023-06-22 16:56:44.000000 merge-downloader-0.0.2/mergedownloader/downloader.py
--rw-r--r--   0 cordmaur   (501) staff       (20)     1835 2023-06-22 16:56:44.000000 merge-downloader-0.0.2/mergedownloader/enums.py
--rw-r--r--   0 cordmaur   (501) staff       (20)    24725 2023-06-22 16:56:44.000000 merge-downloader-0.0.2/mergedownloader/inpeparser.py
--rw-r--r--   0 cordmaur   (501) staff       (20)    10878 2023-06-22 16:56:44.000000 merge-downloader-0.0.2/mergedownloader/parser.py
--rw-r--r--   0 cordmaur   (501) staff       (20)    17873 2023-06-23 17:27:26.000000 merge-downloader-0.0.2/mergedownloader/utils.py
--rw-r--r--   0 cordmaur   (501) staff       (20)       38 2023-06-28 18:22:06.277079 merge-downloader-0.0.2/setup.cfg
--rw-r--r--   0 cordmaur   (501) staff       (20)      655 2023-06-28 18:19:37.000000 merge-downloader-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:18:30.941546 merge-downloader-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      233 2023-07-24 18:18:30.941546 merge-downloader-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8547 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 18:18:30.922507 merge-downloader-0.0.3/merge_downloader.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-07-24 18:18:30.000000 merge-downloader-0.0.3/merge_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-07-24 18:18:30.000000 merge-downloader-0.0.3/merge_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:18:30.000000 merge-downloader-0.0.3/merge_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-24 18:18:30.000000 merge-downloader-0.0.3/merge_downloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-07-24 18:18:30.000000 merge-downloader-0.0.3/merge_downloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-24 18:18:30.000000 merge-downloader-0.0.3/merge_downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 18:18:30.936536 merge-downloader-0.0.3/mergedownloader/
+-rw-rw-rw-   0        0        0       59 2023-07-24 18:12:09.000000 merge-downloader-0.0.3/mergedownloader/__init__.py
+-rw-rw-rw-   0        0        0     8602 2023-07-24 18:10:30.000000 merge-downloader-0.0.3/mergedownloader/cli.py
+-rw-rw-rw-   0        0        0    16088 2023-07-24 17:22:38.000000 merge-downloader-0.0.3/mergedownloader/downloader.py
+-rw-rw-rw-   0        0        0     1900 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/mergedownloader/enums.py
+-rw-rw-rw-   0        0        0    25421 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/mergedownloader/inpeparser.py
+-rw-rw-rw-   0        0        0    11251 2023-07-24 17:53:02.000000 merge-downloader-0.0.3/mergedownloader/parser.py
+-rw-rw-rw-   0        0        0    19548 2023-07-24 18:00:08.000000 merge-downloader-0.0.3/mergedownloader/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-24 18:18:30.941546 merge-downloader-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:18:30.940545 merge-downloader-0.0.3/tests/
+-rw-rw-rw-   0        0        0     4582 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/tests/test_date_processor.py
+-rw-rw-rw-   0        0        0     4025 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/tests/test_downloader.py
+-rw-rw-rw-   0        0        0     1335 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/tests/test_inpe.py
+-rw-rw-rw-   0        0        0     3144 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/tests/test_parser.py
+-rw-rw-rw-   0        0        0     2726 2023-07-11 18:44:26.000000 merge-downloader-0.0.3/tests/test_utils.py
```

### Comparing `merge-downloader-0.0.2/LICENSE` & `merge-downloader-0.0.3/LICENSE`

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

### Comparing `merge-downloader-0.0.2/README.md` & `merge-downloader-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-# MERGE Downloader
-The `merge-downloader` package is an unofficial Python library to download MERGE products from the Brazilian National Institute for Space Research (INPE). These products include daily precipitation raster files calibrated for South America and obtained from the MERGE model (Rozante et al. 2010), as well as other climatology data.
-
-![Example Gif](data/south_america_anim.gif)
-
-These products include daily precipitation raster files calibrated for South America and obtained from the MERGE model (Rozante et al. 2010). The MERGE model is built upon the IMERGE/GPM model and calibrated using thousands of in-situ rain gauges to deliver bias-free results. 
-Besides the daily raster precipitation from MERGE, INPE provides also other climatology data such as Year Accumulated, Monthly Average, Daily Average and others according to the following table: 
-
-![image](https://github.com/cordmaur/merge-downloader/assets/19617404/8a6e0c13-a755-4373-b303-3f43e550be6d)
-
-<b>Note:</b> The files are downloaded in the original format provided by INPE (i.e., .nc and .grib2).
-
-Additionally, the `merge-downloader` automates the procedure of spatial clipping the raster data to geometries of interest, that can be given in spatial formats supported by GeoPandas such as shapefile (i.e., `.shp`) or GeoJSON (i.e., `.geojson`). 
-
-# Install
-The easiest way to install the `merge-downloader` is through `pip install merge-downloader`. 
-Alternatively, if you want to contribute to this package, you can clone the repository and install it in edit mode:
-```
-git clone https://github.com/cordmaur/merge-downloader.git
-cd merge-downloader
-pip install -e .
-```
-
-## Dependencies
-The following libraries are required to run the package:
-```
-gdal
-geopandas
-rioxarray
-pystac-client
-matplotlib
-pytest
-cfgrib
-netCDF4
-contextily
-eccodes
-adjustText
-notebook
-```
-Pip will try to install them automatically, however it's recomended to have at least `GDAL` pre-installed in the environment. 
-
-## Docker image
-For a seamless experience, I recommend using <b>docker image</b> created specifically for the project. It is available at `https://hub.docker.com/r/cordmaur/merge-downloader/` and can be downloaded with `docker pull cordmaur/merge-downloader:v1`. This image comes with all the necessary libraries. 
-
-The following articles brings a quick intro to using docker for geospatial development. 
-* https://medium.com/towards-data-science/configuring-a-minimal-docker-image-for-spatial-analysis-with-python-dc9970ca8a8a
-* https://medium.com/towards-data-science/why-you-should-use-devcontainers-for-your-geospatial-development-600f42c7b7e1
-
-# CLI Interface
-The `merge-downloader` package offers a CLI that can be used for simple workflows such as downloading a series of files in their original format or exporting a `.csv` file with a time series. When opening the files through the library, additional post-processing to adjust the coordinates is automatically performed and those are not available in the CLI. 
-
-Once installed via `pip`, the CLI will be accessible through the `merge-downloader` command:
-```
-root@c272deddb0f1:/# merge-downloader
-usage: merge-downloader [-h] {reset,init,series,download} ...
-
-Merge Downloader
-
-positional arguments:
-  {reset,init,series,download}
-    reset               Reset default configuration
-    init                Initialize the environment
-    series              Calculate the rain and create a time-series for the specified period.
-    download            Download raster data
-
-options:
-  -h, --help            show this help message and exit
-```
-
-## Setting up the environment
-Before starting, we need to setup the download folder. This is done through `merge-downloader init` command. The `-f` flag is used to specify the folder and the `-url` flag can be used to change the FTP server that defaults to `ftp.cptec.inpe.br`. 
-```
-root@c272deddb0f1:/# merge-downloader init -h
-usage: merge-downloader init [-h] -f FOLDER [-url URL]
-
-The init command is used to set the FTP URL to pull the data from and the local download directory.
-
-options:
-  -h, --help            show this help message and exit
-  -f FOLDER, --folder FOLDER
-                        Local folder to download the files (relative path).
-  -url URL              FTP URL of the server. Defaults to 'ftp.cptec.inpe.br'
-root@c272deddb0f1:/# merge-downloader init -f /downloads
-Initializing...
-Setting downloading folder to '/downloads'
-```
-
-## Downloading data
-To download raw data, we use the `download` command. We need to specify the start and end dates through the `-d` flag. It accepts common ISO formats that can be parsed by `dateutils` library (e.g., `-d 20230501 20230515`). Additionally, it's necessary to specify the data type to be downloaded. The list of currently available types is available in the help and contains:
-```
-DAILY_RAIN,
-MONTHLY_ACCUM_YEARLY,
-DAILY_AVERAGE,
-MONTHLY_ACCUM,
-MONTHLY_ACCUM_MANUAL,
-YEARLY_ACCUM,
-HOURLY_WRF,
-DAILY_WRF
-```
-
-So, to download the daily rain, from 1st to 10th of June 2023, we can use the following command. Once the download is complete, it will display the list of files available.
-```
-root@c272deddb0f1:/# merge-downloader download -d 20230601 20230610 -t DAILY_RAIN
-Downloading INPETypes.DAILY_RAIN series for range: ['01-06-2023', '10-06-2023']
-The following files are available:
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230601.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230602.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230603.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230604.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230605.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230606.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230607.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230608.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230609.grib2
-/downloads/DAILY_RAIN/MERGE_CPTEC_20230610.grib2
-```
-
-## Downloading Series
-When creating a time-series, the `merge-downloader` will automatically reduce the X (i.e., longitude) and Y (i.e., latitude) axes through the `mean` operator to have the value alongside the `time` dimension. If a geometry is given (e.g., shapefile or geojson), the computation will be performed within the given geometries, otherwise the values will be computed for the entire raster. 
-
-Similarly to `download`, the `series` command requires the flags `-d` and `-t` for dates and data type, as well as the optional `-s` for the geometry and `-f` to specify the output file. Besides, one can also use the flags `--anim` and `--chart` to output a simple `.png` chart and an animated GIF automatically. 
-
-For example, in the following code we compute the monthly rain occurred in 2022 in the Amazonas Brazlilian state and output it to a file named `amazon.csv` (the sample `.geojson` files are located inside the `data/` folder of the project.
-
-```
-root@c272deddb0f1:/workspaces/merge-downloader# merge-downloader series -d 2022-01 2022-12 -t MONTHLY_ACCUM_YEARLY -s ./data/amazon.geojson -f tmp/amazon.csv --anim --chart
-Downloading INPETypes.MONTHLY_ACCUM_YEARLY series for range: ['26-01-2022', '26-12-2022']
-Cutting raster to: data/amazon.geojson
-Coverting shp CRS to EPSG:4326
-Series exported to: tmp/amazon.csv
-Creating bar chart: tmp/amazon.png
-Creating animation file: tmp/amazon.gif
-Appending: 2022-01-01T12:00:00.000000000
-Appending: 2022-02-01T12:00:00.000000000
-Appending: 2022-03-01T12:00:00.000000000
-Appending: 2022-04-01T12:00:00.000000000
-Appending: 2022-05-01T12:00:00.000000000
-Appending: 2022-06-01T12:00:00.000000000
-Appending: 2022-07-01T12:00:00.000000000
-Appending: 2022-08-01T12:00:00.000000000
-Appending: 2022-09-01T12:00:00.000000000
-Appending: 2022-10-01T12:00:00.000000000
-Appending: 2022-11-01T12:00:00.000000000
-Appending: 2022-12-01T12:00:00.000000000
-```
-
-The series (`.csv`) and the chart (`.png`) can be seen in the following picture.
-![image](https://github.com/cordmaur/merge-downloader/assets/19617404/e49dffdf-6cfc-4807-b747-8b15e0ddfe68)
-
-# Usage from Jupyter
-To use the package from a Jupyter or a python script, you can refer to the notebooks available in the `nbs/` folder. 
-
-# References
-Rozante, José Roberto, Demerval Soares Moreira, Luis Gustavo G. De Goncalves, and Daniel A. Vila. “Combining TRMM and Surface Observations of Precipitation: Technique and Validation over South America.” Weather and Forecasting 25, no. 3 (June 1, 2010): 885–94. https://doi.org/10.1175/2010WAF2222325.1.
+# MERGE Downloader
+The `merge-downloader` package is an unofficial Python library to download MERGE products from the Brazilian National Institute for Space Research (INPE). These products include daily precipitation raster files calibrated for South America and obtained from the MERGE model (Rozante et al. 2010), as well as other climatology data.
+
+![Example Gif](data/south_america_anim.gif)
+
+These products include daily precipitation raster files calibrated for South America and obtained from the MERGE model (Rozante et al. 2010). The MERGE model is built upon the IMERGE/GPM model and calibrated using thousands of in-situ rain gauges to deliver bias-free results. 
+Besides the daily raster precipitation from MERGE, INPE provides also other climatology data such as Year Accumulated, Monthly Average, Daily Average and others according to the following table: 
+
+![image](https://github.com/cordmaur/merge-downloader/assets/19617404/8a6e0c13-a755-4373-b303-3f43e550be6d)
+
+<b>Note:</b> The files are downloaded in the original format provided by INPE (i.e., .nc and .grib2).
+
+Additionally, the `merge-downloader` automates the procedure of spatial clipping the raster data to geometries of interest, that can be given in spatial formats supported by GeoPandas such as shapefile (i.e., `.shp`) or GeoJSON (i.e., `.geojson`). 
+
+# Install
+The easiest way to install the `merge-downloader` is through `pip install merge-downloader`. 
+Alternatively, if you want to contribute to this package, you can clone the repository and install it in edit mode:
+```
+git clone https://github.com/cordmaur/merge-downloader.git
+cd merge-downloader
+pip install -e .
+```
+
+## Dependencies
+The following libraries are required to run the package:
+```
+gdal
+geopandas
+rioxarray
+pystac-client
+matplotlib
+pytest
+cfgrib
+netCDF4
+contextily
+eccodes
+adjustText
+notebook
+```
+Pip will try to install them automatically, however it's recomended to have at least `GDAL` pre-installed in the environment. 
+
+## Docker image
+For a seamless experience, I recommend using <b>docker image</b> created specifically for the project. It is available at `https://hub.docker.com/r/cordmaur/merge-downloader/` and can be downloaded with `docker pull cordmaur/merge-downloader:v1`. This image comes with all the necessary libraries. 
+
+The following articles brings a quick intro to using docker for geospatial development. 
+* https://medium.com/towards-data-science/configuring-a-minimal-docker-image-for-spatial-analysis-with-python-dc9970ca8a8a
+* https://medium.com/towards-data-science/why-you-should-use-devcontainers-for-your-geospatial-development-600f42c7b7e1
+
+# CLI Interface
+The `merge-downloader` package offers a CLI that can be used for simple workflows such as downloading a series of files in their original format or exporting a `.csv` file with a time series. When opening the files through the library, additional post-processing to adjust the coordinates is automatically performed and those are not available in the CLI. 
+
+Once installed via `pip`, the CLI will be accessible through the `merge-downloader` command:
+```
+root@c272deddb0f1:/# merge-downloader
+usage: merge-downloader [-h] {reset,init,series,download} ...
+
+Merge Downloader
+
+positional arguments:
+  {reset,init,series,download}
+    reset               Reset default configuration
+    init                Initialize the environment
+    series              Calculate the rain and create a time-series for the specified period.
+    download            Download raster data
+
+options:
+  -h, --help            show this help message and exit
+```
+
+## Setting up the environment
+Before starting, we need to setup the download folder. This is done through `merge-downloader init` command. The `-f` flag is used to specify the folder and the `-url` flag can be used to change the FTP server that defaults to `ftp.cptec.inpe.br`. 
+```
+root@c272deddb0f1:/# merge-downloader init -h
+usage: merge-downloader init [-h] -f FOLDER [-url URL]
+
+The init command is used to set the FTP URL to pull the data from and the local download directory.
+
+options:
+  -h, --help            show this help message and exit
+  -f FOLDER, --folder FOLDER
+                        Local folder to download the files (relative path).
+  -url URL              FTP URL of the server. Defaults to 'ftp.cptec.inpe.br'
+root@c272deddb0f1:/# merge-downloader init -f /downloads
+Initializing...
+Setting downloading folder to '/downloads'
+```
+
+## Downloading data
+To download raw data, we use the `download` command. We need to specify the start and end dates through the `-d` flag. It accepts common ISO formats that can be parsed by `dateutils` library (e.g., `-d 20230501 20230515`). Additionally, it's necessary to specify the data type to be downloaded. The list of currently available types is available in the help and contains:
+```
+DAILY_RAIN,
+MONTHLY_ACCUM_YEARLY,
+DAILY_AVERAGE,
+MONTHLY_ACCUM,
+MONTHLY_ACCUM_MANUAL,
+YEARLY_ACCUM,
+HOURLY_WRF,
+DAILY_WRF
+```
+
+So, to download the daily rain, from 1st to 10th of June 2023, we can use the following command. Once the download is complete, it will display the list of files available.
+```
+root@c272deddb0f1:/# merge-downloader download -d 20230601 20230610 -t DAILY_RAIN
+Downloading INPETypes.DAILY_RAIN series for range: ['01-06-2023', '10-06-2023']
+The following files are available:
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230601.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230602.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230603.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230604.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230605.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230606.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230607.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230608.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230609.grib2
+/downloads/DAILY_RAIN/MERGE_CPTEC_20230610.grib2
+```
+
+## Downloading Series
+When creating a time-series, the `merge-downloader` will automatically reduce the X (i.e., longitude) and Y (i.e., latitude) axes through the `mean` operator to have the value alongside the `time` dimension. If a geometry is given (e.g., shapefile or geojson), the computation will be performed within the given geometries, otherwise the values will be computed for the entire raster. 
+
+Similarly to `download`, the `series` command requires the flags `-d` and `-t` for dates and data type, as well as the optional `-s` for the geometry and `-f` to specify the output file. Besides, one can also use the flags `--anim` and `--chart` to output a simple `.png` chart and an animated GIF automatically. 
+
+For example, in the following code we compute the monthly rain occurred in 2022 in the Amazonas Brazlilian state and output it to a file named `amazon.csv` (the sample `.geojson` files are located inside the `data/` folder of the project.
+
+```
+root@c272deddb0f1:/workspaces/merge-downloader# merge-downloader series -d 2022-01 2022-12 -t MONTHLY_ACCUM_YEARLY -s ./data/amazon.geojson -f tmp/amazon.csv --anim --chart
+Downloading INPETypes.MONTHLY_ACCUM_YEARLY series for range: ['26-01-2022', '26-12-2022']
+Cutting raster to: data/amazon.geojson
+Coverting shp CRS to EPSG:4326
+Series exported to: tmp/amazon.csv
+Creating bar chart: tmp/amazon.png
+Creating animation file: tmp/amazon.gif
+Appending: 2022-01-01T12:00:00.000000000
+Appending: 2022-02-01T12:00:00.000000000
+Appending: 2022-03-01T12:00:00.000000000
+Appending: 2022-04-01T12:00:00.000000000
+Appending: 2022-05-01T12:00:00.000000000
+Appending: 2022-06-01T12:00:00.000000000
+Appending: 2022-07-01T12:00:00.000000000
+Appending: 2022-08-01T12:00:00.000000000
+Appending: 2022-09-01T12:00:00.000000000
+Appending: 2022-10-01T12:00:00.000000000
+Appending: 2022-11-01T12:00:00.000000000
+Appending: 2022-12-01T12:00:00.000000000
+```
+
+The series (`.csv`) and the chart (`.png`) can be seen in the following picture.
+![image](https://github.com/cordmaur/merge-downloader/assets/19617404/e49dffdf-6cfc-4807-b747-8b15e0ddfe68)
+
+# Usage from Jupyter
+To use the package from a Jupyter or a python script, you can refer to the notebooks available in the `nbs/` folder. 
+
+# References
+Rozante, José Roberto, Demerval Soares Moreira, Luis Gustavo G. De Goncalves, and Daniel A. Vila. “Combining TRMM and Surface Observations of Precipitation: Technique and Validation over South America.” Weather and Forecasting 25, no. 3 (June 1, 2010): 885–94. https://doi.org/10.1175/2010WAF2222325.1.
```

### Comparing `merge-downloader-0.0.2/mergedownloader/cli.py` & `merge-downloader-0.0.3/mergedownloader/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-"""This module has the functions for the Command Line Interface"""
-
-import argparse
-from configparser import ConfigParser
-from pathlib import Path
-
-import geopandas as gpd
-import xarray as xr
-
-from mergedownloader.inpeparser import INPEParsers, INPETypes
-from mergedownloader.downloader import Downloader
-from mergedownloader.utils import DateProcessor, GISUtil, ChartUtil
-
-
-def reset(_):
-    """Clear default configuration"""
-    file = config_file()
-
-    if file.exists():
-        print(f"Deleting file {file}")
-        file.unlink()
-
-    else:
-        print("No default config to reset")
-
-
-def init(args):
-    """Initialize the package"""
-    print("Initializing...")
-
-    # setup the folder
-    folder = args.folder.absolute()
-    folder.mkdir(parents=False, exist_ok=True)
-    print(f"Setting downloading folder to '{folder}'")
-
-    config = ConfigParser()
-    config["DEFAULT"] = {"url": args.url, "folder": folder.as_posix()}
-
-    with open(config_file(), "w", encoding="utf-8") as configfile:
-        config.write(configfile)
-
-
-def config_file() -> Path:
-    """Returns the configuration file path"""
-    return Path(__file__).with_name("config.ini")
-
-
-def open_config() -> ConfigParser:
-    """Return the configuration"""
-    file = config_file()
-    if not file.exists():
-        raise FileNotFoundError((f"Config file '{file}' not found"))
-
-    config = ConfigParser()
-    config.read(config_file())
-
-    return config
-
-
-def validate_config(config: ConfigParser):
-    """Validate the configuration"""
-    validated = False
-    try:
-        config = open_config()
-
-        _ = config["DEFAULT"]["url"]
-        folder = Path(config["DEFAULT"]["folder"])
-
-        if not folder.exists():
-            raise FileNotFoundError(f"Folder specified in config '{folder}' not found")
-
-        validated = True
-
-    except KeyError as error:
-        print(f"Invalid configuration, missing key: {error}")
-
-    except FileNotFoundError as error:
-        print(error)
-
-    finally:
-        if not validated:
-            print("Config file not initialized correctly.")
-            print("Please run 'merge-downloader init' first.")
-
-    return validated
-
-
-def create_downloader() -> Downloader:
-    """Create a Downloader instance"""
-
-    config = open_config()
-    validate_config(config)
-
-    downloader = Downloader(
-        server=config["DEFAULT"]["url"],
-        parsers=INPEParsers.parsers,
-        local_folder=config["DEFAULT"]["folder"],
-    )
-
-    return downloader
-
-
-def series(args):
-    """Download a series"""
-
-    dates = list(map(DateProcessor.pretty_date, args.dates))
-    print(f"Downloading {args.type} series for range: {dates}")
-
-    # first, create the cube
-    downloader = create_downloader()
-    cube = downloader.create_cube(
-        start_date=args.dates[0],
-        end_date=args.dates[1],
-        datatype=args.type,
-    )
-
-    # Creating time-series
-    if not args.shp:
-        print("No shapefile provided. Evaluating rain for whole region (South America)")
-        series_xr = cube.mean(dim=["latitude", "longitude"])
-        series_pd = series_xr.to_series()
-        shp = None
-
-    else:
-        shp = gpd.read_file(args.shp)
-
-        print(f"Cutting raster to: {args.shp}")
-        series_pd = downloader.get_time_series(
-            cube=cube, shp=shp, reducer=xr.DataArray.mean
-        )
-
-    # Now we have the series in a Pandas Series object
-    # save to file
-    series_pd.to_csv(args.file.with_suffix(".csv"))
-    print(f"Series exported to: {args.file.with_suffix('.csv')}")
-
-    # if chart flag is True, plot a bar chart
-    if args.chart:
-        # create a thumbnail
-        print(f"Creating bar chart: {args.file.with_suffix('.png')}")
-        ChartUtil.save_bar(
-            series=series_pd, datatype=args.type, filename=args.file.with_suffix(".png")
-        )
-
-    # if animation flag is True, create a gif file
-    if args.anim:
-        print(f"Creating animation file: {args.file.with_suffix('.gif')}")
-        GISUtil.animate_cube(cube=cube, shp=shp, filename=args.file.with_suffix(".gif"))
-
-
-def download(args):
-    """Download merge/climatologic files"""
-
-    dates = list(map(DateProcessor.pretty_date, args.dates))
-    print(f"Downloading {args.type} series for range: {dates}")
-
-    downloader = create_downloader()
-
-    files = downloader.get_range(
-        start_date=args.dates[0],
-        end_date=args.dates[1],
-        datatype=args.type,
-    )
-
-    print("The following files are available:")
-    for file in files:
-        print(file)
-
-
-def main():
-    """Main entry point for the CLI"""
-    parser = argparse.ArgumentParser(description="Merge Downloader")
-
-    ### Define subparsers
-    subparsers = parser.add_subparsers()
-
-    #### Create parent parser with DEFAULT args
-    default_args = argparse.ArgumentParser(add_help=False)
-    default_args.add_argument(
-        "-d",
-        "--dates",
-        nargs=2,
-        type=DateProcessor.parse_date,
-        help="Date range 'start_date end_date'. "
-        "Dates can be specified any format that can be parsed e.g.: yyyymmdd, yyyy-mm, etc.",
-    )
-    default_args.add_argument(
-        "-t",
-        "--type",
-        required=True,
-        type=INPETypes.from_name,
-        help=f"Data type to download. It can be any of: {INPETypes.types()}",
-    )
-    # ------------------------------------------
-
-    #### Define the RESET subcommand ####
-    parser_init = subparsers.add_parser(
-        "reset",
-        help="Reset default configuration",
-        description="The default configuration is saved to 'config.ini' file within"
-        " the package's folder.",
-    )
-    parser_init.set_defaults(func=reset)
-    # ------------------------------------------
-
-    #### Define the INIT subcommand ####
-    parser_init = subparsers.add_parser(
-        "init",
-        help="Initialize the environment",
-        description="The init command is used to set the FTP URL to pull the data from and the "
-        " local download directory.",
-    )
-    parser_init.add_argument(
-        "-f",
-        "--folder",
-        help="Local folder to download the files (relative path).",
-        required=True,
-        type=Path,
-    )
-    parser_init.add_argument(
-        "-url",
-        help=f"FTP URL of the server. Defaults to '{INPEParsers.FTPurl}'",
-        default=INPEParsers.FTPurl,
-    )
-    parser_init.set_defaults(func=init)
-    # ------------------------------------------
-
-    #### Define the SERIES subcommand ####
-    parser_series = subparsers.add_parser(
-        "series",
-        help="Calculate the rain and create a time-series for the specified period.",
-        description="If a shapefile is provided the rain is evaluated within the polygons."
-        " It averages the rain spatially in the region.",
-        parents=[default_args],
-    )
-    parser_series.add_argument(
-        "-s",
-        "--shp",
-        help="Shapefile with polygon to cut the raster. If not specified, averages for "
-        "the whole region (South America)",
-        type=Path,
-    )
-    parser_series.add_argument(
-        "-f",
-        "--file",
-        required=True,
-        help="Specifies the .csv file to save the series to",
-        type=Path,
-    )
-    parser_series.add_argument(
-        "--chart",
-        action="store_true",
-        default=False,
-        help="Exports a chart (.png) with the series",
-    )
-    parser_series.add_argument(
-        "--anim",
-        action="store_true",
-        default=False,
-        help="Exports an animated GIF (.gif) with the series",
-    )
-    parser_series.set_defaults(func=series)
-    # ------------------------------------------
-
-    #### Define the DOWNLOAD subcommand ####
-    parser_download = subparsers.add_parser(
-        "download",
-        help="Download raster data",
-        description="The raster data is downloaded in the original format (i.e., .nc or .grib2)",
-        parents=[default_args],
-    )
-    parser_download.set_defaults(func=download)
-    # ------------------------------------------
-
-    # Parse the arguments
-    args = parser.parse_args()
-
-    # Call the appropriate function
-    # The 'func' attribute contains a reference to the function to be called
-    if hasattr(args, "func"):
-        args.func(args)
-    else:
-        parser.print_help()
-
-
-# if __name__ == "__main__":
-#     main()
+"""This module has the functions for the Command Line Interface"""
+
+import argparse
+from configparser import ConfigParser
+from pathlib import Path
+
+import geopandas as gpd
+import xarray as xr
+
+from mergedownloader.inpeparser import INPEParsers, INPETypes
+from mergedownloader.downloader import Downloader
+from mergedownloader.utils import DateProcessor, GISUtil, ChartUtil
+
+
+def reset(_):
+    """Clear default configuration"""
+    file = config_file()
+
+    if file.exists():
+        print(f"Deleting file {file}")
+        file.unlink()
+
+    else:
+        print("No default config to reset")
+
+
+def init(args):
+    """Initialize the package"""
+    print("Initializing...")
+
+    # setup the folder
+    folder = args.folder.absolute()
+    folder.mkdir(parents=False, exist_ok=True)
+    print(f"Setting downloading folder to '{folder}'")
+
+    config = ConfigParser()
+    config["DEFAULT"] = {"url": args.url, "folder": folder.as_posix()}
+
+    with open(config_file(), "w", encoding="utf-8") as configfile:
+        config.write(configfile)
+
+
+def config_file() -> Path:
+    """Returns the configuration file path"""
+    return Path(__file__).with_name("config.ini")
+
+
+def open_config() -> ConfigParser:
+    """Return the configuration"""
+    file = config_file()
+    if not file.exists():
+        raise FileNotFoundError((f"Config file '{file}' not found. Run merge-downloader init first!"))
+
+    config = ConfigParser()
+    config.read(config_file())
+
+    return config
+
+
+def validate_config(config: ConfigParser):
+    """Validate the configuration"""
+    validated = False
+    try:
+        config = open_config()
+
+        _ = config["DEFAULT"]["url"]
+        folder = Path(config["DEFAULT"]["folder"])
+
+        if not folder.exists():
+            raise FileNotFoundError(f"Folder specified in config '{folder}' not found")
+
+        validated = True
+
+    except KeyError as error:
+        print(f"Invalid configuration, missing key: {error}")
+
+    except FileNotFoundError as error:
+        print(error)
+
+    finally:
+        if not validated:
+            print("Config file not initialized correctly.")
+            print("Please run 'merge-downloader init' first.")
+
+    return validated
+
+
+def create_downloader() -> Downloader:
+    """Create a Downloader instance"""
+
+    config = open_config()
+    validate_config(config)
+
+    downloader = Downloader(
+        server=config["DEFAULT"]["url"],
+        parsers=INPEParsers.parsers,
+        local_folder=config["DEFAULT"]["folder"],
+    )
+
+    return downloader
+
+
+def series(args):
+    """Download a series"""
+
+    dates = list(map(DateProcessor.pretty_date, args.dates))
+    print(f"Downloading {args.type} series for range: {dates}")
+
+    # first, create the cube
+    downloader = create_downloader()
+    cube = downloader.create_cube(
+        start_date=args.dates[0],
+        end_date=args.dates[1],
+        datatype=args.type,
+    )
+
+    # Creating time-series
+    if not args.shp:
+        print("No shapefile provided. Evaluating rain for whole region (South America)")
+        series_xr = cube.mean(dim=["latitude", "longitude"])
+        series_pd = series_xr.to_series()
+        shp = None
+
+    else:
+        shp = gpd.read_file(args.shp)
+
+        print(f"Cutting raster to: {args.shp}")
+        series_pd = downloader.get_time_series(
+            cube=cube, shp=shp, reducer=xr.DataArray.mean
+        )
+
+    # Now we have the series in a Pandas Series object
+    # save to file
+    series_pd.to_csv(args.file.with_suffix(".csv"))
+    print(f"Series exported to: {args.file.with_suffix('.csv')}")
+
+    # if chart flag is True, plot a bar chart
+    if args.chart:
+        # create a thumbnail
+        print(f"Creating bar chart: {args.file.with_suffix('.png')}")
+        ChartUtil.save_bar(
+            series=series_pd, datatype=args.type, filename=args.file.with_suffix(".png")
+        )
+
+    # if animation flag is True, create a gif file
+    if args.anim:
+        print(f"Creating animation file: {args.file.with_suffix('.gif')}")
+        GISUtil.animate_cube(cube=cube, shp=shp, filename=args.file.with_suffix(".gif"))
+
+
+def download(args):
+    """Download merge/climatologic files"""
+
+    dates = list(map(DateProcessor.pretty_date, args.dates))
+    print(f"Downloading {args.type} series for range: {dates}")
+
+    downloader = create_downloader()
+
+    files = downloader.get_range(
+        start_date=args.dates[0],
+        end_date=args.dates[1],
+        datatype=args.type,
+    )
+
+    print("The following files are available:")
+    for file in files:
+        print(file)
+
+
+def main():
+    """Main entry point for the CLI"""
+    parser = argparse.ArgumentParser(description="Merge Downloader")
+
+    ### Define subparsers
+    subparsers = parser.add_subparsers()
+
+    #### Create parent parser with DEFAULT args
+    default_args = argparse.ArgumentParser(add_help=False)
+    default_args.add_argument(
+        "-d",
+        "--dates",
+        nargs=2,
+        type=DateProcessor.parse_date,
+        help="Date range 'start_date end_date'. "
+        "Dates can be specified any format that can be parsed e.g.: yyyymmdd, yyyy-mm, etc.",
+    )
+    default_args.add_argument(
+        "-t",
+        "--type",
+        required=True,
+        type=INPETypes.from_name,
+        help=f"Data type to download. It can be any of: {INPETypes.types()}",
+    )
+    # ------------------------------------------
+
+    #### Define the RESET subcommand ####
+    parser_init = subparsers.add_parser(
+        "reset",
+        help="Reset default configuration",
+        description="The default configuration is saved to 'config.ini' file within"
+        " the package's folder.",
+    )
+    parser_init.set_defaults(func=reset)
+    # ------------------------------------------
+
+    #### Define the INIT subcommand ####
+    parser_init = subparsers.add_parser(
+        "init",
+        help="Initialize the environment",
+        description="The init command is used to set the FTP URL to pull the data from and the "
+        " local download directory.",
+    )
+    parser_init.add_argument(
+        "-f",
+        "--folder",
+        help="Local folder to download the files (relative path).",
+        required=True,
+        type=Path,
+    )
+    parser_init.add_argument(
+        "-url",
+        help=f"FTP URL of the server. Defaults to '{INPEParsers.FTPurl}'",
+        default=INPEParsers.FTPurl,
+    )
+    parser_init.set_defaults(func=init)
+    # ------------------------------------------
+
+    #### Define the SERIES subcommand ####
+    parser_series = subparsers.add_parser(
+        "series",
+        help="Calculate the rain and create a time-series for the specified period.",
+        description="If a shapefile is provided the rain is evaluated within the polygons."
+        " It averages the rain spatially in the region.",
+        parents=[default_args],
+    )
+    parser_series.add_argument(
+        "-s",
+        "--shp",
+        help="Shapefile with polygon to cut the raster. If not specified, averages for "
+        "the whole region (South America)",
+        type=Path,
+    )
+    parser_series.add_argument(
+        "-f",
+        "--file",
+        required=True,
+        help="Specifies the .csv file to save the series to",
+        type=Path,
+    )
+    parser_series.add_argument(
+        "--chart",
+        action="store_true",
+        default=False,
+        help="Exports a chart (.png) with the series",
+    )
+    parser_series.add_argument(
+        "--anim",
+        action="store_true",
+        default=False,
+        help="Exports an animated GIF (.gif) with the series",
+    )
+    parser_series.set_defaults(func=series)
+    # ------------------------------------------
+
+    #### Define the DOWNLOAD subcommand ####
+    parser_download = subparsers.add_parser(
+        "download",
+        help="Download raster data",
+        description="The raster data is downloaded in the original format (i.e., .nc or .grib2)",
+        parents=[default_args],
+    )
+    parser_download.set_defaults(func=download)
+    # ------------------------------------------
+
+    # Parse the arguments
+    args = parser.parse_args()
+
+    # Call the appropriate function
+    # The 'func' attribute contains a reference to the function to be called
+    if hasattr(args, "func"):
+        args.func(args)
+    else:
+        parser.print_help()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `merge-downloader-0.0.2/mergedownloader/downloader.py` & `merge-downloader-0.0.3/mergedownloader/downloader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,473 +1,474 @@
-"""
-Module with specialized classes to understand the INPE FTP Structure
-"""
-
-from pathlib import Path
-from enum import Enum
-from typing import Union, List, Optional, Callable, Iterable
-from datetime import datetime, timedelta
-import logging
-from logging import handlers
-
-import geopandas as gpd
-import xarray as xr
-
-from .utils import FTPUtil, OSUtil, DateProcessor
-from .enums import INPETypes
-from .parser import BaseParser
-
-
-class Downloader:
-    """Business logic to download files from a given structure"""
-
-    def __init__(
-        self,
-        server: str,
-        parsers: List[BaseParser],
-        local_folder: Union[str, Path],
-        avoid_update: bool = True,
-        log_level: int = logging.INFO,
-    ) -> None:
-        """
-        :param server: FTP server to connect to (should accept Anonymous)
-        :param parsers: List of parsers to understand the FTP filesystem. Each parser will
-        be responsible for parsing one file type (e.g., Daily Rain, Monthly Accumulated, etc.)
-        For a list of available parsers, take a look at INPEParsers (from raindownloader.inpeparser import INPEParsers)
-        :param local_folder: Local folder to download the images and save the .log
-        :param avoid_update: Avoid looking for updates in the remote file, every time it is requested, defaults to True
-        :param post_processors: Any function that should be applied to the image after download.
-        This argument should be a dictionary of file extension and function.
-        For default processor, check NPEParsers.post_processors. Defaults to None
-        """
-
-        # store initialization variables
-        self.ftp = FTPUtil(server)
-        self.parsers = parsers
-        self.local_folder = Path(local_folder)
-        self.avoid_update = avoid_update
-
-        self.logger = self.init_logger(log_level)
-
-        self.logger.info("Initializing the Downloader class")
-
-        # update the parsers with global configs
-        for parser in self.parsers:
-            parser.ftp = self.ftp
-            parser.avoid_update = self.avoid_update
-            parser.clean_local_folder(local_folder=local_folder)
-
-    def init_logger(self, log_level: int):
-        """Initialize the loggers (downloader and parsers)"""
-
-        # create the logger
-        logger = logging.getLogger(__name__)
-        logger.setLevel(log_level)
-
-        # if the logger doesn't have any handlers, setup everything
-        if logger.hasHandlers():
-            logger.handlers.clear()
-        handler = Downloader.create_logger_handler(self.local_folder, log_level)
-        logger.addHandler(handler)
-
-        # setup FTP logger
-        if self.ftp.logger.hasHandlers():
-            self.ftp.logger.handlers.clear()
-        self.ftp.logger.addHandler(handler)
-
-        # setup parser loggers
-        for parser in self.parsers:
-            if parser.logger.hasHandlers():
-                parser.logger.handlers.clear()
-            parser.logger.addHandler(handler)
-            parser.logger.setLevel(log_level)
-
-        return logger
-
-    @staticmethod
-    def create_logger_handler(folder: Union[str, Path], level: int):
-        """
-        Create a logger file handler for all the project
-        :param folder: Folder to put the log gile
-        :return: file handler
-        """
-        # set the base level as DEBUG
-        logging.basicConfig(level=logging.DEBUG)
-
-        # clear the handler of the root logger to avoid messages being sent to console
-        logging.getLogger().handlers.clear()
-
-        path = Path(folder)
-        file_handler = handlers.RotatingFileHandler(
-            path / "downloader.log", maxBytes=1024 * 1024, backupCount=5
-        )
-        file_handler.setLevel(level)
-        file_handler.setFormatter(
-            logging.Formatter(
-                "[%(asctime)s:%(levelname)s:%(name)s] %(message)s",
-                datefmt="%Y%m%d-%H%M%S",
-            )
-        )
-        return file_handler
-
-    @staticmethod
-    def get_time_series(
-        cube: xr.DataArray,
-        shp: gpd.GeoDataFrame,
-        reducer: Callable,
-        keep_dim: str = "time",  # specify the dimension along with we will retrieve the TS
-    ):
-        """Get a time series of values within the shape, given a reducer method"""
-        if cube.rio.crs != shp.crs:
-            print(f"Coverting shp CRS to {cube.rio.crs}")
-            shp = shp.to_crs(cube.rio.crs)  # type: ignore
-
-        # clip to the desired area
-        area = cube.rio.clip(shp.geometry)
-
-        # get the dimensions to be reduced
-        reduce_dims = list(cube.dims)
-        reduce_dims.remove(keep_dim)
-
-        series = reducer(area, dim=reduce_dims).to_series()
-
-        return series
-
-    @property
-    def data_types(self) -> List[Union[Enum, str]]:
-        """Return the data types available in the parsers"""
-        return [parse.datatype for parse in self.parsers]
-
-    def is_downloaded(
-        self,
-        date_str: str,
-        # local_folder: Union[str, Path],
-        datatype: Union[INPETypes, str],
-    ):
-        """Return if the desired file is downloaded. Dispatch to the correct parser"""
-
-        self.logger.debug("Checking if %s/%s is downloaded", datatype, date_str)
-
-        parser = self.get_parser(datatype=datatype)
-        return parser.is_downloaded(
-            date=date_str,
-            local_folder=self.local_folder,
-        )
-
-    def compare_files(
-        self,
-        date_str: str,
-        datatype: Union[INPETypes, str],
-    ) -> None:
-        """Compare remote and local files visually"""
-        remote_file = self.remote_file_path(date_str, datatype=datatype)
-        remote_info = self.ftp.get_ftp_file_info(remote_file=remote_file)
-
-        local_file = self.local_file_path(date_str, datatype=datatype)
-        local_info = OSUtil.get_local_file_info(local_file)
-
-        self.logger.debug("Comparing %s to %s", remote_file, local_file)
-
-        print(remote_info)
-        print(local_info)
-
-    def get_parser(self, datatype: Union[Enum, str]) -> BaseParser:
-        """Get the correct parser for the specified datatype"""
-
-        for parser in self.parsers:
-            if parser.datatype == datatype:
-                return parser
-
-        raise ValueError(f"Parser not found for data type {datatype}")
-
-    def remote_file_path(
-        self, date: Union[str, datetime], datatype: Union[Enum, str]
-    ) -> str:
-        """Create the remote file path given a date"""
-        parser = self.get_parser(datatype=datatype)
-
-        return parser.remote_target(date=date)
-
-    def remote_file_exists(
-        self, date: Union[str, datetime], datatype: Union[Enum, str]
-    ) -> bool:
-        """Check if a remote file exists"""
-
-        remote_file = self.remote_file_path(date, datatype=datatype)
-        return self.ftp.file_exists(remote_file=remote_file)
-
-    def local_file_exists(
-        self, date: Union[str, datetime], datatype: Union[Enum, str]
-    ) -> bool:
-        """Verify if a specific local file exists"""
-        parser = self.get_parser(datatype=datatype)
-        local_target = parser.local_target(date=date, local_folder=self.local_folder)
-
-        return local_target.exists()
-
-    def local_file_path(
-        self,
-        date: Union[str, datetime],
-        datatype: Union[Enum, str],
-    ) -> Path:
-        """
-        Create the path for the local file, depending on the folder and file type.
-        It uses the filename function to derive the final filename.
-        """
-        parser = self.get_parser(datatype=datatype)
-        return parser.local_target(date=date, local_folder=self.local_folder)
-
-    def files_range(
-        self, start_date_str: str, end_date_str: str, datatype: Union[INPETypes, str]
-    ) -> List[str]:
-        """Docstring"""
-        dates = self.get_parser(datatype).dates_range(
-            start_date=start_date_str, end_date=end_date_str
-        )
-        return [self.remote_file_path(date, datatype=datatype) for date in dates]
-
-    def download_file(
-        self, date: Union[str, datetime], datatype: Union[Enum, str], **kwargs
-    ) -> Path:
-        """
-        Download a file from the FTP server to the a local folder. The filename and ftp location
-        folder filename will be obtained from the respective parsers.
-        """
-        parser = self.get_parser(datatype=datatype)
-        return parser.download_file(date=date, local_folder=self.local_folder, **kwargs)
-
-    def get_file(
-        self,
-        date: Union[str, datetime],
-        datatype: Union[Enum, str],
-        force_download: bool = False,
-        **kwargs,
-    ) -> Path:
-        """
-        Get a specific file. If it is not available locally, download it just in time.
-        If it is available locally and avoid_update is not True, check if the file has
-        changed in the server.
-        """
-        parser = self.get_parser(datatype=datatype)
-        return parser.get_file(
-            date=date,
-            local_folder=self.local_folder,
-            force_download=force_download,
-            **kwargs,
-        )
-
-    def get_files(
-        self,
-        dates: Iterable[Union[str, datetime]],
-        datatype: Union[Enum, str],
-        force_download: bool = False,
-        **kwargs,
-    ) -> List[Path]:
-        """
-        Download files from a list of dates and receives a list pointing to the files.
-        If there is a problem during the download of one file, a message error will be in the list.
-        """
-        parser = self.get_parser(datatype=datatype)
-        return parser.get_files(
-            dates=dates,
-            local_folder=self.local_folder,
-            force_download=force_download,
-            **kwargs,
-        )
-
-    def get_range(
-        self,
-        start_date: str,
-        end_date: str,
-        datatype: Union[Enum, str],
-        force_download: bool = False,
-        **kwargs,
-    ) -> List[Path]:
-        """
-        Download a range of files from start to end dates and receives a list pointing to the files.
-        If there is a problem during the download of one file, a message error will be in the list.
-        """
-
-        parser = self.get_parser(datatype=datatype)
-        return parser.get_range(
-            start_date=start_date,
-            end_date=end_date,
-            local_folder=self.local_folder,
-            force_download=force_download,
-            **kwargs,
-        )
-
-    def open_file(
-        self,
-        date_str: str,
-        datatype: Union[Enum, str],
-        force_download: bool = False,
-        return_array: bool = True,
-        **kwargs,
-    ) -> Union[xr.Dataset, xr.DataArray]:
-        """
-        Open a file and apply the post processing, if existent.
-        If return_array is True, it will try to access the corresponding variable
-        from the dataset, otherwise return the dataset.
-        """
-
-        self.logger.debug("Asked to open file %s/%s", date_str, datatype)
-
-        # get the file
-        file = self.get_file(
-            date=date_str, datatype=datatype, force_download=force_download, **kwargs
-        )
-
-        # open the file as is
-        dset = xr.open_dataset(file)
-
-        # get the parser to check if there is a post processing associated with it
-        parser = self.get_parser(datatype=datatype)
-        if parser.post_proc is not None:
-            dset = parser.post_proc(dset, date_str=date_str)
-
-        # transform the dataset into array
-        if return_array:
-            if isinstance(datatype, Enum):
-                return dset[datatype.value["var"]]
-            else:
-                return dset.to_array()
-        else:
-            return dset
-
-    def _create_cube(
-        self,
-        dates: List,
-        datatype: Union[Enum, str],
-        dim_key: Optional[str] = "time",
-        force_download: bool = False,
-        **kwargs,
-    ) -> xr.DataArray:
-        """
-        Stack the images in the list as one XARRAY Dataset cube.
-        """
-
-        # set the stacked dimension name
-        dim = "time" if dim_key is None else dim_key
-
-        # create a cube with the files
-        data_arrays = [
-            self.open_file(date, datatype, force_download, **kwargs).astype("float32")
-            for date in dates
-        ]
-
-        cube = xr.concat(data_arrays, dim=dim)  # type: ignore
-
-        return cube
-
-    def create_cube(
-        self,
-        start_date: Union[str, datetime],
-        end_date: Union[str, datetime],
-        datatype: Union[Enum, str],
-        dim_key: Optional[str] = "time",
-        force_download: bool = False,
-        **kwargs,
-    ) -> xr.DataArray:
-        """Create a cube from the range and apply the post_processor of the downloader"""
-
-        self.logger.info(
-            "Creating cube from %s to %s (%s)", start_date, end_date, datatype
-        )
-
-        # first, let's grab the desired dates
-        dates = self.get_parser(datatype).dates_range(
-            start_date=start_date, end_date=end_date
-        )
-
-        # then, create the cube
-        cube = self._create_cube(
-            dates=dates,
-            datatype=datatype,
-            dim_key=dim_key,
-            force_download=force_download,
-            **kwargs,
-        )
-
-        return cube
-
-    def create_forecast_cube(
-        self,
-        start_date: str,
-        end_date: str,
-        dim_key: Optional[str] = "time",
-        forecast_lag: int = 7,
-    ) -> xr.DataArray:
-        """Create a cube from the range and apply the post_processor of the downloader"""
-
-        self.logger.info(
-            "Creating daily forecast cube from %s to %s (forecast_lag=%s)",
-            start_date,
-            end_date,
-            forecast_lag,
-        )
-
-        # first, let's grab the desired dates
-        dates = self.get_parser(INPETypes.DAILY_WRF).dates_range(
-            start_date=start_date, end_date=end_date
-        )
-
-        timelag = timedelta(days=forecast_lag)
-        lagged_dates = [
-            DateProcessor.normalize_date(DateProcessor.parse_date(date) - timelag)
-            for date in dates
-        ]
-        # set the stacked dimension name
-        dim = "time" if dim_key is None else dim_key
-
-        # create a cube with the files
-        data_arrays = [
-            self.open_file(
-                date, INPETypes.DAILY_WRF, False, ref_date=lagged_date
-            ).astype("float32")
-            for date, lagged_date in zip(dates, lagged_dates)
-        ]
-
-        cube = xr.concat(data_arrays, dim=dim)  # type: ignore
-
-        return cube
-
-    def accum_rain(
-        self,
-        start_date: str,
-        end_date: str,
-        datatype: INPETypes,
-        force_download: bool = False,
-    ) -> xr.DataArray:
-        """Accumulate the rain in the given period"""
-
-        # first, get the cube
-        cube = self.create_cube(
-            start_date=start_date,
-            end_date=end_date,
-            datatype=datatype,
-            force_download=force_download,
-        )
-
-        dset = cube.sum(dim="time")
-        dset = dset.assign_coords({"time": cube.time[0].values})
-
-        return dset
-
-    def accum_periodically_rain(
-        self, periods: List, data_type: INPETypes, force_download: bool = False
-    ) -> xr.DataArray:
-        """Accumulate the rain in given periods."""
-
-        # get the arrays with the accumulated rain in each period
-        rains = [
-            self.accum_rain(
-                start_date=start,
-                end_date=end,
-                datatype=data_type,
-                force_download=force_download,
-            )
-            for start, end in periods
-        ]
-
-        cube = xr.concat(rains, dim="time")
-        return cube
+"""
+Module with specialized classes to understand the INPE FTP Structure
+"""
+
+from pathlib import Path
+from enum import Enum
+from typing import Union, List, Optional, Callable, Iterable
+from datetime import datetime, timedelta
+import logging
+from logging import handlers
+
+import geopandas as gpd
+import xarray as xr
+
+from .utils import FTPUtil, OSUtil, DateProcessor
+from .enums import INPETypes
+from .parser import BaseParser
+
+
+class Downloader:
+    """Business logic to download files from a given structure"""
+
+    def __init__(
+        self,
+        server: str,
+        parsers: List[BaseParser],
+        local_folder: Union[str, Path],
+        avoid_update: bool = True,
+        log_level: int = logging.INFO,
+        wget: bool = True,
+    ) -> None:
+        """
+        :param server: FTP server to connect to (should accept Anonymous)
+        :param parsers: List of parsers to understand the FTP filesystem. Each parser will
+        be responsible for parsing one file type (e.g., Daily Rain, Monthly Accumulated, etc.)
+        For a list of available parsers, take a look at INPEParsers (from raindownloader.inpeparser import INPEParsers)
+        :param local_folder: Local folder to download the images and save the .log
+        :param avoid_update: Avoid looking for updates in the remote file, every time it is requested, defaults to True
+        :param post_processors: Any function that should be applied to the image after download.
+        This argument should be a dictionary of file extension and function.
+        For default processor, check NPEParsers.post_processors. Defaults to None
+        """
+
+        # store initialization variables
+        self.ftp = FTPUtil(server, wget)
+        self.parsers = parsers
+        self.local_folder = Path(local_folder)
+        self.avoid_update = avoid_update
+
+        self.logger = self.init_logger(log_level)
+
+        self.logger.info("Initializing the Downloader class")
+
+        # update the parsers with global configs
+        for parser in self.parsers:
+            parser.ftp = self.ftp
+            parser.avoid_update = self.avoid_update
+            parser.clean_local_folder(local_folder=local_folder)
+
+    def init_logger(self, log_level: int):
+        """Initialize the loggers (downloader and parsers)"""
+
+        # create the logger
+        logger = logging.getLogger(__name__)
+        logger.setLevel(log_level)
+
+        # if the logger doesn't have any handlers, setup everything
+        if logger.hasHandlers():
+            logger.handlers.clear()
+        handler = Downloader.create_logger_handler(self.local_folder, log_level)
+        logger.addHandler(handler)
+
+        # setup FTP logger
+        if self.ftp.logger.hasHandlers():
+            self.ftp.logger.handlers.clear()
+        self.ftp.logger.addHandler(handler)
+
+        # setup parser loggers
+        for parser in self.parsers:
+            if parser.logger.hasHandlers():
+                parser.logger.handlers.clear()
+            parser.logger.addHandler(handler)
+            parser.logger.setLevel(log_level)
+
+        return logger
+
+    @staticmethod
+    def create_logger_handler(folder: Union[str, Path], level: int):
+        """
+        Create a logger file handler for all the project
+        :param folder: Folder to put the log gile
+        :return: file handler
+        """
+        # set the base level as DEBUG
+        logging.basicConfig(level=logging.DEBUG)
+
+        # clear the handler of the root logger to avoid messages being sent to console
+        logging.getLogger().handlers.clear()
+
+        path = Path(folder)
+        file_handler = handlers.RotatingFileHandler(
+            path / "downloader.log", maxBytes=1024 * 1024, backupCount=5
+        )
+        file_handler.setLevel(level)
+        file_handler.setFormatter(
+            logging.Formatter(
+                "[%(asctime)s:%(levelname)s:%(name)s] %(message)s",
+                datefmt="%Y%m%d-%H%M%S",
+            )
+        )
+        return file_handler
+
+    @staticmethod
+    def get_time_series(
+        cube: xr.DataArray,
+        shp: gpd.GeoDataFrame,
+        reducer: Callable,
+        keep_dim: str = "time",  # specify the dimension along with we will retrieve the TS
+    ):
+        """Get a time series of values within the shape, given a reducer method"""
+        if cube.rio.crs != shp.crs:
+            print(f"Coverting shp CRS to {cube.rio.crs}")
+            shp = shp.to_crs(cube.rio.crs)  # type: ignore
+
+        # clip to the desired area
+        area = cube.rio.clip(shp.geometry)
+
+        # get the dimensions to be reduced
+        reduce_dims = list(cube.dims)
+        reduce_dims.remove(keep_dim)
+
+        series = reducer(area, dim=reduce_dims).to_series()
+
+        return series
+
+    @property
+    def data_types(self) -> List[Union[Enum, str]]:
+        """Return the data types available in the parsers"""
+        return [parse.datatype for parse in self.parsers]
+
+    def is_downloaded(
+        self,
+        date_str: str,
+        # local_folder: Union[str, Path],
+        datatype: Union[INPETypes, str],
+    ):
+        """Return if the desired file is downloaded. Dispatch to the correct parser"""
+
+        self.logger.debug("Checking if %s/%s is downloaded", datatype, date_str)
+
+        parser = self.get_parser(datatype=datatype)
+        return parser.is_downloaded(
+            date=date_str,
+            local_folder=self.local_folder,
+        )
+
+    def compare_files(
+        self,
+        date_str: str,
+        datatype: Union[INPETypes, str],
+    ) -> None:
+        """Compare remote and local files visually"""
+        remote_file = self.remote_file_path(date_str, datatype=datatype)
+        remote_info = self.ftp.get_ftp_file_info(remote_file=remote_file)
+
+        local_file = self.local_file_path(date_str, datatype=datatype)
+        local_info = OSUtil.get_local_file_info(local_file)
+
+        self.logger.debug("Comparing %s to %s", remote_file, local_file)
+
+        print(remote_info)
+        print(local_info)
+
+    def get_parser(self, datatype: Union[Enum, str]) -> BaseParser:
+        """Get the correct parser for the specified datatype"""
+
+        for parser in self.parsers:
+            if parser.datatype == datatype:
+                return parser
+
+        raise ValueError(f"Parser not found for data type {datatype}")
+
+    def remote_file_path(
+        self, date: Union[str, datetime], datatype: Union[Enum, str]
+    ) -> str:
+        """Create the remote file path given a date"""
+        parser = self.get_parser(datatype=datatype)
+
+        return parser.remote_target(date=date)
+
+    def remote_file_exists(
+        self, date: Union[str, datetime], datatype: Union[Enum, str]
+    ) -> bool:
+        """Check if a remote file exists"""
+
+        remote_file = self.remote_file_path(date, datatype=datatype)
+        return self.ftp.file_exists(remote_file=remote_file)
+
+    def local_file_exists(
+        self, date: Union[str, datetime], datatype: Union[Enum, str]
+    ) -> bool:
+        """Verify if a specific local file exists"""
+        parser = self.get_parser(datatype=datatype)
+        local_target = parser.local_target(date=date, local_folder=self.local_folder)
+
+        return local_target.exists()
+
+    def local_file_path(
+        self,
+        date: Union[str, datetime],
+        datatype: Union[Enum, str],
+    ) -> Path:
+        """
+        Create the path for the local file, depending on the folder and file type.
+        It uses the filename function to derive the final filename.
+        """
+        parser = self.get_parser(datatype=datatype)
+        return parser.local_target(date=date, local_folder=self.local_folder)
+
+    def files_range(
+        self, start_date_str: str, end_date_str: str, datatype: Union[INPETypes, str]
+    ) -> List[str]:
+        """Docstring"""
+        dates = self.get_parser(datatype).dates_range(
+            start_date=start_date_str, end_date=end_date_str
+        )
+        return [self.remote_file_path(date, datatype=datatype) for date in dates]
+
+    def download_file(
+        self, date: Union[str, datetime], datatype: Union[Enum, str], **kwargs
+    ) -> Path:
+        """
+        Download a file from the FTP server to the a local folder. The filename and ftp location
+        folder filename will be obtained from the respective parsers.
+        """
+        parser = self.get_parser(datatype=datatype)
+        return parser.download_file(date=date, local_folder=self.local_folder, **kwargs)
+
+    def get_file(
+        self,
+        date: Union[str, datetime],
+        datatype: Union[Enum, str],
+        force_download: bool = False,
+        **kwargs,
+    ) -> Path:
+        """
+        Get a specific file. If it is not available locally, download it just in time.
+        If it is available locally and avoid_update is not True, check if the file has
+        changed in the server.
+        """
+        parser = self.get_parser(datatype=datatype)
+        return parser.get_file(
+            date=date,
+            local_folder=self.local_folder,
+            force_download=force_download,
+            **kwargs,
+        )
+
+    def get_files(
+        self,
+        dates: Iterable[Union[str, datetime]],
+        datatype: Union[Enum, str],
+        force_download: bool = False,
+        **kwargs,
+    ) -> List[Path]:
+        """
+        Download files from a list of dates and receives a list pointing to the files.
+        If there is a problem during the download of one file, a message error will be in the list.
+        """
+        parser = self.get_parser(datatype=datatype)
+        return parser.get_files(
+            dates=dates,
+            local_folder=self.local_folder,
+            force_download=force_download,
+            **kwargs,
+        )
+
+    def get_range(
+        self,
+        start_date: str,
+        end_date: str,
+        datatype: Union[Enum, str],
+        force_download: bool = False,
+        **kwargs,
+    ) -> List[Path]:
+        """
+        Download a range of files from start to end dates and receives a list pointing to the files.
+        If there is a problem during the download of one file, a message error will be in the list.
+        """
+
+        parser = self.get_parser(datatype=datatype)
+        return parser.get_range(
+            start_date=start_date,
+            end_date=end_date,
+            local_folder=self.local_folder,
+            force_download=force_download,
+            **kwargs,
+        )
+
+    def open_file(
+        self,
+        date_str: str,
+        datatype: Union[Enum, str],
+        force_download: bool = False,
+        return_array: bool = True,
+        **kwargs,
+    ) -> Union[xr.Dataset, xr.DataArray]:
+        """
+        Open a file and apply the post processing, if existent.
+        If return_array is True, it will try to access the corresponding variable
+        from the dataset, otherwise return the dataset.
+        """
+
+        self.logger.debug("Asked to open file %s/%s", date_str, datatype)
+
+        # get the file
+        file = self.get_file(
+            date=date_str, datatype=datatype, force_download=force_download, **kwargs
+        )
+
+        # open the file as is
+        dset = xr.open_dataset(file)
+
+        # get the parser to check if there is a post processing associated with it
+        parser = self.get_parser(datatype=datatype)
+        if parser.post_proc is not None:
+            dset = parser.post_proc(dset, date_str=date_str)
+
+        # transform the dataset into array
+        if return_array:
+            if isinstance(datatype, Enum):
+                return dset[datatype.value["var"]]
+            else:
+                return dset.to_array()
+        else:
+            return dset
+
+    def _create_cube(
+        self,
+        dates: List,
+        datatype: Union[Enum, str],
+        dim_key: Optional[str] = "time",
+        force_download: bool = False,
+        **kwargs,
+    ) -> xr.DataArray:
+        """
+        Stack the images in the list as one XARRAY Dataset cube.
+        """
+
+        # set the stacked dimension name
+        dim = "time" if dim_key is None else dim_key
+
+        # create a cube with the files
+        data_arrays = [
+            self.open_file(date, datatype, force_download, **kwargs).astype("float32")
+            for date in dates
+        ]
+
+        cube = xr.concat(data_arrays, dim=dim)  # type: ignore
+
+        return cube
+
+    def create_cube(
+        self,
+        start_date: Union[str, datetime],
+        end_date: Union[str, datetime],
+        datatype: Union[Enum, str],
+        dim_key: Optional[str] = "time",
+        force_download: bool = False,
+        **kwargs,
+    ) -> xr.DataArray:
+        """Create a cube from the range and apply the post_processor of the downloader"""
+
+        self.logger.info(
+            "Creating cube from %s to %s (%s)", start_date, end_date, datatype
+        )
+
+        # first, let's grab the desired dates
+        dates = self.get_parser(datatype).dates_range(
+            start_date=start_date, end_date=end_date
+        )
+
+        # then, create the cube
+        cube = self._create_cube(
+            dates=dates,
+            datatype=datatype,
+            dim_key=dim_key,
+            force_download=force_download,
+            **kwargs,
+        )
+
+        return cube
+
+    def create_forecast_cube(
+        self,
+        start_date: str,
+        end_date: str,
+        dim_key: Optional[str] = "time",
+        forecast_lag: int = 7,
+    ) -> xr.DataArray:
+        """Create a cube from the range and apply the post_processor of the downloader"""
+
+        self.logger.info(
+            "Creating daily forecast cube from %s to %s (forecast_lag=%s)",
+            start_date,
+            end_date,
+            forecast_lag,
+        )
+
+        # first, let's grab the desired dates
+        dates = self.get_parser(INPETypes.DAILY_WRF).dates_range(
+            start_date=start_date, end_date=end_date
+        )
+
+        timelag = timedelta(days=forecast_lag)
+        lagged_dates = [
+            DateProcessor.normalize_date(DateProcessor.parse_date(date) - timelag)
+            for date in dates
+        ]
+        # set the stacked dimension name
+        dim = "time" if dim_key is None else dim_key
+
+        # create a cube with the files
+        data_arrays = [
+            self.open_file(
+                date, INPETypes.DAILY_WRF, False, ref_date=lagged_date
+            ).astype("float32")
+            for date, lagged_date in zip(dates, lagged_dates)
+        ]
+
+        cube = xr.concat(data_arrays, dim=dim)  # type: ignore
+
+        return cube
+
+    def accum_rain(
+        self,
+        start_date: str,
+        end_date: str,
+        datatype: INPETypes,
+        force_download: bool = False,
+    ) -> xr.DataArray:
+        """Accumulate the rain in the given period"""
+
+        # first, get the cube
+        cube = self.create_cube(
+            start_date=start_date,
+            end_date=end_date,
+            datatype=datatype,
+            force_download=force_download,
+        )
+
+        dset = cube.sum(dim="time")
+        dset = dset.assign_coords({"time": cube.time[0].values})
+
+        return dset
+
+    def accum_periodically_rain(
+        self, periods: List, data_type: INPETypes, force_download: bool = False
+    ) -> xr.DataArray:
+        """Accumulate the rain in given periods."""
+
+        # get the arrays with the accumulated rain in each period
+        rains = [
+            self.accum_rain(
+                start_date=start,
+                end_date=end,
+                datatype=data_type,
+                force_download=force_download,
+            )
+            for start, end in periods
+        ]
+
+        cube = xr.concat(rains, dim="time")
+        return cube
```

### Comparing `merge-downloader-0.0.2/mergedownloader/inpeparser.py` & `merge-downloader-0.0.3/mergedownloader/inpeparser.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,696 +1,696 @@
-"""
-Module with specialized classes to understand the INPE FTP Structure
-The idea is to have several classes that implement the following interface:
-remote_file_path(date: str)
-"""
-import os
-
-# from abc import ABC, abstractmethod
-from enum import Enum, auto
-from pathlib import Path
-from typing import Callable, Optional, Union, List
-
-import calendar
-from datetime import datetime, timedelta
-from dateutil.relativedelta import relativedelta
-
-import matplotlib.colors as colors
-
-import xarray as xr
-
-from .parser import BaseParser
-from .utils import DateProcessor, FTPUtil, GISUtil, OSUtil, INPETypes
-from .enums import DateFrequency, INPETypes
-
-
-class INPE:
-    """Create the structure, given a root path (remote or local) and date/time of the file"""
-
-    # DailyMERGEroot = "/modelos/tempo/MERGE/GPM/DAILY"
-
-    # Define the colors and positions of the color stops
-    cmap_colors = [(1.0, 1.0, 1.0), (1, 1, 1.0), (0.5, 0.5, 1.0), (1.0, 0.4, 0.6)]
-    positions = [0.0, 0.1, 0.7, 1.0]
-
-    # Create the colormap using LinearSegmentedColormap
-    cmap = colors.LinearSegmentedColormap.from_list(
-        "my_colormap", list(zip(positions, cmap_colors))
-    )
-
-    def __init__(self, root_path: str) -> None:
-        self.root = os.path.normpath(root_path)
-
-    @staticmethod
-    def MERGE_structure(date: datetime) -> str:  # pylint: disable=invalid-name
-        """Given a date that can be parsed by dateutil, create the structure of the MERGE files"""
-        year = str(date.year)
-        month = str(date.month).zfill(2)
-        return "/".join([year, month])
-
-    @staticmethod
-    def MERGE_filename(date: datetime) -> str:  # pylint: disable=invalid-name
-        """Create the filename of the MERGE file, given a specific date"""
-        date_str = DateProcessor.normalize_date(date)
-        return f"MERGE_CPTEC_{date_str}.grib2"
-
-    @staticmethod
-    def MERGE_MAY_filename(date: datetime) -> str:  # pylint: disable=invalid-name
-        """
-        Monthly Accumulated Yearly:
-        Create the filename of the MERGE file, given a specific date
-        """
-        month_year = DateProcessor.month_abrev(date) + "_" + str(date.year)
-        return f"MERGE_CPTEC_acum_{month_year}.nc"
-
-    @staticmethod
-    def MERGE_DA_filename(date: datetime) -> str:  # pylint: disable=invalid-name
-        """
-        Daily Average
-        Create the filename of the MERGE file, given a specific date
-        """
-        day_month = f"{date.day:02d}{DateProcessor.month_abrev(date)}"
-        return f"MERGE_CPTEC_12Z{day_month}.nc"
-
-    @staticmethod
-    def MERGE_MA_filename(date: datetime) -> str:  # pylint: disable=invalid-name
-        """
-        Monthly Accumulated - Create the filename fot the Monthly Accumulated files from MERGE/INPE
-        E.g.: MERGE_CPTEC_acum_sep.nc
-        """
-        month_abrev = DateProcessor.month_abrev(date)
-        return f"MERGE_CPTEC_acum_{month_abrev}.nc"
-
-    @staticmethod
-    def MERGE_YA_filename(date: datetime) -> str:  # pylint: disable=invalid-name
-        """
-        Yearly Accumulated - Create the filename fot the Yearly Accumulated files from MERGE/INPE
-            E.g.: MERGE_CPTEC_acum_2003.nc
-        """
-        return f"MERGE_CPTEC_acum_{date.year}.nc"
-
-    @staticmethod
-    def yearly_post_proc(dset: xr.Dataset, date_str, **_) -> xr.Dataset:
-        """Adjust the time for the dataset"""
-
-        # first, perform the same adjust for all NCs
-        dset = INPE.nc_post_proc(dset)
-
-        date = DateProcessor.parse_date(date_str)
-        # fix month and day as 1
-        date = date + relativedelta(day=1, month=1)
-
-        return dset.assign_coords({"time": [date]})
-
-    @staticmethod
-    def grib2_post_proc(dset: xr.Dataset, **_) -> xr.Dataset:
-        """Adjust the longitude in INPE's grib2 files and sets the CRS"""
-
-        dset = dset.assign_coords({"longitude": dset.longitude - 360})
-        dset = dset.rio.write_crs("epsg:4326")
-        return dset
-
-    @staticmethod
-    def nc_post_proc(dset: xr.Dataset, **_) -> xr.Dataset:
-        """Adjust variable names in the netCDF files and set CRS"""
-        if "lon" in dset.dims:
-            dset = dset.rename_dims({"lon": "longitude", "lat": "latitude"})
-            dset = dset.rename_vars({"lon": "longitude", "lat": "latitude"})
-
-        dset = dset.rio.write_crs("epsg:4326")
-
-        return dset
-
-    @staticmethod
-    def WRF_foldername(date: datetime, **kwargs) -> str:  # pylint: disable=invalid-name
-        """
-        Given a date that can be parsed by dateutil, create the structure of the WRF files
-        E.g., 2023/05/22/00
-        """
-        date = DateProcessor.parse_date(kwargs["ref_date"])
-        year = str(date.year)
-        month = str(date.month).zfill(2)
-        day = str(date.day).zfill(2)
-
-        return "/".join([year, month, day, "00"])
-
-    @staticmethod
-    def WRF_filename(  # pylint: disable=invalid-name
-        date: datetime, ref_date: Union[str, datetime]
-    ) -> str:
-        """
-        WRF Hourly Filename - Create the filename fot the Hourly Forecast from WRF/INPE
-            E.g.: WRF_cpt_07KM_2023052200_2023052312.grib2
-        """
-        date1 = DateProcessor.normalize_date(ref_date) + "00"
-
-        date2 = DateProcessor.parse_date(date)
-        date2 = DateProcessor.pretty_date(date2, "%Y%m%d%H")
-        return f"WRF_cpt_07KM_{date1}_{date2}.grib2"
-
-
-class MonthAccumParser(BaseParser):
-    """Docstring"""
-
-    def __init__(
-        self,
-        datatype: Union[Enum, str],
-        fn_creator: Callable,
-        daily_parser: BaseParser,
-        fl_creator: Optional[Callable] = None,
-        date_freq: DateFrequency = DateFrequency.DAILY,
-        ftp: Optional[FTPUtil] = None,
-        avoid_update: bool = True,
-    ):
-        super().__init__(
-            datatype=datatype,
-            root="",
-            filename_fn=fn_creator,
-            foldername_fn=fl_creator,
-            date_freq=date_freq,
-            ftp=ftp,
-            avoid_update=avoid_update,
-        )
-
-        self.daily_parser = daily_parser
-
-    def download_file(self, date: Union[str, datetime], local_folder: Union[str, Path]):
-        """Actually this function performs as accum_monthly_rain"""
-        # accumulate the daily rain
-        return self.accum_monthly_rain(
-            date=date, local_folder=local_folder, force_download=True
-        )
-
-    def accum_monthly_rain(
-        self,
-        date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        force_download: bool,
-    ) -> Path:
-        """Docstring"""
-
-        # create a cube with the daily rain in the given month
-        start_date, end_date = DateProcessor.start_end_dates(date=date)
-
-        # here, we will check for the current month
-        now = datetime.now()
-        today = datetime(now.year, now.month, now.day)
-
-        if DateProcessor.parse_date(end_date) >= today:
-            # if the end date is future, it meansn we are trying to get the current month
-            # in this case, let's start going backwards to see the last available file in the FTP
-            for day in range(today.day, 0, -1):
-                end_date = today + relativedelta(day=day)
-                remote_file = self.daily_parser.remote_target(
-                    DateProcessor.normalize_date(end_date)
-                )
-
-                # if the file exists, then we have our end date
-                if self.ftp.file_exists(remote_file):
-                    break
-
-                # otherwise, raise exception if we reached the first day
-                if day == 1:
-                    raise Exception(f"No avilable file to calculate month {date}")
-
-        end_date = DateProcessor.normalize_date(end_date)
-
-        daily_files = self.daily_parser.get_range(
-            start_date=start_date,
-            end_date=end_date,
-            local_folder=local_folder,
-            force_download=force_download,
-        )
-
-        dset = GISUtil.create_cube(files=daily_files, dim_key="time")
-        cube = INPE.grib2_post_proc(dset)
-
-        # get the reference datetime
-        ref_time = cube.time[0].values
-
-        accum = cube[INPETypes.DAILY_RAIN.value["var"]].sum(dim="time")
-        accum = accum.rename(INPETypes.MONTHLY_ACCUM_MANUAL.value["var"])
-
-        # once the reduction is being done in the time dimension, create a new dimension for time
-        accum = accum.assign_coords({"time": ref_time}).expand_dims(dim="time")
-
-        # save the file to disk
-        target_file = self.local_target(date=date, local_folder=local_folder)
-        dset = accum.to_dataset()
-
-        # update the creation date for this file
-        dset.attrs["updated"] = str(now)
-        dset.attrs["last_day"] = end_date
-        dset.attrs["days"] = len(daily_files)
-
-        dset.to_netcdf(target_file)
-
-        return target_file
-
-    def get_file(
-        self,
-        date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        force_download: bool = False,
-    ) -> Path:
-        """
-        Get a specific file. If it is not available locally, download it just in time.
-        If it is available locally and avoid_update is not True, check if the file has
-        changed in the server
-        """
-
-        must_update = False
-        dset = None
-        local_target = self.local_target(date=date, local_folder=local_folder)
-
-        self.logger.debug("Getting file %s", local_target.name)
-
-        # first check verifies if the file exists and has the new attributes
-        if not local_target.exists() or force_download:
-            must_update = True
-
-        else:
-            # the file exists, try to open it and check if it is updated
-            try:
-                dset = xr.open_dataset(local_target)
-
-                if (
-                    ("updated" not in dset.attrs)
-                    or ("days" not in dset.attrs)
-                    or ("last_day" not in dset.attrs)
-                ):
-                    self.logger.debug(
-                        "Forcing update for date %s to add the new attributes ", date
-                    )
-                    must_update = True
-
-            except Exception as error:
-                self.logger.error(error)
-                must_update = True
-
-        # now, we have to decide if the file must be updated
-        if dset is not None and not must_update:
-            # first, let's get the dates from the file
-            date = DateProcessor.parse_date(date)
-            now = datetime.now()
-            last_day = DateProcessor.parse_date(dset.attrs["last_day"])
-            updated = DateProcessor.parse_date(dset.attrs["updated"])
-
-            # if file was updated in the last 30 min, return it regardless anything.
-            update_delta = now - updated
-            if update_delta.seconds < (30 * 60):
-                return local_target
-
-            # check if it is complete (has all the necessary days)
-            if (date.year == now.year) and (date.month == now.month):
-                ref_days = now.day
-            else:
-                _, ref_days = calendar.monthrange(date.year, date.month)
-
-            if dset.attrs["days"] != ref_days:
-                self.logger.debug(
-                    "File was created with %s days, expected: %s days",
-                    dset.attrs["days"],
-                    ref_days,
-                )
-                must_update = True
-
-            else:
-                # now, let's check how far are the days in the past
-                timedelta = now - last_day
-                if timedelta.days < 30:
-                    # file references nearby dates, let's check if it was updated recently
-                    self.logger.debug("Month within 30 days limit.")
-
-                    if update_delta.seconds > (2 * 60 * 60):
-                        # last update was more than 2 hours ago
-                        self.logger.debug(
-                            "Last file update was %s. Forcing new update.", updated
-                        )
-                        must_update = True
-                    else:
-                        self.logger.debug("File updated recently (%s)", updated)
-
-                else:
-                    self.logger.debug(
-                        "Monthly file refers to old files. Not necessary to update."
-                    )
-
-        # close the dataset
-        if dset is not None:
-            dset.close()
-
-        if must_update:
-            # store the old avoid update status
-            avoid_update = self.daily_parser.avoid_update
-            self.daily_parser.avoid_update = True  # False
-
-            file = self.accum_monthly_rain(
-                date=date,
-                local_folder=local_folder,
-                force_download=force_download,
-            )
-
-            # retrieve the avoid_update status
-            self.daily_parser.avoid_update = avoid_update
-            return file
-
-        return local_target
-
-        # must_update = False
-        # local_target = self.local_target(date=date, local_folder=local_folder)
-
-        # # if the file does not exist or we ask to download it again, we set the must_update flag
-        # # to True
-        # if not local_target.exists() or force_download:
-        #     must_update = True
-
-        # # otherwise we have to open the file and check update conditions
-        # else:
-        #     dset = xr.open_dataset(local_target)
-
-        #     ### Check attributes to conform the files to the new version
-        #     if (
-        #         ("updated" not in dset.attrs)
-        #         or ("days" not in dset.attrs)
-        #         or ("last_day" not in dset.attrs)
-        #     ):
-        #         self.logger.debug(
-        #             "Forcing update for date %s to add the new attributes ", date
-        #         )
-        #         must_update = True
-
-        #     else:
-        #         # get the dates from the file
-        #         date = DateProcessor.parse_date(date)
-        #         now = datetime.now()
-        #         last_day = DateProcessor.parse_date(dset.attrs["last_day"])
-        #         updated = DateProcessor.parse_date(dset.attrs["updated"])
-
-        #         # Now, let's treat separately if we are in the current month or not
-        #         if (date.year == now.year) and (date.month == now.month):
-        #             # if we are in the current month, check the last day used in the file
-        #             # force update if last update was more than 2 hour ago.
-        #             timedelta = now - updated
-        #             if (now.day >= last_day.day) or (timedelta.seconds > 2 * 60 * 60):
-        #                 self.logger.debug(
-        #                     "Last update was %s minutes ago", timedelta.seconds / 60
-        #                 )
-        #                 if now.day >= last_day.day:
-        #                     self.logger.debug("Last_day %s < today", last_day)
-
-        #                 self.logger.debug("Forcing update")
-        #                 must_update = True
-
-        #             else:
-        #                 must_update = False
-
-        #         else:
-        #             # let's check if the file was updated with all the necessary days.
-        #             _, days = calendar.monthrange(date.year, date.month)
-
-        #             # update the file if the number of days differ or if the last day is recent??
-        #             if dset["days"] != days:
-        #                 self.logger.debug(
-        #                     "File was created with %s, expected: %s", dset["days"], days
-        #                 )
-        #                 must_update = True
-
-        # if must_update:
-        #     # store the old avoid update status
-        #     avoid_update = self.daily_parser.avoid_update
-        #     self.daily_parser.avoid_update = True  # False
-
-        #     file = self.accum_monthly_rain(
-        #         date=date,
-        #         local_folder=local_folder,
-        #         force_download=force_download,
-        #     )
-
-        #     # retrieve the avoid_update status
-        #     self.daily_parser.avoid_update = avoid_update
-        #     return file
-
-        # else:
-        #     return local_target
-
-        # # we will force the accum_monthly rain if the month is the current month
-        # date = DateProcessor.parse_date(date) + relativedelta(day=1)
-
-        # now = datetime.now() + relativedelta(
-        #     day=1, hour=0, minute=0, second=0, microsecond=0
-        # )
-
-        # # check if we are in the same month... if that's the case, force the parsers to check if the files
-        # # were updated in the server
-        # if now == date or force_download or not local_target.exists():
-        #     # store the old avoid update status
-        #     avoid_update = self.daily_parser.avoid_update
-        #     self.daily_parser.avoid_update = True  # False
-
-        #     file = self.accum_monthly_rain(
-        #         date=date,
-        #         local_folder=local_folder,
-        #         force_download=force_download,
-        #     )
-
-        #     # retrieve the avoid_update status
-        #     self.daily_parser.avoid_update = avoid_update
-
-        #     return file
-
-        # else:
-        #     return local_target
-
-
-class HourlyWRFParser(BaseParser):
-    """Docstring"""
-
-    def download_file(
-        self,
-        date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        ref_date: Union[str, datetime],
-    ) -> Path:
-        """Instead of downloading a specific hour, we have to actually calculate it"""
-        # convert the date to datetime
-        date = DateProcessor.parse_date(date)
-
-        # download this specific date/hour
-        file1 = super().download_file(
-            date, local_folder=local_folder, ref_date=ref_date
-        )
-
-        # download the previous hour
-        prev_date = date - timedelta(hours=1)
-        tmp_folder = Path(local_folder) / "tmp"
-        if not tmp_folder.exists():
-            tmp_folder.mkdir(parents=True, exist_ok=True)
-        file2 = super().download_file(
-            prev_date, local_folder=tmp_folder, ref_date=ref_date
-        )
-
-        # open both files and subtract file1 - file2
-        dset1 = xr.open_dataset(file1)
-        dset2 = xr.open_dataset(file2)
-        dset = dset1 - dset2
-
-        # save the hourly rain to disk and delete the temporary
-        dset.attrs["updated"] = str(datetime.now())
-
-        dset = dset.rename_vars({"unknown": "hour_wrf"})
-        dset = dset.assign_coords({"longitude": dset.longitude - 360})
-        dset = dset.rio.write_crs("epsg:4326")
-
-        # close the datasets and clear the temp folder
-        dset.to_netcdf(file1)
-        # file1 = file1.with_suffix(".tif")
-        # dset.to_array().squeeze().rio.to_raster(file1)
-
-        dset1.close()
-        dset2.close()
-        OSUtil.clear_folder(tmp_folder)
-
-        return file1
-
-
-class DailyWRFParser(BaseParser):
-    """Docstring"""
-
-    @staticmethod
-    def _foldername_fn(_: datetime, **kwargs) -> str:
-        """Create a foldername for the local storage"""
-        return DateProcessor.normalize_date(kwargs["ref_date"])
-
-    @staticmethod
-    def _filename_fn(date: datetime, ref_date: Union[str, datetime]) -> str:
-        """Create the filename for local storage"""
-        date1 = DateProcessor.normalize_date(ref_date)
-        date2 = DateProcessor.normalize_date(date)
-        return f"WRF_{date1}_{date2}.grib2"
-
-    def __init__(
-        self,
-        datatype: Union[Enum, str],
-        root: str,
-        hourly_parser: BaseParser,
-        ftp: Optional[FTPUtil] = None,
-        avoid_update: bool = True,
-        post_proc: Optional[Callable] = None,
-    ):
-        super().__init__(
-            datatype=datatype,
-            root=root,
-            filename_fn=DailyWRFParser._filename_fn,
-            foldername_fn=DailyWRFParser._foldername_fn,
-            date_freq=DateFrequency.DAILY,
-            ftp=ftp,
-            avoid_update=avoid_update,
-            mirror_folder=True,
-            post_proc=post_proc,
-        )
-
-        self.hourly_parser = hourly_parser
-
-        if ftp is not None:
-            self.hourly_parser.ftp = ftp
-
-    def download_file(
-        self,
-        date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        ref_date: Union[str, datetime],
-    ):
-        """Actually this function performs as accum_monthly_rain"""
-        # accumulate the daily forecast
-        return self.accum_daily_forecast(
-            date=date, local_folder=local_folder, force_download=True, ref_date=ref_date
-        )
-
-    def accum_daily_forecast(
-        self,
-        date: Union[str, datetime],
-        ref_date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        force_download: bool = False,
-    ):
-        """Docstring"""
-
-        ### create a CUBE with the hourly forecast in the given date
-        # get the hourly dates to process
-        date = DateProcessor.parse_date(date).replace(hour=12, minute=0, second=0)
-
-        files = self.hourly_parser.get_range(
-            start_date=date - timedelta(hours=23),
-            end_date=date,
-            local_folder=local_folder,
-            force_download=force_download,
-            ref_date=ref_date,
-        )
-
-        # create the cube and get the correct variable
-        cube = GISUtil.create_cube(files=files, dim_key="time")
-        if self.hourly_parser.post_proc:
-            cube = self.hourly_parser.post_proc(cube)
-
-        accum = cube[self.hourly_parser.varname].sum(dim="time")
-        accum = accum.rename(self.datatype.value["var"])  # type: ignore
-
-        # once the reduction is being done in the time dimension, create a new dimension for time
-        accum = accum.assign_coords({"time": date}).expand_dims(dim="time")
-
-        # save the file to disk
-        target_file = self.local_target(
-            date=date, local_folder=local_folder, ref_date=ref_date
-        )
-        dset = accum.to_dataset()
-
-        # update the creation date for this file
-        dset.attrs["updated"] = str(datetime.now())
-
-        dset.to_netcdf(target_file)
-
-        # return self.local_path(date=date)
-        return target_file
-
-
-class INPEParsers:
-    """Just a structure to store the parsers for the INPE FTP"""
-
-    FTPurl = "ftp.cptec.inpe.br"
-
-    daily_rain_parser = BaseParser(
-        datatype=INPETypes.DAILY_RAIN,
-        root="/modelos/tempo/MERGE/GPM/DAILY/",
-        filename_fn=INPE.MERGE_filename,
-        foldername_fn=INPE.MERGE_structure,
-        post_proc=INPE.grib2_post_proc,
-    )
-
-    monthly_accum_yearly = BaseParser(
-        datatype=INPETypes.MONTHLY_ACCUM_YEARLY,
-        root="modelos/tempo/MERGE/GPM/CLIMATOLOGY/MONTHLY_ACCUMULATED_YEARLY/",
-        filename_fn=INPE.MERGE_MAY_filename,
-        date_freq=DateFrequency.MONTHLY,
-        post_proc=INPE.nc_post_proc,
-    )
-
-    daily_average = BaseParser(
-        datatype=INPETypes.DAILY_AVERAGE,
-        root="/modelos/tempo/MERGE/GPM/CLIMATOLOGY/DAILY_AVERAGE",
-        filename_fn=INPE.MERGE_DA_filename,
-        date_freq=DateFrequency.DAILY,
-        post_proc=INPE.nc_post_proc,
-    )
-
-    monthly_accum = BaseParser(
-        datatype=INPETypes.MONTHLY_ACCUM,
-        root="/modelos/tempo/MERGE/GPM/CLIMATOLOGY/MONTHLY_ACCUMULATED/",
-        filename_fn=INPE.MERGE_MA_filename,
-        date_freq=DateFrequency.MONTHLY,
-        post_proc=INPE.nc_post_proc,
-    )
-
-    month_accum_manual = MonthAccumParser(
-        datatype=INPETypes.MONTHLY_ACCUM_MANUAL,
-        fn_creator=INPE.MERGE_MAY_filename,
-        date_freq=DateFrequency.MONTHLY,
-        daily_parser=daily_rain_parser,
-    )
-
-    year_accum = BaseParser(
-        datatype=INPETypes.YEARLY_ACCUM,
-        root="/modelos/tempo/MERGE/GPM/CLIMATOLOGY/YEAR_ACCUMULATED",
-        filename_fn=INPE.MERGE_YA_filename,
-        date_freq=DateFrequency.YEARLY,
-        post_proc=INPE.yearly_post_proc,
-    )
-
-    hourly_wrf = HourlyWRFParser(
-        datatype=INPETypes.HOURLY_WRF,
-        root="/modelos/tempo/WRF/ams_07km/recortes/prec/",
-        filename_fn=INPE.WRF_filename,
-        foldername_fn=INPE.WRF_foldername,
-        mirror_folder=True,
-        date_freq=DateFrequency.HOURLY,
-        post_proc=lambda x, **_: x.rio.write_crs("epsg:4326"),
-    )
-
-    daily_wrf = DailyWRFParser(
-        datatype=INPETypes.DAILY_WRF,
-        root="/modelos/tempo/WRF/ams_07km/recortes/prec/",
-        hourly_parser=hourly_wrf,
-        post_proc=lambda x, **_: x.rio.write_crs("epsg:4326"),
-    )
-
-    parsers = [
-        daily_rain_parser,
-        monthly_accum_yearly,
-        daily_average,
-        monthly_accum,
-        month_accum_manual,
-        year_accum,
-        hourly_wrf,
-        daily_wrf,
-    ]
-
-    # post_processors = {".grib2": INPE.grib2_post_proc, ".nc": INPE.nc_post_proc}
+"""
+Module with specialized classes to understand the INPE FTP Structure
+The idea is to have several classes that implement the following interface:
+remote_file_path(date: str)
+"""
+import os
+
+# from abc import ABC, abstractmethod
+from enum import Enum, auto
+from pathlib import Path
+from typing import Callable, Optional, Union, List
+
+import calendar
+from datetime import datetime, timedelta
+from dateutil.relativedelta import relativedelta
+
+import matplotlib.colors as colors
+
+import xarray as xr
+
+from .parser import BaseParser
+from .utils import DateProcessor, FTPUtil, GISUtil, OSUtil, INPETypes
+from .enums import DateFrequency, INPETypes
+
+
+class INPE:
+    """Create the structure, given a root path (remote or local) and date/time of the file"""
+
+    # DailyMERGEroot = "/modelos/tempo/MERGE/GPM/DAILY"
+
+    # Define the colors and positions of the color stops
+    cmap_colors = [(1.0, 1.0, 1.0), (1, 1, 1.0), (0.5, 0.5, 1.0), (1.0, 0.4, 0.6)]
+    positions = [0.0, 0.1, 0.7, 1.0]
+
+    # Create the colormap using LinearSegmentedColormap
+    cmap = colors.LinearSegmentedColormap.from_list(
+        "my_colormap", list(zip(positions, cmap_colors))
+    )
+
+    def __init__(self, root_path: str) -> None:
+        self.root = os.path.normpath(root_path)
+
+    @staticmethod
+    def MERGE_structure(date: datetime) -> str:  # pylint: disable=invalid-name
+        """Given a date that can be parsed by dateutil, create the structure of the MERGE files"""
+        year = str(date.year)
+        month = str(date.month).zfill(2)
+        return "/".join([year, month])
+
+    @staticmethod
+    def MERGE_filename(date: datetime) -> str:  # pylint: disable=invalid-name
+        """Create the filename of the MERGE file, given a specific date"""
+        date_str = DateProcessor.normalize_date(date)
+        return f"MERGE_CPTEC_{date_str}.grib2"
+
+    @staticmethod
+    def MERGE_MAY_filename(date: datetime) -> str:  # pylint: disable=invalid-name
+        """
+        Monthly Accumulated Yearly:
+        Create the filename of the MERGE file, given a specific date
+        """
+        month_year = DateProcessor.month_abrev(date) + "_" + str(date.year)
+        return f"MERGE_CPTEC_acum_{month_year}.nc"
+
+    @staticmethod
+    def MERGE_DA_filename(date: datetime) -> str:  # pylint: disable=invalid-name
+        """
+        Daily Average
+        Create the filename of the MERGE file, given a specific date
+        """
+        day_month = f"{date.day:02d}{DateProcessor.month_abrev(date)}"
+        return f"MERGE_CPTEC_12Z{day_month}.nc"
+
+    @staticmethod
+    def MERGE_MA_filename(date: datetime) -> str:  # pylint: disable=invalid-name
+        """
+        Monthly Accumulated - Create the filename fot the Monthly Accumulated files from MERGE/INPE
+        E.g.: MERGE_CPTEC_acum_sep.nc
+        """
+        month_abrev = DateProcessor.month_abrev(date)
+        return f"MERGE_CPTEC_acum_{month_abrev}.nc"
+
+    @staticmethod
+    def MERGE_YA_filename(date: datetime) -> str:  # pylint: disable=invalid-name
+        """
+        Yearly Accumulated - Create the filename fot the Yearly Accumulated files from MERGE/INPE
+            E.g.: MERGE_CPTEC_acum_2003.nc
+        """
+        return f"MERGE_CPTEC_acum_{date.year}.nc"
+
+    @staticmethod
+    def yearly_post_proc(dset: xr.Dataset, date_str, **_) -> xr.Dataset:
+        """Adjust the time for the dataset"""
+
+        # first, perform the same adjust for all NCs
+        dset = INPE.nc_post_proc(dset)
+
+        date = DateProcessor.parse_date(date_str)
+        # fix month and day as 1
+        date = date + relativedelta(day=1, month=1)
+
+        return dset.assign_coords({"time": [date]})
+
+    @staticmethod
+    def grib2_post_proc(dset: xr.Dataset, **_) -> xr.Dataset:
+        """Adjust the longitude in INPE's grib2 files and sets the CRS"""
+
+        dset = dset.assign_coords({"longitude": dset.longitude - 360})
+        dset = dset.rio.write_crs("epsg:4326")
+        return dset
+
+    @staticmethod
+    def nc_post_proc(dset: xr.Dataset, **_) -> xr.Dataset:
+        """Adjust variable names in the netCDF files and set CRS"""
+        if "lon" in dset.dims:
+            dset = dset.rename_dims({"lon": "longitude", "lat": "latitude"})
+            dset = dset.rename_vars({"lon": "longitude", "lat": "latitude"})
+
+        dset = dset.rio.write_crs("epsg:4326")
+
+        return dset
+
+    @staticmethod
+    def WRF_foldername(date: datetime, **kwargs) -> str:  # pylint: disable=invalid-name
+        """
+        Given a date that can be parsed by dateutil, create the structure of the WRF files
+        E.g., 2023/05/22/00
+        """
+        date = DateProcessor.parse_date(kwargs["ref_date"])
+        year = str(date.year)
+        month = str(date.month).zfill(2)
+        day = str(date.day).zfill(2)
+
+        return "/".join([year, month, day, "00"])
+
+    @staticmethod
+    def WRF_filename(  # pylint: disable=invalid-name
+        date: datetime, ref_date: Union[str, datetime]
+    ) -> str:
+        """
+        WRF Hourly Filename - Create the filename fot the Hourly Forecast from WRF/INPE
+            E.g.: WRF_cpt_07KM_2023052200_2023052312.grib2
+        """
+        date1 = DateProcessor.normalize_date(ref_date) + "00"
+
+        date2 = DateProcessor.parse_date(date)
+        date2 = DateProcessor.pretty_date(date2, "%Y%m%d%H")
+        return f"WRF_cpt_07KM_{date1}_{date2}.grib2"
+
+
+class MonthAccumParser(BaseParser):
+    """Docstring"""
+
+    def __init__(
+        self,
+        datatype: Union[Enum, str],
+        fn_creator: Callable,
+        daily_parser: BaseParser,
+        fl_creator: Optional[Callable] = None,
+        date_freq: DateFrequency = DateFrequency.DAILY,
+        ftp: Optional[FTPUtil] = None,
+        avoid_update: bool = True,
+    ):
+        super().__init__(
+            datatype=datatype,
+            root="",
+            filename_fn=fn_creator,
+            foldername_fn=fl_creator,
+            date_freq=date_freq,
+            ftp=ftp,
+            avoid_update=avoid_update,
+        )
+
+        self.daily_parser = daily_parser
+
+    def download_file(self, date: Union[str, datetime], local_folder: Union[str, Path]):
+        """Actually this function performs as accum_monthly_rain"""
+        # accumulate the daily rain
+        return self.accum_monthly_rain(
+            date=date, local_folder=local_folder, force_download=True
+        )
+
+    def accum_monthly_rain(
+        self,
+        date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        force_download: bool,
+    ) -> Path:
+        """Docstring"""
+
+        # create a cube with the daily rain in the given month
+        start_date, end_date = DateProcessor.start_end_dates(date=date)
+
+        # here, we will check for the current month
+        now = datetime.now()
+        today = datetime(now.year, now.month, now.day)
+
+        if DateProcessor.parse_date(end_date) >= today:
+            # if the end date is future, it meansn we are trying to get the current month
+            # in this case, let's start going backwards to see the last available file in the FTP
+            for day in range(today.day, 0, -1):
+                end_date = today + relativedelta(day=day)
+                remote_file = self.daily_parser.remote_target(
+                    DateProcessor.normalize_date(end_date)
+                )
+
+                # if the file exists, then we have our end date
+                if self.ftp.file_exists(remote_file):
+                    break
+
+                # otherwise, raise exception if we reached the first day
+                if day == 1:
+                    raise Exception(f"No avilable file to calculate month {date}")
+
+        end_date = DateProcessor.normalize_date(end_date)
+
+        daily_files = self.daily_parser.get_range(
+            start_date=start_date,
+            end_date=end_date,
+            local_folder=local_folder,
+            force_download=force_download,
+        )
+
+        dset = GISUtil.create_cube(files=daily_files, dim_key="time")
+        cube = INPE.grib2_post_proc(dset)
+
+        # get the reference datetime
+        ref_time = cube.time[0].values
+
+        accum = cube[INPETypes.DAILY_RAIN.value["var"]].sum(dim="time")
+        accum = accum.rename(INPETypes.MONTHLY_ACCUM_MANUAL.value["var"])
+
+        # once the reduction is being done in the time dimension, create a new dimension for time
+        accum = accum.assign_coords({"time": ref_time}).expand_dims(dim="time")
+
+        # save the file to disk
+        target_file = self.local_target(date=date, local_folder=local_folder)
+        dset = accum.to_dataset()
+
+        # update the creation date for this file
+        dset.attrs["updated"] = str(now)
+        dset.attrs["last_day"] = end_date
+        dset.attrs["days"] = len(daily_files)
+
+        dset.to_netcdf(target_file)
+
+        return target_file
+
+    def get_file(
+        self,
+        date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        force_download: bool = False,
+    ) -> Path:
+        """
+        Get a specific file. If it is not available locally, download it just in time.
+        If it is available locally and avoid_update is not True, check if the file has
+        changed in the server
+        """
+
+        must_update = False
+        dset = None
+        local_target = self.local_target(date=date, local_folder=local_folder)
+
+        self.logger.debug("Getting file %s", local_target.name)
+
+        # first check verifies if the file exists and has the new attributes
+        if not local_target.exists() or force_download:
+            must_update = True
+
+        else:
+            # the file exists, try to open it and check if it is updated
+            try:
+                dset = xr.open_dataset(local_target)
+
+                if (
+                    ("updated" not in dset.attrs)
+                    or ("days" not in dset.attrs)
+                    or ("last_day" not in dset.attrs)
+                ):
+                    self.logger.debug(
+                        "Forcing update for date %s to add the new attributes ", date
+                    )
+                    must_update = True
+
+            except Exception as error:
+                self.logger.error(error)
+                must_update = True
+
+        # now, we have to decide if the file must be updated
+        if dset is not None and not must_update:
+            # first, let's get the dates from the file
+            date = DateProcessor.parse_date(date)
+            now = datetime.now()
+            last_day = DateProcessor.parse_date(dset.attrs["last_day"])
+            updated = DateProcessor.parse_date(dset.attrs["updated"])
+
+            # if file was updated in the last 30 min, return it regardless anything.
+            update_delta = now - updated
+            if update_delta.seconds < (30 * 60):
+                return local_target
+
+            # check if it is complete (has all the necessary days)
+            if (date.year == now.year) and (date.month == now.month):
+                ref_days = now.day
+            else:
+                _, ref_days = calendar.monthrange(date.year, date.month)
+
+            if dset.attrs["days"] != ref_days:
+                self.logger.debug(
+                    "File was created with %s days, expected: %s days",
+                    dset.attrs["days"],
+                    ref_days,
+                )
+                must_update = True
+
+            else:
+                # now, let's check how far are the days in the past
+                timedelta = now - last_day
+                if timedelta.days < 30:
+                    # file references nearby dates, let's check if it was updated recently
+                    self.logger.debug("Month within 30 days limit.")
+
+                    if update_delta.seconds > (2 * 60 * 60):
+                        # last update was more than 2 hours ago
+                        self.logger.debug(
+                            "Last file update was %s. Forcing new update.", updated
+                        )
+                        must_update = True
+                    else:
+                        self.logger.debug("File updated recently (%s)", updated)
+
+                else:
+                    self.logger.debug(
+                        "Monthly file refers to old files. Not necessary to update."
+                    )
+
+        # close the dataset
+        if dset is not None:
+            dset.close()
+
+        if must_update:
+            # store the old avoid update status
+            avoid_update = self.daily_parser.avoid_update
+            self.daily_parser.avoid_update = True  # False
+
+            file = self.accum_monthly_rain(
+                date=date,
+                local_folder=local_folder,
+                force_download=force_download,
+            )
+
+            # retrieve the avoid_update status
+            self.daily_parser.avoid_update = avoid_update
+            return file
+
+        return local_target
+
+        # must_update = False
+        # local_target = self.local_target(date=date, local_folder=local_folder)
+
+        # # if the file does not exist or we ask to download it again, we set the must_update flag
+        # # to True
+        # if not local_target.exists() or force_download:
+        #     must_update = True
+
+        # # otherwise we have to open the file and check update conditions
+        # else:
+        #     dset = xr.open_dataset(local_target)
+
+        #     ### Check attributes to conform the files to the new version
+        #     if (
+        #         ("updated" not in dset.attrs)
+        #         or ("days" not in dset.attrs)
+        #         or ("last_day" not in dset.attrs)
+        #     ):
+        #         self.logger.debug(
+        #             "Forcing update for date %s to add the new attributes ", date
+        #         )
+        #         must_update = True
+
+        #     else:
+        #         # get the dates from the file
+        #         date = DateProcessor.parse_date(date)
+        #         now = datetime.now()
+        #         last_day = DateProcessor.parse_date(dset.attrs["last_day"])
+        #         updated = DateProcessor.parse_date(dset.attrs["updated"])
+
+        #         # Now, let's treat separately if we are in the current month or not
+        #         if (date.year == now.year) and (date.month == now.month):
+        #             # if we are in the current month, check the last day used in the file
+        #             # force update if last update was more than 2 hour ago.
+        #             timedelta = now - updated
+        #             if (now.day >= last_day.day) or (timedelta.seconds > 2 * 60 * 60):
+        #                 self.logger.debug(
+        #                     "Last update was %s minutes ago", timedelta.seconds / 60
+        #                 )
+        #                 if now.day >= last_day.day:
+        #                     self.logger.debug("Last_day %s < today", last_day)
+
+        #                 self.logger.debug("Forcing update")
+        #                 must_update = True
+
+        #             else:
+        #                 must_update = False
+
+        #         else:
+        #             # let's check if the file was updated with all the necessary days.
+        #             _, days = calendar.monthrange(date.year, date.month)
+
+        #             # update the file if the number of days differ or if the last day is recent??
+        #             if dset["days"] != days:
+        #                 self.logger.debug(
+        #                     "File was created with %s, expected: %s", dset["days"], days
+        #                 )
+        #                 must_update = True
+
+        # if must_update:
+        #     # store the old avoid update status
+        #     avoid_update = self.daily_parser.avoid_update
+        #     self.daily_parser.avoid_update = True  # False
+
+        #     file = self.accum_monthly_rain(
+        #         date=date,
+        #         local_folder=local_folder,
+        #         force_download=force_download,
+        #     )
+
+        #     # retrieve the avoid_update status
+        #     self.daily_parser.avoid_update = avoid_update
+        #     return file
+
+        # else:
+        #     return local_target
+
+        # # we will force the accum_monthly rain if the month is the current month
+        # date = DateProcessor.parse_date(date) + relativedelta(day=1)
+
+        # now = datetime.now() + relativedelta(
+        #     day=1, hour=0, minute=0, second=0, microsecond=0
+        # )
+
+        # # check if we are in the same month... if that's the case, force the parsers to check if the files
+        # # were updated in the server
+        # if now == date or force_download or not local_target.exists():
+        #     # store the old avoid update status
+        #     avoid_update = self.daily_parser.avoid_update
+        #     self.daily_parser.avoid_update = True  # False
+
+        #     file = self.accum_monthly_rain(
+        #         date=date,
+        #         local_folder=local_folder,
+        #         force_download=force_download,
+        #     )
+
+        #     # retrieve the avoid_update status
+        #     self.daily_parser.avoid_update = avoid_update
+
+        #     return file
+
+        # else:
+        #     return local_target
+
+
+class HourlyWRFParser(BaseParser):
+    """Docstring"""
+
+    def download_file(
+        self,
+        date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        ref_date: Union[str, datetime],
+    ) -> Path:
+        """Instead of downloading a specific hour, we have to actually calculate it"""
+        # convert the date to datetime
+        date = DateProcessor.parse_date(date)
+
+        # download this specific date/hour
+        file1 = super().download_file(
+            date, local_folder=local_folder, ref_date=ref_date
+        )
+
+        # download the previous hour
+        prev_date = date - timedelta(hours=1)
+        tmp_folder = Path(local_folder) / "tmp"
+        if not tmp_folder.exists():
+            tmp_folder.mkdir(parents=True, exist_ok=True)
+        file2 = super().download_file(
+            prev_date, local_folder=tmp_folder, ref_date=ref_date
+        )
+
+        # open both files and subtract file1 - file2
+        dset1 = xr.open_dataset(file1)
+        dset2 = xr.open_dataset(file2)
+        dset = dset1 - dset2
+
+        # save the hourly rain to disk and delete the temporary
+        dset.attrs["updated"] = str(datetime.now())
+
+        dset = dset.rename_vars({"unknown": "hour_wrf"})
+        dset = dset.assign_coords({"longitude": dset.longitude - 360})
+        dset = dset.rio.write_crs("epsg:4326")
+
+        # close the datasets and clear the temp folder
+        dset.to_netcdf(file1)
+        # file1 = file1.with_suffix(".tif")
+        # dset.to_array().squeeze().rio.to_raster(file1)
+
+        dset1.close()
+        dset2.close()
+        OSUtil.clear_folder(tmp_folder)
+
+        return file1
+
+
+class DailyWRFParser(BaseParser):
+    """Docstring"""
+
+    @staticmethod
+    def _foldername_fn(_: datetime, **kwargs) -> str:
+        """Create a foldername for the local storage"""
+        return DateProcessor.normalize_date(kwargs["ref_date"])
+
+    @staticmethod
+    def _filename_fn(date: datetime, ref_date: Union[str, datetime]) -> str:
+        """Create the filename for local storage"""
+        date1 = DateProcessor.normalize_date(ref_date)
+        date2 = DateProcessor.normalize_date(date)
+        return f"WRF_{date1}_{date2}.grib2"
+
+    def __init__(
+        self,
+        datatype: Union[Enum, str],
+        root: str,
+        hourly_parser: BaseParser,
+        ftp: Optional[FTPUtil] = None,
+        avoid_update: bool = True,
+        post_proc: Optional[Callable] = None,
+    ):
+        super().__init__(
+            datatype=datatype,
+            root=root,
+            filename_fn=DailyWRFParser._filename_fn,
+            foldername_fn=DailyWRFParser._foldername_fn,
+            date_freq=DateFrequency.DAILY,
+            ftp=ftp,
+            avoid_update=avoid_update,
+            mirror_folder=True,
+            post_proc=post_proc,
+        )
+
+        self.hourly_parser = hourly_parser
+
+        if ftp is not None:
+            self.hourly_parser.ftp = ftp
+
+    def download_file(
+        self,
+        date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        ref_date: Union[str, datetime],
+    ):
+        """Actually this function performs as accum_monthly_rain"""
+        # accumulate the daily forecast
+        return self.accum_daily_forecast(
+            date=date, local_folder=local_folder, force_download=True, ref_date=ref_date
+        )
+
+    def accum_daily_forecast(
+        self,
+        date: Union[str, datetime],
+        ref_date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        force_download: bool = False,
+    ):
+        """Docstring"""
+
+        ### create a CUBE with the hourly forecast in the given date
+        # get the hourly dates to process
+        date = DateProcessor.parse_date(date).replace(hour=12, minute=0, second=0)
+
+        files = self.hourly_parser.get_range(
+            start_date=date - timedelta(hours=23),
+            end_date=date,
+            local_folder=local_folder,
+            force_download=force_download,
+            ref_date=ref_date,
+        )
+
+        # create the cube and get the correct variable
+        cube = GISUtil.create_cube(files=files, dim_key="time")
+        if self.hourly_parser.post_proc:
+            cube = self.hourly_parser.post_proc(cube)
+
+        accum = cube[self.hourly_parser.varname].sum(dim="time")
+        accum = accum.rename(self.datatype.value["var"])  # type: ignore
+
+        # once the reduction is being done in the time dimension, create a new dimension for time
+        accum = accum.assign_coords({"time": date}).expand_dims(dim="time")
+
+        # save the file to disk
+        target_file = self.local_target(
+            date=date, local_folder=local_folder, ref_date=ref_date
+        )
+        dset = accum.to_dataset()
+
+        # update the creation date for this file
+        dset.attrs["updated"] = str(datetime.now())
+
+        dset.to_netcdf(target_file)
+
+        # return self.local_path(date=date)
+        return target_file
+
+
+class INPEParsers:
+    """Just a structure to store the parsers for the INPE FTP"""
+
+    FTPurl = "ftp.cptec.inpe.br"
+
+    daily_rain_parser = BaseParser(
+        datatype=INPETypes.DAILY_RAIN,
+        root="/modelos/tempo/MERGE/GPM/DAILY/",
+        filename_fn=INPE.MERGE_filename,
+        foldername_fn=INPE.MERGE_structure,
+        post_proc=INPE.grib2_post_proc,
+    )
+
+    monthly_accum_yearly = BaseParser(
+        datatype=INPETypes.MONTHLY_ACCUM_YEARLY,
+        root="modelos/tempo/MERGE/GPM/CLIMATOLOGY/MONTHLY_ACCUMULATED_YEARLY/",
+        filename_fn=INPE.MERGE_MAY_filename,
+        date_freq=DateFrequency.MONTHLY,
+        post_proc=INPE.nc_post_proc,
+    )
+
+    daily_average = BaseParser(
+        datatype=INPETypes.DAILY_AVERAGE,
+        root="/modelos/tempo/MERGE/GPM/CLIMATOLOGY/DAILY_AVERAGE",
+        filename_fn=INPE.MERGE_DA_filename,
+        date_freq=DateFrequency.DAILY,
+        post_proc=INPE.nc_post_proc,
+    )
+
+    monthly_accum = BaseParser(
+        datatype=INPETypes.MONTHLY_ACCUM,
+        root="/modelos/tempo/MERGE/GPM/CLIMATOLOGY/MONTHLY_ACCUMULATED/",
+        filename_fn=INPE.MERGE_MA_filename,
+        date_freq=DateFrequency.MONTHLY,
+        post_proc=INPE.nc_post_proc,
+    )
+
+    month_accum_manual = MonthAccumParser(
+        datatype=INPETypes.MONTHLY_ACCUM_MANUAL,
+        fn_creator=INPE.MERGE_MAY_filename,
+        date_freq=DateFrequency.MONTHLY,
+        daily_parser=daily_rain_parser,
+    )
+
+    year_accum = BaseParser(
+        datatype=INPETypes.YEARLY_ACCUM,
+        root="/modelos/tempo/MERGE/GPM/CLIMATOLOGY/YEAR_ACCUMULATED",
+        filename_fn=INPE.MERGE_YA_filename,
+        date_freq=DateFrequency.YEARLY,
+        post_proc=INPE.yearly_post_proc,
+    )
+
+    hourly_wrf = HourlyWRFParser(
+        datatype=INPETypes.HOURLY_WRF,
+        root="/modelos/tempo/WRF/ams_07km/recortes/prec/",
+        filename_fn=INPE.WRF_filename,
+        foldername_fn=INPE.WRF_foldername,
+        mirror_folder=True,
+        date_freq=DateFrequency.HOURLY,
+        post_proc=lambda x, **_: x.rio.write_crs("epsg:4326"),
+    )
+
+    daily_wrf = DailyWRFParser(
+        datatype=INPETypes.DAILY_WRF,
+        root="/modelos/tempo/WRF/ams_07km/recortes/prec/",
+        hourly_parser=hourly_wrf,
+        post_proc=lambda x, **_: x.rio.write_crs("epsg:4326"),
+    )
+
+    parsers = [
+        daily_rain_parser,
+        monthly_accum_yearly,
+        daily_average,
+        monthly_accum,
+        month_accum_manual,
+        year_accum,
+        hourly_wrf,
+        daily_wrf,
+    ]
+
+    # post_processors = {".grib2": INPE.grib2_post_proc, ".nc": INPE.nc_post_proc}
```

### Comparing `merge-downloader-0.0.2/mergedownloader/parser.py` & `merge-downloader-0.0.3/mergedownloader/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,319 +1,318 @@
-"""
-The parser module defines the template of a Parser Class.
-"""
-
-# from abc import ABC, abstractmethod
-
-import os
-from pathlib import Path
-from enum import Enum
-from typing import Callable, Optional, Union, List, Iterable
-from datetime import datetime
-import logging
-
-import xarray as xr
-
-from .utils import DateProcessor, DateFrequency, FTPUtil, OSUtil
-
-
-class BaseParser:
-    """
-    This class implements a Base Parser that is responsible for getting to the
-    desired file and downloading it. For that, we should provide:
-
-    datatype: To which type this data refers to. This can be a string (e.g., 'MonthlyAverage')
-    root: The root folder in the FTP that stores this data (e.g., /modelos/tempo/MERGE/GPM/CLIMATOLOGY/MONTHLY_AVERAGE/)
-    fn_creator: This is the FileName creator. This function is responsible for getting a datetime
-                and providing the target filename, for example: MERGE_CPTEC_mean_apr.nc
-    fl_creator: This is the Folder creator. This funciton is responsible for getting a date string
-                and providing the target folder, when it has sub-structures, for example:
-                '/DAILY/2001/02/' in the case of Daily rain
-    date_freq: The frequency of the file. DateFrequency.[DAILY, MONTHLY, YEARLY]
-    mirror_folder: If True, reproduces the same folder structure locally
-    """
-
-    def __init__(
-        self,
-        datatype: Union[Enum, str],
-        root: str,
-        filename_fn: Callable,
-        foldername_fn: Optional[Callable] = None,
-        date_freq: DateFrequency = DateFrequency.DAILY,
-        ftp: Optional[FTPUtil] = None,
-        avoid_update: bool = True,
-        post_proc: Optional[Callable] = None,
-        mirror_folder: bool = False,
-    ):
-        self.datatype = datatype
-        self.root = Path(root).as_posix()
-        self.filename_fn = filename_fn
-        self.foldername_fn = foldername_fn
-        self.date_freq = date_freq
-        self._ftp = ftp
-        self.avoid_update = avoid_update
-        self.post_proc = post_proc
-        self.mirror_folder = mirror_folder
-        self.logger = logging.getLogger(str(datatype))
-
-    @property
-    def ftp(self):
-        """Retrieve the internal ftp object"""
-        if self._ftp is None:
-            raise ValueError(
-                f"FTPUtil instance not initialized in the parser {self.datatype}. \nSet it in .ftp."
-            )
-        else:
-            return self._ftp
-
-    @property
-    def varname(self) -> str:
-        """Return the variable name that comes inside the file"""
-        if isinstance(self.datatype, str):
-            return self.datatype
-        else:
-            return self.datatype.value["var"]
-
-    @ftp.setter
-    def ftp(self, ftp: FTPUtil):
-        """Set internal ftp object"""
-        self._ftp = ftp
-
-    @property
-    def subfolder(self) -> Path:
-        """Return the subfolder to place files based on the datatype"""
-
-        if isinstance(self.datatype, Enum):
-            subfolder = Path(self.datatype.name)
-        else:
-            subfolder = Path(self.datatype)
-
-        return subfolder
-
-    def clean_local_folder(self, local_folder: Union[str, Path]) -> None:
-        """Clear the .idx files in the local download folder"""
-
-        # get the local path
-        local_path = Path(local_folder) / self.subfolder
-
-        self.logger.debug("Cleaning folder: %s", local_path)
-
-        # get idx files
-        for file in local_path.rglob("*.idx"):
-            file.unlink()
-
-    ### File/folder structure functions
-    def filename(self, date: Union[str, datetime], **kwargs) -> str:
-        """Return just the filename given a date string"""
-        # get the datetime
-        date = DateProcessor.parse_date(date)
-
-        return self.filename_fn(date, **kwargs)
-
-    def local_path(
-        self,
-        local_folder: Union[Path, str],
-        date: Optional[Union[str, datetime]] = None,
-        **kwargs,
-    ) -> Path:
-        """Create the local path based on the data type"""
-
-        # create the local path (raises exception if local_folder does not exists)
-        local_path = Path(local_folder) / self.subfolder
-
-        if self.mirror_folder and date is not None:
-            # extract the folder
-            remote_folder = Path(self.remote_path(date=date, **kwargs)).relative_to(
-                self.root
-            )
-            local_path /= remote_folder
-
-        local_path.mkdir(parents=True, exist_ok=True)
-        return local_path
-
-    def local_target(
-        self, date: Union[str, datetime], local_folder: Union[Path, str], **kwargs
-    ) -> Path:
-        """
-        Local target is the full path of the local file, given a date_str
-        """
-        return self.local_path(
-            local_folder=local_folder, date=date, **kwargs
-        ) / self.filename(date, **kwargs)
-
-    def remote_path(self, date: Union[str, datetime], **kwargs) -> str:
-        """Return just the base path given a date string"""
-        # get the datetime
-        date = DateProcessor.parse_date(date)
-
-        if self.foldername_fn:
-            return os.path.join(self.root, self.foldername_fn(date, **kwargs))
-        else:
-            return self.root
-
-    def remote_target(self, date: Union[str, datetime], **kwargs) -> str:
-        """Target is composed by root / folder / filename"""
-        return os.path.join(
-            self.remote_path(date, **kwargs), self.filename(date, **kwargs)
-        )
-
-    def dates_range(
-        self, start_date: Union[str, datetime], end_date: Union[str, datetime]
-    ) -> List[str]:
-        """Return the dates range within the specified period"""
-        return DateProcessor.dates_range(
-            start_date=start_date, end_date=end_date, date_freq=self.date_freq
-        )
-
-    ### Download functions
-    def download_file(
-        self, date: Union[str, datetime], local_folder: Union[Path, str], **kwargs
-    ) -> Path:
-        """
-        Download the parsed file to a local subfolder (according to the parser datatype).
-        OBS: Download file always force the download. Otherwise, use the `get_file` function
-        """
-
-        remote_target = self.remote_target(date=date, **kwargs)
-        self.logger.info("Downloading file %s", remote_target)
-
-        # Download the file directly
-        downloaded_file = self.ftp.download_ftp_file(
-            remote_file=remote_target,
-            local_folder=self.local_path(
-                date=date, local_folder=local_folder, **kwargs
-            ),
-        )
-
-        return downloaded_file
-
-    def is_downloaded(
-        self, date: Union[str, datetime], local_folder: Union[str, Path], **kwargs
-    ) -> bool:
-        """Compare remote and local files and return if they are equal"""
-
-        # create target to the local file
-        local_target = self.local_target(date=date, local_folder=local_folder, **kwargs)
-
-        self.logger.debug("Checking if %s exists", local_target)
-
-        # if the file does not exist, exit with false
-        if not local_target.exists():
-            self.logger.debug("File %s does not exist", local_target)
-            return False
-
-        # if it exists locally and avoid update is True, we can confirm it is already downloaded
-        if self.avoid_update:
-            self.logger.debug("File %s exists, and avoiding its update", local_target)
-            return True
-
-        ### Check if file has changed in the server
-        # create a string pointing to the remote file and get its info
-        remote_file = self.remote_target(date)
-
-        # Now we need to compare the remote and local files
-        local_info = OSUtil.get_local_file_info(local_target)
-
-        changed = self.ftp.file_changed(remote_file=remote_file, file_info=local_info)
-
-        self.logger.debug(
-            "File %s has %s on the server", local_target.name, "" if changed else "NOT"
-        )
-
-        return False if changed else True
-
-    def get_file(
-        self,
-        date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        force_download: bool = False,
-        **kwargs,
-    ) -> Path:
-        """
-        Get a specific file. If it is not available locally, download it just in time.
-        If it is available locally and avoid_update is not True, check if the file has
-        changed in the server
-        """
-        self.logger.info(
-            "Getting %s/%s", self.datatype, DateProcessor.pretty_date(date)
-        )
-
-        if force_download or not self.is_downloaded(
-            date=date, local_folder=local_folder, **kwargs
-        ):
-            return self.download_file(date=date, local_folder=local_folder, **kwargs)
-
-        else:
-            return self.local_target(date=date, local_folder=local_folder, **kwargs)
-
-    def open_file(
-        self,
-        date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        force_download: bool = False,
-        **kwargs,
-    ) -> xr.Dataset:
-        """
-        Open a file and process it using the processor.
-        """
-
-        file = self.get_file(date, local_folder, force_download, **kwargs)
-        dset = xr.open_dataset(file)
-
-        if self.post_proc:
-            return self.post_proc(dset)
-        else:
-            return dset
-
-    def get_files(
-        self,
-        dates: Iterable[Union[str, datetime]],
-        local_folder: Union[str, Path],
-        force_download: bool = False,
-        **kwargs,
-    ) -> List[Path]:
-        """
-        Download files from a list of dates and receives a list pointing to the files.
-        If there is a problem during the download of one file, a message error will be in the list.
-        """
-        files = []
-        for date in dates:
-            files.append(
-                self.get_file(
-                    date=date,
-                    local_folder=local_folder,
-                    force_download=force_download,
-                    **kwargs,
-                )
-            )
-
-        return files
-
-    def get_range(
-        self,
-        start_date: Union[str, datetime],
-        end_date: Union[str, datetime],
-        local_folder: Union[str, Path],
-        force_download: bool = False,
-        **kwargs,
-    ) -> List[Path]:
-        """
-        Download a range of files from start to end dates and receives a list pointing to the files.
-        If there is a problem during the download of one file, a message error will be in the list.
-        """
-        dates = self.dates_range(start_date, end_date)
-
-        return self.get_files(
-            dates=dates,
-            local_folder=local_folder,
-            force_download=force_download,
-            **kwargs,
-        )
-
-    def __repr__(self):
-        """String representation for the parser"""
-        if isinstance(self.datatype, Enum):
-            str_dtype = self.datatype.name
-        else:
-            str_dtype = self.datatype
-        s = f"Parser instance: {str_dtype}"
-        return s
+"""
+The parser module defines the template of a Parser Class.
+"""
+
+# from abc import ABC, abstractmethod
+
+import os
+from pathlib import Path
+from enum import Enum
+from typing import Callable, Optional, Union, List, Iterable
+from datetime import datetime
+import logging
+
+import xarray as xr
+
+from .utils import DateProcessor, DateFrequency, FTPUtil, OSUtil
+
+
+class BaseParser:
+    """
+    This class implements a Base Parser that is responsible for getting to the
+    desired file and downloading it. For that, we should provide:
+
+    datatype: To which type this data refers to. This can be a string (e.g., 'MonthlyAverage')
+    root: The root folder in the FTP that stores this data (e.g., /modelos/tempo/MERGE/GPM/CLIMATOLOGY/MONTHLY_AVERAGE/)
+    fn_creator: This is the FileName creator. This function is responsible for getting a datetime
+                and providing the target filename, for example: MERGE_CPTEC_mean_apr.nc
+    fl_creator: This is the Folder creator. This funciton is responsible for getting a date string
+                and providing the target folder, when it has sub-structures, for example:
+                '/DAILY/2001/02/' in the case of Daily rain
+    date_freq: The frequency of the file. DateFrequency.[DAILY, MONTHLY, YEARLY]
+    mirror_folder: If True, reproduces the same folder structure locally
+    """
+
+    def __init__(
+        self,
+        datatype: Union[Enum, str],
+        root: str,
+        filename_fn: Callable,
+        foldername_fn: Optional[Callable] = None,
+        date_freq: DateFrequency = DateFrequency.DAILY,
+        ftp: Optional[FTPUtil] = None,
+        avoid_update: bool = True,
+        post_proc: Optional[Callable] = None,
+        mirror_folder: bool = False,
+    ):
+        self.datatype = datatype
+        self.root = Path(root).as_posix()
+        self.filename_fn = filename_fn
+        self.foldername_fn = foldername_fn
+        self.date_freq = date_freq
+        self._ftp = ftp
+        self.avoid_update = avoid_update
+        self.post_proc = post_proc
+        self.mirror_folder = mirror_folder
+        self.logger = logging.getLogger(str(datatype))
+
+    @property
+    def ftp(self):
+        """Retrieve the internal ftp object"""
+        if self._ftp is None:
+            raise ValueError(
+                f"FTPUtil instance not initialized in the parser {self.datatype}. \nSet it in .ftp."
+            )
+        else:
+            return self._ftp
+
+    @property
+    def varname(self) -> str:
+        """Return the variable name that comes inside the file"""
+        if isinstance(self.datatype, str):
+            return self.datatype
+        else:
+            return self.datatype.value["var"]
+
+    @ftp.setter
+    def ftp(self, ftp: FTPUtil):
+        """Set internal ftp object"""
+        self._ftp = ftp
+
+    @property
+    def subfolder(self) -> Path:
+        """Return the subfolder to place files based on the datatype"""
+
+        if isinstance(self.datatype, Enum):
+            subfolder = Path(self.datatype.name)
+        else:
+            subfolder = Path(self.datatype)
+
+        return subfolder
+
+    def clean_local_folder(self, local_folder: Union[str, Path]) -> None:
+        """Clear the .idx files in the local download folder"""
+
+        # get the local path
+        local_path = Path(local_folder) / self.subfolder
+
+        self.logger.debug("Cleaning folder: %s", local_path)
+
+        # get idx files
+        for file in local_path.rglob("*.idx"):
+            file.unlink()
+
+    ### File/folder structure functions
+    def filename(self, date: Union[str, datetime], **kwargs) -> str:
+        """Return just the filename given a date string"""
+        # get the datetime
+        date = DateProcessor.parse_date(date)
+
+        return self.filename_fn(date, **kwargs)
+
+    def local_path(
+        self,
+        local_folder: Union[Path, str],
+        date: Optional[Union[str, datetime]] = None,
+        **kwargs,
+    ) -> Path:
+        """Create the local path based on the data type"""
+
+        # create the local path (raises exception if local_folder does not exists)
+        local_path = Path(local_folder) / self.subfolder
+
+        if self.mirror_folder and date is not None:
+            # extract the folder
+            remote_folder = Path(self.remote_path(date=date, **kwargs)).relative_to(
+                self.root
+            )
+            local_path /= remote_folder
+
+        local_path.mkdir(parents=True, exist_ok=True)
+        return local_path
+
+    def local_target(
+        self, date: Union[str, datetime], local_folder: Union[Path, str], **kwargs
+    ) -> Path:
+        """
+        Local target is the full path of the local file, given a date_str
+        """
+        return self.local_path(
+            local_folder=local_folder, date=date, **kwargs
+        ) / self.filename(date, **kwargs)
+
+    def remote_path(self, date: Union[str, datetime], **kwargs) -> str:
+        """Return just the base path given a date string"""
+        # get the datetime
+        date = DateProcessor.parse_date(date)
+
+        if self.foldername_fn:
+            return '/'.join([self.root, self.foldername_fn(date, **kwargs)])
+            # return os.path.join(self.root, self.foldername_fn(date, **kwargs))
+        else:
+            return self.root
+
+    def remote_target(self, date: Union[str, datetime], **kwargs) -> str:
+        """Target is composed by root / folder / filename"""
+        return '/'.join([self.remote_path(date, **kwargs), self.filename(date, **kwargs)])
+
+    def dates_range(
+        self, start_date: Union[str, datetime], end_date: Union[str, datetime]
+    ) -> List[str]:
+        """Return the dates range within the specified period"""
+        return DateProcessor.dates_range(
+            start_date=start_date, end_date=end_date, date_freq=self.date_freq
+        )
+
+    ### Download functions
+    def download_file(
+        self, date: Union[str, datetime], local_folder: Union[Path, str], **kwargs
+    ) -> Path:
+        """
+        Download the parsed file to a local subfolder (according to the parser datatype).
+        OBS: Download file always force the download. Otherwise, use the `get_file` function
+        """
+
+        remote_target = self.remote_target(date=date, **kwargs)
+        self.logger.info("Downloading file %s", remote_target)
+
+        # Download the file directly
+        downloaded_file = self.ftp.download_ftp_file(
+            remote_file=remote_target,
+            local_folder=self.local_path(
+                date=date, local_folder=local_folder, **kwargs
+            ),
+        )
+
+        return downloaded_file
+
+    def is_downloaded(
+        self, date: Union[str, datetime], local_folder: Union[str, Path], **kwargs
+    ) -> bool:
+        """Compare remote and local files and return if they are equal"""
+
+        # create target to the local file
+        local_target = self.local_target(date=date, local_folder=local_folder, **kwargs)
+
+        self.logger.debug("Checking if %s exists", local_target)
+
+        # if the file does not exist, exit with false
+        if not local_target.exists():
+            self.logger.debug("File %s does not exist", local_target)
+            return False
+
+        # if it exists locally and avoid update is True, we can confirm it is already downloaded
+        if self.avoid_update:
+            self.logger.debug("File %s exists, and avoiding its update", local_target)
+            return True
+
+        ### Check if file has changed in the server
+        # create a string pointing to the remote file and get its info
+        remote_file = self.remote_target(date)
+
+        # Now we need to compare the remote and local files
+        local_info = OSUtil.get_local_file_info(local_target)
+
+        changed = self.ftp.file_changed(remote_file=remote_file, file_info=local_info)
+
+        self.logger.debug(
+            "File %s has %s on the server", local_target.name, "" if changed else "NOT"
+        )
+
+        return False if changed else True
+
+    def get_file(
+        self,
+        date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        force_download: bool = False,
+        **kwargs,
+    ) -> Path:
+        """
+        Get a specific file. If it is not available locally, download it just in time.
+        If it is available locally and avoid_update is not True, check if the file has
+        changed in the server
+        """
+        self.logger.info(
+            "Getting %s/%s", self.datatype, DateProcessor.pretty_date(date)
+        )
+
+        if force_download or not self.is_downloaded(
+            date=date, local_folder=local_folder, **kwargs
+        ):
+            return self.download_file(date=date, local_folder=local_folder, **kwargs)
+
+        else:
+            return self.local_target(date=date, local_folder=local_folder, **kwargs)
+
+    def open_file(
+        self,
+        date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        force_download: bool = False,
+        **kwargs,
+    ) -> xr.Dataset:
+        """
+        Open a file and process it using the processor.
+        """
+
+        file = self.get_file(date, local_folder, force_download, **kwargs)
+        dset = xr.open_dataset(file)
+
+        if self.post_proc:
+            return self.post_proc(dset)
+        else:
+            return dset
+
+    def get_files(
+        self,
+        dates: Iterable[Union[str, datetime]],
+        local_folder: Union[str, Path],
+        force_download: bool = False,
+        **kwargs,
+    ) -> List[Path]:
+        """
+        Download files from a list of dates and receives a list pointing to the files.
+        If there is a problem during the download of one file, a message error will be in the list.
+        """
+        files = []
+        for date in dates:
+            files.append(
+                self.get_file(
+                    date=date,
+                    local_folder=local_folder,
+                    force_download=force_download,
+                    **kwargs,
+                )
+            )
+
+        return files
+
+    def get_range(
+        self,
+        start_date: Union[str, datetime],
+        end_date: Union[str, datetime],
+        local_folder: Union[str, Path],
+        force_download: bool = False,
+        **kwargs,
+    ) -> List[Path]:
+        """
+        Download a range of files from start to end dates and receives a list pointing to the files.
+        If there is a problem during the download of one file, a message error will be in the list.
+        """
+        dates = self.dates_range(start_date, end_date)
+
+        return self.get_files(
+            dates=dates,
+            local_folder=local_folder,
+            force_download=force_download,
+            **kwargs,
+        )
+
+    def __repr__(self):
+        """String representation for the parser"""
+        if isinstance(self.datatype, Enum):
+            str_dtype = self.datatype.name
+        else:
+            str_dtype = self.datatype
+        s = f"Parser instance: {str_dtype}"
+        return s
```

