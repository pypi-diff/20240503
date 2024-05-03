# Comparing `tmp/pyFUME-0.3.1.tar.gz` & `tmp/pyfume-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFUME-0.3.1.tar", last modified: Tue Mar  5 17:08:53 2024, max compression
+gzip compressed data, was "pyfume-0.3.4.tar", last modified: Fri May  3 11:41:52 2024, max compression
```

## Comparing `pyFUME-0.3.1.tar` & `pyfume-0.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:08:53.495713 pyFUME-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-05 17:08:46.000000 pyFUME-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-03-05 17:08:53.495713 pyFUME-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-03-05 17:08:46.000000 pyFUME-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:08:53.495713 pyFUME-0.3.1/pyFUME.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-03-05 17:08:53.000000 pyFUME-0.3.1/pyFUME.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-05 17:08:53.000000 pyFUME-0.3.1/pyFUME.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 17:08:53.000000 pyFUME-0.3.1/pyFUME.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 17:08:53.000000 pyFUME-0.3.1/pyFUME.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-05 17:08:53.000000 pyFUME-0.3.1/pyFUME.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:08:53.495713 pyFUME-0.3.1/pyfume/
--rw-r--r--   0 runner    (1001) docker     (127)    34721 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/BuildTakagiSugeno.py
--rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/Clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/EstimateAntecendentSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/EstimateConsequentParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/FeatureSelection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/FireStrengthCalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/SimpfulModelBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/Splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/Tester.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/pyfume.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-03-05 17:08:46.000000 pyFUME-0.3.1/pyfume/simpfulfier.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 17:08:53.495713 pyFUME-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-05 17:08:46.000000 pyFUME-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:41:52.068058 pyfume-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-05-03 11:41:46.000000 pyfume-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-05-03 11:41:52.068058 pyfume-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-05-03 11:41:46.000000 pyfume-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:41:52.068058 pyfume-0.3.4/pyFUME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-05-03 11:41:52.000000 pyfume-0.3.4/pyFUME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-03 11:41:52.000000 pyfume-0.3.4/pyFUME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:41:52.000000 pyfume-0.3.4/pyFUME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 11:41:52.000000 pyfume-0.3.4/pyFUME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 11:41:52.000000 pyfume-0.3.4/pyFUME.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:41:52.068058 pyfume-0.3.4/pyfume/
+-rw-r--r--   0 runner    (1001) docker     (127)    35414 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/BuildTakagiSugeno.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26403 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/Clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18534 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/EstimateAntecendentSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/EstimateConsequentParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30409 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/FeatureSelection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/FireStrengthCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/SimpfulModelBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/Splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/Tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25043 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/pyfume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-03 11:41:46.000000 pyfume-0.3.4/pyfume/simpfulfier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:41:52.068058 pyfume-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 11:41:46.000000 pyfume-0.3.4/setup.py
```

### Comparing `pyFUME-0.3.1/LICENSE` & `pyfume-0.3.4/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
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
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
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
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
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
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
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
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `pyFUME-0.3.1/PKG-INFO` & `pyfume-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: pyFUME
-Version: 0.3.1
+Version: 0.3.4
 Summary: A Python package for fuzzy model estimation
 Home-page: https://github.com/CaroFuchs/pyFUME
 Author: Caro Fuchs
 Author-email: c.e.m.fuchs@tue.nl
 License: LICENSE.txt
 Keywords: fuzzy logic,fuzzy inference systems,fuzzy model,data-driven,model estimation,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: simpful
-Requires-Dist: fst-pso
-Requires-Dist: pandas
-Requires-Dist: typing_extensions
+Requires-Dist: scipy==1.10.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: simpful==2.12.0
+Requires-Dist: fst-pso==1.8.1
+Requires-Dist: pandas==1.5.3
 
 # pyFUME
 
 pyFUME is a Python package for automatic Fuzzy Models Estimation from data [1].
 pyFUME contains functions to estimate the antecedent sets and the consequent parameters of a Takagi-Sugeno fuzzy model directly from data. This information is then used to create an executable fuzzy model using the Simpful library.
 pyFUME also provides facilities for the evaluation of performance.
 For more information about pyFUME's functionalities, please check the [online documentation](https://pyfume.readthedocs.io/en/latest/).
```

### Comparing `pyFUME-0.3.1/README.md` & `pyfume-0.3.4/pyFUME.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: pyFUME
+Version: 0.3.4
+Summary: A Python package for fuzzy model estimation
+Home-page: https://github.com/CaroFuchs/pyFUME
+Author: Caro Fuchs
+Author-email: c.e.m.fuchs@tue.nl
+License: LICENSE.txt
+Keywords: fuzzy logic,fuzzy inference systems,fuzzy model,data-driven,model estimation,machine learning
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scipy==1.10.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: simpful==2.12.0
+Requires-Dist: fst-pso==1.8.1
+Requires-Dist: pandas==1.5.3
+
 # pyFUME
 
 pyFUME is a Python package for automatic Fuzzy Models Estimation from data [1].
 pyFUME contains functions to estimate the antecedent sets and the consequent parameters of a Takagi-Sugeno fuzzy model directly from data. This information is then used to create an executable fuzzy model using the Simpful library.
 pyFUME also provides facilities for the evaluation of performance.
 For more information about pyFUME's functionalities, please check the [online documentation](https://pyfume.readthedocs.io/en/latest/).
```

### Comparing `pyFUME-0.3.1/pyFUME.egg-info/PKG-INFO` & `pyfume-0.3.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,244 +1,222 @@
-Metadata-Version: 2.1
-Name: pyFUME
-Version: 0.3.1
-Summary: A Python package for fuzzy model estimation
-Home-page: https://github.com/CaroFuchs/pyFUME
-Author: Caro Fuchs
-Author-email: c.e.m.fuchs@tue.nl
-License: LICENSE.txt
-Keywords: fuzzy logic,fuzzy inference systems,fuzzy model,data-driven,model estimation,machine learning
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: simpful
-Requires-Dist: fst-pso
-Requires-Dist: pandas
-Requires-Dist: typing_extensions
-
-# pyFUME
-
-pyFUME is a Python package for automatic Fuzzy Models Estimation from data [1].
-pyFUME contains functions to estimate the antecedent sets and the consequent parameters of a Takagi-Sugeno fuzzy model directly from data. This information is then used to create an executable fuzzy model using the Simpful library.
-pyFUME also provides facilities for the evaluation of performance.
-For more information about pyFUME's functionalities, please check the [online documentation](https://pyfume.readthedocs.io/en/latest/).
-
-## Usage
-For the following example, we use the Concrete Compressive Strength data set [2] as can be found in the UCI repository.
-The  code  in  Example 1  is  simple  and  easy  to  use,  making it  ideal  to  use  for  practitioners  who  wish  to  use  the  default settings or only wish to use few non-default settings using additional input arguments (Example 2). 
-Users that wish to deviate from  the  default  settings  can  use  the code  as shown  in  Example 3.
-The code of the Simpful model that is generated is automatically saved (in the same location as the pyFUME script is ran from) under the name 'Simpful_code.py'
-
-## Note
-Please be aware that pyFUME's feature selection functionality makes use of multiprocessing. 
-When feature selection is used, the main script should always be guarded by including "if \_\_name\_\_ == '\_\_main\_\_':" in the header the script.
-When the Spyder IDE is used, one should include "if \_\_name\_\_ == '\_\_main\_\_' and '\_\_file\_\_' in globals():".
-
-### Example 1
-```
-from pyfume import pyFUME
-
-# Set the path to the data and choose the number of clusters
-path='./Concrete_data.csv'
-nc=3
-
-# Generate the Takagi-Sugeno FIS
-FIS = pyFUME(datapath=path, nr_clus=nc)
-
-# Calculate and print the accuracy of the generated model
-MAE=FIS.calculate_error(method="MAE")
-print ("The estimated error of the developed model is:", MAE)
-
-## Use the FIS to predict the compressive strength of a new concrete sample
-# Extract the model from the FIS object
-model=FIS.get_model()
-
-# Set the values for each variable
-model.set_variable('Cement', 300.0)
-model.set_variable('BlastFurnaceSlag', 50.0)
-model.set_variable('FlyAsh', 0.0)
-model.set_variable('Water', 175.0)
-model.set_variable('Superplasticizer',0.7)
-model.set_variable('CoarseAggregate', 900.0)
-model.set_variable('FineAggregate', 600.0)
-model.set_variable('Age', 45.0)
-
-# Perform inference and print predicted value
-print(model.Sugeno_inference(['OUTPUT']))
-```
-
-### Example 2
-```
-from pyfume import pyFUME
-
-# Set the path to the data and choose the number of clusters
-path='./Concrete_data.csv'
-nc=3
-
-# Generate the Takagi-Sugeno FIS
-FIS = pyFUME(datapath=path, nr_clus=nc, feature_selection='fst-pso')
-
-# Calculate and print the accuracy of the generated model
-MAE=FIS.calculate_error(method="MAE")
-print ("The estimated error of the developed model is:", MAE)
-
-## Use the FIS to predict the compressive strength of a new concrete sample
-# Extract the model from the FIS object
-model=FIS.get_model()
-
-# Set the values for each variable
-model.set_variable('Cement', 300.0)
-model.set_variable('BlastFurnaceSlag', 50.0)
-model.set_variable('FlyAsh', 0.0)
-model.set_variable('Water', 175.0)
-model.set_variable('Superplasticizer',0.7)
-model.set_variable('CoarseAggregate', 900.0)
-model.set_variable('FineAggregate', 600.0)
-model.set_variable('Age', 45.0)
-
-# Perform inference and print predicted value
-print(model.Sugeno_inference(['OUTPUT']))
-```
-
-### Example 3
-
-```
-from pyfume import *
-
-# Set the path to the data and choose the number of clusters
-path='./Concrete_data.csv'
-nr_clus=3
-
-# Load and normalize the data using min-max normalization
-dl=DataLoader(path,normalize='minmax')
-variable_names=dl.variable_names 
-dataX=dl.dataX
-dataY=dl.dataY
-
-# Split the data using the hold-out method in a training (default: 75%) 
-# and test set (default: 25%).
-ds = DataSplitter()
-x_train, y_train, x_test, y_test = ds.holdout(dataX=dl.dataX, dataY=dl.dataY)
-
-# Select features relevant to the problem
-fs=FeatureSelector(dataX=x_train, dataY=y_train, nr_clus=nr_clus, variable_names=variable_names)
-selected_feature_indices, variable_names=fs.wrapper()
-
-# Adapt the training and test input data after feature selection
-x_train = x_train[:, selected_feature_indices]
-x_test = x_test[:, selected_feature_indices]
-      
-# Cluster the training data (in input-output space) using FCM with default settings
-cl = Clusterer(x_train=x_train, y_train=y_train, nr_clus=nr_clus)
-cluster_centers, partition_matrix, _ = cl.cluster(method="fcm")
-     
-# Estimate the membership funtions of the system (default: mf_shape = gaussian)
-ae = AntecedentEstimator(x_train=x_train, partition_matrix=partition_matrix)
-antecedent_parameters = ae.determineMF()
-
-# Calculate the firing strength of each rule for each data instance        
-fsc=FireStrengthCalculator(antecedent_parameters=antecedent_parameters, nr_clus=nr_clus, variable_names=variable_names)
-firing_strengths = fsc.calculate_fire_strength(data=x_train)
-
-# Estimate the parameters of the consequent functions
-ce = ConsequentEstimator(x_train=x_train, y_train=y_train, firing_strengths=firing_strengths)
-consequent_parameters = ce.suglms()
-        
-# Build a first-order Takagi-Sugeno model using Simpful. Specify the optional 
-# 'extreme_values' argument to specify the universe of discourse of the input
-# variables if you which to use Simpful's membership function plot functionalities.
-simpbuilder = SugenoFISBuilder(antecedent_sets=antecedent_parameters, consequent_parameters=consequent_parameters, variable_names=variable_names)
-model = simpbuilder.get_model()
-
-# Calculate the mean squared error (MSE) of the model using the test data set
-test=SugenoFISTester(model=model, test_data=x_test, variable_names=variable_names, golden_standard=y_test)
-MSE = test.calculate_MSE()
-
-print('The mean squared error of the created model is', MSE)
-```
-
-### Example 4
-
-```
-from pyfume import pyFUME
-import pandas as pd
-import numpy as np
-
-# Read a Pandas dataframe (using the Pandas library)
-df = pd.read_csv('.\Concrete_data.csv')
-
-# Generate the Takagi-Sugeno FIS
-FIS = pyFUME(dataframe=df, nr_clus=2)
-
-# Calculate and print the accuracy of the generated model
-MAE=FIS.calculate_error(method="MAE")
-print ("The estimated error of the developed model is:", MAE)
-
-### Use the FIS to predict the compressive strength of a new concrete samples
-
-## Using Simpful's syntax (NOTE: This approach ONLY works for models built using non-normalized data!)   
-# Extract the model from the FIS object
-model=FIS.get_model()
-
-# Set the values for each variable
-model.set_variable('Cement', 300.0)
-model.set_variable('BlastFurnaceSlag', 50.0)
-model.set_variable('FlyAsh', 0.0)
-model.set_variable('Water', 175.0)
-model.set_variable('Superplasticizer',0.7)
-model.set_variable('CoarseAggregate', 900.0)
-model.set_variable('FineAggregate', 600.0)
-model.set_variable('Age', 45.0)
-
-# Perform inference and print predicted value
-print('The output using Simpfuls "set_variable" functionality is:', model.Sugeno_inference(['OUTPUT']))
-
-## Using pyFUME's syntax (NOTE: This approach DOES work for models built using normalized data!)
-# Create numpy array (matrix) in which each row is a data instance to be processed
-new_data_one_instance=np.array([[300, 50,0,175,0.7,900,600,45]]) 
-prediction_labels_one_instance=FIS.predict_label(new_data_one_instance)
-print('The output using pyFUMEs "predict_label" functionality is:', prediction_labels_one_instance)
-
-# Example in which output for multiple data instances is computed
-new_data_multiple_instances=np.array([[300, 50,0,175,0.7,900,600,45],[500, 75,30,200,0.9,600,760,39],[250, 40,10,175,0.3,840,360,51]]) 
-prediction_labels_multiple_instance=FIS.predict_label(new_data_multiple_instances)
-print('The output using pyFUMEs "predict_label" functionality is:', prediction_labels_multiple_instance)
-
-### Plot the actual values vs the predicted values of the test data using the matplotlib library
-
-# Predict the labels of the test data
-pred = FIS.predict_test_data()
-
-# Get the actual labels of the test data
-_, actual = FIS.get_data(data_set='test')
-
-# Create scatterplot
-import matplotlib.pyplot as plt 
-plt.scatter(actual, pred)
-plt.xlabel('Actual value') 
-plt.ylabel('Predicted value')
-plt.plot([0,85],[0,85],'r')     # Add a reference line
-plt.show()
-
-
-```
-
-## Installation
-
-`pip install pyfume`
-
-
-## Further information
-If you need further information, please write an e-mail to Caro Fuchs: c.e.m.fuchs(at)tue.nl.
-
-
-## References
-[1] Fuchs, C., Spolaor, S., Nobile, M. S., & Kaymak, U. (2020) "pyFUME: a Python package for fuzzy model estimation". In 2020 IEEE International Conference on Fuzzy Systems (FUZZ-IEEE) (pp. 1-8). IEEE.
-
-[2] I-Cheng Yeh, "Modeling of strength of high performance concrete using artificial neural networks," Cement and Concrete Research, Vol. 28, No. 12, pp. 1797-1808 (1998). http://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength
-
-
+# pyFUME
+
+pyFUME is a Python package for automatic Fuzzy Models Estimation from data [1].
+pyFUME contains functions to estimate the antecedent sets and the consequent parameters of a Takagi-Sugeno fuzzy model directly from data. This information is then used to create an executable fuzzy model using the Simpful library.
+pyFUME also provides facilities for the evaluation of performance.
+For more information about pyFUME's functionalities, please check the [online documentation](https://pyfume.readthedocs.io/en/latest/).
+
+## Usage
+For the following example, we use the Concrete Compressive Strength data set [2] as can be found in the UCI repository.
+The  code  in  Example 1  is  simple  and  easy  to  use,  making it  ideal  to  use  for  practitioners  who  wish  to  use  the  default settings or only wish to use few non-default settings using additional input arguments (Example 2). 
+Users that wish to deviate from  the  default  settings  can  use  the code  as shown  in  Example 3.
+The code of the Simpful model that is generated is automatically saved (in the same location as the pyFUME script is ran from) under the name 'Simpful_code.py'
+
+## Note
+Please be aware that pyFUME's feature selection functionality makes use of multiprocessing. 
+When feature selection is used, the main script should always be guarded by including "if \_\_name\_\_ == '\_\_main\_\_':" in the header the script.
+When the Spyder IDE is used, one should include "if \_\_name\_\_ == '\_\_main\_\_' and '\_\_file\_\_' in globals():".
+
+### Example 1
+```
+from pyfume import pyFUME
+
+# Set the path to the data and choose the number of clusters
+path='./Concrete_data.csv'
+nc=3
+
+# Generate the Takagi-Sugeno FIS
+FIS = pyFUME(datapath=path, nr_clus=nc)
+
+# Calculate and print the accuracy of the generated model
+MAE=FIS.calculate_error(method="MAE")
+print ("The estimated error of the developed model is:", MAE)
+
+## Use the FIS to predict the compressive strength of a new concrete sample
+# Extract the model from the FIS object
+model=FIS.get_model()
+
+# Set the values for each variable
+model.set_variable('Cement', 300.0)
+model.set_variable('BlastFurnaceSlag', 50.0)
+model.set_variable('FlyAsh', 0.0)
+model.set_variable('Water', 175.0)
+model.set_variable('Superplasticizer',0.7)
+model.set_variable('CoarseAggregate', 900.0)
+model.set_variable('FineAggregate', 600.0)
+model.set_variable('Age', 45.0)
+
+# Perform inference and print predicted value
+print(model.Sugeno_inference(['OUTPUT']))
+```
+
+### Example 2
+```
+from pyfume import pyFUME
+
+# Set the path to the data and choose the number of clusters
+path='./Concrete_data.csv'
+nc=3
+
+# Generate the Takagi-Sugeno FIS
+FIS = pyFUME(datapath=path, nr_clus=nc, feature_selection='fst-pso')
+
+# Calculate and print the accuracy of the generated model
+MAE=FIS.calculate_error(method="MAE")
+print ("The estimated error of the developed model is:", MAE)
+
+## Use the FIS to predict the compressive strength of a new concrete sample
+# Extract the model from the FIS object
+model=FIS.get_model()
+
+# Set the values for each variable
+model.set_variable('Cement', 300.0)
+model.set_variable('BlastFurnaceSlag', 50.0)
+model.set_variable('FlyAsh', 0.0)
+model.set_variable('Water', 175.0)
+model.set_variable('Superplasticizer',0.7)
+model.set_variable('CoarseAggregate', 900.0)
+model.set_variable('FineAggregate', 600.0)
+model.set_variable('Age', 45.0)
+
+# Perform inference and print predicted value
+print(model.Sugeno_inference(['OUTPUT']))
+```
+
+### Example 3
+
+```
+from pyfume import *
+
+# Set the path to the data and choose the number of clusters
+path='./Concrete_data.csv'
+nr_clus=3
+
+# Load and normalize the data using min-max normalization
+dl=DataLoader(path,normalize='minmax')
+variable_names=dl.variable_names 
+dataX=dl.dataX
+dataY=dl.dataY
+
+# Split the data using the hold-out method in a training (default: 75%) 
+# and test set (default: 25%).
+ds = DataSplitter()
+x_train, y_train, x_test, y_test = ds.holdout(dataX=dl.dataX, dataY=dl.dataY)
+
+# Select features relevant to the problem
+fs=FeatureSelector(dataX=x_train, dataY=y_train, nr_clus=nr_clus, variable_names=variable_names)
+selected_feature_indices, variable_names=fs.wrapper()
+
+# Adapt the training and test input data after feature selection
+x_train = x_train[:, selected_feature_indices]
+x_test = x_test[:, selected_feature_indices]
+      
+# Cluster the training data (in input-output space) using FCM with default settings
+cl = Clusterer(x_train=x_train, y_train=y_train, nr_clus=nr_clus)
+cluster_centers, partition_matrix, _ = cl.cluster(method="fcm")
+     
+# Estimate the membership funtions of the system (default: mf_shape = gaussian)
+ae = AntecedentEstimator(x_train=x_train, partition_matrix=partition_matrix)
+antecedent_parameters = ae.determineMF()
+
+# Calculate the firing strength of each rule for each data instance        
+fsc=FireStrengthCalculator(antecedent_parameters=antecedent_parameters, nr_clus=nr_clus, variable_names=variable_names)
+firing_strengths = fsc.calculate_fire_strength(data=x_train)
+
+# Estimate the parameters of the consequent functions
+ce = ConsequentEstimator(x_train=x_train, y_train=y_train, firing_strengths=firing_strengths)
+consequent_parameters = ce.suglms()
+        
+# Build a first-order Takagi-Sugeno model using Simpful. Specify the optional 
+# 'extreme_values' argument to specify the universe of discourse of the input
+# variables if you which to use Simpful's membership function plot functionalities.
+simpbuilder = SugenoFISBuilder(antecedent_sets=antecedent_parameters, consequent_parameters=consequent_parameters, variable_names=variable_names)
+model = simpbuilder.get_model()
+
+# Calculate the mean squared error (MSE) of the model using the test data set
+test=SugenoFISTester(model=model, test_data=x_test, variable_names=variable_names, golden_standard=y_test)
+MSE = test.calculate_MSE()
+
+print('The mean squared error of the created model is', MSE)
+```
+
+### Example 4
+
+```
+from pyfume import pyFUME
+import pandas as pd
+import numpy as np
+
+# Read a Pandas dataframe (using the Pandas library)
+df = pd.read_csv('.\Concrete_data.csv')
+
+# Generate the Takagi-Sugeno FIS
+FIS = pyFUME(dataframe=df, nr_clus=2)
+
+# Calculate and print the accuracy of the generated model
+MAE=FIS.calculate_error(method="MAE")
+print ("The estimated error of the developed model is:", MAE)
+
+### Use the FIS to predict the compressive strength of a new concrete samples
+
+## Using Simpful's syntax (NOTE: This approach ONLY works for models built using non-normalized data!)   
+# Extract the model from the FIS object
+model=FIS.get_model()
+
+# Set the values for each variable
+model.set_variable('Cement', 300.0)
+model.set_variable('BlastFurnaceSlag', 50.0)
+model.set_variable('FlyAsh', 0.0)
+model.set_variable('Water', 175.0)
+model.set_variable('Superplasticizer',0.7)
+model.set_variable('CoarseAggregate', 900.0)
+model.set_variable('FineAggregate', 600.0)
+model.set_variable('Age', 45.0)
+
+# Perform inference and print predicted value
+print('The output using Simpfuls "set_variable" functionality is:', model.Sugeno_inference(['OUTPUT']))
+
+## Using pyFUME's syntax (NOTE: This approach DOES work for models built using normalized data!)
+# Create numpy array (matrix) in which each row is a data instance to be processed
+new_data_one_instance=np.array([[300, 50,0,175,0.7,900,600,45]]) 
+prediction_labels_one_instance=FIS.predict_label(new_data_one_instance)
+print('The output using pyFUMEs "predict_label" functionality is:', prediction_labels_one_instance)
+
+# Example in which output for multiple data instances is computed
+new_data_multiple_instances=np.array([[300, 50,0,175,0.7,900,600,45],[500, 75,30,200,0.9,600,760,39],[250, 40,10,175,0.3,840,360,51]]) 
+prediction_labels_multiple_instance=FIS.predict_label(new_data_multiple_instances)
+print('The output using pyFUMEs "predict_label" functionality is:', prediction_labels_multiple_instance)
+
+### Plot the actual values vs the predicted values of the test data using the matplotlib library
+
+# Predict the labels of the test data
+pred = FIS.predict_test_data()
+
+# Get the actual labels of the test data
+_, actual = FIS.get_data(data_set='test')
+
+# Create scatterplot
+import matplotlib.pyplot as plt 
+plt.scatter(actual, pred)
+plt.xlabel('Actual value') 
+plt.ylabel('Predicted value')
+plt.plot([0,85],[0,85],'r')     # Add a reference line
+plt.show()
+
+
+```
+
+## Installation
+
+`pip install pyfume`
+
+
+## Further information
+If you need further information, please write an e-mail to Caro Fuchs: c.e.m.fuchs(at)tue.nl.
+
+
+## References
+[1] Fuchs, C., Spolaor, S., Nobile, M. S., & Kaymak, U. (2020) "pyFUME: a Python package for fuzzy model estimation". In 2020 IEEE International Conference on Fuzzy Systems (FUZZ-IEEE) (pp. 1-8). IEEE.
+
+[2] I-Cheng Yeh, "Modeling of strength of high performance concrete using artificial neural networks," Cement and Concrete Research, Vol. 28, No. 12, pp. 1797-1808 (1998). http://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength
+
+
```

### Comparing `pyFUME-0.3.1/pyFUME.egg-info/SOURCES.txt` & `pyfume-0.3.4/pyFUME.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyFUME-0.3.1/pyfume/BuildTakagiSugeno.py` & `pyfume-0.3.4/pyfume/BuildTakagiSugeno.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,547 +1,549 @@
-from .LoadData import DataLoader
-from .Splitter import DataSplitter
-from .SimpfulModelBuilder import SugenoFISBuilder
-from .Clustering import Clusterer
-from .EstimateAntecendentSet import AntecedentEstimator
-from .FireStrengthCalculator import FireStrengthCalculator
-from .EstimateConsequentParameters import ConsequentEstimator
-from .Tester import SugenoFISTester
-from .FeatureSelection import FeatureSelector
-from .Sampler import Sampler
-import numpy as np
-
-
-class BuildTSFIS(object):
-    """
-        Learns a a new  Takagi-Sugeno fuzzy model.
-        
-        Args:
-            datapath: The path to the csv file containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
-            dataframe: Pandas dataframe containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
-            nr_clus: Number of clusters that should be identified in the data (default = 2).
-            process_categorical: Boolean to indicate whether categorical variables should be processed (default = False).
-            method: At this moment, only Takagi Sugeno models are supported (default = 'Takagi-Sugeno')
-            variable_names: Names of the variables, if not specified the names will be read from the first row of the csv file (default = None).
-            merge_threshold: Threshold for GRABS to drop fuzzy sets from the model. If the jaccard similarity between two sets is higher than this threshold, the fuzzy set will be dropped from the model.
-            **kwargs: Additional arguments to change settings of the fuzzy model.
-
-        Returns:
-            An object containing the fuzzy model, information about its setting (such as its antecedent and consequent parameters) and the different splits of the data.
-    """
-    def __init__(self, datapath=None, dataframe=None, nr_clus=None, variable_names=None, 
-            process_categorical=False, merge_threshold=1.0, setnes_threshold=1.0, verbose=False, **kwargs):
-
-        self.datapath = datapath
-        self.nr_clus = nr_clus
-        self.variable_names = variable_names
-        self._antecedent_estimator = None
-        self.verbose = verbose
-
-        # Check keyword-arguments and complete with default settings if necessary
-        if 'model_order' not in kwargs.keys(): kwargs['model_order'] = 'first'
-        if 'normalization' in kwargs.keys(): kwargs['normalize'] = kwargs['normalization']
-        if 'normalize' not in kwargs.keys(): kwargs['normalize'] = False
-        if 'imputation' not in kwargs.keys(): kwargs['imputation'] = 'knn'  # new
-        if 'percentage_training' not in kwargs.keys(): kwargs['percentage_training'] = 0.75
-        if 'oversampling' not in kwargs.keys(): kwargs['oversampling'] = False
-        if kwargs['oversampling'] is True:
-            if 'sampling_number_of_bins' not in kwargs.keys(): kwargs['sampling_number_of_bins'] = 2
-            if 'sampling_histogram' not in kwargs.keys(): kwargs['sampling_histogram'] = False
-        if 'data_delimiter' not in kwargs.keys(): kwargs['data_delimiter'] = ','
-        if 'data_split_method' not in kwargs.keys(): kwargs['data_split_method'] = 'hold-out'
-        if 'feature_selection' not in kwargs.keys(): kwargs['feature_selection'] = None
-        if 'fs_max_iter' not in kwargs.keys(): kwargs['fs_max_iter'] = 100
-        if 'cluster_method' not in kwargs.keys(): kwargs['cluster_method'] = 'fcm'
-        if 'm' not in kwargs.keys(): kwargs['m'] = '2'
-        if kwargs['cluster_method'] == 'fcm':
-            if 'fcm_max_iter' not in kwargs.keys(): kwargs['fcm_maxiter'] = 1000
-            if 'fcm_error' not in kwargs.keys(): kwargs['fcm_error'] = 0.005
-        elif kwargs['cluster_method'] == 'fst-pso':
-            if 'fstpso_n_particles' not in kwargs.keys(): kwargs['fstpso_n_particles'] = None
-            if 'fstpso_max_iter' not in kwargs.keys(): kwargs['fstpso_max_iter'] = 100
-            if 'fstpso_path_fit_dump' not in kwargs.keys(): kwargs['fstpso_path_fit_dump'] = None
-            if 'fstpso_path_sol_dump' not in kwargs.keys(): kwargs['fstpso_path_sol_dump'] = None
-        elif kwargs['cluster_method'] == 'gk':
-            if 'gk_max_iter' not in kwargs.keys(): kwargs['gk_maxiter'] = 1000
-        if 'mf_shape' not in kwargs.keys(): kwargs['mf_shape'] = 'gauss'
-        if 'operators' not in kwargs.keys(): kwargs['operators'] = None
-        if 'global_fit' not in kwargs.keys(): kwargs['global_fit'] = False
-        if 'save_simpful_code' not in kwargs.keys(): kwargs['save_simpful_code'] = True
-        if 'cv_randomID' not in kwargs.keys(): kwargs['cv_randomID'] = False
-        if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
-        if 'log_variables' not in kwargs.keys(): kwargs['log_variables'] = None
-        if 'categorical_indices' not in kwargs.keys(): kwargs['categorical_indices'] = None
-
-        if self.nr_clus is None and kwargs['feature_selection'] is None:
-            print('Error: please set pyFUME`s argument "nr_clus".')
-            import sys
-            sys.exit()
-
-        # Load the data
-        if self.datapath is None:
-            dl = DataLoader(dataframe=dataframe, normalize=kwargs['normalize'], process_categorical=process_categorical, delimiter=kwargs['data_delimiter'], log_variables=kwargs['log_variables'], categorical_indices=kwargs['categorical_indices'], verbose=self.verbose)
-        else:
-            dl = DataLoader(self.datapath, normalize=kwargs['normalize'],  process_categorical=process_categorical, delimiter=kwargs['data_delimiter'], log_variables=kwargs['log_variables'], categorical_indices=kwargs['categorical_indices'], verbose=self.verbose)
-        self.variable_names = dl.get_variable_names()
-
-        if kwargs['normalize'] is not False and kwargs['normalize'] != 'zscore':
-            self.normalization_values = list(dl.get_normalization_values())
-            self.minmax_norm_flag = True
-        else:
-            self.minmax_norm_flag = False
-            self.normalization_values = None
-
-        self.dataX = dl.get_input_data()
-        self.dataY = dl.get_target_data()
-
-        # Create a DataSplitter object
-        ds = DataSplitter()
-
-        if kwargs['data_split_method'] == 'hold-out' or kwargs['data_split_method'] == 'holdout':
-
-            if self.verbose: print(' * Hold-out method selected.')
-
-            # Split the data using the hold-out method in a training (default: 75%) 
-            # and test set (default: 25%).
-            self.x_train, self.y_train, self.x_test, self.y_test = ds.holdout(dataX=self.dataX, dataY=self.dataY, percentage_training=kwargs['percentage_training'])
-            # Check if there are any missing variables and impute them
-            if np.isnan(self.dataX).any().any() is True:
-                try:
-                    from sklearn.impute import KNNImputer
-                except ImportError:
-                    raise Exception('pyFUME tried to impute missing values, but couldn`t find \'sklearn\'. Please pip install sklearn to proceed.')
-
-                if self.verbose: print('Warning: Your data contains missing values that will be imputed using KNN.')
-                imputer = KNNImputer(n_neighbors=3, weights="uniform")
-                self.x_train = imputer.fit_transform(self.x_train)
-                self.x_test = imputer.fit_transform(self.x_test)
-
-            if kwargs['oversampling'] is True:
-                sample = Sampler(train_x=self.x_train, train_y=self.y_train, number_of_bins=kwargs['sampling_number_of_bins'], histogram=kwargs['sampling_histogram'])
-                self.x_train, self.y_train = sample.oversample()
-
-            # Perform feature selection if requested
-            if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False:
-                if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
-                fs = FeatureSelector(self.x_train, self.y_train, self.nr_clus, self.variable_names, model_order= kwargs['model_order'], performance_metric = kwargs['performance_metric'], verbose=self.verbose)
-
-                # Keep copies of the training and test set before dropping unselected features
-                self.x_train_before_fs = self.x_train.copy()
-                self.x_test_before_fs = self.x_test.copy()
-
-                if kwargs['feature_selection'] == 'wrapper' or kwargs['feature_selection'] == 'sfs' or kwargs['feature_selection'] == 'SFS':
-                    self.selected_feature_indices, self.variable_names = fs.wrapper()
-                elif kwargs['feature_selection'] == 'logwrapper':
-                    self.selected_feature_indices, self.selected_variable_names, self.log_indices, self.log_variable_names = fs.log_wrapper()
-                elif kwargs['feature_selection'] == 'fst-pso' or kwargs['feature_selection'] == 'fstpso' or kwargs['feature_selection'] == 'pso' or kwargs['feature_selection'] is True:
-                    self.selected_feature_indices, self.selected_variable_names, self.nr_clus = fs.fst_pso_feature_selection(max_iter=kwargs['fstpso_max_iter'], **kwargs)
-                self.x_train = self.x_train[:, self.selected_feature_indices]
-                self.x_test = self.x_test[:, self.selected_feature_indices]
-
-            elif kwargs['feature_selection'] is None:
-                self.selected_variable_names = self.variable_names
-
-            # Cluster the data, log-transform when needed.
-            if kwargs['feature_selection'] == 'logwrapper':
-                # Use log transformed variables if needed
-                self.log_x_train = self.x_train.copy()
-                for i in self.log_indices:
-                    self.log_x_train[i]= np.log(self.x_train[i])
-                cl = Clusterer(x_train=self.log_x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
-            else:
-                # Cluster the training data (in input-output space)
-                cl = Clusterer(x_train=self.x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
-
-            if kwargs['cluster_method'] == 'fcm':
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fcm', fcm_m=kwargs['m'],
-                    fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
-            elif kwargs['cluster_method'] == 'gk':
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='gk')
-            elif kwargs['cluster_method'] == 'fst-pso':
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fstpso',
-                    fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
-                    fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
-            elif kwargs['cluster_method'] == 'fuzzy_k_protoypes' or kwargs['cluster_method'] == 'fkp' or kwargs['cluster_method'] == 'FKP':
-                if 'categorical_indices' in kwargs:
-                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp',
-                                                                                categorical_indices=kwargs['categorical_indices'])
-                else:
-                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp')
-            else:
-                print('ERROR: Choose a valid clustering method.')
-                import sys
-                sys.exit()
-
-            # Estimate the membership funtions of the system (default shape: gauss)
-            self._antecedent_estimator = AntecedentEstimator(x_train=self.x_train, partition_matrix=self.partition_matrix)
-    
-            self.antecedent_parameters = self._antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'], merge_threshold=merge_threshold, setnes_threshold=setnes_threshold, categorical_indices=kwargs['categorical_indices'])
-            what_to_drop = self._antecedent_estimator._info_for_simplification
-
-            # Calculate the firing strengths
-            fsc = FireStrengthCalculator(antecedent_parameters=self.antecedent_parameters, nr_clus=self.nr_clus,
-                                         variable_names=self.selected_variable_names,
-                                         **kwargs)
-            self.firing_strengths = fsc.calculate_fire_strength(data=self.x_train)
-
-            # Estimate the parameters of the consequent
-            ce = ConsequentEstimator(x_train=self.x_train, y_train=self.y_train, firing_strengths=self.firing_strengths,
-                                     categorical_indices=kwargs['categorical_indices'])
-            if kwargs['model_order'] == 'first':
-                self.consequent_parameters = ce.suglms()
-            elif kwargs['model_order'] == 'zero':
-                self.consequent_parameters = ce.zero_order()
-            else:
-                raise Exception("pyFUME currently only supports zero-order (model_order = 'zero') and first-order (model_order = 'first') fuzzy models.")
-
-            # Build a first-order Takagi-Sugeno model using Simpful
-            simpbuilder = SugenoFISBuilder(
-                self.antecedent_parameters,
-                self.consequent_parameters,
-                self.selected_variable_names,
-                normalization_values=self.normalization_values,
-                extreme_values=self._antecedent_estimator._extreme_values,
-                model_order=kwargs["model_order"],
-                operators=kwargs["operators"],
-                save_simpful_code=kwargs['save_simpful_code'],
-                fuzzy_sets_to_drop=what_to_drop,
-                setnes_dropped_antecedents=self._antecedent_estimator._setnes_removed_sets,
-                verbose=self.verbose,
-                categorical_indices=kwargs['categorical_indices'])
-
-            self.model = simpbuilder.simpfulmodel
-
-        elif kwargs['data_split_method'] == 'cross_validation' or kwargs['data_split_method'] == 'k-fold_cross_validation' or kwargs['data_split_method'] == 'crossvalidation' or kwargs['data_split_method'] == 'cv' or kwargs['data_split_method'] == 'kfold':
-            if 'number_of_folds' not in kwargs.keys(): kwargs['number_of_folds'] = 10
-            if self.verbose: print('K-fold cross validation was selected. The number of folds (k) equals', kwargs['number_of_folds'])
-            # if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
-            if 'save_kfold_models' not in kwargs.keys(): kwargs['save_kfold_models'] = True
-            if 'kfold_indices' not in kwargs.keys(): kwargs['kfold_indices'] = None
-            if 'paralellization_kfold' not in kwargs.keys(): kwargs['paralellization_kfold'] = False
-
-            # Create lists with test indices for each fold.
-            if kwargs['kfold_indices'] is None:
-                self.fold_indices = ds.kfold(data_length=len(self.dataX), number_of_folds=kwargs['number_of_folds'])
-            else:
-                self.fold_indices = kwargs['kfold_indices']
-
-            self.performance_metric = kwargs['performance_metric']
-            # fold_indices=pd.read_csv('./fold_indices.csv', header=None)
-            # self.fold_indices=fold_indices.to_numpy()
-
-            # Create folder to store developed models
-            if kwargs['save_kfold_models'] is True:
-                import os, datetime
-
-                if kwargs['cv_randomID'] is True:
-                    try:
-                        import uuid
-                    except ImportError:
-                        raise Exception('pyFUME tried to generate random IDs, but couldn`t find \'uuid\'. Please pip install uuid to proceed.')
-
-                    self.folder_name = 'pyFUME runID ' + str(uuid.uuid4())
-                elif kwargs['cv_randomID'] is False:
-                    self.folder_name = 'pyFUME run ' + datetime.datetime.now().strftime("%Y-%m-%d %H.%M.%S")
-
-                owd = os.getcwd()
-                os.mkdir(self.folder_name)
-                os.chdir('./' + self.folder_name)
-
-            if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False: self.selected_features_per_fold = dict()
-            if kwargs['feature_selection'] == 'logwrapper': self.logged_features_per_fold = dict()
-
-            self.kfold_dict = dict()
-            args = []
-
-            for fold_number in range(0, kwargs['number_of_folds']):
-                if self.verbose: print('Training the model for fold', fold_number)
-                tst_idx = self.fold_indices[fold_number]
-                tst_idx = tst_idx[~np.isnan(tst_idx)]
-                tst_idx = [int(x) for x in tst_idx]
-                #np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
-                trn_idx = np.concatenate(np.delete(self.fold_indices, fold_number, axis=0))
-                trn_idx = trn_idx[~np.isnan(trn_idx)]
-                trn_idx = [int(x) for x in trn_idx]
-
-                self.x_train = np.array([self.dataX[i, :] for i in trn_idx])
-                self.x_test = np.array([self.dataX[i, :] for i in tst_idx])
-                self.y_train = np.array([self.dataY[i] for i in trn_idx])
-                self.y_test = np.array([self.dataY[i] for i in tst_idx])
-
-                if kwargs['feature_selection'] == 'logwrapper':
-                    raw_x_train = dl.get_non_normalized_x_data()
-                    self.raw_x_train = np.array([raw_x_train[i,:] for i in trn_idx])
-
-                args.append([fold_number, self.x_train, self.x_test, self.y_train, self.y_test])
-                nm = 'fold_' + str(fold_number)
-
-                if kwargs['paralellization_kfold'] is False:
-                    self.kfold_dict[nm] = self._create_kfold_model(*args[fold_number], **kwargs)
-
-            if kwargs['paralellization_kfold'] is True:
-                print('Paralellization of code is currently not possible yet. Coming soon!')
-
-            # import sys
-            # sys.exit(1)
-
-            # set working directory back to where script is stored
-            if kwargs['save_kfold_models'] is True:
-                os.chdir(owd)
-
-            self.performance_metric_per_fold = np.array([x['performance'] for x in self.kfold_dict.values()])
-
-            # print('The average ' + self.performance_metric + ' over ' + str(kwargs['number_of_folds']) +' folds is ' + str(np.mean(self.performance_metric_per_fold)) +' (with st. dev. ' + str(np.std(self.performance_metric_per_fold)) + '). \nThe best model was created in fold ' +  str(np.argmin(self.performance_metric_per_fold)) + ' with ' + self.performance_metric +  ' = ' + str(np.min(self.performance_metric_per_fold)) + '.')
-            if self.verbose: print('The average ' + self.performance_metric + ' over ' + str(kwargs['number_of_folds']) + ' folds is ' + str(np.mean(self.performance_metric_per_fold)) + ' (with st. dev. ' + str(np.std(self.performance_metric_per_fold)) + ').')
-
-        elif kwargs['data_split_method'] == 'no_split':
-            if self.verbose: print('No test data will be split off, all data will be used for training.')
-
-            self.x_train = self.dataX.copy()
-            self.y_train = self.dataY.copy()
-
-            if np.isnan(self.dataX).any().any() is True:
-                try:
-                    from sklearn.impute import KNNImputer
-                except ImportError:
-                    raise Exception('pyFUME tried to impute missing values, but couldn`t find \'sklearn\'. Please pip install sklearn to proceed.')
-
-                if self.verbose: print('Warning: Your data contains missing values that will be imputed using KNN.')
-
-                imputer = KNNImputer(n_neighbors=3, weights="uniform")
-                self.x_train = imputer.fit_transform(self.x_train)
-
-            if kwargs['oversampling'] is True:
-                sample = Sampler(train_x=self.x_train, train_y=self.y_train, number_of_bins=kwargs['sampling_number_of_bins'], histogram=kwargs['sampling_histogram'])
-                self.x_train, self.y_train = sample.oversample()
-
-            # Perform feature selection if requested
-            if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False:
-                if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
-                fs = FeatureSelector(self.x_train, self.y_train, self.nr_clus, self.variable_names, model_order=kwargs['model_order'], performance_metric = kwargs['performance_metric'], verbose=self.verbose)
-
-                # Keep copies of the training and test set before dropping unselected features
-                self.x_train_before_fs = self.x_train.copy()
-
-                if kwargs['feature_selection'] == 'wrapper' or kwargs['feature_selection'] == 'sfs' or kwargs['feature_selection'] == 'SFS':
-                    self.selected_feature_indices, self.variable_names = fs.wrapper()
-                elif kwargs['feature_selection'] == 'logwrapper':
-                    self.selected_feature_indices, self.selected_variable_names, self.log_indices, self.log_variable_names = fs.log_wrapper(raw_data = self.raw_x_train)
-                elif kwargs['feature_selection'] == 'fst-pso' or kwargs['feature_selection'] == 'fstpso' or kwargs['feature_selection'] == 'pso' or kwargs['feature_selection'] is True:
-                    self.selected_feature_indices, self.selected_variable_names, self.nr_clus = fs.fst_pso_feature_selection(max_iter=kwargs['fstpso_max_iter'], **kwargs)
-                else:
-                    raise Exception('Feature selection method not (yet) implemented.')
-
-                self.x_train = self.x_train[:, self.selected_feature_indices]
-
-            elif kwargs['feature_selection'] is None:
-                self.selected_variable_names = self.variable_names
-
-            # Cluster the data, log-transform when needed.
-            if kwargs['feature_selection'] == 'logwrapper':
-                # Use log transformed variables if needed
-                self.log_x_train = self.x_train.copy()
-                for i in self.log_indices:
-                    self.log_x_train[i] = np.log(self.x_train[i])
-                cl = Clusterer(x_train=self.log_x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
-            else:
-                # Cluster the training data (in input-output space)
-                cl = Clusterer(x_train=self.x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
-
-            if kwargs['cluster_method'] == 'fcm':
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fcm', fcm_m=kwargs['m'],
-                    fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
-            elif kwargs['cluster_method'] == 'gk':
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='gk')
-            elif kwargs['cluster_method'] == 'fst-pso':
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fstpso',
-                    fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
-                    fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
-            elif kwargs['cluster_method'] == 'fuzzy_k_protoypes' or kwargs['cluster_method'] == 'fkp' or kwargs['cluster_method'] == 'FKP':
-                if 'categorical_indices' in kwargs:
-                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp',
-                                                                                categorical_indices=kwargs['categorical_indices'])
-                else:
-                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp')
-            else:
-                print('ERROR: Choose a valid clustering method.')
-                import sys
-                sys.exit()
-
-            # Estimate the membership funtions of the system (default shape: gauss)
-            self._antecedent_estimator = AntecedentEstimator(self.x_train, self.partition_matrix)
-
-            self.antecedent_parameters = self._antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'],
-                                                                                merge_threshold=merge_threshold,
-                                                                                categorical_indices=kwargs['categorical_indices'])
-            what_to_drop = self._antecedent_estimator._info_for_simplification
-
-            # Calculate the firing strengths
-            fsc = FireStrengthCalculator(self.antecedent_parameters, self.nr_clus, self.selected_variable_names, **kwargs)
-            self.firing_strengths = fsc.calculate_fire_strength(self.x_train)
-
-            # Estimate the parameters of the consequent
-            ce = ConsequentEstimator(self.x_train, self.y_train, self.firing_strengths,
-                                     categorical_indices=kwargs['categorical_indices'])
-            if kwargs['model_order'] == 'first':
-                self.consequent_parameters = ce.suglms()
-            elif kwargs['model_order'] == 'zero':
-                self.consequent_parameters = ce.zero_order()
-            else:
-                raise Exception("pyFUME currently only supports zero-order (model_order = 'zero') and first-order (model_order = 'first') fuzzy models.")
-
-            # Build a first-order Takagi-Sugeno model using Simpful
-            simpbuilder = SugenoFISBuilder(
-                self.antecedent_parameters,
-                self.consequent_parameters,
-                self.selected_variable_names,
-                normalization_values=self.normalization_values,
-                extreme_values=self._antecedent_estimator._extreme_values,
-                model_order=kwargs["model_order"],
-                operators=kwargs["operators"],
-                save_simpful_code=kwargs['save_simpful_code'],
-                fuzzy_sets_to_drop=what_to_drop,
-                verbose=self.verbose,
-                categorical_indices=kwargs['categorical_indices'])
-
-            self.model = simpbuilder.simpfulmodel
-
-        else:
-            print('ERROR: invalid data splitting method chosen. Training will be aborted.')
-            import sys
-            sys.exit()
-
-    def _create_kfold_model(self, fold_number, x_train, x_test, y_train, y_test, merge_threshold=1.0, **kwargs):
-
-        # Create a dictionary to keep track of settings and results
-        fold_dict = dict()
-
-        fold_dict['fold_number'] = fold_number
-        fold_dict['x_train'] = x_train
-        fold_dict['x_test'] = x_test
-        fold_dict['y_train'] = y_train
-        fold_dict['y_test'] = y_test
-        fold_dict['GRABS_threshold'] = merge_threshold
-        fold_dict['nr_clus'] = self.nr_clus
-
-        if np.isnan(fold_dict['x_train']).any().any() is True:
-            try:
-                from sklearn.impute import KNNImputer
-            except ImportError:
-                raise Exception('pyFUME tried to impute missing values, but couldn`t find \'sklearn\'. Please pip install sklearn to proceed.')
-
-            if self.verbose: print('Warning: Your data contains missing values that will be imputed using KNN.')
-            imputer = KNNImputer(n_neighbors=3, weights="uniform")
-            tmp = imputer.fit_transform(fold_dict['x_train'])
-            fold_dict['x_train'] = tmp
-            fold_dict['x_test'] = imputer.fit_transform(fold_dict['x_test'])
-
-        if kwargs['oversampling'] is True:
-            sample = Sampler(train_x=fold_dict['x_train'], train_y=fold_dict['y_train'], number_of_bins=kwargs['sampling_number_of_bins'], histogram=kwargs['sampling_histogram'])
-            fold_dict['x_train'], fold_dict['y_train'] = sample.oversample()
-
-        # Perform feature selection if requested
-        if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False:
-            fs = FeatureSelector(fold_dict['x_train'], fold_dict['y_train'], self.nr_clus, self.variable_names, model_order= kwargs['model_order'], performance_metric = kwargs['performance_metric'], verbose=self.verbose)
-            fold_dict['x_train_before_fs'] = fold_dict['x_train'].copy()
-            fold_dict['x_test_before_fs'] = fold_dict['x_test'].copy()
-
-            if kwargs['feature_selection'] == 'wrapper' or kwargs['feature_selection'] == 'sfs' or kwargs['feature_selection'] == 'SFS':
-                fold_dict['selected_feature_indices'], fold_dict['selected_variable_names']=fs.wrapper()
-            elif kwargs['feature_selection'] == 'logwrapper':
-                raw_xdata = self.raw_x_train
-                fold_dict['selected_feature_indices'], fold_dict['selected_variable_names'], fold_dict['log_indices'], fold_dict['log_variable_names'] = fs.log_wrapper(raw_data = raw_xdata)
-            elif kwargs['feature_selection'] == 'fst-pso' or kwargs['feature_selection'] == 'fstpso' or kwargs['feature_selection'] == 'pso' or kwargs['feature_selection'] == True:
-                fold_dict['selected_feature_indices'], fold_dict['selected_variable_names'], fold_dict['nr_clus'] = fs.fst_pso_feature_selection(max_iter=kwargs['fstpso_max_iter'], **kwargs)
-
-            tmp = fold_dict['x_train']
-            idx = fold_dict['selected_feature_indices']
-            fold_dict['x_train'] = tmp[:, idx]
-
-            tmp = fold_dict['x_test']
-            fold_dict['x_test'] = tmp[:, idx]
-
-        elif kwargs['feature_selection'] is None:
-            fold_dict['selected_variable_names'] = self.variable_names
-
-        # Cluster the data, log-transform when needed.
-        if kwargs['feature_selection'] == 'logwrapper':
-            # Use log transformed variables if needed
-            tmp = fold_dict['x_train'].copy()
-            idx = fold_dict['log_indices']
-            for i in idx:
-                tmp[i] = np.log(tmp[i])
-            fold_dict['log_x_train'] = tmp
-            cl = Clusterer(x_train=fold_dict['log_x_train'], y_train=fold_dict['y_train'], nr_clus=fold_dict['nr_clus'], verbose=self.verbose)
-        else:
-            cl = Clusterer(x_train=fold_dict['x_train'], y_train=fold_dict['y_train'], nr_clus=fold_dict['nr_clus'], verbose=self.verbose)
-
-        if kwargs['cluster_method'] == 'fcm':
-            fold_dict['cluster_centers'], fold_dict['partition_matrix'], _ = cl.cluster(method='fcm', fcm_m=kwargs['m'],
-                fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
-        elif kwargs['cluster_method'] == 'fst-pso':
-            fold_dict['cluster_centers'], fold_dict['partition_matrix'], _ = cl.cluster(method='fstpso',
-                fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
-                fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
-        elif kwargs['cluster_method'] == 'gk':
-            fold_dict['cluster_centers'], fold_dict['partition_matrix'], _ = cl.cluster(method='gk')
-        elif kwargs['cluster_method'] == 'fuzzy_k_protoypes' or kwargs['cluster_method'] == 'fkp' or kwargs['cluster_method'] == 'FKP':
-            if 'categorical_indices' in kwargs:
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp',
-                                                                            categorical_indices=kwargs['categorical_indices'])
-            else:
-                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp')
-        else:
-            print('ERROR: Choose a valid clustering method.')
-            import sys
-            sys.exit()
-
-        # Estimate the membership funtions of the system (default shape: gauss)
-        antecedent_estimator = AntecedentEstimator(fold_dict['x_train'], fold_dict['partition_matrix'])
-
-        fold_dict['antecedent_parameters'] = antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'],
-                                                                              merge_threshold=fold_dict['GRABS_threshold'],
-                                                                              categorical_indices=kwargs['categorical_indices'])
-        fold_dict['what_to_drop'] = antecedent_estimator._info_for_simplification
-
-        # Calculate the firing strengths
-        fsc = FireStrengthCalculator(antecedent_parameters=fold_dict['antecedent_parameters'],
-                                     nr_clus=fold_dict['nr_clus'], variable_names=fold_dict['selected_variable_names'], **kwargs)
-        fold_dict['firing_strengths'] = fsc.calculate_fire_strength(data=fold_dict['x_train'])
-
-        # Estimate the parameters of the consequent
-        ce = ConsequentEstimator(fold_dict['x_train'], fold_dict['y_train'], fold_dict['firing_strengths'],
-                                 categorical_indices=kwargs['categorical_indices'])
-        fold_dict['consequent_parameters'] = ce.suglms()
-
-        # Build a first-order Takagi-Sugeno model using Simpful
-
-        if kwargs['save_kfold_models'] is True:
-            simpbuilder = SugenoFISBuilder(
-                fold_dict['antecedent_parameters'],
-                fold_dict['consequent_parameters'],
-                fold_dict['selected_variable_names'],
-                normalization_values=self.normalization_values,
-                extreme_values=antecedent_estimator._extreme_values,
-                operators=kwargs["operators"],
-                save_simpful_code='Fold_' + str(fold_number) + '_Simpful_code.py',
-                fuzzy_sets_to_drop=fold_dict['what_to_drop'],
-                verbose=False,
-                categorical_indices=kwargs['categorical_indices'])
-        elif kwargs['save_kfold_models'] is False:
-            simpbuilder = SugenoFISBuilder(
-                fold_dict['antecedent_parameters'],
-                fold_dict['consequent_parameters'],
-                fold_dict['selected_variable_names'],
-                normalization_values=self.normalization_values,
-                extreme_values=antecedent_estimator._extreme_values,
-                operators=kwargs["operators"],
-                save_simpful_code=False,
-                fuzzy_sets_to_drop=fold_dict['what_to_drop'],
-                verbose=False,
-                categorical_indices=kwargs['categorical_indices'])
-        fold_dict['model'] = simpbuilder.simpfulmodel
-
-        fold_dict['performance_metric'] = self.performance_metric
-        tester = SugenoFISTester(model=fold_dict['model'], test_data=fold_dict['x_test'], variable_names=fold_dict['selected_variable_names'], golden_standard=fold_dict['y_test'])
-        fold_dict['performance'] = tester.calculate_performance(metric=fold_dict['performance_metric'])
-        return fold_dict
+from .LoadData import DataLoader
+from .Splitter import DataSplitter
+from .SimpfulModelBuilder import SugenoFISBuilder
+from .Clustering import Clusterer
+from .EstimateAntecendentSet import AntecedentEstimator
+from .FireStrengthCalculator import FireStrengthCalculator
+from .EstimateConsequentParameters import ConsequentEstimator
+from .Tester import SugenoFISTester
+from .FeatureSelection import FeatureSelector
+from .Sampler import Sampler
+import numpy as np
+
+
+class BuildTSFIS(object):
+    """
+        Learns a a new  Takagi-Sugeno fuzzy model.
+        
+        Args:
+            datapath: The path to the csv file containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
+            dataframe: Pandas dataframe containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
+            nr_clus: Number of clusters that should be identified in the data (default = 2).
+            process_categorical: Boolean to indicate whether categorical variables should be processed (default = False).
+            method: At this moment, only Takagi Sugeno models are supported (default = 'Takagi-Sugeno')
+            variable_names: Names of the variables, if not specified the names will be read from the first row of the csv file (default = None).
+            merge_threshold: Threshold for GRABS to drop fuzzy sets from the model. If the jaccard similarity between two sets is higher than this threshold, the fuzzy set will be dropped from the model.
+            **kwargs: Additional arguments to change settings of the fuzzy model.
+
+        Returns:
+            An object containing the fuzzy model, information about its setting (such as its antecedent and consequent parameters) and the different splits of the data.
+    """
+    def __init__(self, datapath=None, dataframe=None, nr_clus=None, variable_names=None, 
+            process_categorical=False, merge_threshold=1.0, setnes_threshold=1.0, verbose=False, **kwargs):
+
+        self.datapath = datapath
+        self.nr_clus = nr_clus
+        self.variable_names = variable_names
+        self._antecedent_estimator = None
+        self.verbose = verbose
+
+        # Check keyword-arguments and complete with default settings if necessary
+        if 'model_order' not in kwargs.keys(): kwargs['model_order'] = 'first'
+        if 'normalization' in kwargs.keys(): kwargs['normalize'] = kwargs['normalization']
+        if 'normalize' not in kwargs.keys(): kwargs['normalize'] = False
+        if 'imputation' not in kwargs.keys(): kwargs['imputation'] = 'knn'  # new
+        if 'percentage_training' not in kwargs.keys(): kwargs['percentage_training'] = 0.75
+        if 'oversampling' not in kwargs.keys(): kwargs['oversampling'] = False
+        if kwargs['oversampling'] is True:
+            if 'sampling_number_of_bins' not in kwargs.keys(): kwargs['sampling_number_of_bins'] = 2
+            if 'sampling_histogram' not in kwargs.keys(): kwargs['sampling_histogram'] = False
+        if 'data_delimiter' not in kwargs.keys(): kwargs['data_delimiter'] = ','
+        if 'data_split_method' not in kwargs.keys(): kwargs['data_split_method'] = 'hold-out'
+        if 'feature_selection' not in kwargs.keys(): kwargs['feature_selection'] = None
+        if 'fs_max_iter' not in kwargs.keys(): kwargs['fs_max_iter'] = 100
+        if 'cluster_method' not in kwargs.keys(): kwargs['cluster_method'] = 'fcm'
+        if 'm' not in kwargs.keys(): kwargs['m'] = '2'
+        if kwargs['cluster_method'] == 'fcm':
+            if 'fcm_max_iter' not in kwargs.keys(): kwargs['fcm_maxiter'] = 1000
+            if 'fcm_error' not in kwargs.keys(): kwargs['fcm_error'] = 0.005
+        elif kwargs['cluster_method'] == 'fst-pso':
+            if 'fstpso_n_particles' not in kwargs.keys(): kwargs['fstpso_n_particles'] = None
+            if 'fstpso_max_iter' not in kwargs.keys(): kwargs['fstpso_max_iter'] = 100
+            if 'fstpso_path_fit_dump' not in kwargs.keys(): kwargs['fstpso_path_fit_dump'] = None
+            if 'fstpso_path_sol_dump' not in kwargs.keys(): kwargs['fstpso_path_sol_dump'] = None
+        elif kwargs['cluster_method'] == 'gk':
+            if 'gk_max_iter' not in kwargs.keys(): kwargs['gk_maxiter'] = 1000
+        if 'mf_shape' not in kwargs.keys(): kwargs['mf_shape'] = 'gauss'
+        if 'operators' not in kwargs.keys(): kwargs['operators'] = None
+        if 'global_fit' not in kwargs.keys(): kwargs['global_fit'] = False
+        if 'save_simpful_code' not in kwargs.keys(): kwargs['save_simpful_code'] = True
+        if 'cv_randomID' not in kwargs.keys(): kwargs['cv_randomID'] = False
+        if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
+        if 'log_variables' not in kwargs.keys(): kwargs['log_variables'] = None
+        if 'categorical_indices' not in kwargs.keys(): kwargs['categorical_indices'] = None
+
+        if self.nr_clus is None and kwargs['feature_selection'] is None:
+            print('Error: please set pyFUME`s argument "nr_clus".')
+            import sys
+            sys.exit()
+
+        # Load the data
+        if self.datapath is None:
+            dl = DataLoader(dataframe=dataframe, normalize=kwargs['normalize'], process_categorical=process_categorical, delimiter=kwargs['data_delimiter'], log_variables=kwargs['log_variables'], categorical_indices=kwargs['categorical_indices'], verbose=self.verbose)
+        else:
+            dl = DataLoader(self.datapath, normalize=kwargs['normalize'],  process_categorical=process_categorical, delimiter=kwargs['data_delimiter'], log_variables=kwargs['log_variables'], categorical_indices=kwargs['categorical_indices'], verbose=self.verbose)
+        self.variable_names = dl.get_variable_names()
+
+        if kwargs['normalize'] is not False and kwargs['normalize'] != 'zscore':
+            self.normalization_values = list(dl.get_normalization_values())
+            self.minmax_norm_flag = True
+        else:
+            self.minmax_norm_flag = False
+            self.normalization_values = None
+
+        self.dataX = dl.get_input_data()
+        self.dataY = dl.get_target_data()
+
+        # Create a DataSplitter object
+        ds = DataSplitter()
+
+        if kwargs['data_split_method'] == 'hold-out' or kwargs['data_split_method'] == 'holdout':
+
+            if self.verbose: print(' * Hold-out method selected.')
+
+            # Split the data using the hold-out method in a training (default: 75%) 
+            # and test set (default: 25%).
+            self.x_train, self.y_train, self.x_test, self.y_test = ds.holdout(dataX=self.dataX, dataY=self.dataY, percentage_training=kwargs['percentage_training'])
+            # Check if there are any missing variables and impute them
+            if np.isnan(self.dataX).any().any() is True:
+                try:
+                    from sklearn.impute import KNNImputer
+                except ImportError:
+                    raise Exception('pyFUME tried to impute missing values, but couldn`t find \'sklearn\'. Please pip install sklearn to proceed.')
+
+                if self.verbose: print('Warning: Your data contains missing values that will be imputed using KNN.')
+                imputer = KNNImputer(n_neighbors=3, weights="uniform")
+                self.x_train = imputer.fit_transform(self.x_train)
+                self.x_test = imputer.fit_transform(self.x_test)
+
+            if kwargs['oversampling'] is True:
+                sample = Sampler(train_x=self.x_train, train_y=self.y_train, number_of_bins=kwargs['sampling_number_of_bins'], histogram=kwargs['sampling_histogram'])
+                self.x_train, self.y_train = sample.oversample()
+
+            # Perform feature selection if requested
+            if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False:
+                if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
+                fs = FeatureSelector(self.x_train, self.y_train, self.nr_clus, self.variable_names, model_order= kwargs['model_order'], performance_metric = kwargs['performance_metric'], verbose=self.verbose)
+
+                # Keep copies of the training and test set before dropping unselected features
+                self.x_train_before_fs = self.x_train.copy()
+                self.x_test_before_fs = self.x_test.copy()
+
+                if kwargs['feature_selection'] == 'wrapper' or kwargs['feature_selection'] == 'sfs' or kwargs['feature_selection'] == 'SFS':
+                    self.selected_feature_indices, self.selected_variable_names = fs.wrapper()
+                elif kwargs['feature_selection'] == 'logwrapper':
+                    self.selected_feature_indices, self.selected_variable_names, self.log_indices, self.log_variable_names = fs.log_wrapper()
+                elif kwargs['feature_selection'] == 'fst-pso' or kwargs['feature_selection'] == 'fstpso' or kwargs['feature_selection'] == 'pso' or kwargs['feature_selection'] is True:
+                    fst_pso_maxiter = 100
+                    if "fstpso_max_iter" in kwargs.keys(): fst_pso_maxiter = kwargs['fstpso_max_iter']
+                    self.selected_feature_indices, self.selected_variable_names, self.nr_clus = fs.fst_pso_feature_selection(max_iter=fst_pso_maxiter, **kwargs)
+                self.x_train = self.x_train[:, self.selected_feature_indices]
+                self.x_test = self.x_test[:, self.selected_feature_indices]
+
+            elif kwargs['feature_selection'] is None:
+                self.selected_variable_names = self.variable_names
+
+            # Cluster the data, log-transform when needed.
+            if kwargs['feature_selection'] == 'logwrapper':
+                # Use log transformed variables if needed
+                self.log_x_train = self.x_train.copy()
+                for i in self.log_indices:
+                    self.log_x_train[i]= np.log(self.x_train[i])
+                cl = Clusterer(x_train=self.log_x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
+            else:
+                # Cluster the training data (in input-output space)
+                cl = Clusterer(x_train=self.x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
+
+            if kwargs['cluster_method'] == 'fcm':
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fcm', fcm_m=kwargs['m'],
+                    fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
+            elif kwargs['cluster_method'] == 'gk':
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='gk')
+            elif kwargs['cluster_method'] == 'fst-pso':
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fstpso',
+                    fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
+                    fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
+            elif kwargs['cluster_method'] == 'fuzzy_k_protoypes' or kwargs['cluster_method'] == 'fkp' or kwargs['cluster_method'] == 'FKP':
+                if 'categorical_indices' in kwargs:
+                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp',
+                                                                                categorical_indices=kwargs['categorical_indices'])
+                else:
+                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp')
+            else:
+                print('ERROR: Choose a valid clustering method.')
+                import sys
+                sys.exit()
+
+            # Estimate the membership funtions of the system (default shape: gauss)
+            self._antecedent_estimator = AntecedentEstimator(x_train=self.x_train, partition_matrix=self.partition_matrix)
+    
+            self.antecedent_parameters = self._antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'], merge_threshold=merge_threshold, setnes_threshold=setnes_threshold, categorical_indices=kwargs['categorical_indices'])
+            what_to_drop = self._antecedent_estimator._info_for_simplification
+
+            # Calculate the firing strengths
+            fsc = FireStrengthCalculator(antecedent_parameters=self.antecedent_parameters, nr_clus=self.nr_clus,
+                                         variable_names=self.selected_variable_names,
+                                         **kwargs)
+            self.firing_strengths = fsc.calculate_fire_strength(data=self.x_train)
+
+            # Estimate the parameters of the consequent
+            ce = ConsequentEstimator(x_train=self.x_train, y_train=self.y_train, firing_strengths=self.firing_strengths,
+                                     categorical_indices=kwargs['categorical_indices'])
+            if kwargs['model_order'] == 'first':
+                self.consequent_parameters = ce.suglms()
+            elif kwargs['model_order'] == 'zero':
+                self.consequent_parameters = ce.zero_order()
+            else:
+                raise Exception("pyFUME currently only supports zero-order (model_order = 'zero') and first-order (model_order = 'first') fuzzy models.")
+
+            # Build a first-order Takagi-Sugeno model using Simpful
+            simpbuilder = SugenoFISBuilder(
+                self.antecedent_parameters,
+                self.consequent_parameters,
+                self.selected_variable_names,
+                normalization_values=self.normalization_values,
+                extreme_values=self._antecedent_estimator._extreme_values,
+                model_order=kwargs["model_order"],
+                operators=kwargs["operators"],
+                save_simpful_code=kwargs['save_simpful_code'],
+                fuzzy_sets_to_drop=what_to_drop,
+                setnes_dropped_antecedents=self._antecedent_estimator._setnes_removed_sets,
+                verbose=self.verbose,
+                categorical_indices=kwargs['categorical_indices'])
+
+            self.model = simpbuilder.simpfulmodel
+
+        elif kwargs['data_split_method'] == 'cross_validation' or kwargs['data_split_method'] == 'k-fold_cross_validation' or kwargs['data_split_method'] == 'crossvalidation' or kwargs['data_split_method'] == 'cv' or kwargs['data_split_method'] == 'kfold':
+            if 'number_of_folds' not in kwargs.keys(): kwargs['number_of_folds'] = 10
+            if self.verbose: print('K-fold cross validation was selected. The number of folds (k) equals', kwargs['number_of_folds'])
+            # if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
+            if 'save_kfold_models' not in kwargs.keys(): kwargs['save_kfold_models'] = True
+            if 'kfold_indices' not in kwargs.keys(): kwargs['kfold_indices'] = None
+            if 'paralellization_kfold' not in kwargs.keys(): kwargs['paralellization_kfold'] = False
+
+            # Create lists with test indices for each fold.
+            if kwargs['kfold_indices'] is None:
+                self.fold_indices = ds.kfold(data_length=len(self.dataX), number_of_folds=kwargs['number_of_folds'])
+            else:
+                self.fold_indices = kwargs['kfold_indices']
+
+            self.performance_metric = kwargs['performance_metric']
+            # fold_indices=pd.read_csv('./fold_indices.csv', header=None)
+            # self.fold_indices=fold_indices.to_numpy()
+
+            # Create folder to store developed models
+            if kwargs['save_kfold_models'] is True:
+                import os, datetime
+
+                if kwargs['cv_randomID'] is True:
+                    try:
+                        import uuid
+                    except ImportError:
+                        raise Exception('pyFUME tried to generate random IDs, but couldn`t find \'uuid\'. Please pip install uuid to proceed.')
+
+                    self.folder_name = 'pyFUME runID ' + str(uuid.uuid4())
+                elif kwargs['cv_randomID'] is False:
+                    self.folder_name = 'pyFUME run ' + datetime.datetime.now().strftime("%Y-%m-%d %H.%M.%S")
+
+                owd = os.getcwd()
+                os.mkdir(self.folder_name)
+                os.chdir('./' + self.folder_name)
+
+            if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False: self.selected_features_per_fold = dict()
+            if kwargs['feature_selection'] == 'logwrapper': self.logged_features_per_fold = dict()
+
+            self.kfold_dict = dict()
+            args = []
+
+            for fold_number in range(0, kwargs['number_of_folds']):
+                if self.verbose: print('Training the model for fold', fold_number)
+                tst_idx = self.fold_indices[fold_number]
+                tst_idx = tst_idx[~np.isnan(tst_idx)]
+                tst_idx = [int(x) for x in tst_idx]
+                #np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
+                trn_idx = np.concatenate(np.delete(self.fold_indices, fold_number, axis=0))
+                trn_idx = trn_idx[~np.isnan(trn_idx)]
+                trn_idx = [int(x) for x in trn_idx]
+
+                self.x_train = np.array([self.dataX[i, :] for i in trn_idx])
+                self.x_test = np.array([self.dataX[i, :] for i in tst_idx])
+                self.y_train = np.array([self.dataY[i] for i in trn_idx])
+                self.y_test = np.array([self.dataY[i] for i in tst_idx])
+
+                if kwargs['feature_selection'] == 'logwrapper':
+                    raw_x_train = dl.get_non_normalized_x_data()
+                    self.raw_x_train = np.array([raw_x_train[i,:] for i in trn_idx])
+
+                args.append([fold_number, self.x_train, self.x_test, self.y_train, self.y_test])
+                nm = 'fold_' + str(fold_number)
+
+                if kwargs['paralellization_kfold'] is False:
+                    self.kfold_dict[nm] = self._create_kfold_model(*args[fold_number], **kwargs)
+
+            if kwargs['paralellization_kfold'] is True:
+                print('Paralellization of code is currently not possible yet. Coming soon!')
+
+            # import sys
+            # sys.exit(1)
+
+            # set working directory back to where script is stored
+            if kwargs['save_kfold_models'] is True:
+                os.chdir(owd)
+
+            self.performance_metric_per_fold = np.array([x['performance'] for x in self.kfold_dict.values()])
+
+            # print('The average ' + self.performance_metric + ' over ' + str(kwargs['number_of_folds']) +' folds is ' + str(np.mean(self.performance_metric_per_fold)) +' (with st. dev. ' + str(np.std(self.performance_metric_per_fold)) + '). \nThe best model was created in fold ' +  str(np.argmin(self.performance_metric_per_fold)) + ' with ' + self.performance_metric +  ' = ' + str(np.min(self.performance_metric_per_fold)) + '.')
+            if self.verbose: print('The average ' + self.performance_metric + ' over ' + str(kwargs['number_of_folds']) + ' folds is ' + str(np.mean(self.performance_metric_per_fold)) + ' (with st. dev. ' + str(np.std(self.performance_metric_per_fold)) + ').')
+
+        elif kwargs['data_split_method'] == 'no_split':
+            if self.verbose: print('No test data will be split off, all data will be used for training.')
+
+            self.x_train = self.dataX.copy()
+            self.y_train = self.dataY.copy()
+
+            if np.isnan(self.dataX).any().any() is True:
+                try:
+                    from sklearn.impute import KNNImputer
+                except ImportError:
+                    raise Exception('pyFUME tried to impute missing values, but couldn`t find \'sklearn\'. Please pip install sklearn to proceed.')
+
+                if self.verbose: print('Warning: Your data contains missing values that will be imputed using KNN.')
+
+                imputer = KNNImputer(n_neighbors=3, weights="uniform")
+                self.x_train = imputer.fit_transform(self.x_train)
+
+            if kwargs['oversampling'] is True:
+                sample = Sampler(train_x=self.x_train, train_y=self.y_train, number_of_bins=kwargs['sampling_number_of_bins'], histogram=kwargs['sampling_histogram'])
+                self.x_train, self.y_train = sample.oversample()
+
+            # Perform feature selection if requested
+            if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False:
+                if 'performance_metric' not in kwargs.keys(): kwargs['performance_metric'] = 'MAE'
+                fs = FeatureSelector(self.x_train, self.y_train, self.nr_clus, self.variable_names, model_order=kwargs['model_order'], performance_metric = kwargs['performance_metric'], verbose=self.verbose)
+
+                # Keep copies of the training and test set before dropping unselected features
+                self.x_train_before_fs = self.x_train.copy()
+
+                if kwargs['feature_selection'] == 'wrapper' or kwargs['feature_selection'] == 'sfs' or kwargs['feature_selection'] == 'SFS':
+                    self.selected_feature_indices, self.variable_names = fs.wrapper()
+                elif kwargs['feature_selection'] == 'logwrapper':
+                    self.selected_feature_indices, self.selected_variable_names, self.log_indices, self.log_variable_names = fs.log_wrapper(raw_data = self.raw_x_train)
+                elif kwargs['feature_selection'] == 'fst-pso' or kwargs['feature_selection'] == 'fstpso' or kwargs['feature_selection'] == 'pso' or kwargs['feature_selection'] is True:
+                    self.selected_feature_indices, self.selected_variable_names, self.nr_clus = fs.fst_pso_feature_selection(max_iter=kwargs['fstpso_max_iter'], **kwargs)
+                else:
+                    raise Exception('Feature selection method not (yet) implemented.')
+
+                self.x_train = self.x_train[:, self.selected_feature_indices]
+
+            elif kwargs['feature_selection'] is None:
+                self.selected_variable_names = self.variable_names
+
+            # Cluster the data, log-transform when needed.
+            if kwargs['feature_selection'] == 'logwrapper':
+                # Use log transformed variables if needed
+                self.log_x_train = self.x_train.copy()
+                for i in self.log_indices:
+                    self.log_x_train[i] = np.log(self.x_train[i])
+                cl = Clusterer(x_train=self.log_x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
+            else:
+                # Cluster the training data (in input-output space)
+                cl = Clusterer(x_train=self.x_train, y_train=self.y_train, nr_clus=self.nr_clus, verbose=self.verbose)
+
+            if kwargs['cluster_method'] == 'fcm':
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fcm', fcm_m=kwargs['m'],
+                    fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
+            elif kwargs['cluster_method'] == 'gk':
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='gk')
+            elif kwargs['cluster_method'] == 'fst-pso':
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fstpso',
+                    fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
+                    fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
+            elif kwargs['cluster_method'] == 'fuzzy_k_protoypes' or kwargs['cluster_method'] == 'fkp' or kwargs['cluster_method'] == 'FKP':
+                if 'categorical_indices' in kwargs:
+                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp',
+                                                                                categorical_indices=kwargs['categorical_indices'])
+                else:
+                    self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp')
+            else:
+                print('ERROR: Choose a valid clustering method.')
+                import sys
+                sys.exit()
+
+            # Estimate the membership funtions of the system (default shape: gauss)
+            self._antecedent_estimator = AntecedentEstimator(self.x_train, self.partition_matrix)
+
+            self.antecedent_parameters = self._antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'],
+                                                                                merge_threshold=merge_threshold,
+                                                                                categorical_indices=kwargs['categorical_indices'])
+            what_to_drop = self._antecedent_estimator._info_for_simplification
+
+            # Calculate the firing strengths
+            fsc = FireStrengthCalculator(self.antecedent_parameters, self.nr_clus, self.selected_variable_names, **kwargs)
+            self.firing_strengths = fsc.calculate_fire_strength(self.x_train)
+
+            # Estimate the parameters of the consequent
+            ce = ConsequentEstimator(self.x_train, self.y_train, self.firing_strengths,
+                                     categorical_indices=kwargs['categorical_indices'])
+            if kwargs['model_order'] == 'first':
+                self.consequent_parameters = ce.suglms()
+            elif kwargs['model_order'] == 'zero':
+                self.consequent_parameters = ce.zero_order()
+            else:
+                raise Exception("pyFUME currently only supports zero-order (model_order = 'zero') and first-order (model_order = 'first') fuzzy models.")
+
+            # Build a first-order Takagi-Sugeno model using Simpful
+            simpbuilder = SugenoFISBuilder(
+                self.antecedent_parameters,
+                self.consequent_parameters,
+                self.selected_variable_names,
+                normalization_values=self.normalization_values,
+                extreme_values=self._antecedent_estimator._extreme_values,
+                model_order=kwargs["model_order"],
+                operators=kwargs["operators"],
+                save_simpful_code=kwargs['save_simpful_code'],
+                fuzzy_sets_to_drop=what_to_drop,
+                verbose=self.verbose,
+                categorical_indices=kwargs['categorical_indices'])
+
+            self.model = simpbuilder.simpfulmodel
+
+        else:
+            print('ERROR: invalid data splitting method chosen. Training will be aborted.')
+            import sys
+            sys.exit()
+
+    def _create_kfold_model(self, fold_number, x_train, x_test, y_train, y_test, merge_threshold=1.0, **kwargs):
+
+        # Create a dictionary to keep track of settings and results
+        fold_dict = dict()
+
+        fold_dict['fold_number'] = fold_number
+        fold_dict['x_train'] = x_train
+        fold_dict['x_test'] = x_test
+        fold_dict['y_train'] = y_train
+        fold_dict['y_test'] = y_test
+        fold_dict['GRABS_threshold'] = merge_threshold
+        fold_dict['nr_clus'] = self.nr_clus
+
+        if np.isnan(fold_dict['x_train']).any().any() is True:
+            try:
+                from sklearn.impute import KNNImputer
+            except ImportError:
+                raise Exception('pyFUME tried to impute missing values, but couldn`t find \'sklearn\'. Please pip install sklearn to proceed.')
+
+            if self.verbose: print('Warning: Your data contains missing values that will be imputed using KNN.')
+            imputer = KNNImputer(n_neighbors=3, weights="uniform")
+            tmp = imputer.fit_transform(fold_dict['x_train'])
+            fold_dict['x_train'] = tmp
+            fold_dict['x_test'] = imputer.fit_transform(fold_dict['x_test'])
+
+        if kwargs['oversampling'] is True:
+            sample = Sampler(train_x=fold_dict['x_train'], train_y=fold_dict['y_train'], number_of_bins=kwargs['sampling_number_of_bins'], histogram=kwargs['sampling_histogram'])
+            fold_dict['x_train'], fold_dict['y_train'] = sample.oversample()
+
+        # Perform feature selection if requested
+        if kwargs['feature_selection'] is not None and kwargs['feature_selection'] is not False:
+            fs = FeatureSelector(fold_dict['x_train'], fold_dict['y_train'], self.nr_clus, self.variable_names, model_order= kwargs['model_order'], performance_metric = kwargs['performance_metric'], verbose=self.verbose)
+            fold_dict['x_train_before_fs'] = fold_dict['x_train'].copy()
+            fold_dict['x_test_before_fs'] = fold_dict['x_test'].copy()
+
+            if kwargs['feature_selection'] == 'wrapper' or kwargs['feature_selection'] == 'sfs' or kwargs['feature_selection'] == 'SFS':
+                fold_dict['selected_feature_indices'], fold_dict['selected_variable_names']=fs.wrapper()
+            elif kwargs['feature_selection'] == 'logwrapper':
+                raw_xdata = self.raw_x_train
+                fold_dict['selected_feature_indices'], fold_dict['selected_variable_names'], fold_dict['log_indices'], fold_dict['log_variable_names'] = fs.log_wrapper(raw_data = raw_xdata)
+            elif kwargs['feature_selection'] == 'fst-pso' or kwargs['feature_selection'] == 'fstpso' or kwargs['feature_selection'] == 'pso' or kwargs['feature_selection'] == True:
+                fold_dict['selected_feature_indices'], fold_dict['selected_variable_names'], fold_dict['nr_clus'] = fs.fst_pso_feature_selection(max_iter=kwargs['fstpso_max_iter'], **kwargs)
+
+            tmp = fold_dict['x_train']
+            idx = fold_dict['selected_feature_indices']
+            fold_dict['x_train'] = tmp[:, idx]
+
+            tmp = fold_dict['x_test']
+            fold_dict['x_test'] = tmp[:, idx]
+
+        elif kwargs['feature_selection'] is None:
+            fold_dict['selected_variable_names'] = self.variable_names
+
+        # Cluster the data, log-transform when needed.
+        if kwargs['feature_selection'] == 'logwrapper':
+            # Use log transformed variables if needed
+            tmp = fold_dict['x_train'].copy()
+            idx = fold_dict['log_indices']
+            for i in idx:
+                tmp[i] = np.log(tmp[i])
+            fold_dict['log_x_train'] = tmp
+            cl = Clusterer(x_train=fold_dict['log_x_train'], y_train=fold_dict['y_train'], nr_clus=fold_dict['nr_clus'], verbose=self.verbose)
+        else:
+            cl = Clusterer(x_train=fold_dict['x_train'], y_train=fold_dict['y_train'], nr_clus=fold_dict['nr_clus'], verbose=self.verbose)
+
+        if kwargs['cluster_method'] == 'fcm':
+            fold_dict['cluster_centers'], fold_dict['partition_matrix'], _ = cl.cluster(method='fcm', fcm_m=kwargs['m'],
+                fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
+        elif kwargs['cluster_method'] == 'fst-pso':
+            fold_dict['cluster_centers'], fold_dict['partition_matrix'], _ = cl.cluster(method='fstpso',
+                fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
+                fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
+        elif kwargs['cluster_method'] == 'gk':
+            fold_dict['cluster_centers'], fold_dict['partition_matrix'], _ = cl.cluster(method='gk')
+        elif kwargs['cluster_method'] == 'fuzzy_k_protoypes' or kwargs['cluster_method'] == 'fkp' or kwargs['cluster_method'] == 'FKP':
+            if 'categorical_indices' in kwargs:
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp',
+                                                                            categorical_indices=kwargs['categorical_indices'])
+            else:
+                self.cluster_centers, self.partition_matrix, _ = cl.cluster(method='fkp')
+        else:
+            print('ERROR: Choose a valid clustering method.')
+            import sys
+            sys.exit()
+
+        # Estimate the membership funtions of the system (default shape: gauss)
+        antecedent_estimator = AntecedentEstimator(fold_dict['x_train'], fold_dict['partition_matrix'])
+
+        fold_dict['antecedent_parameters'] = antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'],
+                                                                              merge_threshold=fold_dict['GRABS_threshold'],
+                                                                              categorical_indices=kwargs['categorical_indices'])
+        fold_dict['what_to_drop'] = antecedent_estimator._info_for_simplification
+
+        # Calculate the firing strengths
+        fsc = FireStrengthCalculator(antecedent_parameters=fold_dict['antecedent_parameters'],
+                                     nr_clus=fold_dict['nr_clus'], variable_names=fold_dict['selected_variable_names'], **kwargs)
+        fold_dict['firing_strengths'] = fsc.calculate_fire_strength(data=fold_dict['x_train'])
+
+        # Estimate the parameters of the consequent
+        ce = ConsequentEstimator(fold_dict['x_train'], fold_dict['y_train'], fold_dict['firing_strengths'],
+                                 categorical_indices=kwargs['categorical_indices'])
+        fold_dict['consequent_parameters'] = ce.suglms()
+
+        # Build a first-order Takagi-Sugeno model using Simpful
+
+        if kwargs['save_kfold_models'] is True:
+            simpbuilder = SugenoFISBuilder(
+                fold_dict['antecedent_parameters'],
+                fold_dict['consequent_parameters'],
+                fold_dict['selected_variable_names'],
+                normalization_values=self.normalization_values,
+                extreme_values=antecedent_estimator._extreme_values,
+                operators=kwargs["operators"],
+                save_simpful_code='Fold_' + str(fold_number) + '_Simpful_code.py',
+                fuzzy_sets_to_drop=fold_dict['what_to_drop'],
+                verbose=False,
+                categorical_indices=kwargs['categorical_indices'])
+        elif kwargs['save_kfold_models'] is False:
+            simpbuilder = SugenoFISBuilder(
+                fold_dict['antecedent_parameters'],
+                fold_dict['consequent_parameters'],
+                fold_dict['selected_variable_names'],
+                normalization_values=self.normalization_values,
+                extreme_values=antecedent_estimator._extreme_values,
+                operators=kwargs["operators"],
+                save_simpful_code=False,
+                fuzzy_sets_to_drop=fold_dict['what_to_drop'],
+                verbose=False,
+                categorical_indices=kwargs['categorical_indices'])
+        fold_dict['model'] = simpbuilder.simpfulmodel
+
+        fold_dict['performance_metric'] = self.performance_metric
+        tester = SugenoFISTester(model=fold_dict['model'], test_data=fold_dict['x_test'], variable_names=fold_dict['selected_variable_names'], golden_standard=fold_dict['y_test'])
+        fold_dict['performance'] = tester.calculate_performance(metric=fold_dict['performance_metric'])
+        return fold_dict
```

### Comparing `pyFUME-0.3.1/pyfume/Clustering.py` & `pyfume-0.3.4/pyfume/Clustering.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,624 +1,624 @@
-import numpy as np
-from scipy.spatial.distance import cdist
-from scipy.linalg import norm
-
-
-# from random import seed
-
-# To do:
-# Give option to cluster in input or input-output space?
-# More clustering methods
-# data input argument
-
-
-class Clusterer(object):
-    """
-        Creates a new clusterer object that can cluster the (training) data in the input-output feature space. The user should specify the 'data'argument OR the 'x_train' and 'y_train' argument.
-        
-        Args:
-            nr_clus: Number of clusters that should be identified in the data.  
-            x_train: The input data (default = None).
-            y_train: The output data (true label/golden standard) (default = None).
-            data: The data to be clustered (default = None).
-    """
-
-    def __init__(self, nr_clus, x_train=None, y_train=None, data=None, relational_data=None, verbose=False):
-        self.x_train = x_train
-        self.y_train = y_train
-        self.nr_clus = nr_clus
-        self._verbose = verbose
-
-        if data is None and (x_train is None or y_train is None) and relational_data is None:
-            raise Exception("Please specify a valid dataset for clustering.")
-        elif data is not None:
-            self.data = data
-        elif relational_data is not None:
-            self.relational_data = relational_data
-        else:
-            self.data = np.concatenate((self.x_train, np.expand_dims(self.y_train, axis=1)),
-                                       axis=1)  # .reshape(len(self.y_train),1)),axis=1)
-
-    def cluster(self, method="fcm", **kwargs):
-        """
-        Clusters the data using the clustering method as specified by the user.
-            
-        Args:
-                method: The method used for the clustering. The user can choose 'fcm' (fuzzy c-means), 'fst-pso' (fst-pso based clustering) and 'gk' (Gustafson-Kessel).
-                **kwargs: Additional arguments to change settings of the clustering method.     
-                
-        Returns: 
-                Tuple containing (centers, partion_matrix, jm)   
-                    - centers: The location of the identified cluster centers.
-                    -  partition_matrix: A matrix containing the cluster memberships of each data point to each of the clusters.
-                    - jm: Fitness function of the best solution.
-        """
-
-        if self._verbose:
-            print(" * Clustering method:", method)
-
-        try:
-            self.m = kwargs["m"]
-        except:
-            self.m = 2
-
-        if method == "fcm" or method == 'gk' or method == 'GK' or method == 'Gustafson-Kessel' or method == 'gustafson-kessel' or method == 'g-k' or method == "pfcm" or method == "fst-pso" or method == "fstpso":
-            assert self.data is not None or (
-                        self.x_train is not None and self.y_train is not None), 'Please specify the data tobe clustered.'
-        elif method == 'RFCM' or method == "relational_clustering" or method == "relational" or method == "RC":
-            assert self.relational_data is not None, 'Please specify the relational data matrix.'
-
-        if method == "fcm":
-            try:
-                max_iter = kwargs["fcm_max_iter"]
-            except:
-                max_iter = 1000
-            try:
-                error = kwargs["fcm_error"]
-            except:
-                error = 0.005
-
-            centers, partition_matrix, jm = self._fcm(data=self.data, n_clusters=self.nr_clus, m=self.m,
-                                                      max_iter=max_iter, error=error)
-
-        elif method == 'gk' or method == 'GK' or method == 'Gustafson-Kessel' or method == 'gustafson-kessel' or method == 'g-k':
-            try:
-                max_iter = kwargs["gk_max_iter"]
-            except:
-                max_iter = 1000
-            try:
-                error = kwargs["gk_error"]
-            except:
-                error = 0.005
-            centers, partition_matrix, jm = self._gk(m=self.m, max_iter=max_iter)
-
-        elif method == "pfcm":
-            try:
-                n = kwargs["pfcm_n"]
-            except:
-                n = 2
-            try:
-                max_iter = kwargs["pfcm_max_iter"]
-            except:
-                max_iter = 1000
-            try:
-                error = kwargs["pfcm_error"]
-            except:
-                error = 0.005
-            try:
-                a = kwargs["pfcm_a"]
-            except:
-                a = 0.5
-            try:
-                b = kwargs["pfcm_b"]
-            except:
-                b = 0.5
-
-            centers, partition_matrix, typicality_matrix, jm = self._pfcm(data=self.data, n_clusters=self.nr_clus,
-                                                                          m=self.m, n=n, max_iter=max_iter, error=error,
-                                                                          a=a, b=b)
-
-        elif method == "fst-pso" or method == "fstpso":
-            try:
-                max_iter = kwargs["fstpso_max_iter"]
-            except:
-                max_iter = 100
-            try:
-                n_particles = kwargs["fstpso_n_particles"]
-            except:
-                n_particles = None
-            try:
-                path_fit_dump = kwargs["fstpso_path_fit_dump"]
-            except:
-                path_fit_dump = None
-            try:
-                path_sol_dump = kwargs["fstpso_path_sol_dump"]
-            except:
-                path_sol_dump = None
-            centers, partition_matrix, jm = self._fstpso(data=self.data, n_clusters=self.nr_clus, max_iter=max_iter,
-                                                         n_particles=n_particles, m=self.m, path_fit_dump=path_fit_dump,
-                                                         path_sol_dump=path_sol_dump)
-
-        elif method == 'RFCM' or method == 'rfcm' or method == "relational_clustering" or method == "relational" or method == "RC":
-            try:
-                max_iter = kwargs["RFCM_max_iter"]
-            except:
-                max_iter = 100
-            try:
-                error = kwargs["RFCM_error"]
-            except:
-                error = 0.005
-            try:
-                initialization = kwargs["RFCM_initialization"]
-            except:
-                initialization = 'random_initialization'
-
-            centers, partition_matrix, jm = self._rfcm(R=self.relational_data, c=self.nr_clus, m=self.m, epsilon=error,
-                                                       maxIter=max_iter, initType=initialization)
-
-        elif method == 'FKP' or method == 'fkp' or method == "fuzzy_k_protoypes":
-            try:
-                max_iter = kwargs["FKP_max_iter"]
-            except:
-                max_iter = 100
-            try:
-                error = kwargs["FKP_error"]
-            except:
-                error = 0.005
-            try:
-                cat_ind = kwargs["categorical_indices"]
-            except:
-                import pandas as pd
-                df = pd.DataFrame(self.data)
-                catvar = df.apply(pd.Series.nunique) == 2
-                if self._verbose:
-                    print('The following variables were recognized as being binaries, and are therefore treated '
-                          'as categorical variables for clustering: ', catvar[catvar == True])
-                cat_ind = np.where(catvar)[0]
-                # raise Exception('To utilize fuzzy K-prototypes clustering, the keyword "categorical_indices" should be specified.')
-
-            centers, partition_matrix, jm = self._fuzzy_k_protoypes(data=self.data, categorical_indices=cat_ind,
-                                                                    n_clusters=self.nr_clus, m=self.m,
-                                                                    max_iter=max_iter, error=error)
-
-        return centers, partition_matrix, jm
-
-    def _fcm(self, data, n_clusters, m=2, max_iter=1000, error=0.005):
-        # data: 2d array, size (N, S). N is the number of instances; S is the number of variables
-        # n_clusters: number of clusters
-        # m: fuzzy clustering coefficient
-        # max_it: maximum number of iterations, default=1000
-        # error: stopping criterion, default=0.005
-        # seed: seed for random initialization of u matrix
-
-        n_instances = data.shape[0]
-
-        # randomly initaliaze u
-        u = np.random.rand(n_instances, n_clusters)
-        u = np.fmax(u, np.finfo(np.float64).eps)
-        ut = u.T
-
-        for it in range(0, max_iter):
-            # copy old u matrix
-            u_old = ut.copy()
-            u_old /= np.ones((n_clusters, 1)).dot(np.atleast_2d(u_old.sum(axis=0)))
-            u_old = np.fmax(u_old, np.finfo(np.float64).eps)
-
-            # elevate to m
-            um = u_old ** m
-
-            # calculate cluster centers
-            centers = um.dot(data) / (np.ones((data.shape[1], 1)).dot(np.atleast_2d(um.sum(axis=1))).T)
-
-            # calculate distances
-            dist = cdist(centers, data, metric='euclidean')
-            dist = np.fmax(dist, np.finfo(np.float64).eps)
-
-            # calculate objective
-            jm = (um * dist ** 2).sum()
-
-            # calculate new u matrix
-            ut = dist ** (- 2. / (m - 1))
-            ut /= np.ones((n_clusters, 1)).dot(np.atleast_2d(ut.sum(axis=0)))
-
-            # stopping criterion
-            if np.linalg.norm(ut - u_old) < error:
-                break
-
-        partition_matrix = ut.T
-        return centers, partition_matrix, jm
-
-    def _fuzzy_k_protoypes(self, data, categorical_indices, n_clusters, m=2, max_iter=1000, error=0.005):
-        # data: 2d array, size (N, S). N is the number of instances; S is the number of variables
-        # n_clusters: number of clusters
-        # m: fuzzy clustering coefficient
-        # max_it: maximum number of iterations, default=1000
-        # error: stopping criterion, default=0.005
-        # seed: seed for random initialization of u matrix
-
-        n_instances = data.shape[0]
-
-        # randomly initaliaze u
-        u = np.random.rand(n_instances, n_clusters)
-        u = np.fmax(u, np.finfo(np.float64).eps)
-        ut = u.T
-
-        for it in range(0, max_iter):
-            # copy old u matrix
-            u_old = ut.copy()
-            u_old /= np.ones((n_clusters, 1)).dot(np.atleast_2d(u_old.sum(axis=0)))
-            u_old = np.fmax(u_old, np.finfo(np.float64).eps)
-
-            # elevate to m
-            um = u_old ** m
-
-            # calculate cluster centers
-            prototypes = self._FKP_prototypes(um, data, n_clusters, categorical_indices)
-
-            # calculate distances
-            dist = self._FKP_distances(prototypes, data, categorical_indices, numerical_metric='euclidean')
-            dist = np.fmax(dist, np.finfo(np.float64).eps)
-
-            # calculate objective
-            jm = (um * dist ** 2).sum()
-
-            # calculate new u matrix
-            ut = dist ** (- 2. / (m - 1))
-            ut /= np.ones((n_clusters, 1)).dot(np.atleast_2d(ut.sum(axis=0)))
-
-            # stopping criterion
-            if np.linalg.norm(ut - u_old) < error:
-                break
-
-        partition_matrix = ut.T
-
-        return prototypes, partition_matrix, jm
-
-    def _FKP_prototypes(self, um, data, n_clusters, categorical_indices):
-        # Find the means to locate the cluster centers
-        prototypes = um.dot(data) / (np.ones((data.shape[1], 1)).dot(np.atleast_2d(um.sum(axis=1))).T)
-
-        # Transpose um
-        um = um.T
-
-        # Replace the mean with the mode if the variable is categorical
-        for col_idx in categorical_indices:
-            cats = np.unique([data[:, col_idx]])  # Find unique categories
-            for clus in range(n_clusters):  # Find for each cluster the max summed membership
-                freq = dict()
-                for c in cats:
-                    umpc = um[data[:, col_idx] == c, :]
-                    freq[c] = sum(umpc[:, clus])
-                prototypes[clus, col_idx] = max(freq, key=freq.get)
-        return prototypes
-
-    def _FKP_distances(self, prototypes, data, categorical_indices, numerical_metric='euclidean'):
-        # If the data is categorical, determine if value is different from the mode
-        # if data point == mode, distance = np.finfo(np.float64).eps
-        # if data point ~= mode, distance i= 1
-        dummy_proto = prototypes.copy()
-        dummy_proto[:, categorical_indices] = 1
-
-        distances = np.empty([prototypes.shape[0], data.shape[0]])
-        for i in range(prototypes.shape[0]):
-            dummy_data = data.copy()
-            for cat in categorical_indices:
-                dummy_data[:, cat] = np.where(data[:, cat] == prototypes[i, cat], 1, 0)
-            # If the data is numerical use euclidean distance
-            distances[i, :] = cdist(dummy_proto[i, :, None].T, dummy_data, metric='euclidean')
-        return distances
-
-    def _fstpso(self, data, n_clusters, max_iter=100, n_particles=None, m=2, path_fit_dump=None, path_sol_dump=None):
-        # data: 2d array, size (N, S). N is the number of instances; S is the number of variables
-        # n_clusters: number of clusters
-        # max_iter: number of maximum iterations of FST-PSO, default is 100
-        # n_particles: number of particles in the swarm, if None it is automatically set by FST-PSO
-        # m: fuzzy clustering coefficient
-        # path_fit_dump: path to the file where the best fitness score at each iteration will be dumped
-        # path_sol_dump: path to the file where the best solution at each iteration will be dumped
-
-        try:
-            from fstpso import FuzzyPSO
-        except:
-            print("ERROR: please, pip install fst-pso to use this functionality.")
-
-        # n_instances = data.shape[0]
-        n_variables = data.shape[1]
-
-        # set search space boundaries
-        bounds = [0] * n_variables
-        for i in range(n_variables):
-            x = min([row[i] for row in data])
-            y = max([row[i] for row in data])
-            bounds[i] = [x, y]
-
-        search_space = []
-        for i in bounds:
-            search_space.extend([i] * n_clusters)
-
-        # initializing FST-PSO
-        FP = FuzzyPSO()
-        FP.set_search_space(search_space)
-        if n_particles != None: FP.set_swarm_size(n_particles)
-
-        # generally better results are obtained with this rule disabled
-        FP.disable_fuzzyrule_minvelocity()
-
-        # fitness function definition
-        def fitness(particle):
-            particle = list(map(float, particle))
-            centers = np.reshape(particle, (n_variables, n_clusters)).T
-
-            # calculating fitness value of found solution
-            dist = cdist(data, centers, metric='sqeuclidean')
-
-            um = np.zeros(np.shape(dist))
-            for i in range(np.shape(um)[0]):
-                for j in range(np.shape(um)[1]):
-                    um[i][j] = np.sum(np.power(np.divide(dist[i][j], dist[i]), float(1 / (m - 1))))
-            um = np.reciprocal(um)
-
-            um_power = np.power(um, m)
-
-            fitness_value = np.sum(np.multiply(um_power, dist))
-            return fitness_value
-
-        # fitness function setting
-        FP.set_fitness(fitness, skip_test=True)
-
-        # execute optimization
-        result = FP.solve_with_fstpso(max_iter=max_iter, dump_best_fitness=path_fit_dump,
-                                      dump_best_solution=path_sol_dump)
-
-        # reshaping centers
-        solution = list(map(float, result[0].X))
-        centers = np.reshape(solution, (n_variables, n_clusters)).T
-
-        # calculating membership matrix
-        dist = cdist(data, centers, metric='sqeuclidean')
-        um = np.zeros(np.shape(dist))
-        for i in range(np.shape(um)[0]):
-            for j in range(np.shape(um)[1]):
-                um[i][j] = np.sum(np.power(np.divide(dist[i][j], dist[i]), float(1 / (m - 1))))
-        partition_matrix = np.reciprocal(um)
-
-        # final fitness value
-        jm = result[1]
-
-        return centers, partition_matrix, jm
-
-    def _pfcm(self, data, n_clusters, m=2, max_iter=1000, error=0.005, a=0.5, b=0.5, n=2):
-
-        # data: Dataset to be clustered, with size M-by-N, where M is the number of data points
-        # and N is the number of coordinates for each data point.
-        # c : Number of clusters
-        # m: fuzzy clustering coefficient (default = 2)
-        # max_iter: Maximum number of iterations (default = 1000)
-        # error : stopping criterion (default=0.005)
-        # a: Relative importane of fuzzy membership (default = 0.5)
-        # b: Relative importane of typicality values (default = 0.5)
-        # n: User-defined constant n (default = 2)
-
-        # Return values:
-        # centers: The locations of the found clusters centers
-        # partition_matrix: Partition matrix
-        # typicality_matrix: Typicality Matrix
-        # jm: The objective funtion for U and T
-
-        # Randomly initiaize the partitioning matrix and typicality matrix
-        n_instances = len(data)
-        partition_matrix = np.random.rand(n_instances, n_clusters)
-        partition_matrix = np.fmax(partition_matrix, np.finfo(np.float64).eps)  # avoid 0's in the matrix
-        typicality_matrix = np.random.rand(n_instances, n_clusters)
-        typicality_matrix = np.fmax(typicality_matrix, np.finfo(np.float64).eps)  # avoid 0's in the matrix
-
-        # Pre-allocation
-        jm = np.zeros(shape=(max_iter, 1))
-        g = np.zeros(shape=(n_clusters, data.shape[0]))
-
-        for i in range(max_iter):
-
-            # Perform one iteration of PFCM
-            partition_matrix, typicality_matrix, centers, jm[i], g = self._pstepfcm(data=data, U=partition_matrix,
-                                                                                    T=typicality_matrix, m=m, a=a, b=b,
-                                                                                    n=n_clusters, g=g)
-
-            # Stopping criterion: Stop if objective value does inrease < error
-            if abs(jm[i] - jm[i - 1]) < error:
-                break
-
-        return centers, partition_matrix, typicality_matrix, jm
-
-    def _pstepfcm(self, data, U, T, g, m=2, n=2, a=0.5, b=0.5):
-        # copy old u and t matrix and center locations
-        um = U ** m
-        tf = T ** n
-        tfo = (1 - T) ** n
-        centers = (np.dot(a * um + b * tf, data).T / np.sum(a * um + b * tf, axis=1).T).T
-
-        # Calculate distances between data points and cluster centers            
-        dist = cdist(centers, data, metric='euclidean')
-        dist = np.fmax(dist, np.finfo(np.float64).eps)
-
-        # calculate value of objective funtion
-        jm = np.sum(np.sum(np.power(dist, 2) * (a * um + b * tf), axis=0)) + np.sum(g * np.sum(tfo, axis=0))
-
-        # calculate new u and t matrix
-        g = um * np.power(dist, 2) / (np.sum(um, axis=0))
-        tmp = np.power(dist, (-2 / (m - 1)))
-        U = tmp / (np.sum(tmp, axis=0))
-        tmpt = np.power((b / g) * np.power(dist, 2), (1 / (n - 1)))
-        T = 1 / (1 + tmpt)
-
-        return U, T, centers, jm, g
-
-    ### Gustafson-Kessel
-
-    def _gk(self, m=2, max_iter=1000, error=0.01):
-
-        # Initialize the partition matrix
-        u = np.random.dirichlet(np.ones(self.data.shape[0]), size=self.nr_clus)
-
-        centers = []
-        iteration = 0
-
-        while iteration < max_iter:
-            u_old = u.copy()  # keep old partition matrix to evaluate stopping criterium
-
-            # Caluculate the locations of the cluster centers
-            centers = self._next_centers_gk(data=self.data, u=u, m=m)
-
-            # Calculate the covariance matrix
-            f = self._covariance_gk(data=self.data, v=centers, u=u, m=m)
-
-            # Calculate the distance between cluster centers and data points
-            dist = self._distance_gk(data=self.data, v=centers, f=f)
-
-            # calculate objective
-            jm = (u * dist ** 2).sum()
-
-            # Update the partition matrix
-            u = self._next_u_gk(dist)
-            iteration += 1
-
-            # Stopping criteria
-            if norm(u - u_old) < error:
-                iteration = max_iter
-
-        u = np.transpose(u)
-        return centers, u, jm
-
-    def _next_centers_gk(self, data, u, m=2):
-        um = u ** m
-        return ((um @ data).T / um.sum(axis=1)).T
-
-    def _covariance_gk(self, data, v, u, m=2):
-        um = u ** self.m
-
-        denominator = um.sum(axis=1).reshape(-1, 1, 1)
-        temp = np.expand_dims(data.reshape(data.shape[0], 1, -1) - v.reshape(1, v.shape[0], -1), axis=3)
-        temp = np.matmul(temp, temp.transpose((0, 1, 3, 2)))
-        numerator = um.transpose().reshape(um.shape[1], um.shape[0], 1, 1) * temp
-        numerator = numerator.sum(0)
-
-        return numerator / denominator
-
-    def _distance_gk(self, data, v, f):
-        dif = np.expand_dims(data.reshape(data.shape[0], 1, -1) - v.reshape(1, v.shape[0], -1), axis=3)
-        determ = np.sign(np.linalg.det(f)) * (np.abs(np.linalg.det(f))) ** (1 / self.m)
-        det_time_inv = determ.reshape(-1, 1, 1) * np.linalg.pinv(f)
-        temp = np.matmul(dif.transpose((0, 1, 3, 2)), det_time_inv)
-        output = np.matmul(temp, dif).squeeze().T
-        return np.fmax(output, 1e-8)
-
-    def _next_u_gk(self, d):
-        power = float(1 / (self.m - 1))
-        d = d.transpose()
-        new_u = d.reshape((d.shape[0], 1, -1)).repeat(d.shape[-1], axis=1)
-        new_u = np.power(d[:, None, :] / new_u.transpose((0, 2, 1)), power)
-        new_u = 1 / new_u.sum(1)
-        new_u = new_u.transpose()
-        return new_u
-
-    ### Relational Clustering
-
-    def _RF_init_centers(self, number_of_clusters, number_of_data_points, relational_data,
-                         method='random_initialization'):
-        # Initialize the cluster cenetrs for  relational fuzzy clustering
-        if method == 'random_initialization':  # Use random numbers
-            V = np.random.rand(number_of_clusters, number_of_data_points)
-            V = V / V.sum(axis=1, keepdims=True)
-        elif method == 'randomly_choose_c_rows':  # Use randomly selected data points as initial centers
-            idx = np.random.choice(number_of_data_points, size=number_of_clusters, replace=False)
-            V = relational_data[idx, :]
-            V = V / V.sum(axis=1, keepdims=True)
-
-        return V
-
-    def _rfcm(self, R, c, m=2, epsilon=0.005, maxIter=1000, initType='random_initialization'):
-
-        #  Relational Fuzzy c-Means (RFCM) for clustering dissimilarity data as
-        #  proposed in [1]. RFCM is the relational dual of Fuzzy c-Means (FCM),
-        #  so it expects the input relational matrix R to be Euclidean.
-        #
-        # Output:
-        #               U: fuzzy partition matrix / membership matrix
-        #               V: cluster centers/coefficients
-        #               jm: Fitness function of the best solution
-        #
-        # Input:
-        # R         - the relational (dissimilarity) data matrix of size n x n
-        # c         - number of clusters to be identified
-        # m         - fuzzifier, default 2
-        # epsilon   - convergence criteria, default 0.0001
-        # initType  - initialize relational cluster centers V, default random initialization
-        #               random initialization
-        #               randomly choose c rows from D
-        # maxIter   - the maximum number fo iterations, default 100
-        #
-        # Refs:
-        #   [1] Hathaway, R. J., Davenport, J. W., & Bezdek, J. C. (1989). Relational duals 
-        #   of the c-means clustering algorithms. Pattern recognition, 22(2), 205-212. 
-
-        # Initialize variables
-        D = np.array(R)  # Relational data
-        n = len(D)  # Number of data points
-        d = np.zeros([c, n])
-        numIter = 0
-        stepSize = epsilon
-
-        # Initialize the membership matrix randomly
-        U = np.random.rand(c, n)
-        U = np.fmax(U, np.finfo(np.float64).eps)
-
-        # Initialize the (relational) cluster centers
-        V = self._RF_init_centers(number_of_clusters=c, number_of_data_points=n, relational_data=D, method=initType)
-
-        # Begin the main loop:
-        while numIter < maxIter and stepSize >= epsilon:
-            U0 = U
-
-            # Compute the relational distances d between clusters centers V and data points D
-            d = np.zeros([c, n])
-            for i in range(0, c):
-                Vi = V[i, :]
-                tmp1 = D @ Vi.T
-                tmp2 = Vi @ D @ Vi.T / 2
-                d[i, :] = tmp1 - tmp2
-                print('d', np.min(d), np.max(d))
-
-                # Update the partition matrix U
-            d = np.power(d, 1 / (m - 1))
-            tmp1 = np.divide(1, d)
-            tmp2 = np.ones([c, 1]) * sum(tmp1)
-            U = np.divide(np.divide(1, d), tmp2)
-
-            # Update cluster centers V
-            V = np.power(U, m)
-            V = V / V.sum(axis=1, keepdims=True)
-
-            # Calculate the fitness value
-            jm = (U * d ** 2).sum()
-
-            # Update the step size
-            stepSize = np.amax(abs(U - U0))
-            print('U', np.min(U), np.max(U))
-            print('U0', np.min(U0), np.max(U0))
-
-            if self._verbose is True:
-                print('pyFUME just finished iteration ' + str(numIter) + ' of the RFCM clustering algoritm.')
-
-            numIter = numIter + 1
-
-        # Return the cluster center location, the membership matrix and the fitness value
-        return V, U, jm
-
-
-if __name__ == '__main__':
-    data = np.genfromtxt('data.csv', delimiter=',')
-    cat_ind = [3]
-
-    cl = Clusterer(data=data, nr_clus=3)
-
-    # Perform FKP
-    cluster_centers, partition_matrix, _ = cl._fuzzy_k_protoypes(data=data, categorical_indices=cat_ind, n_clusters=2,
-                                                                 m=2, max_iter=1000, error=0.005)
+import numpy as np
+from scipy.spatial.distance import cdist
+from scipy.linalg import norm
+
+
+# from random import seed
+
+# To do:
+# Give option to cluster in input or input-output space?
+# More clustering methods
+# data input argument
+
+
+class Clusterer(object):
+    """
+        Creates a new clusterer object that can cluster the (training) data in the input-output feature space. The user should specify the 'data'argument OR the 'x_train' and 'y_train' argument.
+        
+        Args:
+            nr_clus: Number of clusters that should be identified in the data.  
+            x_train: The input data (default = None).
+            y_train: The output data (true label/golden standard) (default = None).
+            data: The data to be clustered (default = None).
+    """
+
+    def __init__(self, nr_clus, x_train=None, y_train=None, data=None, relational_data=None, verbose=False):
+        self.x_train = x_train
+        self.y_train = y_train
+        self.nr_clus = nr_clus
+        self._verbose = verbose
+
+        if data is None and (x_train is None or y_train is None) and relational_data is None:
+            raise Exception("Please specify a valid dataset for clustering.")
+        elif data is not None:
+            self.data = data
+        elif relational_data is not None:
+            self.relational_data = relational_data
+        else:
+            self.data = np.concatenate((self.x_train, np.expand_dims(self.y_train, axis=1)),
+                                       axis=1)  # .reshape(len(self.y_train),1)),axis=1)
+
+    def cluster(self, method="fcm", **kwargs):
+        """
+        Clusters the data using the clustering method as specified by the user.
+            
+        Args:
+                method: The method used for the clustering. The user can choose 'fcm' (fuzzy c-means), 'fst-pso' (fst-pso based clustering) and 'gk' (Gustafson-Kessel).
+                **kwargs: Additional arguments to change settings of the clustering method.     
+                
+        Returns: 
+                Tuple containing (centers, partion_matrix, jm)   
+                    - centers: The location of the identified cluster centers.
+                    -  partition_matrix: A matrix containing the cluster memberships of each data point to each of the clusters.
+                    - jm: Fitness function of the best solution.
+        """
+
+        if self._verbose:
+            print(" * Clustering method:", method)
+
+        try:
+            self.m = kwargs["m"]
+        except:
+            self.m = 2
+
+        if method == "fcm" or method == 'gk' or method == 'GK' or method == 'Gustafson-Kessel' or method == 'gustafson-kessel' or method == 'g-k' or method == "pfcm" or method == "fst-pso" or method == "fstpso":
+            assert self.data is not None or (
+                        self.x_train is not None and self.y_train is not None), 'Please specify the data tobe clustered.'
+        elif method == 'RFCM' or method == "relational_clustering" or method == "relational" or method == "RC":
+            assert self.relational_data is not None, 'Please specify the relational data matrix.'
+
+        if method == "fcm":
+            try:
+                max_iter = kwargs["fcm_max_iter"]
+            except:
+                max_iter = 1000
+            try:
+                error = kwargs["fcm_error"]
+            except:
+                error = 0.005
+
+            centers, partition_matrix, jm = self._fcm(data=self.data, n_clusters=self.nr_clus, m=self.m,
+                                                      max_iter=max_iter, error=error)
+
+        elif method == 'gk' or method == 'GK' or method == 'Gustafson-Kessel' or method == 'gustafson-kessel' or method == 'g-k':
+            try:
+                max_iter = kwargs["gk_max_iter"]
+            except:
+                max_iter = 1000
+            try:
+                error = kwargs["gk_error"]
+            except:
+                error = 0.005
+            centers, partition_matrix, jm = self._gk(m=self.m, max_iter=max_iter)
+
+        elif method == "pfcm":
+            try:
+                n = kwargs["pfcm_n"]
+            except:
+                n = 2
+            try:
+                max_iter = kwargs["pfcm_max_iter"]
+            except:
+                max_iter = 1000
+            try:
+                error = kwargs["pfcm_error"]
+            except:
+                error = 0.005
+            try:
+                a = kwargs["pfcm_a"]
+            except:
+                a = 0.5
+            try:
+                b = kwargs["pfcm_b"]
+            except:
+                b = 0.5
+
+            centers, partition_matrix, typicality_matrix, jm = self._pfcm(data=self.data, n_clusters=self.nr_clus,
+                                                                          m=self.m, n=n, max_iter=max_iter, error=error,
+                                                                          a=a, b=b)
+
+        elif method == "fst-pso" or method == "fstpso":
+            try:
+                max_iter = kwargs["fstpso_max_iter"]
+            except:
+                max_iter = 100
+            try:
+                n_particles = kwargs["fstpso_n_particles"]
+            except:
+                n_particles = None
+            try:
+                path_fit_dump = kwargs["fstpso_path_fit_dump"]
+            except:
+                path_fit_dump = None
+            try:
+                path_sol_dump = kwargs["fstpso_path_sol_dump"]
+            except:
+                path_sol_dump = None
+            centers, partition_matrix, jm = self._fstpso(data=self.data, n_clusters=self.nr_clus, max_iter=max_iter,
+                                                         n_particles=n_particles, m=self.m, path_fit_dump=path_fit_dump,
+                                                         path_sol_dump=path_sol_dump)
+
+        elif method == 'RFCM' or method == 'rfcm' or method == "relational_clustering" or method == "relational" or method == "RC":
+            try:
+                max_iter = kwargs["RFCM_max_iter"]
+            except:
+                max_iter = 100
+            try:
+                error = kwargs["RFCM_error"]
+            except:
+                error = 0.005
+            try:
+                initialization = kwargs["RFCM_initialization"]
+            except:
+                initialization = 'random_initialization'
+
+            centers, partition_matrix, jm = self._rfcm(R=self.relational_data, c=self.nr_clus, m=self.m, epsilon=error,
+                                                       maxIter=max_iter, initType=initialization)
+
+        elif method == 'FKP' or method == 'fkp' or method == "fuzzy_k_protoypes":
+            try:
+                max_iter = kwargs["FKP_max_iter"]
+            except:
+                max_iter = 100
+            try:
+                error = kwargs["FKP_error"]
+            except:
+                error = 0.005
+            try:
+                cat_ind = kwargs["categorical_indices"]
+            except:
+                import pandas as pd
+                df = pd.DataFrame(self.data)
+                catvar = df.apply(pd.Series.nunique) == 2
+                if self._verbose:
+                    print('The following variables were recognized as being binaries, and are therefore treated '
+                          'as categorical variables for clustering: ', catvar[catvar == True])
+                cat_ind = np.where(catvar)[0]
+                # raise Exception('To utilize fuzzy K-prototypes clustering, the keyword "categorical_indices" should be specified.')
+
+            centers, partition_matrix, jm = self._fuzzy_k_protoypes(data=self.data, categorical_indices=cat_ind,
+                                                                    n_clusters=self.nr_clus, m=self.m,
+                                                                    max_iter=max_iter, error=error)
+
+        return centers, partition_matrix, jm
+
+    def _fcm(self, data, n_clusters, m=2, max_iter=1000, error=0.005):
+        # data: 2d array, size (N, S). N is the number of instances; S is the number of variables
+        # n_clusters: number of clusters
+        # m: fuzzy clustering coefficient
+        # max_it: maximum number of iterations, default=1000
+        # error: stopping criterion, default=0.005
+        # seed: seed for random initialization of u matrix
+
+        n_instances = data.shape[0]
+
+        # randomly initaliaze u
+        u = np.random.rand(n_instances, n_clusters)
+        u = np.fmax(u, np.finfo(np.float64).eps)
+        ut = u.T
+
+        for it in range(0, max_iter):
+            # copy old u matrix
+            u_old = ut.copy()
+            u_old /= np.ones((n_clusters, 1)).dot(np.atleast_2d(u_old.sum(axis=0)))
+            u_old = np.fmax(u_old, np.finfo(np.float64).eps)
+
+            # elevate to m
+            um = u_old ** m
+
+            # calculate cluster centers
+            centers = um.dot(data) / (np.ones((data.shape[1], 1)).dot(np.atleast_2d(um.sum(axis=1))).T)
+
+            # calculate distances
+            dist = cdist(centers, data, metric='euclidean')
+            dist = np.fmax(dist, np.finfo(np.float64).eps)
+
+            # calculate objective
+            jm = (um * dist ** 2).sum()
+
+            # calculate new u matrix
+            ut = dist ** (- 2. / (m - 1))
+            ut /= np.ones((n_clusters, 1)).dot(np.atleast_2d(ut.sum(axis=0)))
+
+            # stopping criterion
+            if np.linalg.norm(ut - u_old) < error:
+                break
+
+        partition_matrix = ut.T
+        return centers, partition_matrix, jm
+
+    def _fuzzy_k_protoypes(self, data, categorical_indices, n_clusters, m=2, max_iter=1000, error=0.005):
+        # data: 2d array, size (N, S). N is the number of instances; S is the number of variables
+        # n_clusters: number of clusters
+        # m: fuzzy clustering coefficient
+        # max_it: maximum number of iterations, default=1000
+        # error: stopping criterion, default=0.005
+        # seed: seed for random initialization of u matrix
+
+        n_instances = data.shape[0]
+
+        # randomly initaliaze u
+        u = np.random.rand(n_instances, n_clusters)
+        u = np.fmax(u, np.finfo(np.float64).eps)
+        ut = u.T
+
+        for it in range(0, max_iter):
+            # copy old u matrix
+            u_old = ut.copy()
+            u_old /= np.ones((n_clusters, 1)).dot(np.atleast_2d(u_old.sum(axis=0)))
+            u_old = np.fmax(u_old, np.finfo(np.float64).eps)
+
+            # elevate to m
+            um = u_old ** m
+
+            # calculate cluster centers
+            prototypes = self._FKP_prototypes(um, data, n_clusters, categorical_indices)
+
+            # calculate distances
+            dist = self._FKP_distances(prototypes, data, categorical_indices, numerical_metric='euclidean')
+            dist = np.fmax(dist, np.finfo(np.float64).eps)
+
+            # calculate objective
+            jm = (um * dist ** 2).sum()
+
+            # calculate new u matrix
+            ut = dist ** (- 2. / (m - 1))
+            ut /= np.ones((n_clusters, 1)).dot(np.atleast_2d(ut.sum(axis=0)))
+
+            # stopping criterion
+            if np.linalg.norm(ut - u_old) < error:
+                break
+
+        partition_matrix = ut.T
+
+        return prototypes, partition_matrix, jm
+
+    def _FKP_prototypes(self, um, data, n_clusters, categorical_indices):
+        # Find the means to locate the cluster centers
+        prototypes = um.dot(data) / (np.ones((data.shape[1], 1)).dot(np.atleast_2d(um.sum(axis=1))).T)
+
+        # Transpose um
+        um = um.T
+
+        # Replace the mean with the mode if the variable is categorical
+        for col_idx in categorical_indices:
+            cats = np.unique([data[:, col_idx]])  # Find unique categories
+            for clus in range(n_clusters):  # Find for each cluster the max summed membership
+                freq = dict()
+                for c in cats:
+                    umpc = um[data[:, col_idx] == c, :]
+                    freq[c] = sum(umpc[:, clus])
+                prototypes[clus, col_idx] = max(freq, key=freq.get)
+        return prototypes
+
+    def _FKP_distances(self, prototypes, data, categorical_indices, numerical_metric='euclidean'):
+        # If the data is categorical, determine if value is different from the mode
+        # if data point == mode, distance = np.finfo(np.float64).eps
+        # if data point ~= mode, distance i= 1
+        dummy_proto = prototypes.copy()
+        dummy_proto[:, categorical_indices] = 1
+
+        distances = np.empty([prototypes.shape[0], data.shape[0]])
+        for i in range(prototypes.shape[0]):
+            dummy_data = data.copy()
+            for cat in categorical_indices:
+                dummy_data[:, cat] = np.where(data[:, cat] == prototypes[i, cat], 1, 0)
+            # If the data is numerical use euclidean distance
+            distances[i, :] = cdist(dummy_proto[i, :, None].T, dummy_data, metric='euclidean')
+        return distances
+
+    def _fstpso(self, data, n_clusters, max_iter=100, n_particles=None, m=2, path_fit_dump=None, path_sol_dump=None):
+        # data: 2d array, size (N, S). N is the number of instances; S is the number of variables
+        # n_clusters: number of clusters
+        # max_iter: number of maximum iterations of FST-PSO, default is 100
+        # n_particles: number of particles in the swarm, if None it is automatically set by FST-PSO
+        # m: fuzzy clustering coefficient
+        # path_fit_dump: path to the file where the best fitness score at each iteration will be dumped
+        # path_sol_dump: path to the file where the best solution at each iteration will be dumped
+
+        try:
+            from fstpso import FuzzyPSO
+        except:
+            print("ERROR: please, pip install fst-pso to use this functionality.")
+
+        # n_instances = data.shape[0]
+        n_variables = data.shape[1]
+
+        # set search space boundaries
+        bounds = [0] * n_variables
+        for i in range(n_variables):
+            x = min([row[i] for row in data])
+            y = max([row[i] for row in data])
+            bounds[i] = [x, y]
+
+        search_space = []
+        for i in bounds:
+            search_space.extend([i] * n_clusters)
+
+        # initializing FST-PSO
+        FP = FuzzyPSO()
+        FP.set_search_space(search_space)
+        if n_particles != None: FP.set_swarm_size(n_particles)
+
+        # generally better results are obtained with this rule disabled
+        FP.disable_fuzzyrule_minvelocity()
+
+        # fitness function definition
+        def fitness(particle):
+            particle = list(map(float, particle))
+            centers = np.reshape(particle, (n_variables, n_clusters)).T
+
+            # calculating fitness value of found solution
+            dist = cdist(data, centers, metric='sqeuclidean')
+
+            um = np.zeros(np.shape(dist))
+            for i in range(np.shape(um)[0]):
+                for j in range(np.shape(um)[1]):
+                    um[i][j] = np.sum(np.power(np.divide(dist[i][j], dist[i]), float(1 / (m - 1))))
+            um = np.reciprocal(um)
+
+            um_power = np.power(um, m)
+
+            fitness_value = np.sum(np.multiply(um_power, dist))
+            return fitness_value
+
+        # fitness function setting
+        FP.set_fitness(fitness, skip_test=True)
+
+        # execute optimization
+        result = FP.solve_with_fstpso(max_iter=max_iter, dump_best_fitness=path_fit_dump,
+                                      dump_best_solution=path_sol_dump)
+
+        # reshaping centers
+        solution = list(map(float, result[0].X))
+        centers = np.reshape(solution, (n_variables, n_clusters)).T
+
+        # calculating membership matrix
+        dist = cdist(data, centers, metric='sqeuclidean')
+        um = np.zeros(np.shape(dist))
+        for i in range(np.shape(um)[0]):
+            for j in range(np.shape(um)[1]):
+                um[i][j] = np.sum(np.power(np.divide(dist[i][j], dist[i]), float(1 / (m - 1))))
+        partition_matrix = np.reciprocal(um)
+
+        # final fitness value
+        jm = result[1]
+
+        return centers, partition_matrix, jm
+
+    def _pfcm(self, data, n_clusters, m=2, max_iter=1000, error=0.005, a=0.5, b=0.5, n=2):
+
+        # data: Dataset to be clustered, with size M-by-N, where M is the number of data points
+        # and N is the number of coordinates for each data point.
+        # c : Number of clusters
+        # m: fuzzy clustering coefficient (default = 2)
+        # max_iter: Maximum number of iterations (default = 1000)
+        # error : stopping criterion (default=0.005)
+        # a: Relative importane of fuzzy membership (default = 0.5)
+        # b: Relative importane of typicality values (default = 0.5)
+        # n: User-defined constant n (default = 2)
+
+        # Return values:
+        # centers: The locations of the found clusters centers
+        # partition_matrix: Partition matrix
+        # typicality_matrix: Typicality Matrix
+        # jm: The objective funtion for U and T
+
+        # Randomly initiaize the partitioning matrix and typicality matrix
+        n_instances = len(data)
+        partition_matrix = np.random.rand(n_instances, n_clusters)
+        partition_matrix = np.fmax(partition_matrix, np.finfo(np.float64).eps)  # avoid 0's in the matrix
+        typicality_matrix = np.random.rand(n_instances, n_clusters)
+        typicality_matrix = np.fmax(typicality_matrix, np.finfo(np.float64).eps)  # avoid 0's in the matrix
+
+        # Pre-allocation
+        jm = np.zeros(shape=(max_iter, 1))
+        g = np.zeros(shape=(n_clusters, data.shape[0]))
+
+        for i in range(max_iter):
+
+            # Perform one iteration of PFCM
+            partition_matrix, typicality_matrix, centers, jm[i], g = self._pstepfcm(data=data, U=partition_matrix,
+                                                                                    T=typicality_matrix, m=m, a=a, b=b,
+                                                                                    n=n_clusters, g=g)
+
+            # Stopping criterion: Stop if objective value does inrease < error
+            if abs(jm[i] - jm[i - 1]) < error:
+                break
+
+        return centers, partition_matrix, typicality_matrix, jm
+
+    def _pstepfcm(self, data, U, T, g, m=2, n=2, a=0.5, b=0.5):
+        # copy old u and t matrix and center locations
+        um = U ** m
+        tf = T ** n
+        tfo = (1 - T) ** n
+        centers = (np.dot(a * um + b * tf, data).T / np.sum(a * um + b * tf, axis=1).T).T
+
+        # Calculate distances between data points and cluster centers            
+        dist = cdist(centers, data, metric='euclidean')
+        dist = np.fmax(dist, np.finfo(np.float64).eps)
+
+        # calculate value of objective funtion
+        jm = np.sum(np.sum(np.power(dist, 2) * (a * um + b * tf), axis=0)) + np.sum(g * np.sum(tfo, axis=0))
+
+        # calculate new u and t matrix
+        g = um * np.power(dist, 2) / (np.sum(um, axis=0))
+        tmp = np.power(dist, (-2 / (m - 1)))
+        U = tmp / (np.sum(tmp, axis=0))
+        tmpt = np.power((b / g) * np.power(dist, 2), (1 / (n - 1)))
+        T = 1 / (1 + tmpt)
+
+        return U, T, centers, jm, g
+
+    ### Gustafson-Kessel
+
+    def _gk(self, m=2, max_iter=1000, error=0.01):
+
+        # Initialize the partition matrix
+        u = np.random.dirichlet(np.ones(self.data.shape[0]), size=self.nr_clus)
+
+        centers = []
+        iteration = 0
+
+        while iteration < max_iter:
+            u_old = u.copy()  # keep old partition matrix to evaluate stopping criterium
+
+            # Caluculate the locations of the cluster centers
+            centers = self._next_centers_gk(data=self.data, u=u, m=m)
+
+            # Calculate the covariance matrix
+            f = self._covariance_gk(data=self.data, v=centers, u=u, m=m)
+
+            # Calculate the distance between cluster centers and data points
+            dist = self._distance_gk(data=self.data, v=centers, f=f)
+
+            # calculate objective
+            jm = (u * dist ** 2).sum()
+
+            # Update the partition matrix
+            u = self._next_u_gk(dist)
+            iteration += 1
+
+            # Stopping criteria
+            if norm(u - u_old) < error:
+                iteration = max_iter
+
+        u = np.transpose(u)
+        return centers, u, jm
+
+    def _next_centers_gk(self, data, u, m=2):
+        um = u ** m
+        return ((um @ data).T / um.sum(axis=1)).T
+
+    def _covariance_gk(self, data, v, u, m=2):
+        um = u ** self.m
+
+        denominator = um.sum(axis=1).reshape(-1, 1, 1)
+        temp = np.expand_dims(data.reshape(data.shape[0], 1, -1) - v.reshape(1, v.shape[0], -1), axis=3)
+        temp = np.matmul(temp, temp.transpose((0, 1, 3, 2)))
+        numerator = um.transpose().reshape(um.shape[1], um.shape[0], 1, 1) * temp
+        numerator = numerator.sum(0)
+
+        return numerator / denominator
+
+    def _distance_gk(self, data, v, f):
+        dif = np.expand_dims(data.reshape(data.shape[0], 1, -1) - v.reshape(1, v.shape[0], -1), axis=3)
+        determ = np.sign(np.linalg.det(f)) * (np.abs(np.linalg.det(f))) ** (1 / self.m)
+        det_time_inv = determ.reshape(-1, 1, 1) * np.linalg.pinv(f)
+        temp = np.matmul(dif.transpose((0, 1, 3, 2)), det_time_inv)
+        output = np.matmul(temp, dif).squeeze().T
+        return np.fmax(output, 1e-8)
+
+    def _next_u_gk(self, d):
+        power = float(1 / (self.m - 1))
+        d = d.transpose()
+        new_u = d.reshape((d.shape[0], 1, -1)).repeat(d.shape[-1], axis=1)
+        new_u = np.power(d[:, None, :] / new_u.transpose((0, 2, 1)), power)
+        new_u = 1 / new_u.sum(1)
+        new_u = new_u.transpose()
+        return new_u
+
+    ### Relational Clustering
+
+    def _RF_init_centers(self, number_of_clusters, number_of_data_points, relational_data,
+                         method='random_initialization'):
+        # Initialize the cluster cenetrs for  relational fuzzy clustering
+        if method == 'random_initialization':  # Use random numbers
+            V = np.random.rand(number_of_clusters, number_of_data_points)
+            V = V / V.sum(axis=1, keepdims=True)
+        elif method == 'randomly_choose_c_rows':  # Use randomly selected data points as initial centers
+            idx = np.random.choice(number_of_data_points, size=number_of_clusters, replace=False)
+            V = relational_data[idx, :]
+            V = V / V.sum(axis=1, keepdims=True)
+
+        return V
+
+    def _rfcm(self, R, c, m=2, epsilon=0.005, maxIter=1000, initType='random_initialization'):
+
+        #  Relational Fuzzy c-Means (RFCM) for clustering dissimilarity data as
+        #  proposed in [1]. RFCM is the relational dual of Fuzzy c-Means (FCM),
+        #  so it expects the input relational matrix R to be Euclidean.
+        #
+        # Output:
+        #               U: fuzzy partition matrix / membership matrix
+        #               V: cluster centers/coefficients
+        #               jm: Fitness function of the best solution
+        #
+        # Input:
+        # R         - the relational (dissimilarity) data matrix of size n x n
+        # c         - number of clusters to be identified
+        # m         - fuzzifier, default 2
+        # epsilon   - convergence criteria, default 0.0001
+        # initType  - initialize relational cluster centers V, default random initialization
+        #               random initialization
+        #               randomly choose c rows from D
+        # maxIter   - the maximum number fo iterations, default 100
+        #
+        # Refs:
+        #   [1] Hathaway, R. J., Davenport, J. W., & Bezdek, J. C. (1989). Relational duals 
+        #   of the c-means clustering algorithms. Pattern recognition, 22(2), 205-212. 
+
+        # Initialize variables
+        D = np.array(R)  # Relational data
+        n = len(D)  # Number of data points
+        d = np.zeros([c, n])
+        numIter = 0
+        stepSize = epsilon
+
+        # Initialize the membership matrix randomly
+        U = np.random.rand(c, n)
+        U = np.fmax(U, np.finfo(np.float64).eps)
+
+        # Initialize the (relational) cluster centers
+        V = self._RF_init_centers(number_of_clusters=c, number_of_data_points=n, relational_data=D, method=initType)
+
+        # Begin the main loop:
+        while numIter < maxIter and stepSize >= epsilon:
+            U0 = U
+
+            # Compute the relational distances d between clusters centers V and data points D
+            d = np.zeros([c, n])
+            for i in range(0, c):
+                Vi = V[i, :]
+                tmp1 = D @ Vi.T
+                tmp2 = Vi @ D @ Vi.T / 2
+                d[i, :] = tmp1 - tmp2
+                print('d', np.min(d), np.max(d))
+
+                # Update the partition matrix U
+            d = np.power(d, 1 / (m - 1))
+            tmp1 = np.divide(1, d)
+            tmp2 = np.ones([c, 1]) * sum(tmp1)
+            U = np.divide(np.divide(1, d), tmp2)
+
+            # Update cluster centers V
+            V = np.power(U, m)
+            V = V / V.sum(axis=1, keepdims=True)
+
+            # Calculate the fitness value
+            jm = (U * d ** 2).sum()
+
+            # Update the step size
+            stepSize = np.amax(abs(U - U0))
+            print('U', np.min(U), np.max(U))
+            print('U0', np.min(U0), np.max(U0))
+
+            if self._verbose is True:
+                print('pyFUME just finished iteration ' + str(numIter) + ' of the RFCM clustering algoritm.')
+
+            numIter = numIter + 1
+
+        # Return the cluster center location, the membership matrix and the fitness value
+        return V, U, jm
+
+
+if __name__ == '__main__':
+    data = np.genfromtxt('data.csv', delimiter=',')
+    cat_ind = [3]
+
+    cl = Clusterer(data=data, nr_clus=3)
+
+    # Perform FKP
+    cluster_centers, partition_matrix, _ = cl._fuzzy_k_protoypes(data=data, categorical_indices=cat_ind, n_clusters=2,
+                                                                 m=2, max_iter=1000, error=0.005)
```

### Comparing `pyFUME-0.3.1/pyfume/EstimateAntecendentSet.py` & `pyfume-0.3.4/pyfume/EstimateAntecendentSet.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,431 +1,431 @@
-import numpy as np
-from collections import Counter
-from simpful import SingletonsSet
-from scipy.optimize import curve_fit
-from numpy import linspace, array
-from collections import defaultdict
-
-
-def is_complete(G):
-    nodelist = G.nodes
-    H = G.subgraph(nodelist)
-    n = len(nodelist)
-    return H.size() == n * (n - 1) / 2
-
-
-class AntecedentEstimator(object):
-    """
-        Creates a new antecedent estimator object.
-        
-        Args:
-            x_train: The input data.
-            partition_matrix: The partition matrix of the input data (generated 
-                by a clustering the data).
-    """
-
-    def __init__(self, x_train, partition_matrix):
-        self.xtrain = x_train
-        self.partition_matrix = partition_matrix
-        self._info_for_simplification = None
-        self._calculate_all_extreme_values()
-        self._setnes_removed_sets = defaultdict(list)
-
-    def determineMF(self, mf_shape='gauss', merge_threshold=1.0, categorical_indices=None, setnes_threshold=1.0, global_singleton=None):
-        """
-            Estimates the parameters of the membership functions that are used 
-            as antecedents of the fuzzy rules.
-            
-            Args:
-                mf_shape: The desired shape of the fuzzy sets. The user can choose
-                    from 'gauss' (gaussian), 'gauss2' (double gaussion) or 'sigmf' 
-                    (sigmoidal) (default = gauss).
-                merge_threshold: Threshold for the merging of fuzzy sets for 
-                    the GRABS approach. By default no merging takes place 
-                    (default = 1.0).
-            Returns:
-                A list with the estimated parameters of the membership functions (format if gauss: mu, sigma; if gauss2: mu1, sigma1, mu2, sigma2)
-        """
-        mf_list = []
-
-        # mf_list is structured as follows:
-        # - an outer list of V variables
-        # - each item of the outer list contains C fuzzy set, one for each cluster
-        number_of_variables = self.xtrain.shape[1]
-        for i in range(0, number_of_variables):
-            if categorical_indices is not None and i in categorical_indices:
-                if global_singleton is not None:
-                    unique_values = np.unique(self.xtrain[:, i])
-                    if global_singleton == 'softmax':
-                        from scipy.special import softmax
-                        pm = softmax(self.partition_matrix, axis=0)
-                    else:
-                        pm = self.partition_matrix
-                    pml = []
-                    for uv in unique_values:
-                        pmn = pm[self.xtrain[:, i] == uv].sum(axis=0)
-                        pml.append(list(pmn / pmn.sum()))
-                    sets = list(zip(*pml))
-                    for s in sets:
-                        mf_list.append(('singleton', list(zip(unique_values, s))))
-                else:
-                    xin = self.xtrain[:, i]
-                    cluster_frequencies_counter = [[] for _ in range(0, self.partition_matrix.shape[1])]
-                    unique_values = set()
-                    for j in range(0, self.partition_matrix.shape[0]):
-                        cl = np.argmax(self.partition_matrix[j, :])  # Determine the cluster the instance belongs to the most
-                        unique_values.add(xin[j])
-                        cluster_frequencies_counter[cl].append(xin[j])
-                    cluster_frequencies = {}
-                    value_frequencies = {k: [] for k in unique_values}  # used to force the sum for each variable to 1
-                    for j, clf in enumerate(cluster_frequencies_counter):
-                        total_number = len(clf)
-                        counter = Counter(clf)
-                        # k is the element of the universe of discourse and n / total_number is the membership function
-                        tmp_dict = {}
-                        for k, n in counter.items():
-                            freq = n / total_number
-                            tmp_dict[k] = freq
-                            value_frequencies[k].append(freq)
-                        cluster_frequencies[j] = tmp_dict
-                    # Force sum to 1 for each value of the categorical feature
-                    # Computing the total sum for each value
-                    total_sums = {k: sum(value_frequencies[k]) for k in unique_values}
-                    for j in cluster_frequencies:
-                        mfs = []
-                        for k in unique_values:
-                            if k in cluster_frequencies[j]:
-                                mfs.append((k, cluster_frequencies[j][k] / total_sums[k]))
-                            else:
-                                mfs.append((k, 0.0))
-                        prm = ('singleton', mfs)
-                        mf_list.append(prm)
-            else:
-                xin = self.xtrain[:, i]
-                if all(y in (0, 1) for y in xin):  # Add noise to binary variables
-                    noise = np.random.normal(0, 0.001, xin.shape[0])
-                    xin = xin + noise
-
-                for j in range(0, self.partition_matrix.shape[1]):
-                    mfin = self.partition_matrix[:, j]
-                    mf, xx = self._convexMF(xin=xin, mfin=mfin)
-                    prm = self._fitMF(x=xx, mf=mf, mf_shape=mf_shape)
-                    mf_list.append(prm)
-
-        if merge_threshold < 1.0 or setnes_threshold < 1.0:
-            self._check_similarities(mf_list, number_of_variables, threshold=merge_threshold, setnes_threshold=setnes_threshold)
-
-        # print(self._info_for_simplification)
-
-        return mf_list
-
-    def is_subclique(self, G, nodelist):
-        H = G.subgraph(nodelist)
-        n = len(nodelist)
-        return H.size() == n * (n - 1) / 2
-
-    def _extreme_values_for_variable(self, v):
-        return min(self.xtrain.T[v]), max(self.xtrain.T[v])
-
-    def _calculate_all_extreme_values(self):
-        num_variables = len(self.xtrain.T)
-        self._extreme_values = [self._extreme_values_for_variable(v) for v in range(num_variables)]
-
-    def _check_similarities(self, mf_list, number_of_variables,
-            approx_points=100,
-            threshold=1.,
-            setnes_threshold=1.,
-            verbose=True
-            ):
-
-        number_of_clusters = len(mf_list) // number_of_variables
-
-        from collections import defaultdict
-
-        things_to_be_removed = defaultdict(list)
-
-        """ 
-            This function assesses the pair-wise similarities between 
-            the clusters mapped on each variable.
-            It returns a dictionary of this kind:
-            variable -> list of similar couples for that variable + jaccard sim
-
-        """
-
-        for v in range(number_of_variables):
-
-            if verbose:
-                print(" * Trying to simplify variable", v)
-
-            mi, ma = self._extreme_values_for_variable(v)
-            points = np.linspace(mi, ma, approx_points)
-
-            for c1 in range(number_of_clusters):
-                for c2 in range(c1 + 1, number_of_clusters):
-
-                    index1 = v * number_of_clusters + c1
-                    index2 = v * number_of_clusters + c2
-                    funname1, params1 = mf_list[index1]
-                    funname2, params2 = mf_list[index2]
-
-                    if funname1 == "gauss":
-
-                        from numpy import linspace, array
-
-                        first_cluster = array([self._gaussmf(x, params1[0], params1[1]) for x in points])
-                        second_cluster = array([self._gaussmf(x, params2[0], params2[1]) for x in points])
-
-                        intersection = sum([min(x, y) for x, y in zip(first_cluster, second_cluster)])
-                        union = sum([max(x, y) for x, y in zip(first_cluster, second_cluster)])
-
-                        jaccardsim = (intersection / union)
-
-                        if jaccardsim > threshold:
-                            things_to_be_removed[v].append([c1, c2, jaccardsim])
-
-                            # print("%.2f is fine" % jaccardsim)
-
-                    else:
-                        raise Exception("Not implemented yet")
-
-                # Setnes' rule simplification: detect which sets are similar to the universal set
-                #                              using Jaccard similarity and a threshold.
-                if setnes_threshold<1.:
-
-                    index1 = v*number_of_clusters + c1
-                    funname1, params1 = mf_list[index1]
-
-                    if funname1== "gauss":
-
-                        first_cluster = array([self._gaussmf(x, params1[0], params1[1]) for x in points])
-                        second_cluster = array([1 for x in points]) # universal set
-
-                        intersection = sum([min(x,y) for x,y in zip(first_cluster, second_cluster)])
-                        union        = sum([max(x,y) for x,y in zip(first_cluster, second_cluster)])
-
-                        jaccardsim = (intersection/union)
-
-                        if jaccardsim>setnes_threshold:
-                            self._setnes_removed_sets[v].append(c1)
-                            print (" * Variable %d, cluster %d is too similar to universal set (threshold: %.2f): marked for removal" % (v,c1+1,setnes_threshold))
-
-                    else:
-                        raise Exception("Setnes' simplification for non-Gaussian functions not implemented yet")
-
-
-
-        #for k,v in things_to_be_removed.items():            print (k, v)
-        #exit()
-        """
-            This function must return a dictionary of items like:
-            (variable, cluster) -> mapped_cluster
-        """
-
-        self._info_for_simplification = {}
-        for var_num, value in things_to_be_removed.items():
-
-            subcomponents = self._create_graph(value)
-
-            for subcomp in subcomponents:
-                # print (is_complete(subcomp))
-
-                if is_complete(subcomp):
-                    retained = list(subcomp.nodes())[0]
-                    # print ("retain: %d" % retained)
-                    for el in list(subcomp.nodes()):
-                        if el != retained:
-                            self._info_for_simplification[(var_num, el)] = retained
-
-        dropped_stuff = self.get_number_of_dropped_fuzzy_sets()
-        print (" * %d antecedent clauses will be simplified using a threshold %.2f" % (dropped_stuff, threshold))
-        if verbose:
-            print(" * GRABS remapping info:", self._info_for_simplification)
-            print(" * Setnes simplification dictionary variable ==> list of clusters/fuzzy sets to be removed:", self._setnes_removed_sets)
-
-        self._info_for_simplification
-
-    def get_number_of_dropped_fuzzy_sets(self):
-        return len(self._info_for_simplification)
-
-    def _create_graph(self, list_of_arcs):
-        from networkx import Graph, connected_components
-        G = Graph()
-        nodelist = []
-        for arc in list_of_arcs:
-            G.add_edge(arc[0], arc[1])
-            nodelist.append(arc[0])
-            nodelist.append(arc[1])
-        S = [G.subgraph(c).copy() for c in connected_components(G)]
-        return S
-
-    def _convexMF(self, xin, mfin, norm=1, nc=1000):
-
-        # Calculates the convex membership function that envelopes a given set of
-        # data points and their corresponding membership values. 
-
-        # Input:
-        # Xin: N x 1 input domain (column vector)
-        # MFin: N x 1 corresponding membership values 
-        # nc: number of alpha cut values to consider (default=101)
-        # norm: optional normalization flag (0: do not normalize, 1 : normalize, 
-        # default=1)
-        #
-        # Output:
-        # mf: membership values of convex function
-        # x: output domain values    
-
-        # Normalize the membership values (if requested)
-        if norm == 1:
-            mfin = np.divide(mfin, np.max(mfin))
-
-        # Initialize auxilary variables
-        acut = np.linspace(0, np.max(mfin), nc)
-        mf = np.full(2 * nc, np.nan)
-        x = np.full(2 * nc, np.nan)
-
-        if np.any(mfin > 0):
-            x[0] = np.min(xin[mfin > 0])
-            x[nc] = np.max(xin[mfin > 0])
-            mf[0] = 0
-            mf[nc] = 0
-
-        # Determine the elements in the alpha cuts
-        for i in range(0, nc):
-            if np.any(mfin > acut[i]):
-                x[i] = np.min(xin[mfin > acut[i]])
-                x[i + nc] = np.max(xin[mfin > acut[i]])
-                mf[i] = acut[i]
-                mf[i + nc] = acut[i]
-
-        # # Determine the elements in the alpha cuts    
-        # for i in range(0,nc):
-        #     tmp1 = mfin>acut[i]
-        #     if len(tmp1)==0:
-        #         tmp=xin[tmp1]
-        #         np.sort(tmp)
-        #         x[i]=tmp[0]
-        #         x[i+nc]=tmp[-1]
-        #         mf[i]=acut[i]
-        #         mf[i+nc]=acut[i]
-
-        # Delete NaNs
-        idx = np.isnan(x)
-        x = x[idx == False]
-        mf = mf[idx == False]
-
-        # Sort vectors based on membership value (descending order)
-        indmf = mf.argsort(axis=0)
-        indmf = np.flipud(indmf)
-        mf = mf[indmf]
-        x = x[indmf]
-
-        # Find duplicate values for x and onlykeep the ones with the highest membership value
-        _, ind = np.unique(x, return_index=True, return_inverse=False, return_counts=False, axis=None)
-        mf = mf[ind]
-        x = x[ind]
-
-        # Sort vectors based on x value (ascending order)
-        indx = x.argsort(axis=0)
-        mf = mf[indx]
-        x = x[indx]
-
-        xval = np.linspace(np.min(x), np.max(x), nc)
-        mf = np.interp(xval, x, mf, left=None, right=None, period=None)
-        x = xval
-        return mf, x
-
-    def _fitMF(self, x, mf, mf_shape='gauss'):
-        # Fits parametrized membership functions to a set of pointwise defined 
-        # membership values.
-        #
-        # Input:
-        # x:  N x 1 domain of input variable
-        # mf: N x 1 membership values for input data x 
-        # shape: Type of membership function to fit (possible values: 'gauss', 
-        # 'gauss2' and 'sigmf')
-        #
-        # Output:
-        # param: matrix of membership function parameters
-
-        if mf_shape == 'gauss':
-            # Determine initial parameters
-            mu = sum(x * mf) / sum(mf)
-            mf[mf == 0] = np.finfo(np.float64).eps
-            sig = np.mean(np.sqrt(-((x - mu) ** 2) / (2 * np.log(mf))))
-
-            # Fit parameters to the data using least squares
-            #            print('mu=', mu, 'sig=', sig)
-            param, _ = curve_fit(self._gaussmf, x, mf, p0=[mu, sig], bounds=((-np.inf, 0), (np.inf, np.inf)),
-                                 maxfev=10000)
-
-        elif mf_shape == 'gauss2':
-            # Determine initial parameters
-            mu1 = x[mf >= 0.95][0]
-            mu2 = x[mf >= 0.95][-1]
-            xmf = x[mf >= 0.5]
-            sig1 = (mu1 - xmf[0]) / (np.sqrt(2 * np.log(2)))
-            sig2 = (xmf[-1] - mu2) / (np.sqrt(2 * np.log(2)))
-            if sig1 == 0.0:
-                sig1 = 0.1
-            if sig2 == 0.0:
-                sig2 = 0.1
-
-            # Fit parameters to the data using least squares
-            #            print('mu1',mu1,'sig1',sig1,'mu2',mu2,'sig2',sig2)
-            param, _ = curve_fit(self._gauss2mf, x, mf, p0=[mu1, sig1, mu2, sig2], maxfev=1000,
-                                 bounds=((-np.inf, 0, -np.inf, 0), (np.inf, np.inf, np.inf, np.inf)))
-
-        elif mf_shape == 'sigmf':
-            # Determine initial parameters
-            if np.argmax(mf) - np.argmin(mf) > 0:  # if sloping to the right
-                if len(x[mf >= 0.5]) > 0:
-                    c = x[mf >= 0.5][0]
-                    s = 1
-                elif len(x[mf >= 0.5]) == 0:  # if there are no datapoints with membership larger than 0
-                    c = x[0]
-                    s = 1
-            elif np.argmax(mf) - np.argmin(mf) < 0:  # if sloping to the left
-                if len(x[mf <= 0.5]) > 0:
-                    c = x[mf <= 0.5][0]
-                    s = 1
-                elif len(x[mf <= 0.5]) == 0:  # if there are no datapoints with membership smaller than 0
-                    c = x[-1]
-                    s = 1
-                    # Fit parameters of the function to the data using non-linear least squares
-            try:
-                param, _ = curve_fit(self._sigmf, x, mf, p0=[c, s], maxfev=1000)
-            except RuntimeError:
-                print(
-                    'pyFUME attempted to fit sigmoidal shaped membership functions, but was unable to find fitting parameters. pyFUME will now terminate. Please consider using a different shape for the membership functions.')
-                import sys
-                sys.exit()
-
-        return mf_shape, param
-
-    def _gaussmf(self, x, mu, sigma, a=1):
-        # x:  (1D array)
-        # mu: Center of the bell curve (float)
-        # sigma: Width of the bell curve (float)
-        # a: normalizes the bell curve, for normal fuzzy set a=1 (float) 
-        return a * np.exp(-(x - mu) ** 2 / (2 * sigma ** 2))
-
-    def _gauss2mf(self, x, mu1, sigma1, mu2, sigma2):
-        # x: Data
-        # mu1: Center of the leftside bell curve
-        # sigma1: Standard deviation that determines the width of the leftside bell curve
-        # mu2: Center of the rightside bell curve
-        # sigma2: Standard deviation that determines the width of the rightside bell curve
-        y = np.ones(len(x))
-        idx1 = x <= mu1
-        idx2 = x > mu2
-        y[idx1] = self._gaussmf(x[idx1], mu1, sigma1)
-        y[idx2] = self._gaussmf(x[idx2], mu2, sigma2)
-        return y
-
-    def _sigmf(self, x, c, s):
-        # x: data
-        # b: x where mf is 0.5
-        # c: Controls 'width' of the sigmoidal region about `b` (magnitude); also
-        #    which side of the function is open (sign). A positive value of `a`
-        #    means the left side approaches 0.0 while the right side approaches 1,
-        #    a negative value of `c` means the opposite.
-        return 1. / (1. + np.exp(- s * (x - c)))
+import numpy as np
+from collections import Counter
+from simpful import SingletonsSet
+from scipy.optimize import curve_fit
+from numpy import linspace, array
+from collections import defaultdict
+
+
+def is_complete(G):
+    nodelist = G.nodes
+    H = G.subgraph(nodelist)
+    n = len(nodelist)
+    return H.size() == n * (n - 1) / 2
+
+
+class AntecedentEstimator(object):
+    """
+        Creates a new antecedent estimator object.
+        
+        Args:
+            x_train: The input data.
+            partition_matrix: The partition matrix of the input data (generated 
+                by a clustering the data).
+    """
+
+    def __init__(self, x_train, partition_matrix):
+        self.xtrain = x_train
+        self.partition_matrix = partition_matrix
+        self._info_for_simplification = None
+        self._calculate_all_extreme_values()
+        self._setnes_removed_sets = defaultdict(list)
+
+    def determineMF(self, mf_shape='gauss', merge_threshold=1.0, categorical_indices=None, setnes_threshold=1.0, global_singleton=None):
+        """
+            Estimates the parameters of the membership functions that are used 
+            as antecedents of the fuzzy rules.
+            
+            Args:
+                mf_shape: The desired shape of the fuzzy sets. The user can choose
+                    from 'gauss' (gaussian), 'gauss2' (double gaussion) or 'sigmf' 
+                    (sigmoidal) (default = gauss).
+                merge_threshold: Threshold for the merging of fuzzy sets for 
+                    the GRABS approach. By default no merging takes place 
+                    (default = 1.0).
+            Returns:
+                A list with the estimated parameters of the membership functions (format if gauss: mu, sigma; if gauss2: mu1, sigma1, mu2, sigma2)
+        """
+        mf_list = []
+
+        # mf_list is structured as follows:
+        # - an outer list of V variables
+        # - each item of the outer list contains C fuzzy set, one for each cluster
+        number_of_variables = self.xtrain.shape[1]
+        for i in range(0, number_of_variables):
+            if categorical_indices is not None and i in categorical_indices:
+                if global_singleton is not None:
+                    unique_values = np.unique(self.xtrain[:, i])
+                    if global_singleton == 'softmax':
+                        from scipy.special import softmax
+                        pm = softmax(self.partition_matrix, axis=0)
+                    else:
+                        pm = self.partition_matrix
+                    pml = []
+                    for uv in unique_values:
+                        pmn = pm[self.xtrain[:, i] == uv].sum(axis=0)
+                        pml.append(list(pmn / pmn.sum()))
+                    sets = list(zip(*pml))
+                    for s in sets:
+                        mf_list.append(('singleton', list(zip(unique_values, s))))
+                else:
+                    xin = self.xtrain[:, i]
+                    cluster_frequencies_counter = [[] for _ in range(0, self.partition_matrix.shape[1])]
+                    unique_values = set()
+                    for j in range(0, self.partition_matrix.shape[0]):
+                        cl = np.argmax(self.partition_matrix[j, :])  # Determine the cluster the instance belongs to the most
+                        unique_values.add(xin[j])
+                        cluster_frequencies_counter[cl].append(xin[j])
+                    cluster_frequencies = {}
+                    value_frequencies = {k: [] for k in unique_values}  # used to force the sum for each variable to 1
+                    for j, clf in enumerate(cluster_frequencies_counter):
+                        total_number = len(clf)
+                        counter = Counter(clf)
+                        # k is the element of the universe of discourse and n / total_number is the membership function
+                        tmp_dict = {}
+                        for k, n in counter.items():
+                            freq = n / total_number
+                            tmp_dict[k] = freq
+                            value_frequencies[k].append(freq)
+                        cluster_frequencies[j] = tmp_dict
+                    # Force sum to 1 for each value of the categorical feature
+                    # Computing the total sum for each value
+                    total_sums = {k: sum(value_frequencies[k]) for k in unique_values}
+                    for j in cluster_frequencies:
+                        mfs = []
+                        for k in unique_values:
+                            if k in cluster_frequencies[j]:
+                                mfs.append((k, cluster_frequencies[j][k] / total_sums[k]))
+                            else:
+                                mfs.append((k, 0.0))
+                        prm = ('singleton', mfs)
+                        mf_list.append(prm)
+            else:
+                xin = self.xtrain[:, i]
+                if all(y in (0, 1) for y in xin):  # Add noise to binary variables
+                    noise = np.random.normal(0, 0.001, xin.shape[0])
+                    xin = xin + noise
+
+                for j in range(0, self.partition_matrix.shape[1]):
+                    mfin = self.partition_matrix[:, j]
+                    mf, xx = self._convexMF(xin=xin, mfin=mfin)
+                    prm = self._fitMF(x=xx, mf=mf, mf_shape=mf_shape)
+                    mf_list.append(prm)
+
+        if merge_threshold < 1.0 or setnes_threshold < 1.0:
+            self._check_similarities(mf_list, number_of_variables, threshold=merge_threshold, setnes_threshold=setnes_threshold)
+
+        # print(self._info_for_simplification)
+
+        return mf_list
+
+    def is_subclique(self, G, nodelist):
+        H = G.subgraph(nodelist)
+        n = len(nodelist)
+        return H.size() == n * (n - 1) / 2
+
+    def _extreme_values_for_variable(self, v):
+        return min(self.xtrain.T[v]), max(self.xtrain.T[v])
+
+    def _calculate_all_extreme_values(self):
+        num_variables = len(self.xtrain.T)
+        self._extreme_values = [self._extreme_values_for_variable(v) for v in range(num_variables)]
+
+    def _check_similarities(self, mf_list, number_of_variables,
+            approx_points=100,
+            threshold=1.,
+            setnes_threshold=1.,
+            verbose=True
+            ):
+
+        number_of_clusters = len(mf_list) // number_of_variables
+
+        from collections import defaultdict
+
+        things_to_be_removed = defaultdict(list)
+
+        """ 
+            This function assesses the pair-wise similarities between 
+            the clusters mapped on each variable.
+            It returns a dictionary of this kind:
+            variable -> list of similar couples for that variable + jaccard sim
+
+        """
+
+        for v in range(number_of_variables):
+
+            if verbose:
+                print(" * Trying to simplify variable", v)
+
+            mi, ma = self._extreme_values_for_variable(v)
+            points = np.linspace(mi, ma, approx_points)
+
+            for c1 in range(number_of_clusters):
+                for c2 in range(c1 + 1, number_of_clusters):
+
+                    index1 = v * number_of_clusters + c1
+                    index2 = v * number_of_clusters + c2
+                    funname1, params1 = mf_list[index1]
+                    funname2, params2 = mf_list[index2]
+
+                    if funname1 == "gauss":
+
+                        from numpy import linspace, array
+
+                        first_cluster = array([self._gaussmf(x, params1[0], params1[1]) for x in points])
+                        second_cluster = array([self._gaussmf(x, params2[0], params2[1]) for x in points])
+
+                        intersection = sum([min(x, y) for x, y in zip(first_cluster, second_cluster)])
+                        union = sum([max(x, y) for x, y in zip(first_cluster, second_cluster)])
+
+                        jaccardsim = (intersection / union)
+
+                        if jaccardsim > threshold:
+                            things_to_be_removed[v].append([c1, c2, jaccardsim])
+
+                            # print("%.2f is fine" % jaccardsim)
+
+                    else:
+                        raise Exception("Not implemented yet")
+
+                # Setnes' rule simplification: detect which sets are similar to the universal set
+                #                              using Jaccard similarity and a threshold.
+                if setnes_threshold<1.:
+
+                    index1 = v*number_of_clusters + c1
+                    funname1, params1 = mf_list[index1]
+
+                    if funname1== "gauss":
+
+                        first_cluster = array([self._gaussmf(x, params1[0], params1[1]) for x in points])
+                        second_cluster = array([1 for x in points]) # universal set
+
+                        intersection = sum([min(x,y) for x,y in zip(first_cluster, second_cluster)])
+                        union        = sum([max(x,y) for x,y in zip(first_cluster, second_cluster)])
+
+                        jaccardsim = (intersection/union)
+
+                        if jaccardsim>setnes_threshold:
+                            self._setnes_removed_sets[v].append(c1)
+                            print (" * Variable %d, cluster %d is too similar to universal set (threshold: %.2f): marked for removal" % (v,c1+1,setnes_threshold))
+
+                    else:
+                        raise Exception("Setnes' simplification for non-Gaussian functions not implemented yet")
+
+
+
+        #for k,v in things_to_be_removed.items():            print (k, v)
+        #exit()
+        """
+            This function must return a dictionary of items like:
+            (variable, cluster) -> mapped_cluster
+        """
+
+        self._info_for_simplification = {}
+        for var_num, value in things_to_be_removed.items():
+
+            subcomponents = self._create_graph(value)
+
+            for subcomp in subcomponents:
+                # print (is_complete(subcomp))
+
+                if is_complete(subcomp):
+                    retained = list(subcomp.nodes())[0]
+                    # print ("retain: %d" % retained)
+                    for el in list(subcomp.nodes()):
+                        if el != retained:
+                            self._info_for_simplification[(var_num, el)] = retained
+
+        dropped_stuff = self.get_number_of_dropped_fuzzy_sets()
+        print (" * %d antecedent clauses will be simplified using a threshold %.2f" % (dropped_stuff, threshold))
+        if verbose:
+            print(" * GRABS remapping info:", self._info_for_simplification)
+            print(" * Setnes simplification dictionary variable ==> list of clusters/fuzzy sets to be removed:", self._setnes_removed_sets)
+
+        self._info_for_simplification
+
+    def get_number_of_dropped_fuzzy_sets(self):
+        return len(self._info_for_simplification)
+
+    def _create_graph(self, list_of_arcs):
+        from networkx import Graph, connected_components
+        G = Graph()
+        nodelist = []
+        for arc in list_of_arcs:
+            G.add_edge(arc[0], arc[1])
+            nodelist.append(arc[0])
+            nodelist.append(arc[1])
+        S = [G.subgraph(c).copy() for c in connected_components(G)]
+        return S
+
+    def _convexMF(self, xin, mfin, norm=1, nc=1000):
+
+        # Calculates the convex membership function that envelopes a given set of
+        # data points and their corresponding membership values. 
+
+        # Input:
+        # Xin: N x 1 input domain (column vector)
+        # MFin: N x 1 corresponding membership values 
+        # nc: number of alpha cut values to consider (default=101)
+        # norm: optional normalization flag (0: do not normalize, 1 : normalize, 
+        # default=1)
+        #
+        # Output:
+        # mf: membership values of convex function
+        # x: output domain values    
+
+        # Normalize the membership values (if requested)
+        if norm == 1:
+            mfin = np.divide(mfin, np.max(mfin))
+
+        # Initialize auxilary variables
+        acut = np.linspace(0, np.max(mfin), nc)
+        mf = np.full(2 * nc, np.nan)
+        x = np.full(2 * nc, np.nan)
+
+        if np.any(mfin > 0):
+            x[0] = np.min(xin[mfin > 0])
+            x[nc] = np.max(xin[mfin > 0])
+            mf[0] = 0
+            mf[nc] = 0
+
+        # Determine the elements in the alpha cuts
+        for i in range(0, nc):
+            if np.any(mfin > acut[i]):
+                x[i] = np.min(xin[mfin > acut[i]])
+                x[i + nc] = np.max(xin[mfin > acut[i]])
+                mf[i] = acut[i]
+                mf[i + nc] = acut[i]
+
+        # # Determine the elements in the alpha cuts    
+        # for i in range(0,nc):
+        #     tmp1 = mfin>acut[i]
+        #     if len(tmp1)==0:
+        #         tmp=xin[tmp1]
+        #         np.sort(tmp)
+        #         x[i]=tmp[0]
+        #         x[i+nc]=tmp[-1]
+        #         mf[i]=acut[i]
+        #         mf[i+nc]=acut[i]
+
+        # Delete NaNs
+        idx = np.isnan(x)
+        x = x[idx == False]
+        mf = mf[idx == False]
+
+        # Sort vectors based on membership value (descending order)
+        indmf = mf.argsort(axis=0)
+        indmf = np.flipud(indmf)
+        mf = mf[indmf]
+        x = x[indmf]
+
+        # Find duplicate values for x and onlykeep the ones with the highest membership value
+        _, ind = np.unique(x, return_index=True, return_inverse=False, return_counts=False, axis=None)
+        mf = mf[ind]
+        x = x[ind]
+
+        # Sort vectors based on x value (ascending order)
+        indx = x.argsort(axis=0)
+        mf = mf[indx]
+        x = x[indx]
+
+        xval = np.linspace(np.min(x), np.max(x), nc)
+        mf = np.interp(xval, x, mf, left=None, right=None, period=None)
+        x = xval
+        return mf, x
+
+    def _fitMF(self, x, mf, mf_shape='gauss'):
+        # Fits parametrized membership functions to a set of pointwise defined 
+        # membership values.
+        #
+        # Input:
+        # x:  N x 1 domain of input variable
+        # mf: N x 1 membership values for input data x 
+        # shape: Type of membership function to fit (possible values: 'gauss', 
+        # 'gauss2' and 'sigmf')
+        #
+        # Output:
+        # param: matrix of membership function parameters
+
+        if mf_shape == 'gauss':
+            # Determine initial parameters
+            mu = sum(x * mf) / sum(mf)
+            mf[mf == 0] = np.finfo(np.float64).eps
+            sig = np.mean(np.sqrt(-((x - mu) ** 2) / (2 * np.log(mf))))
+
+            # Fit parameters to the data using least squares
+            #            print('mu=', mu, 'sig=', sig)
+            param, _ = curve_fit(self._gaussmf, x, mf, p0=[mu, sig], bounds=((-np.inf, 0), (np.inf, np.inf)),
+                                 maxfev=10000)
+
+        elif mf_shape == 'gauss2':
+            # Determine initial parameters
+            mu1 = x[mf >= 0.95][0]
+            mu2 = x[mf >= 0.95][-1]
+            xmf = x[mf >= 0.5]
+            sig1 = (mu1 - xmf[0]) / (np.sqrt(2 * np.log(2)))
+            sig2 = (xmf[-1] - mu2) / (np.sqrt(2 * np.log(2)))
+            if sig1 == 0.0:
+                sig1 = 0.1
+            if sig2 == 0.0:
+                sig2 = 0.1
+
+            # Fit parameters to the data using least squares
+            #            print('mu1',mu1,'sig1',sig1,'mu2',mu2,'sig2',sig2)
+            param, _ = curve_fit(self._gauss2mf, x, mf, p0=[mu1, sig1, mu2, sig2], maxfev=1000,
+                                 bounds=((-np.inf, 0, -np.inf, 0), (np.inf, np.inf, np.inf, np.inf)))
+
+        elif mf_shape == 'sigmf':
+            # Determine initial parameters
+            if np.argmax(mf) - np.argmin(mf) > 0:  # if sloping to the right
+                if len(x[mf >= 0.5]) > 0:
+                    c = x[mf >= 0.5][0]
+                    s = 1
+                elif len(x[mf >= 0.5]) == 0:  # if there are no datapoints with membership larger than 0
+                    c = x[0]
+                    s = 1
+            elif np.argmax(mf) - np.argmin(mf) < 0:  # if sloping to the left
+                if len(x[mf <= 0.5]) > 0:
+                    c = x[mf <= 0.5][0]
+                    s = 1
+                elif len(x[mf <= 0.5]) == 0:  # if there are no datapoints with membership smaller than 0
+                    c = x[-1]
+                    s = 1
+                    # Fit parameters of the function to the data using non-linear least squares
+            try:
+                param, _ = curve_fit(self._sigmf, x, mf, p0=[c, s], maxfev=1000)
+            except RuntimeError:
+                print(
+                    'pyFUME attempted to fit sigmoidal shaped membership functions, but was unable to find fitting parameters. pyFUME will now terminate. Please consider using a different shape for the membership functions.')
+                import sys
+                sys.exit()
+
+        return mf_shape, param
+
+    def _gaussmf(self, x, mu, sigma, a=1):
+        # x:  (1D array)
+        # mu: Center of the bell curve (float)
+        # sigma: Width of the bell curve (float)
+        # a: normalizes the bell curve, for normal fuzzy set a=1 (float) 
+        return a * np.exp(-(x - mu) ** 2 / (2 * sigma ** 2))
+
+    def _gauss2mf(self, x, mu1, sigma1, mu2, sigma2):
+        # x: Data
+        # mu1: Center of the leftside bell curve
+        # sigma1: Standard deviation that determines the width of the leftside bell curve
+        # mu2: Center of the rightside bell curve
+        # sigma2: Standard deviation that determines the width of the rightside bell curve
+        y = np.ones(len(x))
+        idx1 = x <= mu1
+        idx2 = x > mu2
+        y[idx1] = self._gaussmf(x[idx1], mu1, sigma1)
+        y[idx2] = self._gaussmf(x[idx2], mu2, sigma2)
+        return y
+
+    def _sigmf(self, x, c, s):
+        # x: data
+        # b: x where mf is 0.5
+        # c: Controls 'width' of the sigmoidal region about `b` (magnitude); also
+        #    which side of the function is open (sign). A positive value of `a`
+        #    means the left side approaches 0.0 while the right side approaches 1,
+        #    a negative value of `c` means the opposite.
+        return 1. / (1. + np.exp(- s * (x - c)))
```

### Comparing `pyFUME-0.3.1/pyfume/EstimateConsequentParameters.py` & `pyfume-0.3.4/pyfume/EstimateConsequentParameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,153 +1,151 @@
-import copy
-import numpy as np
-from scipy.optimize import curve_fit
-import numpy.matlib
-from typing_extensions import Unpack
-
-class ConsequentEstimator(object):
-    """
-        Creates a new consequent estimator object.
-        
-        Args:
-            x_train: The input data.
-            y_train: The output data (true label/golden standard).
-            firing_strengths: Matrix containing the degree to which each rule 
-                fires for each data instance.
-    """
-
-    def __init__(self, x_train, y_train, firing_strengths, categorical_indices=None):
-        self.x_train = copy.deepcopy(x_train)
-        self.categorical_indices = [] if categorical_indices is None else categorical_indices
-        self.y_train = y_train
-        self.firing_strengths = firing_strengths
-
-    def zero_order(self):
-        """
-            Estimates the consequent parameters of the zero-order Sugeno-Takagi model using normalized means.
-        
-            Args:
-                df: default value returned when the sum of grades equals to one (default = 0).
-        
-            Returns:
-                The parameters for the consequent function.
-        """
-        p = np.zeros((self.firing_strengths.shape[1]))
-        for clus in range(0, self.firing_strengths.shape[1]):
-            fs = self.firing_strengths[:, clus]
-            fs = np.fmax(fs, np.finfo(np.float64).eps)  # avoid 0's in the matrix
-            normalized_weights = fs / fs.sum(0)
-            s = np.multiply(normalized_weights, self.y_train)
-            p[clus] = sum(s)
-        return p
-
-    def suglms(self, global_fit=False, df=0):
-        """
-            Estimates the consequent parameters in the first-order Sugeno-Takagi model using least squares.
-        
-            Args:
-                global_fit: Use the local (global_fit=False) or global (global_fit=True) least mean squares estimates. Global estimates functionality is still in beta mode, so use with caution.
-                df: default value returned when the sum of grades equals to one (default = 0).
-        
-            Returns:
-                The parameters for the consequent function.
-        """
-
-        x = self.x_train.copy()
-        y = self.y_train.copy()
-        f = self.firing_strengths.copy()
-
-        # ONE HOT ENCODE CATEGORICAL VARIABLES
-        slices = []
-        for i in range(x.shape[1]):
-            if i in self.categorical_indices:
-                # categorical variables are expected to be INTEGERS in the range 0,...,n
-                col = x[:, i].astype(np.uint32)
-                one_hot = np.zeros((x.shape[0], col.max() + 1))
-                one_hot[np.arange(x.shape[0]), col] = 1
-                slices.append(one_hot[:, :-1])
-            else:
-                slices.append(x[:, i].reshape(-1, 1))
-        # x = np.c_[*slices] 
-        x = np.c_[Unpack[slices]]
-
-        # Check if input X contains one column of ones (for the constant). If not, add it.
-        u = np.unique(x[:, -1])
-        if u.shape[0] != 1 or u[0] != 1:
-            x = np.hstack((x, np.ones((x.shape[0], 1))))
-
-        # Find the number of data points (mx & mf) , the number of variables (nx) and the
-        # number of clusters (nf) 
-        mx, nx = x.shape
-        mf, nf = f.shape
-
-        # Calculate the sum of the degree of fulfillement (DOF) for each data point
-        sumDOF = np.sum(f, 1)
-
-        # When degree of fulfillment is zero (which means no rule is applicable), set to one
-        NoRule = sumDOF == 0
-        sumDOF[NoRule] = 1
-        sumDOF = np.matlib.repmat(sumDOF, nf, 1).T
-
-        if nf == 1:
-            global_fit = False
-
-        if global_fit is True:  # Global least mean squares estimates
-
-            # Still under construction!
-
-            # Auxillary variables
-            f1 = x.flatten()
-            s = np.matlib.repmat(f1, nf, 1).T
-            xx = np.reshape(s, (nx, nf * mx), order='F')
-            s = xx.T
-            x1 = np.reshape(s, (mx, nf * nx), order='F')
-            x = x.T  # reshape data matrix
-
-            # (reshaped) vector of f devided by the sum of each row of f
-            # (normalised membership degree)
-            xx = (f.T.flatten() / sumDOF.T.flatten())
-
-            # reshape partition matrix
-            s = np.matlib.repmat(xx, nx, 1).T
-            f1 = np.reshape(s, (mx, nf * nx), order='F')
-            x1 = f1 * x1
-
-            # Find least squares solution
-            #            xp = np.linalg.lstsq(x1,y,rcond=None)
-
-            # Perform QR decomposition
-            Q, R = np.linalg.qr(x1)  # qr decomposition of A
-            Qy = np.dot(Q.T, y)  # computing Q^T*b (project b onto the range of A)
-            xx = np.linalg.solve(R, Qy)
-
-            p = np.reshape(xx, (nf, nx), order='F')
-
-            # Local models
-            yl = np.transpose(x).dot(np.transpose(p))  #
-
-            # Global model
-            ym = x1.dot(p.flatten()) + df * NoRule
-            ylm = yl.copy()
-
-            # Mask all memberships < 0.2 with NaN's for plots
-            ylm[f < 0.2] = np.NaN
-
-        elif global_fit is False:  # local weighted least mean squares estimates
-            # Pre-allocate variable
-            p = np.zeros([nf, nx])
-
-            for i in range(0, nf):
-                # Select firing strength of the selected rule
-                w = f[:, i]
-
-                # Weight input with firing strength
-                xw = x * np.sqrt(w[:, np.newaxis])
-
-                # Weight output with firing strength
-                yw = y * np.sqrt(w)
-
-                # Perform least squares with weighted input and output
-                prm, _, _, _ = np.linalg.lstsq(xw, yw, rcond=None)
-                p[i] = prm
-
-        return p  # ,ym,yl,ylm
+import copy
+import numpy as np
+from scipy.optimize import curve_fit
+import numpy.matlib
+
+class ConsequentEstimator(object):
+    """
+        Creates a new consequent estimator object.
+        
+        Args:
+            x_train: The input data.
+            y_train: The output data (true label/golden standard).
+            firing_strengths: Matrix containing the degree to which each rule 
+                fires for each data instance.
+    """
+
+    def __init__(self, x_train, y_train, firing_strengths, categorical_indices=None):
+        self.x_train = copy.deepcopy(x_train)
+        self.categorical_indices = [] if categorical_indices is None else categorical_indices
+        self.y_train = y_train
+        self.firing_strengths = firing_strengths
+
+    def zero_order(self):
+        """
+            Estimates the consequent parameters of the zero-order Sugeno-Takagi model using normalized means.
+        
+            Args:
+                df: default value returned when the sum of grades equals to one (default = 0).
+        
+            Returns:
+                The parameters for the consequent function.
+        """
+        p = np.zeros((self.firing_strengths.shape[1]))
+        for clus in range(0, self.firing_strengths.shape[1]):
+            fs = self.firing_strengths[:, clus]
+            fs = np.fmax(fs, np.finfo(np.float64).eps)  # avoid 0's in the matrix
+            normalized_weights = fs / fs.sum(0)
+            s = np.multiply(normalized_weights, self.y_train)
+            p[clus] = sum(s)
+        return p
+
+    def suglms(self, global_fit=False, df=0):
+        """
+            Estimates the consequent parameters in the first-order Sugeno-Takagi model using least squares.
+        
+            Args:
+                global_fit: Use the local (global_fit=False) or global (global_fit=True) least mean squares estimates. Global estimates functionality is still in beta mode, so use with caution.
+                df: default value returned when the sum of grades equals to one (default = 0).
+        
+            Returns:
+                The parameters for the consequent function.
+        """
+
+        x = self.x_train.copy()
+        y = self.y_train.copy()
+        f = self.firing_strengths.copy()
+
+        # ONE HOT ENCODE CATEGORICAL VARIABLES
+        slices = []
+        for i in range(x.shape[1]):
+            if i in self.categorical_indices:
+                # categorical variables are expected to be INTEGERS in the range 0,...,n
+                col = x[:, i].astype(np.uint32)
+                one_hot = np.zeros((x.shape[0], col.max() + 1))
+                one_hot[np.arange(x.shape[0]), col] = 1
+                slices.append(one_hot[:, :-1])
+            else:
+                slices.append(x[:, i].reshape(-1, 1))
+        x = np.concatenate(slices, axis=1)
+
+        # Check if input X contains one column of ones (for the constant). If not, add it.
+        u = np.unique(x[:, -1])
+        if u.shape[0] != 1 or u[0] != 1:
+            x = np.hstack((x, np.ones((x.shape[0], 1))))
+
+        # Find the number of data points (mx & mf) , the number of variables (nx) and the
+        # number of clusters (nf) 
+        mx, nx = x.shape
+        mf, nf = f.shape
+
+        # Calculate the sum of the degree of fulfillement (DOF) for each data point
+        sumDOF = np.sum(f, 1)
+
+        # When degree of fulfillment is zero (which means no rule is applicable), set to one
+        NoRule = sumDOF == 0
+        sumDOF[NoRule] = 1
+        sumDOF = np.matlib.repmat(sumDOF, nf, 1).T
+
+        if nf == 1:
+            global_fit = False
+
+        if global_fit is True:  # Global least mean squares estimates
+
+            # Still under construction!
+
+            # Auxillary variables
+            f1 = x.flatten()
+            s = np.matlib.repmat(f1, nf, 1).T
+            xx = np.reshape(s, (nx, nf * mx), order='F')
+            s = xx.T
+            x1 = np.reshape(s, (mx, nf * nx), order='F')
+            x = x.T  # reshape data matrix
+
+            # (reshaped) vector of f devided by the sum of each row of f
+            # (normalised membership degree)
+            xx = (f.T.flatten() / sumDOF.T.flatten())
+
+            # reshape partition matrix
+            s = np.matlib.repmat(xx, nx, 1).T
+            f1 = np.reshape(s, (mx, nf * nx), order='F')
+            x1 = f1 * x1
+
+            # Find least squares solution
+            #            xp = np.linalg.lstsq(x1,y,rcond=None)
+
+            # Perform QR decomposition
+            Q, R = np.linalg.qr(x1)  # qr decomposition of A
+            Qy = np.dot(Q.T, y)  # computing Q^T*b (project b onto the range of A)
+            xx = np.linalg.solve(R, Qy)
+
+            p = np.reshape(xx, (nf, nx), order='F')
+
+            # Local models
+            yl = np.transpose(x).dot(np.transpose(p))  #
+
+            # Global model
+            ym = x1.dot(p.flatten()) + df * NoRule
+            ylm = yl.copy()
+
+            # Mask all memberships < 0.2 with NaN's for plots
+            ylm[f < 0.2] = np.NaN
+
+        elif global_fit is False:  # local weighted least mean squares estimates
+            # Pre-allocate variable
+            p = np.zeros([nf, nx])
+
+            for i in range(0, nf):
+                # Select firing strength of the selected rule
+                w = f[:, i]
+
+                # Weight input with firing strength
+                xw = x * np.sqrt(w[:, np.newaxis])
+
+                # Weight output with firing strength
+                yw = y * np.sqrt(w)
+
+                # Perform least squares with weighted input and output
+                prm, _, _, _ = np.linalg.lstsq(xw, yw, rcond=None)
+                p[i] = prm
+
+        return p  # ,ym,yl,ylm
```

### Comparing `pyFUME-0.3.1/pyfume/FeatureSelection.py` & `pyfume-0.3.4/pyfume/FeatureSelection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,556 +1,578 @@
-from .LoadData import DataLoader
-from .Splitter import DataSplitter
-from .SimpfulModelBuilder import SugenoFISBuilder
-from .Clustering import Clusterer
-from .EstimateAntecendentSet import AntecedentEstimator
-from .FireStrengthCalculator import FireStrengthCalculator
-from .EstimateConsequentParameters import ConsequentEstimator
-from .Tester import SugenoFISTester
-import numpy as np
-import pandas as pd
-
-class FeatureSelector(object):
-    """
-        Creates a new feature selection object.
-        
-        Args:
-            dataX: The input data.
-            dataY: The output data (true label/golden standard).
-            nr_clus: Number of clusters that should be identified in the data.
-            variable_names: Names of the variables
-            **kwargs: Additional arguments to change settings of the fuzzy model.
-    """
-    def __init__(self, dataX, dataY, nr_clus, variable_names, model_order='first', performance_metric='MAE', verbose=True, **kwargs):
-        self.dataX=dataX
-        self.dataY=dataY
-        self.nr_clus = nr_clus
-        self.variable_names = variable_names
-        self.performance_metric = performance_metric
-        self.model_order=model_order
-        self.verbose=verbose
-        
-    def log_wrapper(self, raw_data, **kwargs):
-        """
-            Performs feature selection using the wrapper method while also checking whether .
-            
-            Args:
-                **kwargs: Additional arguments to change settings of the fuzzy model.
-                
-            Returns:
-                Tuple containing (selected_features, selected_feature_names)
-                    - selected_features: The indices of the selected features.
-                    - selected_feature_names: The names of the selected features. 
-
-        """
-            
-        # Create a training and validation set for the feature selection phase
-        x_feat = self.dataX.copy()
-        y_feat = self.dataY.copy()
-        
-        
-        # Set negative or value == 0 to small number to be able to perform log
-        epsilon = np.finfo(np.float64).eps
-        raw_data[raw_data <= 0] = epsilon
-        
-        x_logged = np.log(raw_data)
-        x_logged_norm = (x_logged - np.nanmin(x_logged, axis =0)) / (np.nanmax(x_logged, axis =0)-np.nanmin(x_logged, axis =0))
-
-        # Set initial values for the performance
-        if self.performance_metric != 'accuracy' and self.performance_metric !=  'AUC': 
-            old_performance=np.inf
-            new_performance=np.inf
-            perfs=[]
-        elif self.performance_metric == 'accuracy' or self.performance_metric == 'AUC':
-            old_performance=-np.inf
-            new_performance=-np.inf
-            perfs=[]
-        else: 
-            raise Exception('Unknown performance metric.')
-    
-        # Create a set with the unselected (currently all) and selected (none yet) variables
-        selected_features=[]
-        unselected_features=list(range(0,np.size(x_feat,axis=1)))
-        
-        # Keep a (at this point empty) lists of which variables should be log-transformed
-        logvars = []
-        logvars_num = []
-        temp_logvars_num = []
-        temp_logvars  = []
-        
-        stop=False
-
-        while stop == False: 
-            
-            if self.performance_metric != 'accuracy': 
-                perfs= [np.inf]*np.size(x_feat,axis=1)
-            elif self.performance_metric == 'accuracy':
-                perfs= [-1*np.inf]*np.size(x_feat,axis=1)
-            else: 
-                raise Exception('Unknown performance metric.')
-            
-            
-            if self.performance_metric != 'accuracy':
-                for f in [x for x in unselected_features if x != -1]:
-                    considered_features = selected_features + [f]
-                    var_names = [self.variable_names[i] for i in considered_features]
-                    
-                    # Prepare training sets
-                    feat=x_feat[:,considered_features]
-                    logged_feature = x_logged_norm[:,f]
-                    
-                    log_feat= feat.copy()
-                    log_feat[:,f]=logged_feature
-    
-                    if self.verbose: print('Evaluating feature sub-set including:', var_names)
-            
-                    normal_perf = self._evaluate_feature_set(x_data=feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
-                    log_perf = self._evaluate_feature_set(x_data=log_feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
-                    if log_perf < normal_perf: 
-                       temp_logvars.append(var_names[-1])
-                       temp_logvars_num.append(f)
-                       if self.verbose: print(" * In this sub-set, the variable(s)", logvars + list([var_names[-1]]), "will be log-transformed.")
-                    elif log_perf > normal_perf and len(logvars)>0:
-                        if self.verbose: print(" * In this sub-set, the variable(s)", logvars, "will be log-transformed.")
-    
-                    perfs[f] = min(normal_perf, log_perf)
-                
-                new_performance=min(perfs)
-                new_feature=unselected_features[perfs.index(new_performance)]
-                    
-                del perfs
-                    
-                if new_performance<old_performance: #*feature_selection_stop:
-                    selected_features.append(new_feature)
-                                    
-                    # Check if the last addded feature should be log-transformed and if so, perform the transformation
-                    if new_feature in temp_logvars_num:
-                           logvars.append(self.variable_names[new_feature])
-                           logvars_num.append(new_feature)
-                           x_feat[new_feature] = x_logged_norm[new_feature]
-                      
-                    unselected_features[new_feature]=-1
-                    old_performance=new_performance
-                    
-                    temp_logvars_num = []
-                    temp_logvars  = []
-    
-                else:
-                    if self.verbose: print('***** FEATURE SELECTION ENDED *****')
-                    if self.verbose: print('The selected features have a', self.performance_metric, 'of:', old_performance)
-                    stop = True 
-                    
-            elif self.performance_metric == 'accuracy':
-                for f in [x for x in unselected_features if x != -1]:
-                    considered_features = selected_features + [f]
-                    var_names = [self.variable_names[i] for i in considered_features]
-                    
-                    # Prepare training sets
-                    feat=x_feat[:,considered_features]
-                    logged_feature = x_logged_norm[:,f]
-                    log_feat = feat.copy()                    
-                    log_feat[:,-1]=logged_feature
-                    
-                    if self.verbose: print('Evaluating feature sub-set including:', var_names)
-            
-                    normal_perf = self._evaluate_feature_set(x_data=feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
-                    log_perf = self._evaluate_feature_set(x_data=log_feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
-                    print("Normal performance:", normal_perf, ", Logged performance:", log_perf)
-                    
-                    if log_perf > normal_perf: 
-                       temp_logvars.append(var_names[-1])
-                       temp_logvars_num.append(f)
-                       if self.verbose: print(" * In this sub-set, the variable(s)", logvars + list([var_names[-1]]), "will be log-transformed.")
-                    elif log_perf < normal_perf and len(logvars)>0:
-                        if self.verbose: print(" * In this sub-set, the variable(s)", logvars, "will be log-transformed.")
-    
-                    perfs[f] = max(normal_perf, log_perf)
-    
-                new_performance=max(perfs)
-                new_feature=unselected_features[perfs.index(new_performance)]
-                    
-                del perfs
-                
-                if new_performance>old_performance: #*feature_selection_stop:
-                    selected_features.append(new_feature)
-                                    
-                    # Check if the last addded feature should be log-transformed and if so, perform the transformation
-                    if new_feature in temp_logvars_num:
-                           logvars.append(self.variable_names[new_feature])
-                           logvars_num.append(new_feature)
-                        
-                           x_feat[new_feature] = x_logged_norm[new_feature]
-                      
-                    unselected_features[new_feature]=-1
-                    old_performance=new_performance
-                    
-                    temp_logvars_num = []
-                    temp_logvars  = []
-    
-                else:
-                    if self.verbose: print('***** FEATURE SELECTION ENDED *****')
-                    if self.verbose: print('The selected features have a', self.performance_metric, 'of:', old_performance)
-                    stop = True                 
-       
-        # Show the user which variables were selected, and which ones were log-transformed.
-        selected_feature_names = [self.variable_names[i] for i in selected_features]
-        if self.verbose: 
-            print('The following features were selected:',  selected_feature_names)
-            if len(logvars)>0:
-                print('The following features were log-transformed:', logvars)
-            elif len(logvars)==0:
-                print('None of the selected features was log-transformed.')
-            
-        return selected_features, selected_feature_names, logvars_num, logvars
-
-        
-    def wrapper(self,**kwargs):
-        """
-            Performs feature selection using the wrapper method.
-            
-            Args:
-                **kwargs: Additional arguments to change settings of the fuzzy model.
-                
-            Returns:
-                Tuple containing (selected_features, selected_feature_names)
-                    - selected_features: The indices of the selected features.
-                    - selected_feature_names: The names of the selected features. 
-
-        """
-            
-        # Create a training and validation set for the feature selection phase
-        ds = DataSplitter()
-        x_feat, y_feat, x_val, y_val = ds.holdout(self.dataX, self.dataY)
-        
-        # Set initial values for the performance
-        old_performance=np.inf
-        new_performance=np.inf
-        perfs=[]
-        
-        # Create a set with the unselected (currently all) and selected (none yet) variables
-        selected_features=[]
-        unselected_features=list(range(0,np.size(x_feat,axis=1)))
-        
-        stop=False
-
-        while stop == False: 
-            perfs= [np.inf]*np.size(x_feat,axis=1)
-            
-            for f in [x for x in unselected_features if x != -1]:
-                considered_features = selected_features + [f]
-                var_names = [self.variable_names[i] for i in considered_features]
-                feat=x_feat[:,considered_features]
-                x_validation=x_val[:,considered_features] 
-                if self.verbose==True: 
-                    print('Evaluating feature sub set including:', var_names)
-                
-                try:
-                    perfs[f] = self._evaluate_feature_set(x_data=feat, y_data=y_feat, x_val=x_validation, y_val=y_val, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
-                except RuntimeError:
-                    raise Exception('ERROR: main module was not safely imported. Feature selection exploits multiprocessing, so please add a `if _name_ == `_main_`: `-line to your main script. See https://docs.python.org/2/library/multiprocessing.html#windows for further info.')
-                    import sys
-                    sys.exit(1)
-                    
-            new_performance=min(perfs)
-            new_feature=unselected_features[perfs.index(new_performance)]
-            
-            #print('new feature', new_feature)
-            del perfs
-            
-            if new_performance<old_performance: #*feature_selection_stop:
-                selected_features.append(new_feature)
-                unselected_features[new_feature]=-1
-                old_performance=new_performance
-            else:
-                if self.verbose: print('The selected features have a', self.performance_metric, 'of:', old_performance)
-                stop = True 
-       
-        # selected_feature_names = self.variable_names[selected_features]
-        selected_feature_names = [self.variable_names[i] for i in selected_features]
-        if self.verbose: print('The following features were selected:',  selected_feature_names)
-        
-        return selected_features, selected_feature_names
-
-    def fst_pso_feature_selection(self, max_iter=100, min_clusters=2, max_clusters=10, performance_metric='MAE', **kwargs):
-        """
-            Perform feature selection using the FST-PSO [1] variant of the Integer and Categorical 
-            PSO (ICPSO) proposed by Strasser and colleagues [2]. ICPSO hybridizes PSO and Estimation of Distribution 
-            Algorithm (EDA), which makes it possible to convert a discrete problem to the (real-valued) 
-            problem of estimating the distribution vector of a probabilistic model. Each fitness 
-            evaluation a random solution is generated according to the probability distribution 
-            encoded by the particle. Because the implementation is a variant on FST-PSO, the optimal 
-            settings for the PSO are set automatically.
-
-            If the number of clusters is set to None, this method simultaneously choses the optimal 
-            number of clusters.
-
-            [1] Nobile, M. S., Cazzaniga, P., Besozzi, D., Colombo, R., Mauri, G., & Pasi, G. (2018). 
-            Fuzzy Self-Tuning PSO: A settings-free algorithm for global optimization. Swarm and 
-            evolutionary computation, 39, 70-85.
-            
-            [2] Strasser, S., Goodman, R., Sheppard, J., & Butcher, S. (2016). A new discrete 
-            particle swarm optimization algorithm. In Proceedings of the Genetic and Evolutionary 
-            Computation Conference 2016 (pp. 53-60). 
-            
-            Args:
-                max_iter: The maximum number of iterations used in the PSO (default = 10).
-                min_clusters: The minimum number of clusters to be identified in the data set (only 
-                when nr_clusters = None)
-                max_clusters: The maximum number of clusters to be identified in the data set (only 
-                when nr_clusters = None)
-                performance_metric: The performance metric on which each solution is evaluated (default
-                Mean Absolute Error (MAE))
-                **kwargs: Additional arguments to change settings of the fuzzy model.
-                
-            Returns:
-                Tuple containing (selected_features, selected_feature_names, optimal_number_clusters)
-                    - selected_features: The indices of the selected features.
-                    - selected_feature_names: The names of the selected features.
-                    - optimal_number_clusters: If initially nr_clusters = None, this argument encodes the optimal number of clusters in the data set. If nr_clusters is not None, the optimal_number_clusters is set to nr_clusters.
-
-        """
-        
-        from fstpso import FuzzyPSO
-
-
-        FP = FuzzyPSO()
-
-        # Create the search space for feature selection with number of dimensions D
-        D = np.size(self.dataX,1)
-        
-        s=list([[True, False]]*D)
-        
-        # Add dimension for cluster number selection
-        if self.nr_clus == None:
-            s.append(list(range(min_clusters,max_clusters+1)))
-        
-        # Set search space
-        FP.set_search_space_discrete(s)
-        
-        # Set the fitness function
-        args={'x_train': self.dataX, 'y_train': self.dataY, 'verbose':self.verbose}
-        FP.set_fitness(self._function, arguments=args)
-        
-        if 'fstpso_n_particles' not in kwargs.keys(): kwargs['fstpso_n_particles'] = None
-        elif kwargs['fstpso_n_particles'] != None:
-            FP.set_swarm_size(kwargs['fstpso_n_particles'])
-                
-        # solve problem with FST-PSO
-        _, self.best_performance, self.best_solution = FP.solve_with_fstpso(max_iter=max_iter,verbose=False)
-        
-        if self.nr_clus == None:
-            selected_features=self.best_solution[:-1]
-        else:
-           selected_features=self.best_solution 
-    
-        
-        # Show best solution with fitness value
-        varnams=[i for indx,i in enumerate(self.variable_names) if selected_features[indx]]
-        if self.verbose: print('The following features have been selected:', varnams, 'with a', self.performance_metric, 'of', round(self.best_performance,2))
-        
-        if self.nr_clus == None:
-            optimal_number_clusters=self.best_solution[-1]
-        else:
-            optimal_number_clusters = self.nr_clus
-            
-            
-        return selected_features, varnams, optimal_number_clusters
-
-#    def fun(self, particle):
-#        return sum(particle)
-    
-    def _function(self, particle, arguments, verbose=False, **kwargs):
-        from itertools import compress 
-        if self.nr_clus == None:
-            A = arguments['x_train'][:,particle[:-1]]
-            varnams=list(compress(self.variable_names, particle[:-1]))
-            nr_clus=particle[-1]
-        else:
-            A = arguments['x_train'][:,particle[:]]
-            varnams=list(compress(self.variable_names, particle[:]))
-            nr_clus=self.nr_clus
-        
-        if A.shape[1]==0: ## If no features are selected, return a infinite high error
-            error=np.inf
-        else:
-            error=self._evaluate_feature_set(x_data=A, y_data=arguments['y_train'], nr_clus=nr_clus, var_names=varnams, model_order=self.model_order, performance_metric=self.performance_metric, **kwargs)
-            
-        if verbose: print(" * Fitness: %.3f" % error)
-        return error
-    
-    def _evaluate_feature_set(self, x_data, y_data, nr_clus, var_names, model_order='first', performance_metric='MAE', fs_number_of_folds=3, **kwargs):
-        # Check settings and complete with default settings when needed
-        if 'merge_threshold' not in kwargs.keys(): kwargs['merge_threshold'] = 1.0
-        if 'cluster_method' not in kwargs.keys(): kwargs['cluster_method'] = 'fcm'        
-        if kwargs['cluster_method'] == 'fcm':
-            if 'fcm_m' not in kwargs.keys(): kwargs['fcm_m'] = 2
-            if 'fcm_max_iter' not in kwargs.keys(): kwargs['fcm_maxiter'] = 1000
-            if 'fcm_error' not in kwargs.keys(): kwargs['fcm_error'] = 0.005
-        elif kwargs['cluster_method'] == 'fstpso':
-            if 'fstpso_n_particles' not in kwargs.keys(): kwargs['fstpso_n_particles'] = None
-            if 'fstpso_max_iter' not in kwargs.keys(): kwargs['fstpso_max_iter'] = 100
-            if 'fstpso_path_fit_dump' not in kwargs.keys(): kwargs['fstpso_path_fit_dump'] = None
-            if 'fstpso_path_sol_dump' not in kwargs.keys(): kwargs['fstpso_path_sol_dump'] = None
-        if 'mf_shape' not in kwargs.keys(): kwargs['mf_shape'] = 'gauss'       
-        if 'operators' not in kwargs.keys(): kwargs['operators'] = None
-        if 'global_fit' not in kwargs.keys(): kwargs['global_fit'] = False  
-        if 'verbose' not in kwargs.keys(): kwargs['verbose'] = False
-        if 'multiprocessing' not in kwargs.keys(): kwargs['multiprocessing'] = True
-
-                        
-        # Split the data using the hold-out method in a training (default: 75%) 
-        # and test set (default: 25%).
-        ds = DataSplitter()
-
-        if fs_number_of_folds==1: ##### feauture selection with hold-out
-            x_train, y_train, x_val, y_val = ds.holdout(x_data, y_data) 
-
-            cl = Clusterer(x_train=x_train, y_train=y_train, nr_clus=nr_clus)               
-                
-            if kwargs['cluster_method'] == 'fcm':
-                cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fcm', fcm_m=kwargs['fcm_m'], 
-                    fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
-            elif kwargs['cluster_method'] == 'fstpso':
-                cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fstpso', 
-                    fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
-                    fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
-            else:
-                print('The requested clustering method is not (yet) implemented')
-                 
-            # Estimate the membership funtions of the system (default shape: gauss)
-            antecedent_estimator = AntecedentEstimator(x_train, partition_matrix)
-
-            antecedent_parameters = antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'], merge_threshold=kwargs['merge_threshold'])
-            what_to_drop = antecedent_estimator._info_for_simplification
-
-            # Build a first-order Takagi-Sugeno model using Simpful using dummy 
-            # consequent parameters to calculate the firing strengths for each 
-            # data instance         
-            fsc=FireStrengthCalculator(antecedent_parameters, nr_clus, var_names, **kwargs)
-            firing_strengths = fsc.calculate_fire_strength(x_train)
-            
-            # Estimate the parameters of the consequent
-            ce = ConsequentEstimator(x_train, y_train, firing_strengths)
-            
-            if self.model_order=='first':
-                consequent_parameters = ce.suglms()
-            elif self.model_order== 'zero':
-                consequent_parameters = ce.zero_order()
-
-            # Build a first-order Takagi-Sugeno model using Simpful
-            simpbuilder = SugenoFISBuilder(
-                antecedent_parameters, 
-                consequent_parameters, 
-                var_names, 
-                extreme_values = antecedent_estimator._extreme_values,
-                operators=kwargs['operators'], 
-                model_order=self.model_order,
-                save_simpful_code=False, 
-                fuzzy_sets_to_drop=what_to_drop,
-                verbose=kwargs['verbose'])
-
-            model = simpbuilder.simpfulmodel
-            
-            # Test the model
-            test = SugenoFISTester(model=model, test_data=x_val, golden_standard=y_val,variable_names=var_names)
-            performance= test.calculate_performance(metric=self.performance_metric)
-        
-        elif fs_number_of_folds>1:  ##### feauture selection with cross validation
-            fold_indices = ds.kfold(data_length=np.shape(x_data)[0], number_of_folds=fs_number_of_folds)
-
-            if kwargs['multiprocessing'] == True: 
-                arg=[]
-            else:
-                perf = np.zeros([1, fs_number_of_folds])
-    
-            for fold_number in range(0, fs_number_of_folds):
-                
-                # Choose the indices for training and testing for this fold
-                tst_idx=fold_indices[fold_number]
-                np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
-                trn_idx=np.concatenate(np.delete(fold_indices, fold_number, axis=0))       # Use all indices, except the ones that are used for testing
-                
-                x_train = np.array([x_data[i,:] for i in trn_idx])
-                x_val = np.array([x_data[i,:] for i in tst_idx])                      
-                y_train = np.array([y_data[i] for i in trn_idx])
-                y_val = np.array([y_data[i] for i in tst_idx]) 
-                
-                if kwargs['multiprocessing'] == True: 
-                    arg.append([x_train, y_train, x_val, y_val, nr_clus, var_names])
-                else:
-                    perf[:,fold_number]=self._create_model(x_train=x_train, y_train=y_train, x_test= x_val, y_test=y_val, nr_clus= self.nr_clus, var_names = self.variable_names, **kwargs)
-            
-            if kwargs['multiprocessing'] == True: 
-                try:
-                    from multiprocessing import Pool
-                except ImportError:
-                        raise Exception('pyFUME uses multiprocessing to parallelize computations, but couldn`t find \'multiprocessing\'. Please pip install multiprocessing to proceed.')
-                
-                try:
-                    with Pool(fs_number_of_folds) as p:
-                        perf=p.starmap(func=self._create_model, iterable=arg)
-                except RuntimeError:
-                    raise Exception('ERROR: main module was not safely imported. Feature selection exploits multiprocessing, so please add a `if _name_ == `_main_`: `-line to your main script. See https://docs.python.org/2/library/multiprocessing.html#windows for further info')
-                    
-            performance = np.mean(perf)
-                  
-            return performance
-
-   
-    def _create_model(self, x_train, y_train, x_test, y_test, nr_clus, var_names, **kwargs):
-        if np.size(x_train, axis = None) == 0 and self.performance_metrics == 'accuracy':
-            perf = 0
-        elif len(x_train) == 0:
-            perf = np.inf
-        else:
-            # Cluster the training data (in input-output space)
-            cl = Clusterer(x_train=x_train, y_train=y_train, nr_clus=nr_clus)
-            cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fcm')                               
-                    
-            # if kwargs['cluster_method'] == 'fcm':
-            #     cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fcm', fcm_m=kwargs['fcm_m'], 
-            #         fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
-            # elif kwargs['cluster_method'] == 'gk':
-            #     cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='gk')
-            # elif kwargs['cluster_method'] == 'fstpso':
-            #     cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fstpso', 
-            #         fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
-            #         fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
-            # else:
-            #     print('The requested clustering method is not (yet) implemented')
-                 
-            # # Estimate the membership funtions of the system (default shape: gauss)
-            antecedent_estimator = AntecedentEstimator(x_train, partition_matrix)
-            
-            antecedent_parameters = antecedent_estimator.determineMF()
-            #antecedent_parameters = antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'], merge_threshold=kwargs['merge_threshold'])
-            what_to_drop = antecedent_estimator._info_for_simplification
-    
-            # Build a first-order Takagi-Sugeno model using Simpful using dummy consequent parameters
-            fsc=FireStrengthCalculator(antecedent_parameters, nr_clus, var_names)
-            firing_strengths = fsc.calculate_fire_strength(x_train)
-    
-            # Estimate the parameters of the consequent
-            ce = ConsequentEstimator(x_train, y_train, firing_strengths)
-        
-            if self.model_order=='first':
-                consequent_parameters = ce.suglms()
-            elif self.model_order== 'zero':
-                consequent_parameters = ce.zero_order()
-                
-            # Build a first-order Takagi-Sugeno model using Simpful
-            simpbuilder = SugenoFISBuilder(
-                antecedent_parameters, 
-                consequent_parameters, 
-                var_names, 
-                extreme_values = antecedent_estimator._extreme_values, 
-                model_order=self.model_order,
-                save_simpful_code=False, 
-                fuzzy_sets_to_drop=what_to_drop,
-                verbose=False)
-    
-            model = simpbuilder.simpfulmodel
-            
-            # Test the model
-            test = SugenoFISTester(model=model, test_data=x_test, golden_standard=y_test, variable_names=var_names)
-            perf = test.calculate_performance(metric=self.performance_metric) 
-        return perf
+from .LoadData import DataLoader
+from .Splitter import DataSplitter
+from .SimpfulModelBuilder import SugenoFISBuilder
+from .Clustering import Clusterer
+from .EstimateAntecendentSet import AntecedentEstimator
+from .FireStrengthCalculator import FireStrengthCalculator
+from .EstimateConsequentParameters import ConsequentEstimator
+from .Tester import SugenoFISTester
+import numpy as np
+import pandas as pd
+
+class FeatureSelector(object):
+    """
+        Creates a new feature selection object.
+        
+        Args:
+            dataX: The input data.
+            dataY: The output data (true label/golden standard).
+            nr_clus: Number of clusters that should be identified in the data.
+            variable_names: Names of the variables
+            **kwargs: Additional arguments to change settings of the fuzzy model.
+    """
+    def __init__(self, dataX, dataY, nr_clus, variable_names, model_order='first', performance_metric='MAE', verbose=True, **kwargs):
+        self.dataX=dataX
+        self.dataY=dataY
+        self.nr_clus = nr_clus
+        self.variable_names = variable_names
+        self.performance_metric = performance_metric
+        self.model_order=model_order
+        self.verbose=verbose
+        
+    def log_wrapper(self, raw_data, **kwargs):
+        """
+            Performs feature selection using the wrapper method while also checking whether .
+            
+            Args:
+                **kwargs: Additional arguments to change settings of the fuzzy model.
+                
+            Returns:
+                Tuple containing (selected_features, selected_feature_names)
+                    - selected_features: The indices of the selected features.
+                    - selected_feature_names: The names of the selected features. 
+
+        """
+            
+        # Create a training and validation set for the feature selection phase
+        x_feat = self.dataX.copy()
+        y_feat = self.dataY.copy()
+        
+        
+        # Set negative or value == 0 to small number to be able to perform log
+        epsilon = np.finfo(np.float64).eps
+        raw_data[raw_data <= 0] = epsilon
+        
+        x_logged = np.log(raw_data)
+        x_logged_norm = (x_logged - np.nanmin(x_logged, axis =0)) / (np.nanmax(x_logged, axis =0)-np.nanmin(x_logged, axis =0))
+
+        # Set initial values for the performance
+        if self.performance_metric != 'accuracy' and self.performance_metric !=  'AUC': 
+            old_performance=np.inf
+            new_performance=np.inf
+            perfs=[]
+        elif self.performance_metric == 'accuracy' or self.performance_metric == 'AUC':
+            old_performance=-np.inf
+            new_performance=-np.inf
+            perfs=[]
+        else: 
+            raise Exception('Unknown performance metric.')
+    
+        # Create a set with the unselected (currently all) and selected (none yet) variables
+        selected_features=[]
+        unselected_features=list(range(0,np.size(x_feat,axis=1)))
+        
+        # Keep a (at this point empty) lists of which variables should be log-transformed
+        logvars = []
+        logvars_num = []
+        temp_logvars_num = []
+        temp_logvars  = []
+        
+        stop=False
+
+        while stop == False: 
+            
+            if self.performance_metric != 'accuracy': 
+                perfs= [np.inf]*np.size(x_feat,axis=1)
+            elif self.performance_metric == 'accuracy':
+                perfs= [-1*np.inf]*np.size(x_feat,axis=1)
+            else: 
+                raise Exception('Unknown performance metric.')
+            
+            
+            if self.performance_metric != 'accuracy':
+                for f in [x for x in unselected_features if x != -1]:
+                    considered_features = selected_features + [f]
+                    var_names = [self.variable_names[i] for i in considered_features]
+                    
+                    # Prepare training sets
+                    feat=x_feat[:,considered_features]
+                    logged_feature = x_logged_norm[:,f]
+                    
+                    log_feat= feat.copy()
+                    log_feat[:,f]=logged_feature
+    
+                    if self.verbose: print('Evaluating feature sub-set including:', var_names)
+            
+                    normal_perf = self._evaluate_feature_set(x_data=feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
+                    log_perf = self._evaluate_feature_set(x_data=log_feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
+                    if log_perf < normal_perf: 
+                       temp_logvars.append(var_names[-1])
+                       temp_logvars_num.append(f)
+                       if self.verbose: print(" * In this sub-set, the variable(s)", logvars + list([var_names[-1]]), "will be log-transformed.")
+                    elif log_perf > normal_perf and len(logvars)>0:
+                        if self.verbose: print(" * In this sub-set, the variable(s)", logvars, "will be log-transformed.")
+    
+                    perfs[f] = min(normal_perf, log_perf)
+                
+                new_performance=min(perfs)
+                new_feature=unselected_features[perfs.index(new_performance)]
+                    
+                del perfs
+                    
+                if new_performance<old_performance: #*feature_selection_stop:
+                    selected_features.append(new_feature)
+                                    
+                    # Check if the last addded feature should be log-transformed and if so, perform the transformation
+                    if new_feature in temp_logvars_num:
+                           logvars.append(self.variable_names[new_feature])
+                           logvars_num.append(new_feature)
+                           x_feat[new_feature] = x_logged_norm[new_feature]
+                      
+                    unselected_features[new_feature]=-1
+                    old_performance=new_performance
+                    
+                    temp_logvars_num = []
+                    temp_logvars  = []
+    
+                else:
+                    if self.verbose: print('***** FEATURE SELECTION ENDED *****')
+                    if self.verbose: print('The selected features have a', self.performance_metric, 'of:', old_performance)
+                    stop = True 
+                    
+            elif self.performance_metric == 'accuracy':
+                for f in [x for x in unselected_features if x != -1]:
+                    considered_features = selected_features + [f]
+                    var_names = [self.variable_names[i] for i in considered_features]
+                    
+                    # Prepare training sets
+                    feat=x_feat[:,considered_features]
+                    logged_feature = x_logged_norm[:,f]
+                    log_feat = feat.copy()                    
+                    log_feat[:,-1]=logged_feature
+                    
+                    if self.verbose: print('Evaluating feature sub-set including:', var_names)
+            
+                    normal_perf = self._evaluate_feature_set(x_data=feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
+                    log_perf = self._evaluate_feature_set(x_data=log_feat, y_data=y_feat, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
+                    print("Normal performance:", normal_perf, ", Logged performance:", log_perf)
+                    
+                    if log_perf > normal_perf: 
+                       temp_logvars.append(var_names[-1])
+                       temp_logvars_num.append(f)
+                       if self.verbose: print(" * In this sub-set, the variable(s)", logvars + list([var_names[-1]]), "will be log-transformed.")
+                    elif log_perf < normal_perf and len(logvars)>0:
+                        if self.verbose: print(" * In this sub-set, the variable(s)", logvars, "will be log-transformed.")
+    
+                    perfs[f] = max(normal_perf, log_perf)
+    
+                new_performance=max(perfs)
+                new_feature=unselected_features[perfs.index(new_performance)]
+                    
+                del perfs
+                
+                if new_performance>old_performance: #*feature_selection_stop:
+                    selected_features.append(new_feature)
+                                    
+                    # Check if the last addded feature should be log-transformed and if so, perform the transformation
+                    if new_feature in temp_logvars_num:
+                           logvars.append(self.variable_names[new_feature])
+                           logvars_num.append(new_feature)
+                        
+                           x_feat[new_feature] = x_logged_norm[new_feature]
+                      
+                    unselected_features[new_feature]=-1
+                    old_performance=new_performance
+                    
+                    temp_logvars_num = []
+                    temp_logvars  = []
+    
+                else:
+                    if self.verbose: print('***** FEATURE SELECTION ENDED *****')
+                    if self.verbose: print('The selected features have a', self.performance_metric, 'of:', old_performance)
+                    stop = True                 
+       
+        # Show the user which variables were selected, and which ones were log-transformed.
+        selected_feature_names = [self.variable_names[i] for i in selected_features]
+        if self.verbose: 
+            print('The following features were selected:',  selected_feature_names)
+            if len(logvars)>0:
+                print('The following features were log-transformed:', logvars)
+            elif len(logvars)==0:
+                print('None of the selected features was log-transformed.')
+            
+        return selected_features, selected_feature_names, logvars_num, logvars
+
+        
+    def wrapper(self,**kwargs):
+        """
+            Performs feature selection using the wrapper method.
+            
+            Args:
+                **kwargs: Additional arguments to change settings of the fuzzy model.
+                
+            Returns:
+                Tuple containing (selected_features, selected_feature_names)
+                    - selected_features: The indices of the selected features.
+                    - selected_feature_names: The names of the selected features. 
+
+        """
+            
+        # Create a training and validation set for the feature selection phase
+        ds = DataSplitter()
+        x_feat, y_feat, x_val, y_val = ds.holdout(self.dataX, self.dataY)
+        
+        # Set initial values for the performance
+        old_performance=np.inf
+        new_performance=np.inf
+        perfs=[]
+        
+        # Create a set with the unselected (currently all) and selected (none yet) variables
+        selected_features=[]
+        unselected_features=list(range(0,np.size(x_feat,axis=1)))
+        
+        stop=False
+
+        while stop == False: 
+            perfs= [np.inf]*np.size(x_feat,axis=1)
+            
+            for f in [x for x in unselected_features if x != -1]:
+                considered_features = selected_features + [f]
+                var_names = [self.variable_names[i] for i in considered_features]
+                feat=x_feat[:,considered_features]
+                x_validation=x_val[:,considered_features] 
+                if self.verbose==True: 
+                    print('Evaluating feature sub set including:', var_names)
+                
+                try:
+                    perfs[f] = self._evaluate_feature_set(x_data=feat, y_data=y_feat, x_val=x_validation, y_val=y_val, nr_clus=self.nr_clus, var_names=var_names, model_order=self.model_order, performance_metric = self.performance_metric, **kwargs)
+                except RuntimeError:
+                    raise Exception('ERROR: main module was not safely imported. Feature selection exploits multiprocessing, so please add a `if _name_ == `_main_`: `-line to your main script. See https://docs.python.org/2/library/multiprocessing.html#windows for further info.')
+                    import sys
+                    sys.exit(1)
+                    
+            new_performance=min(perfs)
+            new_feature=unselected_features[perfs.index(new_performance)]
+            
+            #print('new feature', new_feature)
+            del perfs
+            
+            if new_performance<old_performance: #*feature_selection_stop:
+                selected_features.append(new_feature)
+                unselected_features[new_feature]=-1
+                old_performance=new_performance
+            else:
+                if self.verbose: print('The selected features have a', self.performance_metric, 'of:', old_performance)
+                stop = True 
+       
+        # selected_feature_names = self.variable_names[selected_features]
+        selected_feature_names = [self.variable_names[i] for i in selected_features]
+        if self.verbose: print('The following features were selected:',  selected_feature_names)
+        
+        return selected_features, selected_feature_names
+
+    def fst_pso_feature_selection(self, max_iter=100, min_clusters=2, max_clusters=10, performance_metric='MAE', **kwargs):
+        """
+            Perform feature selection using the FST-PSO [1] variant of the Integer and Categorical 
+            PSO (ICPSO) proposed by Strasser and colleagues [2]. ICPSO hybridizes PSO and Estimation of Distribution 
+            Algorithm (EDA), which makes it possible to convert a discrete problem to the (real-valued) 
+            problem of estimating the distribution vector of a probabilistic model. Each fitness 
+            evaluation a random solution is generated according to the probability distribution 
+            encoded by the particle. Because the implementation is a variant on FST-PSO, the optimal 
+            settings for the PSO are set automatically.
+
+            If the number of clusters is set to None, this method simultaneously choses the optimal 
+            number of clusters.
+
+            [1] Nobile, M. S., Cazzaniga, P., Besozzi, D., Colombo, R., Mauri, G., & Pasi, G. (2018). 
+            Fuzzy Self-Tuning PSO: A settings-free algorithm for global optimization. Swarm and 
+            evolutionary computation, 39, 70-85.
+            
+            [2] Strasser, S., Goodman, R., Sheppard, J., & Butcher, S. (2016). A new discrete 
+            particle swarm optimization algorithm. In Proceedings of the Genetic and Evolutionary 
+            Computation Conference 2016 (pp. 53-60). 
+            
+            Args:
+                max_iter: The maximum number of iterations used in the PSO (default = 10).
+                min_clusters: The minimum number of clusters to be identified in the data set (only 
+                when nr_clusters = None)
+                max_clusters: The maximum number of clusters to be identified in the data set (only 
+                when nr_clusters = None)
+                performance_metric: The performance metric on which each solution is evaluated (default
+                Mean Absolute Error (MAE))
+                **kwargs: Additional arguments to change settings of the fuzzy model.
+                
+            Returns:
+                Tuple containing (selected_features, selected_feature_names, optimal_number_clusters)
+                    - selected_features: The indices of the selected features.
+                    - selected_feature_names: The names of the selected features.
+                    - optimal_number_clusters: If initially nr_clusters = None, this argument encodes the optimal number of clusters in the data set. If nr_clusters is not None, the optimal_number_clusters is set to nr_clusters.
+
+        """
+        
+        from fstpso import FuzzyPSO
+
+
+        FP = FuzzyPSO()
+
+        # Create the search space for feature selection with number of dimensions D
+        D = np.size(self.dataX,1)
+        
+        s=list([[True, False]]*D)
+        
+        # Add dimension for cluster number selection
+        if self.nr_clus == None:
+            s.append(list(range(min_clusters,max_clusters+1)))
+        
+        # Set search space
+        FP.set_search_space_discrete(s)
+        
+        # Set the fitness function
+        args={'x_train': self.dataX, 'y_train': self.dataY, 'verbose':self.verbose}
+        FP.set_fitness(self._function, arguments=args)
+        
+        if 'fstpso_n_particles' not in kwargs.keys(): kwargs['fstpso_n_particles'] = None
+        elif kwargs['fstpso_n_particles'] != None:
+            FP.set_swarm_size(kwargs['fstpso_n_particles'])
+                
+        # solve problem with FST-PSO
+        _, self.best_performance, self.best_solution = FP.solve_with_fstpso(max_iter=max_iter,verbose=False)
+        
+        if self.nr_clus == None:
+            selected_features=self.best_solution[:-1]
+        else:
+           selected_features=self.best_solution 
+    
+        
+        # Show best solution with fitness value
+        varnams=[i for indx,i in enumerate(self.variable_names) if selected_features[indx]]
+        if self.verbose: print('The following features have been selected:', varnams, 'with a', self.performance_metric, 'of', round(self.best_performance,2))
+        
+        if self.nr_clus == None:
+            optimal_number_clusters=self.best_solution[-1]
+        else:
+            optimal_number_clusters = self.nr_clus
+            
+            
+        return selected_features, varnams, optimal_number_clusters
+
+#    def fun(self, particle):
+#        return sum(particle)
+    
+    def _function(self, particle, arguments, verbose=False, **kwargs):
+        from itertools import compress 
+        if self.nr_clus == None:
+            A = arguments['x_train'][:,particle[:-1]]
+            varnams=list(compress(self.variable_names, particle[:-1]))
+            nr_clus=particle[-1]
+        else:
+            A = arguments['x_train'][:,particle[:]]
+            varnams=list(compress(self.variable_names, particle[:]))
+            nr_clus=self.nr_clus
+        
+        if A.shape[1]==0: ## If no features are selected, return a infinite high error
+            error=np.inf
+        else:
+            error=self._evaluate_feature_set(x_data=A, y_data=arguments['y_train'], nr_clus=nr_clus, var_names=varnams, model_order=self.model_order, performance_metric=self.performance_metric, **kwargs)
+            
+        if verbose: print(" * Fitness: %.3f" % error)
+        return error
+    
+    def _evaluate_feature_set(self, x_data, y_data, nr_clus, var_names, model_order='first', performance_metric='MAE', fs_number_of_folds=3, **kwargs):
+        # Check settings and complete with default settings when needed
+        if 'merge_threshold' not in kwargs.keys(): kwargs['merge_threshold'] = 1.0
+        if 'cluster_method' not in kwargs.keys(): kwargs['cluster_method'] = 'fcm'        
+        if kwargs['cluster_method'] == 'fcm':
+            if 'fcm_m' not in kwargs.keys(): kwargs['fcm_m'] = 2
+            if 'fcm_max_iter' not in kwargs.keys(): kwargs['fcm_maxiter'] = 1000
+            if 'fcm_error' not in kwargs.keys(): kwargs['fcm_error'] = 0.005
+        elif kwargs['cluster_method'] == 'fstpso':
+            if 'fstpso_n_particles' not in kwargs.keys(): kwargs['fstpso_n_particles'] = None
+            if 'fstpso_max_iter' not in kwargs.keys(): kwargs['fstpso_max_iter'] = 100
+            if 'fstpso_path_fit_dump' not in kwargs.keys(): kwargs['fstpso_path_fit_dump'] = None
+            if 'fstpso_path_sol_dump' not in kwargs.keys(): kwargs['fstpso_path_sol_dump'] = None
+        if 'mf_shape' not in kwargs.keys(): kwargs['mf_shape'] = 'gauss'       
+        if 'operators' not in kwargs.keys(): kwargs['operators'] = None
+        if 'global_fit' not in kwargs.keys(): kwargs['global_fit'] = False  
+        if 'verbose' not in kwargs.keys(): kwargs['verbose'] = False
+        if 'multiprocessing' not in kwargs.keys(): kwargs['multiprocessing'] = True
+
+                        
+        # Split the data using the hold-out method in a training (default: 75%) 
+        # and test set (default: 25%).
+        ds = DataSplitter()
+
+        if fs_number_of_folds==1: ##### feauture selection with hold-out
+            x_train, y_train, x_val, y_val = ds.holdout(x_data, y_data) 
+
+            cl = Clusterer(x_train=x_train, y_train=y_train, nr_clus=nr_clus)               
+                
+            if kwargs['cluster_method'] == 'fcm':
+                cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fcm', fcm_m=kwargs['fcm_m'], 
+                    fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
+            elif kwargs['cluster_method'] == 'fstpso':
+                cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fstpso', 
+                    fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
+                    fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
+            else:
+                print('The requested clustering method is not (yet) implemented')
+                 
+            # Estimate the membership funtions of the system (default shape: gauss)
+            antecedent_estimator = AntecedentEstimator(x_train, partition_matrix)
+
+            antecedent_parameters = antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'], merge_threshold=kwargs['merge_threshold'])
+            what_to_drop = antecedent_estimator._info_for_simplification
+
+            # Build a first-order Takagi-Sugeno model using Simpful using dummy 
+            # consequent parameters to calculate the firing strengths for each 
+            # data instance         
+            fsc=FireStrengthCalculator(antecedent_parameters, nr_clus, var_names, **kwargs)
+            firing_strengths = fsc.calculate_fire_strength(x_train)
+            
+            # Estimate the parameters of the consequent
+            ce = ConsequentEstimator(x_train, y_train, firing_strengths)
+            
+            if self.model_order=='first':
+                consequent_parameters = ce.suglms()
+            elif self.model_order== 'zero':
+                consequent_parameters = ce.zero_order()
+
+            # Build a first-order Takagi-Sugeno model using Simpful
+            simpbuilder = SugenoFISBuilder(
+                antecedent_parameters, 
+                consequent_parameters, 
+                var_names, 
+                extreme_values = antecedent_estimator._extreme_values,
+                operators=kwargs['operators'], 
+                model_order=self.model_order,
+                save_simpful_code=False, 
+                fuzzy_sets_to_drop=what_to_drop,
+                verbose=kwargs['verbose'])
+
+            model = simpbuilder.simpfulmodel
+            
+            # Test the model
+            test = SugenoFISTester(model=model, test_data=x_val, golden_standard=y_val,variable_names=var_names)
+            performance= test.calculate_performance(metric=self.performance_metric)
+        
+        elif fs_number_of_folds>1:  ##### feauture selection with cross validation
+            fold_indices = ds.kfold(data_length=np.shape(x_data)[0], number_of_folds=fs_number_of_folds)
+
+            if kwargs['multiprocessing'] == True: 
+                arg=[]
+            else:
+                perf = np.zeros([1, fs_number_of_folds])
+    
+            for fold_number in range(0, fs_number_of_folds):
+                
+                # Choose the indices for training and testing for this fold
+                tst_idx=fold_indices[fold_number]
+                #np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
+
+                new_indices = []
+
+                for i in range(fs_number_of_folds):
+                    if i==fold_number:
+                        continue
+                    else:
+                        new_indices.extend(fold_indices[i])
+                
+                """
+                print(new_indices); exit()
+                print (fold_indices)
+                print (fold_number)
+                print (fold_indices[0])
+                mask = np.ones(len(fold_indices), dtype=bool)
+                mask[[fold_number]] = False
+                print(mask)
+                print (fold_indices[mask, ...])
+                exit()
+
+                trn_idx=np.concatenate(np.delete(fold_indices, fold_number, axis=0))       # Use all indices, except the ones that are used for testing
+                """
+                trn_idx = np.array(new_indices)
+
+                x_train = np.array([x_data[i,:] for i in trn_idx])
+                x_val = np.array([x_data[i,:] for i in tst_idx])                      
+                y_train = np.array([y_data[i] for i in trn_idx])
+                y_val = np.array([y_data[i] for i in tst_idx]) 
+                
+                if kwargs['multiprocessing'] == True: 
+                    arg.append([x_train, y_train, x_val, y_val, nr_clus, var_names])
+                else:
+                    perf[:,fold_number]=self._create_model(x_train=x_train, y_train=y_train, x_test= x_val, y_test=y_val, nr_clus= self.nr_clus, var_names = self.variable_names, **kwargs)
+            
+            if kwargs['multiprocessing'] == True: 
+                try:
+                    from multiprocessing import Pool
+                except ImportError:
+                        raise Exception('pyFUME uses multiprocessing to parallelize computations, but couldn`t find \'multiprocessing\'. Please pip install multiprocessing to proceed.')
+                
+                try:
+                    with Pool(fs_number_of_folds) as p:
+                        perf=p.starmap(func=self._create_model, iterable=arg)
+                except RuntimeError:
+                    raise Exception('ERROR: main module was not safely imported. Feature selection exploits multiprocessing, so please add a `if _name_ == `_main_`: `-line to your main script. See https://docs.python.org/2/library/multiprocessing.html#windows for further info')
+                    
+            performance = np.mean(perf)
+                  
+            return performance
+
+   
+    def _create_model(self, x_train, y_train, x_test, y_test, nr_clus, var_names, **kwargs):
+        if np.size(x_train, axis = None) == 0 and self.performance_metrics == 'accuracy':
+            perf = 0
+        elif len(x_train) == 0:
+            perf = np.inf
+        else:
+            # Cluster the training data (in input-output space)
+            cl = Clusterer(x_train=x_train, y_train=y_train, nr_clus=nr_clus)
+            cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fcm')                               
+                    
+            # if kwargs['cluster_method'] == 'fcm':
+            #     cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fcm', fcm_m=kwargs['fcm_m'], 
+            #         fcm_maxiter=kwargs['fcm_maxiter'], fcm_error=kwargs['fcm_error'])
+            # elif kwargs['cluster_method'] == 'gk':
+            #     cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='gk')
+            # elif kwargs['cluster_method'] == 'fstpso':
+            #     cluster_centers, partition_matrix, _ = cl.cluster(cluster_method='fstpso', 
+            #         fstpso_n_particles=kwargs['fstpso_n_particles'], fstpso_max_iter=kwargs['fstpso_max_iter'],
+            #         fstpso_path_fit_dump=kwargs['fstpso_path_fit_dump'], fstpso_path_sol_dump=kwargs['fstpso_path_sol_dump'])
+            # else:
+            #     print('The requested clustering method is not (yet) implemented')
+                 
+            # # Estimate the membership funtions of the system (default shape: gauss)
+            antecedent_estimator = AntecedentEstimator(x_train, partition_matrix)
+            
+            antecedent_parameters = antecedent_estimator.determineMF()
+            #antecedent_parameters = antecedent_estimator.determineMF(mf_shape=kwargs['mf_shape'], merge_threshold=kwargs['merge_threshold'])
+            what_to_drop = antecedent_estimator._info_for_simplification
+    
+            # Build a first-order Takagi-Sugeno model using Simpful using dummy consequent parameters
+            fsc=FireStrengthCalculator(antecedent_parameters, nr_clus, var_names)
+            firing_strengths = fsc.calculate_fire_strength(x_train)
+    
+            # Estimate the parameters of the consequent
+            ce = ConsequentEstimator(x_train, y_train, firing_strengths)
+        
+            if self.model_order=='first':
+                consequent_parameters = ce.suglms()
+            elif self.model_order== 'zero':
+                consequent_parameters = ce.zero_order()
+                
+            # Build a first-order Takagi-Sugeno model using Simpful
+            simpbuilder = SugenoFISBuilder(
+                antecedent_parameters, 
+                consequent_parameters, 
+                var_names, 
+                extreme_values = antecedent_estimator._extreme_values, 
+                model_order=self.model_order,
+                save_simpful_code=False, 
+                fuzzy_sets_to_drop=what_to_drop,
+                verbose=False)
+    
+            model = simpbuilder.simpfulmodel
+            
+            # Test the model
+            test = SugenoFISTester(model=model, test_data=x_test, golden_standard=y_test, variable_names=var_names)
+            perf = test.calculate_performance(metric=self.performance_metric) 
+        return perf
```

### Comparing `pyFUME-0.3.1/pyfume/FireStrengthCalculator.py` & `pyfume-0.3.4/pyfume/FireStrengthCalculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,84 @@
-from .SimpfulModelBuilder import SugenoFISBuilder
-
-import numpy as np
-
-
-class FireStrengthCalculator(object):
-    """
-        Creates a new fire strength calculator object.
-        
-        Args:
-            antecedent_parameters: The parameters of the antecedent sets of the fuzzy model as given as output 
-            by pyFUME's AntecedentEstimator clas (format: shape of the mf, parameters).
-            nr_clus: Number of clusters in the data.
-            variable_names: Names of the variables.
-            fuzzy_sets_to_drop = Fuzzy sets identified by GRsABS to be dropped from the model (default = None).
-            **kwargs: Additional arguments to change settings of the fuzzy model.
-    """
-
-    def __init__(self, antecedent_parameters, nr_clus, variable_names,
-                 fuzzy_sets_to_drop=None, **kwargs):
-
-        self.antecedent_parameters = antecedent_parameters
-        self.nr_clus = nr_clus
-        self.variable_names = variable_names
-        self.what_to_drop = fuzzy_sets_to_drop
-        if 'operators' not in kwargs.keys(): kwargs['operators'] = None
-
-        # Build a first-order Takagi-Sugeno model using Simpful using dummy consequent parameters
-        categorical_indices = kwargs['categorical_indices'] if kwargs['categorical_indices'] is not None else []
-        categorical_extra_rows = sum(len(antecedent_parameters[nr_clus * i][1]) - 2 for i in categorical_indices)
-        simpbuilder = SugenoFISBuilder(
-            self.antecedent_parameters,
-            np.tile(1, (self.nr_clus, len(self.variable_names) + 1 + categorical_extra_rows)),
-            self.variable_names,
-            extreme_values=None,
-            operators=kwargs["operators"],
-            save_simpful_code=False,
-            fuzzy_sets_to_drop=self.what_to_drop,
-            verbose=False,
-            categorical_indices=kwargs['categorical_indices']
-        )
-
-        self.dummymodel = simpbuilder.simpfulmodel
-
-    def calculate_fire_strength(self, data):
-        """
-            Calculates the firing strength per rule of the fuzzy model given a data set.
-            
-            Args:
-                data: The data of which the firing strengths per rule should be calculated.
-                
-            Returns:
-                The firing strengths per rule per data point (rows: data point index, column: rule/cluster number).
-        """
-
-        self.data = data
-
-        # Create a dictionary to pass to Simpful
-        input_dict = {}
-        for i in range(len(self.variable_names)):
-            input_dict[self.variable_names[i]] = self.data[:, i]
-
-        # Calculate the firing strengths for each rule for each data point         
-        self.firing_strengths = np.array(self.dummymodel.get_firing_strengths(input_values=input_dict))
-
-        # firing_strengths=[]
-        # for i in range(0,len(self.data)):
-        #     for j in range (0,len(self.variable_names)):
-        #         self.dummymodel.set_variable(self.variable_names[j], self.data[i,j])
-        #     firing_strengths.append(self.dummymodel.get_firing_strengths())
-        # self.firing_strengths=np.array(firing_strengths)
-        return self.firing_strengths
+from .SimpfulModelBuilder import SugenoFISBuilder
+
+import numpy as np
+
+
+class FireStrengthCalculator(object):
+    """
+        Creates a new fire strength calculator object.
+        
+        Args:
+            antecedent_parameters: The parameters of the antecedent sets of the fuzzy model as given as output 
+            by pyFUME's AntecedentEstimator clas (format: shape of the mf, parameters).
+            nr_clus: Number of clusters in the data.
+            variable_names: Names of the variables.
+            fuzzy_sets_to_drop = Fuzzy sets identified by GRsABS to be dropped from the model (default = None).
+            **kwargs: Additional arguments to change settings of the fuzzy model.
+    """
+
+    def __init__(self, antecedent_parameters, nr_clus, variable_names,
+                 fuzzy_sets_to_drop=None, **kwargs):
+
+        self.antecedent_parameters = antecedent_parameters
+        self.nr_clus = nr_clus
+        self.variable_names = variable_names
+        self.what_to_drop = fuzzy_sets_to_drop
+        if 'operators' not in kwargs.keys(): kwargs['operators'] = None
+
+        # Build a first-order Takagi-Sugeno model using Simpful using dummy consequent parameters
+        # categorical_indices = kwargs['categorical_indices'] if kwargs['categorical_indices'] is not None else []
+        
+        if "categorical_indices" in kwargs.keys():
+            categorical_indices = kwargs['categorical_indices']
+            if categorical_indices is not None:
+                categorical_extra_rows = sum(len(antecedent_parameters[nr_clus * i][1]) - 2 for i in categorical_indices)
+            else:
+                categorical_indices = []
+                categorical_extra_rows = 0
+        else:
+            categorical_indices = []
+            categorical_extra_rows = 0
+         
+        print(self.variable_names) 
+        simpbuilder = SugenoFISBuilder(
+            self.antecedent_parameters,
+            np.tile(1, (self.nr_clus, len(self.variable_names) + 1 + categorical_extra_rows)),
+            self.variable_names,
+            extreme_values=None,
+            operators=kwargs["operators"],
+            save_simpful_code=False,
+            fuzzy_sets_to_drop=self.what_to_drop,
+            verbose=False,
+            categorical_indices=categorical_indices
+        )
+
+        self.dummymodel = simpbuilder.simpfulmodel
+
+    def calculate_fire_strength(self, data):
+        """
+            Calculates the firing strength per rule of the fuzzy model given a data set.
+            
+            Args:
+                data: The data of which the firing strengths per rule should be calculated.
+                
+            Returns:
+                The firing strengths per rule per data point (rows: data point index, column: rule/cluster number).
+        """
+
+        self.data = data
+
+        # Create a dictionary to pass to Simpful
+        input_dict = {}
+        for i in range(len(self.variable_names)):
+            input_dict[self.variable_names[i]] = self.data[:, i]
+
+        # Calculate the firing strengths for each rule for each data point         
+        self.firing_strengths = np.array(self.dummymodel.get_firing_strengths(input_values=input_dict))
+
+        # firing_strengths=[]
+        # for i in range(0,len(self.data)):
+        #     for j in range (0,len(self.variable_names)):
+        #         self.dummymodel.set_variable(self.variable_names[j], self.data[i,j])
+        #     firing_strengths.append(self.dummymodel.get_firing_strengths())
+        # self.firing_strengths=np.array(firing_strengths)
+        return self.firing_strengths
```

### Comparing `pyFUME-0.3.1/pyfume/Sampler.py` & `pyfume-0.3.4/pyfume/Sampler.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import numpy as np
-
-
-class Sampler(object):
-    """
-        Creates a new Sampler object that makes it possible to oversample unbalanced data sets to make them more balanced.
-        
-        Args:
-            train_x: The input data.
-            train_y: The output data (true label/golden standard) on basis which will be sampled.
-            number_of_bins: Number of clusters that should be identified in the data.
-            histogram: True/False flag that determines whether a histogram of the frequencies of the output data will be plotted of both the old and new (= sampled) situation (default = False). The package 'matplotlib.pyplot' is required for this functionality.
-    """
-
-    def __init__(self, train_x, train_y, number_of_bins=5, histogram=False):
-        self.train_x = train_x
-        self.train_y = train_y
-        self.number_of_bins = number_of_bins
-        self.histogram = histogram
-
-    def oversample(self):
-        """
-        Created a more balanced data set by oversampling underrepresented data instances (based on values of the output variable) in the data set.
-
-        Returns:
-            Tuple containing (new_train_x, new_train_y)
-                - new_train_x: The  oversampled input data metrix.
-                - new_train_y: The oversampled output data matrix.
-        """
-        print('Your training data will be oversampled.')
-        data = np.append(self.train_x, self.train_y.reshape(len(self.train_y), 1), axis=1)
-        hist, bins = np.histogram(self.train_y, bins=self.number_of_bins)
-        max_len = max(hist)
-
-        for i in range(1, self.number_of_bins):
-            if i == 1:
-                c = data[self.train_y <= bins[i]]
-                indices = np.random.choice(len(c), max_len - len(c), replace=True)
-                data_new = np.append(data, c[indices], axis=0)
-            elif i > 1 & i != self.number_of_bins - 1:
-                c = data[(self.train_y > bins[i - 1]) & (self.train_y <= bins[i])]
-                indices = np.random.choice(len(c), max_len - len(c), replace=True)
-                data_new = np.append(data_new, c[indices], axis=0)
-
-        new_train_x = data_new[:, :-1]
-        new_train_y = data_new[:, -1]
-
-        if self.histogram is True:
-            import matplotlib.pyplot as plt
-            plt.hist(new_train_y, bins=self.number_of_bins, alpha=0.5, label='Oversampled data', color='blue')
-            plt.hist(self.train_y, bins=self.number_of_bins, alpha=0.5, label='Raw data', color='red')
-            plt.legend(loc='upper right')
-            plt.show()
-
-        return new_train_x, new_train_y
+import numpy as np
+
+
+class Sampler(object):
+    """
+        Creates a new Sampler object that makes it possible to oversample unbalanced data sets to make them more balanced.
+        
+        Args:
+            train_x: The input data.
+            train_y: The output data (true label/golden standard) on basis which will be sampled.
+            number_of_bins: Number of clusters that should be identified in the data.
+            histogram: True/False flag that determines whether a histogram of the frequencies of the output data will be plotted of both the old and new (= sampled) situation (default = False). The package 'matplotlib.pyplot' is required for this functionality.
+    """
+
+    def __init__(self, train_x, train_y, number_of_bins=5, histogram=False):
+        self.train_x = train_x
+        self.train_y = train_y
+        self.number_of_bins = number_of_bins
+        self.histogram = histogram
+
+    def oversample(self):
+        """
+        Created a more balanced data set by oversampling underrepresented data instances (based on values of the output variable) in the data set.
+
+        Returns:
+            Tuple containing (new_train_x, new_train_y)
+                - new_train_x: The  oversampled input data metrix.
+                - new_train_y: The oversampled output data matrix.
+        """
+        print('Your training data will be oversampled.')
+        data = np.append(self.train_x, self.train_y.reshape(len(self.train_y), 1), axis=1)
+        hist, bins = np.histogram(self.train_y, bins=self.number_of_bins)
+        max_len = max(hist)
+
+        for i in range(1, self.number_of_bins):
+            if i == 1:
+                c = data[self.train_y <= bins[i]]
+                indices = np.random.choice(len(c), max_len - len(c), replace=True)
+                data_new = np.append(data, c[indices], axis=0)
+            elif i > 1 & i != self.number_of_bins - 1:
+                c = data[(self.train_y > bins[i - 1]) & (self.train_y <= bins[i])]
+                indices = np.random.choice(len(c), max_len - len(c), replace=True)
+                data_new = np.append(data_new, c[indices], axis=0)
+
+        new_train_x = data_new[:, :-1]
+        new_train_y = data_new[:, -1]
+
+        if self.histogram is True:
+            import matplotlib.pyplot as plt
+            plt.hist(new_train_y, bins=self.number_of_bins, alpha=0.5, label='Oversampled data', color='blue')
+            plt.hist(self.train_y, bins=self.number_of_bins, alpha=0.5, label='Raw data', color='red')
+            plt.legend(loc='upper right')
+            plt.show()
+
+        return new_train_x, new_train_y
```

### Comparing `pyFUME-0.3.1/pyfume/SimpfulModelBuilder.py` & `pyfume-0.3.4/pyfume/SimpfulModelBuilder.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from .simpfulfier import *
-import sys
-
-
-class SugenoFISBuilder(object):
-    """
-        Builds the executable Simpful model.
-        
-        Args:
-            antecedent_sets: The parameters for the antecedent sets.
-            consequent_parameters: The parameters for the consequent function.
-            variable_names: The names of the variables.
-            extreme_values: Extreme values to determine the universe of discourse. 
-                If these are not set, the model will function but it will not 
-                be possible to plot the membership functions (default = None).
-            operators=None
-            save_simpful_code: True/False, determines if the Simpful code will 
-                be saved to the same folder as the script (default = True).
-            fuzzy_sets_to_drop: Fuzzy sets that should be droppped from the 
-                model (default = None).
-    
-    """
-
-    def __init__(self, antecedent_sets, consequent_parameters,
-                 variable_names, normalization_values=None, model_order='first', extreme_values=None,
-                 operators=None, save_simpful_code=True, fuzzy_sets_to_drop=None, setnes_dropped_antecedents=None, verbose=True, categorical_indices=None):
-        # super(SugenoFISBuilder, self).__init__()
-        super().__init__()
-
-        # if normalization_values != None:
-        #     print('variable names:', variable_names)
-        #     print('Antecedent sets:', antecedent_sets)
-        #     print('Consequent parameters:', consequent_parameters)
-        #     print('Normalization values:', normalization_values)
-        #     sys.exit()            
-
-        self._SC = SimpfulConverter(
-            input_variables_names=variable_names,
-            consequents_matrix=consequent_parameters,
-            fuzzy_sets=antecedent_sets,
-            operators=operators,
-            extreme_values=extreme_values,
-            model_order=model_order,
-            fuzzy_sets_to_drop=fuzzy_sets_to_drop,
-            setnes_dropped_antecedents=setnes_dropped_antecedents,
-            verbose=verbose,
-            categorical_indices=categorical_indices)
-        # save_simpful_code can be either True (save on default file), 
-        # False (not not save anything), or a path to a file.
-        if save_simpful_code is True:
-            self._SC.save_code("Simpful_code.py")
-        elif save_simpful_code is not False:
-            self._SC.save_code(save_simpful_code)
-
-        self._SC.generate_object()
-
-        self.simpfulmodel = self._SC._fuzzyreasoner
-
-    def get_model(self):
-        return self.simpfulmodel
+from .simpfulfier import *
+import sys
+
+
+class SugenoFISBuilder(object):
+    """
+        Builds the executable Simpful model.
+        
+        Args:
+            antecedent_sets: The parameters for the antecedent sets.
+            consequent_parameters: The parameters for the consequent function.
+            variable_names: The names of the variables.
+            extreme_values: Extreme values to determine the universe of discourse. 
+                If these are not set, the model will function but it will not 
+                be possible to plot the membership functions (default = None).
+            operators=None
+            save_simpful_code: True/False, determines if the Simpful code will 
+                be saved to the same folder as the script (default = True).
+            fuzzy_sets_to_drop: Fuzzy sets that should be droppped from the 
+                model (default = None).
+    
+    """
+
+    def __init__(self, antecedent_sets, consequent_parameters,
+                 variable_names, normalization_values=None, model_order='first', extreme_values=None,
+                 operators=None, save_simpful_code=True, fuzzy_sets_to_drop=None, setnes_dropped_antecedents=None, verbose=True, categorical_indices=None):
+        # super(SugenoFISBuilder, self).__init__()
+        super().__init__()
+
+        # if normalization_values != None:
+        #     print('variable names:', variable_names)
+        #     print('Antecedent sets:', antecedent_sets)
+        #     print('Consequent parameters:', consequent_parameters)
+        #     print('Normalization values:', normalization_values)
+        #     sys.exit()            
+
+        self._SC = SimpfulConverter(
+            input_variables_names=variable_names,
+            consequents_matrix=consequent_parameters,
+            fuzzy_sets=antecedent_sets,
+            operators=operators,
+            extreme_values=extreme_values,
+            model_order=model_order,
+            fuzzy_sets_to_drop=fuzzy_sets_to_drop,
+            setnes_dropped_antecedents=setnes_dropped_antecedents,
+            verbose=verbose,
+            categorical_indices=categorical_indices)
+        # save_simpful_code can be either True (save on default file), 
+        # False (not not save anything), or a path to a file.
+        if save_simpful_code is True:
+            self._SC.save_code("Simpful_code.py")
+        elif save_simpful_code is not False:
+            self._SC.save_code(save_simpful_code)
+
+        self._SC.generate_object()
+
+        self.simpfulmodel = self._SC._fuzzyreasoner
+
+    def get_model(self):
+        return self.simpfulmodel
```

### Comparing `pyFUME-0.3.1/pyfume/Splitter.py` & `pyfume-0.3.4/pyfume/Splitter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import numpy as np
-import random
-
-
-class DataSplitter(object):
-    """
-        Creates an object that can (provide the indices to) split the data in a 
-            training and test for model validation.
-    """
-
-    def __init__(self, seed=None):
-        random.seed(seed)
-    #    def __init__(self):#, dataX, dataY):
-    #        self.data=np.loadtxt(datapath,delimiter=',')
-    #        self.dataX=self.data[:,0:-1]
-    #        self.dataY=self.data[:,-1]
-    #        self.dataX=dataX
-    #        self.dataY=dataY
-
-    def holdout(self, dataX, dataY, percentage_training=0.75):
-        """
-            Splits the data in a training and test set using the hold-out method.
-            
-                Args:
-                    dataX: The input data.
-                    dataY: The output data (true label/golden standard).
-                    percentage_training: Number between 0 and 1 that indicates the 
-                        percentage of data that should be in the training data set 
-                        (default = 0.75).
-                    
-                Returns:
-                Tuple containing (x_train, y_train, x_test, y_test)
-                        - x_train: Input variables of the training data.
-                        - y_train: Output variables (true label/golden standard) of the training data.
-                        - x_test: Input variables of the test data.
-                        - y_test: Output variables (true label/golden standard) of the test data.
-        """
-
-        universe = set(range(0, np.shape(dataX)[0]))
-        trn = np.random.choice(dataX.shape[0], int(round(percentage_training * dataX.shape[0])), replace=False)
-        tst = list(universe - set(trn))
-
-        x_train = dataX[trn]
-        x_test = dataX[tst]
-        y_train = dataY[trn]
-        y_test = dataY[tst]
-
-        return x_train, y_train, x_test, y_test
-
-    def kfold(self, data_length, number_of_folds=10):
-        """
-            Provides the user with indices for 'k' number of  folds for the training 
-                and testing of the model.
-            
-            Args:
-                data_length: The total number of instances in the data sets 
-                    (number of rows).
-                number_of_folds: The number of folds the data should be split in 
-                    (default = 10)
-    
-            Returns:
-                A list with k (non-overlapping) sublists each containing the indices for one fold.
-        """
-
-        idx = np.arange(0, data_length)
-        random.shuffle(idx)
-
-        fold_indices = np.array_split(idx, number_of_folds)
-
-        return fold_indices
+import numpy as np
+import random
+
+
+class DataSplitter(object):
+    """
+        Creates an object that can (provide the indices to) split the data in a 
+            training and test for model validation.
+    """
+
+    def __init__(self, seed=None):
+        random.seed(seed)
+    #    def __init__(self):#, dataX, dataY):
+    #        self.data=np.loadtxt(datapath,delimiter=',')
+    #        self.dataX=self.data[:,0:-1]
+    #        self.dataY=self.data[:,-1]
+    #        self.dataX=dataX
+    #        self.dataY=dataY
+
+    def holdout(self, dataX, dataY, percentage_training=0.75):
+        """
+            Splits the data in a training and test set using the hold-out method.
+            
+                Args:
+                    dataX: The input data.
+                    dataY: The output data (true label/golden standard).
+                    percentage_training: Number between 0 and 1 that indicates the 
+                        percentage of data that should be in the training data set 
+                        (default = 0.75).
+                    
+                Returns:
+                Tuple containing (x_train, y_train, x_test, y_test)
+                        - x_train: Input variables of the training data.
+                        - y_train: Output variables (true label/golden standard) of the training data.
+                        - x_test: Input variables of the test data.
+                        - y_test: Output variables (true label/golden standard) of the test data.
+        """
+
+        universe = set(range(0, np.shape(dataX)[0]))
+        trn = np.random.choice(dataX.shape[0], int(round(percentage_training * dataX.shape[0])), replace=False)
+        tst = list(universe - set(trn))
+
+        x_train = dataX[trn]
+        x_test = dataX[tst]
+        y_train = dataY[trn]
+        y_test = dataY[tst]
+
+        return x_train, y_train, x_test, y_test
+
+    def kfold(self, data_length, number_of_folds=10):
+        """
+            Provides the user with indices for 'k' number of  folds for the training 
+                and testing of the model.
+            
+            Args:
+                data_length: The total number of instances in the data sets 
+                    (number of rows).
+                number_of_folds: The number of folds the data should be split in 
+                    (default = 10)
+    
+            Returns:
+                A list with k (non-overlapping) sublists each containing the indices for one fold.
+        """
+
+        idx = np.arange(0, data_length)
+        random.shuffle(idx)
+
+        fold_indices = np.array_split(idx, number_of_folds)
+
+        return fold_indices
```

### Comparing `pyFUME-0.3.1/pyfume/Tester.py` & `pyfume-0.3.4/pyfume/Tester.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-from collections import defaultdict
-from math import sqrt
-import numpy as np
-
-
-class SugenoFISTester(object):
-    """
-    Creates a new Tester object to be able to calculate performance metrics of the fuzzy model.
-    
-    Args:
-        model: The model for which the performance metrics should be calculated
-        test_data: The data to be used to compute the performance metrics
-        variable_names: A list of the variables names of the test data (which 
-            should correspond with the variable names used in the model).
-        golden_standard: The 'True' labels of the test data. If not provided, the 
-            only predictions labels can be generated, but the error will not be 
-            calculated (default = None).
-        list_of_outputs: List of the output names (which should correspond with 
-            the output names used in the model) (default: OUTPUT).
-    """
-
-    def __init__(self, model, test_data, variable_names, golden_standard=None, list_of_outputs=['OUTPUT'], categorical_indices=None):
-        super().__init__()
-        self._model_to_test = model
-        self._data_to_test = test_data
-        self._golden_standard = golden_standard
-        self._variable_names = variable_names
-        self._list_of_outputs = list_of_outputs
-        self._categorical_indices = categorical_indices if categorical_indices is not None else []
-
-    def predict(self):
-        """
-        Calculates the predictions labels of the test data using the fuzzy model.
-
-        Returns:
-            Tuple containing (result, error)
-                - result: Prediction labels.
-                - error: The difference between the prediction label and the 'true' label.
-        """
-        result = []
-        for sample in self._data_to_test:
-            for i, variable in enumerate(self._variable_names):
-                if i in self._categorical_indices:
-                    self._model_to_test.set_variable(variable, sample[i])
-                else:
-                    self._model_to_test.set_variable(variable, sample[i])
-            result.append(self._model_to_test.Sugeno_inference().get('OUTPUT'))
-        result = np.array(result)
-        if self._golden_standard is not None:
-            error = self._golden_standard - result
-        else:
-            error = np.nan
-            # print('The true labels (golden standard) were not provided, so the error could not be calculated.')
-        return result, error
-
-    def calculate_performance(self, metric='MAE'):
-        """
-        Calculates the performance of the model given the test data.
-
-            Args:
-                metric: The performance metric to be used to evaluate the model. Choose from: Mean Absolute Error 
-                ('MAE'), Mean Squared Error ('MSE'),  Root Mean Squared Error ('RMSE'), Mean Absolute Percentage 
-                Error ('MAPE').
-        
-        Returns:
-            The performance as expressed by the chosen performance metric.
-        """
-        if metric == 'MAE':
-            err = self.calculate_MAE()
-        elif metric == 'MSE':
-            err = self.calculate_MSE()
-        elif metric == 'RMSE':
-            err = self.calculate_RMSE()
-        elif metric == 'MAPE':
-            err = self.calculate_MAPE()
-        elif metric == 'accuracy':
-            err = self.calculate_accuracy()
-        elif metric == 'AUC':
-            err = self.calculate_AUC()
-        else:
-            print('The requested performance metric has not been implemented (yet).')
-
-        return err
-
-    def calculate_RMSE(self):
-        """
-        Calculates the Root Mean Squared Error of the model given the test data.
-        
-        Returns:
-            The Root Mean Squared Error of the fuzzy model.
-        """
-        _, error = self.predict()
-        return sqrt(np.mean(np.square(error)))
-
-    def calculate_MSE(self):
-        """
-        Calculates the Mean Squared Error of the model given the test data.
-        
-        Returns:
-            The Mean Squared Error of the fuzzy model.
-        """
-        _, error = self.predict()
-        return np.mean(np.square(error))
-
-    def calculate_MAE(self):
-        """
-        Calculates the Mean Absolute Error of the model given the test data.
-        
-        Returns:
-            The Mean Absolute Error of the fuzzy model.
-        """
-        _, error = self.predict()
-        return np.mean(np.abs(error))
-
-    def calculate_MAPE(self):
-        """
-        Calculates the Mean Absolute Percentage Error of the model given the test data.
-        
-        Returns:
-            The Mean Absolute Percentage Error of the fuzzy model.
-        """
-
-        if self._golden_standard is None:
-            raise Exception('To compute the MAPE the true label (golden standard) of the test data should be provided.')
-
-        _, error = self.predict()
-        return np.mean(np.abs((error) / self._golden_standard)) * 100
-
-    def calculate_accuracy(self, threshold=0.5):
-        """
-        Calculates the accuracy of the model for binary problems, given the test data and a discretization threshold .
-        
-        Args:
-            treshold: The treshold to discretize the predicted output in binary categories.
-        Returns:
-            The accuracy of the fuzzy model.
-        """
-
-        confusion_matrix = self.generate_confusion_matrix(threshold=threshold)
-        acc = round((confusion_matrix['TP'] + confusion_matrix['TN']) / (
-                    confusion_matrix['TP'] + confusion_matrix['TN'] + confusion_matrix['FP'] + confusion_matrix['FN']),
-                    3)
-        return acc
-
-    def generate_confusion_matrix(self, threshold=0.5):
-        """
-        Calculates the confusion matrix for binary output data.
-        
-        Args:
-            treshold: The treshold to discretize the predicted output in binary categories.
-        
-        Returns:
-            Dictionary containing the confusion martrix.
-        """
-        # Check if golden standard is present
-        if self._golden_standard is None:
-            raise Exception(
-                'To calculate the confusion matrix, the true label (golden standard) of the test data should be provided.')
-
-            # Get the predicted values for the test data
-        ypred, _ = self.predict()
-
-        # discretize ypred using a user-specified thresehold
-        discrete_ypred = np.digitize(ypred, bins=[threshold])
-
-        # Create the confusion matrix as a dictionary
-        confusion_matrix = dict()
-
-        confusion_matrix['TP'] = np.sum(np.logical_and(discrete_ypred == 1, self._golden_standard == 1))
-        confusion_matrix['TN'] = np.sum(np.logical_and(discrete_ypred == 0, self._golden_standard == 0))
-        confusion_matrix['FP'] = np.sum(np.logical_and(discrete_ypred == 1, self._golden_standard == 0))
-        confusion_matrix['FN'] = np.sum(np.logical_and(discrete_ypred == 0, self._golden_standard == 1))
-        return confusion_matrix
-
-    def calculate_AUC(self, number_of_slices=25, show_plot=False):
-        """
-        Calculates the area under the ROC curve (AUC) for models with binary output data.
-        
-        Args:
-            number_of_slices: More slices give a higher precision of the AUC, against the cost of higher computational costs.
-        
-        Returns:
-            AUC.
-        """
-
-        ROC = np.array([])
-        for T in np.linspace(0, 1, number_of_slices):
-            con_mat = self.generate_confusion_matrix(threshold=T)
-            TPR = self.calculate_TPR(con_mat)
-            FPR = self.calculate_FPR(con_mat)
-            ROC = np.append(ROC, [FPR, TPR])
-        ROC = ROC.reshape(-1, 2)
-
-        fpr, tpr = ROC[:, 0], ROC[:, 1]
-        AUC = 0
-        for k in range(0, number_of_slices - 1):
-            AUC = AUC + ((fpr[k] - fpr[k + 1]) * tpr[k + 1]) + ((1 / 2) * (fpr[k] - fpr[k + 1]) * (tpr[k] - tpr[k + 1]))
-
-        if show_plot:
-            import matplotlib.pyplot as plt
-            plt.figure(figsize=(16, 8))
-            plt.scatter(ROC[:, 0], ROC[:, 1], s=100)
-            plt.plot([0, 1], [0, 1], ls='--', c='darkgrey')
-            plt.title('ROC Curve with AUC = %.2f' % AUC)
-            plt.xlabel('False Positive Rate')
-            plt.ylabel('True Positive Rate')
-
-        return AUC
-
-    def calculate_TPR(self, confusion_matrix):
-        """
-        Calculates the true positive rate, given the confusion matrix for binary output data.
-        
-        Args:
-            confusion matrix: confusion matrix (dict) containing TP, FP, TN and FN.
-        
-        Returns:
-            True positive rate.
-        """
-        return confusion_matrix['TP'] / (confusion_matrix['TP'] + confusion_matrix['FN'])
-
-    def calculate_FPR(self, confusion_matrix):
-        """
-        Calculates the false positive rate, given the confusion matrix for binary output data.
-        
-        Args:
-            confusion matrix: confusion matrix (dict) containing TP, FP, TN and FN.
-        
-        Returns:
-            False positive rate.
-        """
-        return confusion_matrix['FP'] / (confusion_matrix['FP'] + confusion_matrix['TN'])
+from collections import defaultdict
+from math import sqrt
+import numpy as np
+
+
+class SugenoFISTester(object):
+    """
+    Creates a new Tester object to be able to calculate performance metrics of the fuzzy model.
+    
+    Args:
+        model: The model for which the performance metrics should be calculated
+        test_data: The data to be used to compute the performance metrics
+        variable_names: A list of the variables names of the test data (which 
+            should correspond with the variable names used in the model).
+        golden_standard: The 'True' labels of the test data. If not provided, the 
+            only predictions labels can be generated, but the error will not be 
+            calculated (default = None).
+        list_of_outputs: List of the output names (which should correspond with 
+            the output names used in the model) (default: OUTPUT).
+    """
+
+    def __init__(self, model, test_data, variable_names, golden_standard=None, list_of_outputs=['OUTPUT'], categorical_indices=None):
+        super().__init__()
+        self._model_to_test = model
+        self._data_to_test = test_data
+        self._golden_standard = golden_standard
+        self._variable_names = variable_names
+        self._list_of_outputs = list_of_outputs
+        self._categorical_indices = categorical_indices if categorical_indices is not None else []
+
+    def predict(self):
+        """
+        Calculates the predictions labels of the test data using the fuzzy model.
+
+        Returns:
+            Tuple containing (result, error)
+                - result: Prediction labels.
+                - error: The difference between the prediction label and the 'true' label.
+        """
+        result = []
+        for sample in self._data_to_test:
+            for i, variable in enumerate(self._variable_names):
+                if i in self._categorical_indices:
+                    self._model_to_test.set_variable(variable, sample[i])
+                else:
+                    self._model_to_test.set_variable(variable, sample[i])
+            result.append(self._model_to_test.Sugeno_inference().get('OUTPUT'))
+        result = np.array(result)
+        if self._golden_standard is not None:
+            error = self._golden_standard - result
+        else:
+            error = np.nan
+            # print('The true labels (golden standard) were not provided, so the error could not be calculated.')
+        return result, error
+
+    def calculate_performance(self, metric='MAE'):
+        """
+        Calculates the performance of the model given the test data.
+
+            Args:
+                metric: The performance metric to be used to evaluate the model. Choose from: Mean Absolute Error 
+                ('MAE'), Mean Squared Error ('MSE'),  Root Mean Squared Error ('RMSE'), Mean Absolute Percentage 
+                Error ('MAPE').
+        
+        Returns:
+            The performance as expressed by the chosen performance metric.
+        """
+        if metric == 'MAE':
+            err = self.calculate_MAE()
+        elif metric == 'MSE':
+            err = self.calculate_MSE()
+        elif metric == 'RMSE':
+            err = self.calculate_RMSE()
+        elif metric == 'MAPE':
+            err = self.calculate_MAPE()
+        elif metric == 'accuracy':
+            err = self.calculate_accuracy()
+        elif metric == 'AUC':
+            err = self.calculate_AUC()
+        else:
+            print('The requested performance metric has not been implemented (yet).')
+
+        return err
+
+    def calculate_RMSE(self):
+        """
+        Calculates the Root Mean Squared Error of the model given the test data.
+        
+        Returns:
+            The Root Mean Squared Error of the fuzzy model.
+        """
+        _, error = self.predict()
+        return sqrt(np.mean(np.square(error)))
+
+    def calculate_MSE(self):
+        """
+        Calculates the Mean Squared Error of the model given the test data.
+        
+        Returns:
+            The Mean Squared Error of the fuzzy model.
+        """
+        _, error = self.predict()
+        return np.mean(np.square(error))
+
+    def calculate_MAE(self):
+        """
+        Calculates the Mean Absolute Error of the model given the test data.
+        
+        Returns:
+            The Mean Absolute Error of the fuzzy model.
+        """
+        _, error = self.predict()
+        return np.mean(np.abs(error))
+
+    def calculate_MAPE(self):
+        """
+        Calculates the Mean Absolute Percentage Error of the model given the test data.
+        
+        Returns:
+            The Mean Absolute Percentage Error of the fuzzy model.
+        """
+
+        if self._golden_standard is None:
+            raise Exception('To compute the MAPE the true label (golden standard) of the test data should be provided.')
+
+        _, error = self.predict()
+        return np.mean(np.abs((error) / self._golden_standard)) * 100
+
+    def calculate_accuracy(self, threshold=0.5):
+        """
+        Calculates the accuracy of the model for binary problems, given the test data and a discretization threshold .
+        
+        Args:
+            treshold: The treshold to discretize the predicted output in binary categories.
+        Returns:
+            The accuracy of the fuzzy model.
+        """
+
+        confusion_matrix = self.generate_confusion_matrix(threshold=threshold)
+        acc = round((confusion_matrix['TP'] + confusion_matrix['TN']) / (
+                    confusion_matrix['TP'] + confusion_matrix['TN'] + confusion_matrix['FP'] + confusion_matrix['FN']),
+                    3)
+        return acc
+
+    def generate_confusion_matrix(self, threshold=0.5):
+        """
+        Calculates the confusion matrix for binary output data.
+        
+        Args:
+            treshold: The treshold to discretize the predicted output in binary categories.
+        
+        Returns:
+            Dictionary containing the confusion martrix.
+        """
+        # Check if golden standard is present
+        if self._golden_standard is None:
+            raise Exception(
+                'To calculate the confusion matrix, the true label (golden standard) of the test data should be provided.')
+
+            # Get the predicted values for the test data
+        ypred, _ = self.predict()
+
+        # discretize ypred using a user-specified thresehold
+        discrete_ypred = np.digitize(ypred, bins=[threshold])
+
+        # Create the confusion matrix as a dictionary
+        confusion_matrix = dict()
+
+        confusion_matrix['TP'] = np.sum(np.logical_and(discrete_ypred == 1, self._golden_standard == 1))
+        confusion_matrix['TN'] = np.sum(np.logical_and(discrete_ypred == 0, self._golden_standard == 0))
+        confusion_matrix['FP'] = np.sum(np.logical_and(discrete_ypred == 1, self._golden_standard == 0))
+        confusion_matrix['FN'] = np.sum(np.logical_and(discrete_ypred == 0, self._golden_standard == 1))
+        return confusion_matrix
+
+    def calculate_AUC(self, number_of_slices=25, show_plot=False):
+        """
+        Calculates the area under the ROC curve (AUC) for models with binary output data.
+        
+        Args:
+            number_of_slices: More slices give a higher precision of the AUC, against the cost of higher computational costs.
+        
+        Returns:
+            AUC.
+        """
+
+        ROC = np.array([])
+        for T in np.linspace(0, 1, number_of_slices):
+            con_mat = self.generate_confusion_matrix(threshold=T)
+            TPR = self.calculate_TPR(con_mat)
+            FPR = self.calculate_FPR(con_mat)
+            ROC = np.append(ROC, [FPR, TPR])
+        ROC = ROC.reshape(-1, 2)
+
+        fpr, tpr = ROC[:, 0], ROC[:, 1]
+        AUC = 0
+        for k in range(0, number_of_slices - 1):
+            AUC = AUC + ((fpr[k] - fpr[k + 1]) * tpr[k + 1]) + ((1 / 2) * (fpr[k] - fpr[k + 1]) * (tpr[k] - tpr[k + 1]))
+
+        if show_plot:
+            import matplotlib.pyplot as plt
+            plt.figure(figsize=(16, 8))
+            plt.scatter(ROC[:, 0], ROC[:, 1], s=100)
+            plt.plot([0, 1], [0, 1], ls='--', c='darkgrey')
+            plt.title('ROC Curve with AUC = %.2f' % AUC)
+            plt.xlabel('False Positive Rate')
+            plt.ylabel('True Positive Rate')
+
+        return AUC
+
+    def calculate_TPR(self, confusion_matrix):
+        """
+        Calculates the true positive rate, given the confusion matrix for binary output data.
+        
+        Args:
+            confusion matrix: confusion matrix (dict) containing TP, FP, TN and FN.
+        
+        Returns:
+            True positive rate.
+        """
+        return confusion_matrix['TP'] / (confusion_matrix['TP'] + confusion_matrix['FN'])
+
+    def calculate_FPR(self, confusion_matrix):
+        """
+        Calculates the false positive rate, given the confusion matrix for binary output data.
+        
+        Args:
+            confusion matrix: confusion matrix (dict) containing TP, FP, TN and FN.
+        
+        Returns:
+            False positive rate.
+        """
+        return confusion_matrix['FP'] / (confusion_matrix['FP'] + confusion_matrix['TN'])
```

### Comparing `pyFUME-0.3.1/pyfume/__init__.py` & `pyfume-0.3.4/pyfume/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from .pyfume import pyFUME
-
-
-from .BuildTakagiSugeno import BuildTSFIS
-from .Clustering import Clusterer
-from .EstimateAntecendentSet import AntecedentEstimator
-from .EstimateConsequentParameters import ConsequentEstimator
-from .FeatureSelection import FeatureSelector
-from .FireStrengthCalculator import FireStrengthCalculator
-from .LoadData import DataLoader
-from .Sampler import Sampler
-from .simpfulfier import SimpfulConverter
-from .SimpfulModelBuilder import SugenoFISBuilder
-from .Splitter import DataSplitter
-from .Tester import SugenoFISTester
+from .pyfume import pyFUME
+
+
+from .BuildTakagiSugeno import BuildTSFIS
+from .Clustering import Clusterer
+from .EstimateAntecendentSet import AntecedentEstimator
+from .EstimateConsequentParameters import ConsequentEstimator
+from .FeatureSelection import FeatureSelector
+from .FireStrengthCalculator import FireStrengthCalculator
+from .LoadData import DataLoader
+from .Sampler import Sampler
+from .simpfulfier import SimpfulConverter
+from .SimpfulModelBuilder import SugenoFISBuilder
+from .Splitter import DataSplitter
+from .Tester import SugenoFISTester
```

### Comparing `pyFUME-0.3.1/pyfume/pyfume.py` & `pyfume-0.3.4/pyfume/pyfume.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,532 +1,536 @@
-from .BuildTakagiSugeno import BuildTSFIS
-from .LoadData import DataLoader
-from .Splitter import DataSplitter
-from .SimpfulModelBuilder import SugenoFISBuilder
-from .Clustering import Clusterer
-from .EstimateAntecendentSet import AntecedentEstimator
-from .FireStrengthCalculator import FireStrengthCalculator
-from .EstimateConsequentParameters import ConsequentEstimator
-from .Tester import SugenoFISTester
-from .FeatureSelection import FeatureSelector
-from .Sampler import Sampler
-from .simpfulfier import SimpfulConverter
-
-import numpy as np
-
-
-class pyFUME(object):
-    """
-        Creates a new fuzzy model.
-        
-        Args:
-            datapath: The path to the csv file containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
-            dataframe: Pandas dataframe containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
-            nr_clus: Number of clusters that should be identified in the data (default = 2).
-            process_categorical: Boolean to indicate whether categorical variables should be processed (default = False).
-            method: At this moment, only Takagi Sugeno models are supported (default = 'Takagi-Sugeno')
-            variable_names: Names of the variables, if not specified the names will be read from the first row of the csv file (default = None).
-            merge_threshold: Threshold for GRABS to drop fuzzy sets from the model. If the jaccard similarity between two sets is higher than this threshold, the fuzzy set will be dropped from the model.
-            remove_flat_threshold: Threshold for FlaMeR to drop fuzzy sets with constant membership from the antecedents. It uses the coefficient of variation (sigma/mu) of the Gaussian MF to estimate the "flatness" of the variable.
-            **kwargs: Additional arguments to change settings of the fuzzy model.
-
-        Returns:
-            An object containing the fuzzy model, information about its setting (such as its antecedent and consequent parameters) and the different splits of the data.
-    """
-    def __init__(self, datapath=None, dataframe=None,
-        nr_clus=2, process_categorical=False,
-        method='Takagi-Sugeno',
-        variable_names=None,
-        merge_threshold=1.,
-        remove_flat_threshold=None,
-        setnes_threshold=0.8,
-        **kwargs):
-      
-        if datapath is None and dataframe is None:
-            raise Exception(
-                "ERROR: a dataset was not specified. Please either use the datapath or dataframe arguments.")
-
-        # if nr_clus<2 and nr_clus!=None:
-        #    raise Exception("Number of clusters should be greater than 1.")
-
-        self.datapath = datapath
-        self.nr_clus = nr_clus
-        self.method = method
-        self.dropped_fuzzy_sets = 0
-        # self.variable_names=variable_names
-
-        if method == 'Takagi-Sugeno' or method == 'Sugeno':
-            if datapath is not None:
-                self.FIS = BuildTSFIS(datapath=self.datapath, nr_clus=self.nr_clus, variable_names=variable_names, process_categorical=process_categorical, merge_threshold=merge_threshold, setnes_threshold=setnes_threshold, **kwargs)
-            else:
-                self.FIS = BuildTSFIS(dataframe=dataframe, nr_clus=self.nr_clus, variable_names=variable_names, process_categorical=process_categorical, merge_threshold=merge_threshold, setnes_threshold=setnes_threshold, **kwargs)
-            if merge_threshold < 1.0 or setnes_threshold < 1.0:
-                self.dropped_fuzzy_sets = self.FIS._antecedent_estimator.get_number_of_dropped_fuzzy_sets()
-        else:
-            raise Exception("This modeling technique has not yet been implemented.")
-
-    def calculate_error(self, method="MAE"):
-        """
-        Calculates the performance of the model given the test data.
-
-            Args:
-                method: The performance metric to be used to evaluate the model (default = 'MAE'). Choose from: Mean Absolute Error 
-                ('MAE'), Mean Squared Error ('MSE'),  Root Mean Squared Error ('RMSE'), Mean Absolute Percentage 
-                Error ('MAPE').
-        
-        Returns:
-            The performance as expressed by the chosen performance metric.
-        """
-        if method == "MSE":
-            return self._get_MSE()
-        elif method == "MAE":
-            return self._get_MAE()
-        elif method == "MAPE":
-            return self._get_MAPE()
-        elif method == "RMSE":
-            return self._get_RMSE()
-        else:
-            # return self._get_MSE()
-            raise Exception("Method '%s' not implemented yet" % (method))
-
-    def predict_test_data(self):
-        """
-        Calculates the predictions labels of the test data using the fuzzy model.
-
-        Returns:
-            Prediction labels.
-        """
-        # get the prediction for the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, variable_names=self.FIS.variable_names,
-                               golden_standard=self.FIS.y_test)
-        pred, _ = test.predict()
-        return pred
-
-    def predict_label(self, xdata):
-        """
-        Calculates the predictions labels of a data set using the fuzzy model.
-
-        Args:
-            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the labels should be calculated. 
-
-        Returns:
-            Prediction labels.
-        """
-        # Normalize the input data if needed
-        if self.FIS.minmax_norm_flag == True:
-            norm_val = self.FIS.normalization_values
-            variable_names, min_values, max_values = zip(*norm_val)
-            xdata = (xdata - np.array(min_values)) / (np.array(max_values) - np.array(min_values))
-
-        # get the prediction for a new data set
-        model = self.get_model()
-        test = SugenoFISTester(model=model, test_data=xdata, golden_standard=None,
-                               variable_names=self.FIS.variable_names)
-        pred, _ = test.predict()
-        return pred
-
-    def normalize_values(self, data):
-        """
-        Calculates the normalized values of a data point, using the same scaling 
-        that was used to training data of the model. This method only works when 
-        the data was normalized using the min-max method.
-
-        Args:
-            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the normalized values should be calculated. 
-
-        Returns:
-            Normalized values.
-        """
-        if self.FIS.minmax_norm_flag == True:
-            norm_val = self.FIS.normalization_values
-            variable_names, min_values, max_values = zip(*norm_val)
-            normalized_data = (data - np.array(min_values)) / (np.array(max_values) - np.array(min_values))
-
-        elif self.FIS.minmax_norm_flag == False:
-            raise Exception('The model was not trained on normalized data, normalization is aborted.')
-
-        return normalized_data
-
-    def denormalize_values(self, data):
-        """
-        Takes normalized data points, and returns the denormalized (raw) values
-        of that data point. This method only works when during modeling the 
-        data was normalized using the min-max method.
-
-        Args:
-            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the normalized values should be calculated. 
-
-        Returns:
-            Normalized values.
-        """
-        if self.FIS.minmax_norm_flag is True:
-            if np.amin(data) < 0 or np.amax(data) > 1:
-                print(
-                    'WARNING: The given value(s) are not between 0 and 1, the denormalization is performed by extrapolating.')
-
-            norm_val = self.FIS.normalization_values
-            variable_names, min_values, max_values = zip(*norm_val)
-            # print(min_values, max_values)
-            denormalized_data = (data * (np.array(max_values) - np.array(min_values))) + np.array(min_values)
-        elif not self.FIS.minmax_norm_flag:
-            raise Exception('The model was not trained on normalized data, normalization is aborted.')
-
-        return denormalized_data
-
-    def test_model(self, xdata, ydata, error_metric='MAE'):
-        """
-        Calculates the performance of the model using the given data.
-
-        Args:
-            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the labels should be calculated. 
-            ydata: The target data (as single-column numpy array).
-            error_metric: The error metric in which the performance should be expressed (default = 'MAE'). Choose from: Mean Absolute Error ('MAE'), Mean Squared Error ('MSE'),  Root Mean Squared Error ('RMSE'), Mean Absolute Percentage Error ('MAPE').
-
-        Returns:
-            The performance as expressed in the chosen metric.
-        """
-        # get the prediction for a new data set
-        model = self.get_model()
-        test = SugenoFISTester(model=model, test_data=xdata, golden_standard=ydata,
-                               variable_names=self.FIS.variable_names)
-        metric = test.calculate_performance(metric=error_metric)
-        return metric
-
-    #######################
-    ###     GETTERS     ###
-    #######################
-
-    def get_model(self):
-        """
-        Returns the fuzzy model created by pyFUME.
-
-        Returns:
-            The fuzzy model (as an executable object).
-        """
-        if self.FIS.model is None:
-            raise Exception("ERROR: model was not created correctly, aborting.")
-        else:
-            return self.FIS.model
-
-    def get_firing_strengths(self, data, normalize=True):
-        """
-        Calculates the (normalized) firing strength/ activition level of each rule for each data instance of the given data.
-
-        Args:
-            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the labels should be calculated. 
-            normalize: Boolean that indicates whether the retuned fiing strengths should be normalized (normalize = True) or not (normalize = False), When the firing strenghts are nomalized the summed fiing strengths for each data instance equals one.
-        Returns:
-            Firing strength/activition level of each rule (columns) for each data instance (rows).
-        """
-
-        # Calculate the firing strengths
-        fsc = FireStrengthCalculator(self.FIS.antecedent_parameters, self.FIS.nr_clus, self.FIS.variable_names)
-        firing_strengths = fsc.calculate_fire_strength(data)
-        if normalize == True:
-            firing_strengths = firing_strengths / firing_strengths.sum(axis=1)[:, None]
-        return firing_strengths
-
-    def get_performance_per_fold(self):
-        """
-        Returns a list with the performances of each model that is created if crossvalidation is used when training..
-
-        Returns:
-            Perfomance of each cross-validation model.
-        """
-        return self.FIS.performance_metric_per_fold
-
-    def get_fold_indices(self):
-        """
-        Returns a list with the fold indices of each model that is created if crossvalidation is used when training.
-
-        Returns:
-            Fold indices.
-        """
-        return self.FIS.fold_indices
-
-    def _get_RMSE(self):
-        # Calculate the mean squared error of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
-                               variable_names=self.FIS.variable_names)
-        RMSE = test.calculate_RMSE()
-        # RMSE = list(RMSE.values())
-        # print('The RMSE of the fuzzy system is', RMSE)
-        return RMSE
-
-    def _get_MSE(self):
-        # Calculate the mean squared error of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
-                               variable_names=self.FIS.variable_names)
-        MSE = test.calculate_MSE()
-        # RMSE = list(RMSE.values())
-        # print('The RMSE of the fuzzy system is', RMSE)
-        return MSE
-
-    def _get_MAE(self):
-        # Calculate the mean absolute error of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, variable_names=self.FIS.variable_names,
-                               golden_standard=self.FIS.y_test)
-        MAE = test.calculate_MAE()
-        return MAE
-
-    def _get_MAPE(self):
-        # Calculate the mean absolute percentage error of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
-                               variable_names=self.FIS.variable_names)
-        MAPE = test.calculate_MAPE()
-        return MAPE
-
-    def _get_accuracy(self):
-        # Calculate the accuraccy of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
-                               variable_names=self.FIS.variable_names)
-        accuracy = test.calculate_accuracy()
-        return accuracy
-
-    def calculate_AUC(self, number_of_slices=100, show_plot=False):
-        # Calculate the area under the ROC curve of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
-                               variable_names=self.FIS.variable_names)
-        AUC = test.calculate_AUC(number_of_slices, show_plot)
-        return AUC
-
-    def get_confusion_matrix(self):
-        # Calculate the confusion matrix of the model using the test data set
-        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
-                               variable_names=self.FIS.variable_names)
-        con_mat = test.generate_confusion_matrix()
-        return con_mat
-
-    def get_data(self, data_set='test'):
-        """
-        Returns the test or training data set.
-        
-        Args:
-            data_set: Used to specify whether the function should return the training (data_set = "train"), test set (data_set = "test") or both training and test data (data_set = "all"). By default, the function returns the test set. 
-
-        Returns:
-            Tuple (x_data, y_data) containing the test or training data set.
-        """
-
-        if data_set == 'train':
-            return self.FIS.x_train, self.FIS.y_train
-        elif data_set == 'test':
-            return self.FIS.x_test, self.FIS.y_test
-        elif data_set == 'all':
-            xdata = np.concatenate((self.FIS.x_train, self.FIS.x_test), axis=0)
-            ydata = np.concatenate((self.FIS.y_train, self.FIS.y_test), axis=0)
-            return xdata, ydata
-        else:
-            print(
-                'Please specify whether you would like to receive the training (data_set = "train"), test set (data_set = "test") or all data (data_set = "all").')
-
-    def get_cluster_centers(self):
-        """
-        Returns the cluster centers as identified by pyFUME.
-        
-        Returns:
-            cluster centers.
-        """
-        return self.FIS.cluster_centers
-
-        #######################
-
-    ### PLOT FACILITIES ###
-    #######################
-
-    def plot_mf(self, variable_name, output_file='', highlight_element=None, highlight_mf=None, ax=None,
-                xscale='linear'):
-        """
-        Uses Simpful's plotting facilities to plot the membership functions of
-        the pyFUME model.
-
-        Args:
-            variable_name: The variable name whose membership functions should be plotted.
-            output_file: Path and filename where the plot must be saved. By default, the file is not saved.
-            highlight_element: Show the memberships of a specific element of the universe of discourse in the figure.
-            highlight_mf: String indicating the linguistic term/fuzzy set to highlight in the plot.
-            ax: The motplotlib ax where the variable will be plotted.
-
-        """
-        self.get_model().plot_variable(var_name=variable_name, outputfile=output_file, TGT=highlight_element,
-                                       highlight=highlight_mf, ax=ax, xscale=xscale)
-
-    def plot_all_mfs(self, output_file='', figures_per_row=4):
-        """
-        Plots the membership functions of all the variables  in the pyFUME model,
-        each in their own sub figure.
-
-        Args:
-            output_file: path and filename where the plot must be saved.
-            figures_per_row: The number of sub figures per row in the figure.
-        """
-        self.get_model().produce_figure(outputfile=output_file, max_figures_per_row=figures_per_row)
-
-    def plot_consequent_parameters(self, rule_number, output_file='', set_title=True, set_legend=True, ax=None):
-        """
-        Plots the consequent coeffecients of a given rule in a bar chart. If 
-        the training data was normalized, the coeffiecients are plotted as-is. 
-        If the data was not normalized, the coefficients are normalized to 
-        enhance comparability.
-
-        Args:
-            output_file: path and filename where the plot must be saved.
-            figures_per_row: The number of figures per row.
-        """
-        import matplotlib.pyplot as plt
-        from matplotlib.patches import Patch
-
-        # Start counting from 1 instead of 0
-        rule_number = rule_number - 1
-
-        # Get the required data from the pyFUME model
-        labels = self.FIS.selected_variable_names
-        consequent_parameters = self.FIS.consequent_parameters
-        nr_rules = len(consequent_parameters)
-        nr_variables = len(labels)
-
-        # Standardize the parameters if data was not normalized
-        if self.FIS.minmax_norm_flag == False:
-            standard_deviations = np.std(self.FIS.x_train, axis=0)
-            std_y = np.std(self.FIS.y_train)
-            parameters = np.zeros((nr_variables, nr_rules))
-            for rule in range(0, nr_rules):
-                consequent = consequent_parameters[rule]
-                n = np.zeros(nr_variables)
-                for var in range(0, nr_variables):
-                    std = standard_deviations[var]
-                    parameter = consequent[var]
-                    norm = (std / std_y) * parameter
-                    n[var] = norm
-                parameters[:, rule] = n
-
-        # Used the raw values if data was normalized        
-        elif self.FIS.minmax_norm_flag == True:
-            parameters = np.zeros((nr_variables, nr_rules))
-            for rule in range(0, nr_rules):
-                consequent = consequent_parameters[rule]
-                n = np.zeros(nr_variables)
-                for var in range(0, nr_variables):
-                    n[var] = consequent[var]
-                parameters[:, rule] = n
-
-        # Color the bars in the plot based on the relationship to the target variable
-        cc = ['colors'] * len(parameters[:, rule_number])
-        for n, val in enumerate(parameters[:, rule_number]):
-            if val < 0:
-                cc[n] = 'firebrick'
-            elif val >= 0:
-                cc[n] = 'navy'
-
-        # Create the information for the legend
-        legend_elements = [Patch(facecolor='firebrick', label="Negatively related to target variable"),
-                           Patch(facecolor='navy', label="Positively related to target variable")]
-
-        # Create the plot
-        ax.barh(labels, np.abs(parameters[:, rule_number]), align='center', color=cc)
-        ax.grid(color='grey', linestyle='dotted', linewidth=1.5)
-        ax.invert_yaxis()
-        if self.FIS.minmax_norm_flag == False:
-            fig_title = 'Standardized consequent parameters for rule ' + str(rule_number + 1)
-        elif self.FIS.minmax_norm_flag == True:
-            fig_title = 'Consequent parameters for rule ' + str(rule_number + 1)
-        if set_title == True: ax.set_title(fig_title);
-        if set_legend == True: ax.legend(handles=legend_elements)
-        # fig.tight_layout()
-
-        # Save the plot if requested, otherwise just show the plot to the user
-        if ax != None:
-            return ax
-        elif output_file != "":
-            fig = ax.get_figure()
-            fig.savefig(output_file)
-        else:
-            plt.show()
-
-    def _denormalize_antecedent_set(self, data, normalization_values):
-        """
-        Takes a normalized antecedent set, and returns the denormalized parameters
-        defining that set. This method only works when during modeling the 
-        data was normalized using the min-max method.
-    
-        Args:
-            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the normalized values should be calculated. 
-    
-        Returns:
-            Normalized values.
-        """
-
-        (_, min_value, max_value) = normalization_values
-
-        x = data[-1]
-
-        denormalized_mu = (x[0] * (np.array(max_value) - np.array(min_value))) + np.array(min_value)
-        denormalized_sigma = (x[1] * (np.array(max_value) - np.array(min_value)))
-
-        denormalized_set = tuple([data[0], [denormalized_mu, denormalized_sigma]])
-
-        return denormalized_set
-
-    def plot_denormalized_mf(self, variable_name, output_file='', highlight_element=None, highlight_mf=None, ax=None,
-                             xscale='linear'):
-        normalization_values = self.FIS.normalization_values
-        antecedent_sets = self.FIS.antecedent_parameters
-
-        if normalization_values is None:
-            raise Exception(
-                'ERROR: The input data for the pyFUME model was not normalized during training. Denormaliztaion is therefore not possible.')
-
-        # Check if variables were removed (during feature selection)
-        to_keep = []
-        for i in range(0, len(normalization_values)):
-            if normalization_values[i][0] in self.FIS.selected_variable_names:
-                to_keep.append(i)
-
-        # Keep only the values for variables that were selected
-        normalization_values = [normalization_values[i] for i in to_keep]
-
-        # Denormalize the antecedent set parameters
-        denormed_antecedent_sets = []
-
-        x = 0
-        cnt = 0
-        for i in range(0, len(antecedent_sets)):
-            norm_vals = normalization_values[x]
-            denormed_set = self._denormalize_antecedent_set(antecedent_sets[i], norm_vals)
-            denormed_antecedent_sets.append(denormed_set)
-            cnt += 1
-
-            if cnt == self.nr_clus:
-                x += 1
-                cnt = 0
-
-        UoD = []
-        _, mi, ma = zip(*self.FIS.normalization_values)
-        for i in range(0, len(mi)):
-            # UoD.append(tuple((mi[i]-0.05*ma[i],ma[i]+0.05*ma[i])))
-            UoD.append(tuple((mi[i], ma[i])))
-
-        simpbuilder = SugenoFISBuilder(
-            denormed_antecedent_sets,
-            np.tile(1, (self.nr_clus, len(self.FIS.selected_variable_names) + 1)),
-            self.FIS.selected_variable_names,
-            extreme_values=UoD,
-            save_simpful_code='trial.py',
-            fuzzy_sets_to_drop=self.FIS._antecedent_estimator._info_for_simplification,
-            verbose=False)
-        dummymodel = simpbuilder.simpfulmodel
-
-        # Plot the requested variable using Simpful
-        dummymodel.plot_variable(var_name=variable_name, outputfile=output_file, TGT=highlight_element,
-                                 highlight=highlight_mf, ax=ax, xscale=xscale)
-
-
-if __name__ == '__main__':
-    from numpy.random import seed
-
-    seed(4)
-
-    FIS = pyFUME(datapath='Concrete_data.csv', nr_clus=3, method='Takagi-Sugeno',
-                 merge_threshold=.8, operators=None)
-    print("The calculated error is:", FIS.calculate_error())
-
-    FIS.get_model().produce_figure("bla.pdf")
+from .BuildTakagiSugeno import BuildTSFIS
+from .LoadData import DataLoader
+from .Splitter import DataSplitter
+from .SimpfulModelBuilder import SugenoFISBuilder
+from .Clustering import Clusterer
+from .EstimateAntecendentSet import AntecedentEstimator
+from .FireStrengthCalculator import FireStrengthCalculator
+from .EstimateConsequentParameters import ConsequentEstimator
+from .Tester import SugenoFISTester
+from .FeatureSelection import FeatureSelector
+from .Sampler import Sampler
+from .simpfulfier import SimpfulConverter
+
+import numpy as np
+
+
+class pyFUME(object):
+    """
+        Creates a new fuzzy model.
+        
+        Args:
+            datapath: The path to the csv file containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
+            dataframe: Pandas dataframe containing the input data (argument 'datapath' or 'dataframe' should be specified by the user).
+            nr_clus: Number of clusters that should be identified in the data (default = 2).
+            process_categorical: Boolean to indicate whether categorical variables should be processed (default = False).
+            method: At this moment, only Takagi Sugeno models are supported (default = 'Takagi-Sugeno')
+            variable_names: Names of the variables, if not specified the names will be read from the first row of the csv file (default = None).
+            merge_threshold: Threshold for GRABS to drop fuzzy sets from the model. If the jaccard similarity between two sets is higher than this threshold, the fuzzy set will be dropped from the model.
+            remove_flat_threshold: Threshold for FlaMeR to drop fuzzy sets with constant membership from the antecedents. It uses the coefficient of variation (sigma/mu) of the Gaussian MF to estimate the "flatness" of the variable.
+            **kwargs: Additional arguments to change settings of the fuzzy model.
+
+        Returns:
+            An object containing the fuzzy model, information about its setting (such as its antecedent and consequent parameters) and the different splits of the data.
+    """
+    def __init__(self, datapath=None, dataframe=None,
+        nr_clus=2, process_categorical=False,
+        method='Takagi-Sugeno',
+        variable_names=None,
+        merge_threshold=1.,
+        remove_flat_threshold=None,
+        setnes_threshold=0.9,
+        **kwargs):
+      
+        if datapath is None and dataframe is None:
+            raise Exception(
+                "ERROR: a dataset was not specified. Please either use the datapath or dataframe arguments.")
+
+        # if nr_clus<2 and nr_clus!=None:
+        #    raise Exception("Number of clusters should be greater than 1.")
+
+        self.datapath = datapath
+        self.nr_clus = nr_clus
+        self.method = method
+        self.dropped_fuzzy_sets = 0
+        # self.variable_names=variable_names
+
+        if method == 'Takagi-Sugeno' or method == 'Sugeno':
+            if datapath is not None:
+                self.FIS = BuildTSFIS(datapath=self.datapath, 
+                    nr_clus=self.nr_clus, variable_names=variable_names, 
+                    process_categorical=process_categorical, 
+                    merge_threshold=merge_threshold, 
+                    setnes_threshold=setnes_threshold, **kwargs)
+            else:
+                self.FIS = BuildTSFIS(dataframe=dataframe, nr_clus=self.nr_clus, variable_names=variable_names, process_categorical=process_categorical, merge_threshold=merge_threshold, setnes_threshold=setnes_threshold, **kwargs)
+            if merge_threshold < 1.0 or setnes_threshold < 1.0:
+                self.dropped_fuzzy_sets = self.FIS._antecedent_estimator.get_number_of_dropped_fuzzy_sets()
+        else:
+            raise Exception("This modeling technique has not yet been implemented.")
+
+    def calculate_error(self, method="MAE"):
+        """
+        Calculates the performance of the model given the test data.
+
+            Args:
+                method: The performance metric to be used to evaluate the model (default = 'MAE'). Choose from: Mean Absolute Error 
+                ('MAE'), Mean Squared Error ('MSE'),  Root Mean Squared Error ('RMSE'), Mean Absolute Percentage 
+                Error ('MAPE').
+        
+        Returns:
+            The performance as expressed by the chosen performance metric.
+        """
+        if method == "MSE":
+            return self._get_MSE()
+        elif method == "MAE":
+            return self._get_MAE()
+        elif method == "MAPE":
+            return self._get_MAPE()
+        elif method == "RMSE":
+            return self._get_RMSE()
+        else:
+            # return self._get_MSE()
+            raise Exception("Method '%s' not implemented yet" % (method))
+
+    def predict_test_data(self):
+        """
+        Calculates the predictions labels of the test data using the fuzzy model.
+
+        Returns:
+            Prediction labels.
+        """
+        # get the prediction for the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, variable_names=self.FIS.selected_variable_names,
+                               golden_standard=self.FIS.y_test)
+        pred, _ = test.predict()
+        return pred
+
+    def predict_label(self, xdata):
+        """
+        Calculates the predictions labels of a data set using the fuzzy model.
+
+        Args:
+            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the labels should be calculated. 
+
+        Returns:
+            Prediction labels.
+        """
+        # Normalize the input data if needed
+        if self.FIS.minmax_norm_flag == True:
+            norm_val = self.FIS.normalization_values
+            variable_names, min_values, max_values = zip(*norm_val)
+            xdata = (xdata - np.array(min_values)) / (np.array(max_values) - np.array(min_values))
+
+        # get the prediction for a new data set
+        model = self.get_model()
+        test = SugenoFISTester(model=model, test_data=xdata, golden_standard=None,
+                               variable_names=self.FIS.selected_variable_names)
+        pred, _ = test.predict()
+        return pred
+
+    def normalize_values(self, data):
+        """
+        Calculates the normalized values of a data point, using the same scaling 
+        that was used to training data of the model. This method only works when 
+        the data was normalized using the min-max method.
+
+        Args:
+            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the normalized values should be calculated. 
+
+        Returns:
+            Normalized values.
+        """
+        if self.FIS.minmax_norm_flag == True:
+            norm_val = self.FIS.normalization_values
+            variable_names, min_values, max_values = zip(*norm_val)
+            normalized_data = (data - np.array(min_values)) / (np.array(max_values) - np.array(min_values))
+
+        elif self.FIS.minmax_norm_flag == False:
+            raise Exception('The model was not trained on normalized data, normalization is aborted.')
+
+        return normalized_data
+
+    def denormalize_values(self, data):
+        """
+        Takes normalized data points, and returns the denormalized (raw) values
+        of that data point. This method only works when during modeling the 
+        data was normalized using the min-max method.
+
+        Args:
+            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the normalized values should be calculated. 
+
+        Returns:
+            Normalized values.
+        """
+        if self.FIS.minmax_norm_flag is True:
+            if np.amin(data) < 0 or np.amax(data) > 1:
+                print(
+                    'WARNING: The given value(s) are not between 0 and 1, the denormalization is performed by extrapolating.')
+
+            norm_val = self.FIS.normalization_values
+            variable_names, min_values, max_values = zip(*norm_val)
+            # print(min_values, max_values)
+            denormalized_data = (data * (np.array(max_values) - np.array(min_values))) + np.array(min_values)
+        elif not self.FIS.minmax_norm_flag:
+            raise Exception('The model was not trained on normalized data, normalization is aborted.')
+
+        return denormalized_data
+
+    def test_model(self, xdata, ydata, error_metric='MAE'):
+        """
+        Calculates the performance of the model using the given data.
+
+        Args:
+            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the labels should be calculated. 
+            ydata: The target data (as single-column numpy array).
+            error_metric: The error metric in which the performance should be expressed (default = 'MAE'). Choose from: Mean Absolute Error ('MAE'), Mean Squared Error ('MSE'),  Root Mean Squared Error ('RMSE'), Mean Absolute Percentage Error ('MAPE').
+
+        Returns:
+            The performance as expressed in the chosen metric.
+        """
+        # get the prediction for a new data set
+        model = self.get_model()
+        test = SugenoFISTester(model=model, test_data=xdata, golden_standard=ydata,
+                               variable_names=self.FIS.selected_variable_names)
+        metric = test.calculate_performance(metric=error_metric)
+        return metric
+
+    #######################
+    ###     GETTERS     ###
+    #######################
+
+    def get_model(self):
+        """
+        Returns the fuzzy model created by pyFUME.
+
+        Returns:
+            The fuzzy model (as an executable object).
+        """
+        if self.FIS.model is None:
+            raise Exception("ERROR: model was not created correctly, aborting.")
+        else:
+            return self.FIS.model
+
+    def get_firing_strengths(self, data, normalize=True):
+        """
+        Calculates the (normalized) firing strength/ activition level of each rule for each data instance of the given data.
+
+        Args:
+            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the labels should be calculated. 
+            normalize: Boolean that indicates whether the retuned fiing strengths should be normalized (normalize = True) or not (normalize = False), When the firing strenghts are nomalized the summed fiing strengths for each data instance equals one.
+        Returns:
+            Firing strength/activition level of each rule (columns) for each data instance (rows).
+        """
+
+        # Calculate the firing strengths
+        fsc = FireStrengthCalculator(self.FIS.antecedent_parameters, self.FIS.nr_clus, self.FIS.variable_names)
+        firing_strengths = fsc.calculate_fire_strength(data)
+        if normalize == True:
+            firing_strengths = firing_strengths / firing_strengths.sum(axis=1)[:, None]
+        return firing_strengths
+
+    def get_performance_per_fold(self):
+        """
+        Returns a list with the performances of each model that is created if crossvalidation is used when training..
+
+        Returns:
+            Perfomance of each cross-validation model.
+        """
+        return self.FIS.performance_metric_per_fold
+
+    def get_fold_indices(self):
+        """
+        Returns a list with the fold indices of each model that is created if crossvalidation is used when training.
+
+        Returns:
+            Fold indices.
+        """
+        return self.FIS.fold_indices
+
+    def _get_RMSE(self):
+        # Calculate the mean squared error of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
+                               variable_names=self.FIS.selected_variable_names)
+        RMSE = test.calculate_RMSE()
+        # RMSE = list(RMSE.values())
+        # print('The RMSE of the fuzzy system is', RMSE)
+        return RMSE
+
+    def _get_MSE(self):
+        # Calculate the mean squared error of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
+                               variable_names=self.FIS.selected_variable_names)
+        MSE = test.calculate_MSE()
+        # RMSE = list(RMSE.values())
+        # print('The RMSE of the fuzzy system is', RMSE)
+        return MSE
+
+    def _get_MAE(self):
+        # Calculate the mean absolute error of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, variable_names=self.FIS.selected_variable_names,
+                               golden_standard=self.FIS.y_test)
+        MAE = test.calculate_MAE()
+        return MAE
+
+    def _get_MAPE(self):
+        # Calculate the mean absolute percentage error of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
+                               variable_names=self.FIS.variable_names)
+        MAPE = test.calculate_MAPE()
+        return MAPE
+
+    def _get_accuracy(self):
+        # Calculate the accuraccy of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
+                               variable_names=self.FIS.selected_variable_names)
+        accuracy = test.calculate_accuracy()
+        return accuracy
+
+    def calculate_AUC(self, number_of_slices=100, show_plot=False):
+        # Calculate the area under the ROC curve of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
+                               variable_names=self.FIS.selected_variable_names)
+        AUC = test.calculate_AUC(number_of_slices, show_plot)
+        return AUC
+
+    def get_confusion_matrix(self):
+        # Calculate the confusion matrix of the model using the test data set
+        test = SugenoFISTester(model=self.FIS.model, test_data=self.FIS.x_test, golden_standard=self.FIS.y_test,
+                               variable_names=self.FIS.selected_variable_names)
+        con_mat = test.generate_confusion_matrix()
+        return con_mat
+
+    def get_data(self, data_set='test'):
+        """
+        Returns the test or training data set.
+        
+        Args:
+            data_set: Used to specify whether the function should return the training (data_set = "train"), test set (data_set = "test") or both training and test data (data_set = "all"). By default, the function returns the test set. 
+
+        Returns:
+            Tuple (x_data, y_data) containing the test or training data set.
+        """
+
+        if data_set == 'train':
+            return self.FIS.x_train, self.FIS.y_train
+        elif data_set == 'test':
+            return self.FIS.x_test, self.FIS.y_test
+        elif data_set == 'all':
+            xdata = np.concatenate((self.FIS.x_train, self.FIS.x_test), axis=0)
+            ydata = np.concatenate((self.FIS.y_train, self.FIS.y_test), axis=0)
+            return xdata, ydata
+        else:
+            print(
+                'Please specify whether you would like to receive the training (data_set = "train"), test set (data_set = "test") or all data (data_set = "all").')
+
+    def get_cluster_centers(self):
+        """
+        Returns the cluster centers as identified by pyFUME.
+        
+        Returns:
+            cluster centers.
+        """
+        return self.FIS.cluster_centers
+
+        #######################
+
+    ### PLOT FACILITIES ###
+    #######################
+
+    def plot_mf(self, variable_name, output_file='', highlight_element=None, highlight_mf=None, ax=None,
+                xscale='linear'):
+        """
+        Uses Simpful's plotting facilities to plot the membership functions of
+        the pyFUME model.
+
+        Args:
+            variable_name: The variable name whose membership functions should be plotted.
+            output_file: Path and filename where the plot must be saved. By default, the file is not saved.
+            highlight_element: Show the memberships of a specific element of the universe of discourse in the figure.
+            highlight_mf: String indicating the linguistic term/fuzzy set to highlight in the plot.
+            ax: The motplotlib ax where the variable will be plotted.
+
+        """
+        self.get_model().plot_variable(var_name=variable_name, outputfile=output_file, TGT=highlight_element,
+                                       highlight=highlight_mf, ax=ax, xscale=xscale)
+
+    def plot_all_mfs(self, output_file='', figures_per_row=4):
+        """
+        Plots the membership functions of all the variables  in the pyFUME model,
+        each in their own sub figure.
+
+        Args:
+            output_file: path and filename where the plot must be saved.
+            figures_per_row: The number of sub figures per row in the figure.
+        """
+        self.get_model().produce_figure(outputfile=output_file, max_figures_per_row=figures_per_row)
+
+    def plot_consequent_parameters(self, rule_number, output_file='', set_title=True, set_legend=True, ax=None):
+        """
+        Plots the consequent coeffecients of a given rule in a bar chart. If 
+        the training data was normalized, the coeffiecients are plotted as-is. 
+        If the data was not normalized, the coefficients are normalized to 
+        enhance comparability.
+
+        Args:
+            output_file: path and filename where the plot must be saved.
+            figures_per_row: The number of figures per row.
+        """
+        import matplotlib.pyplot as plt
+        from matplotlib.patches import Patch
+
+        # Start counting from 1 instead of 0
+        rule_number = rule_number - 1
+
+        # Get the required data from the pyFUME model
+        labels = self.FIS.selected_variable_names
+        consequent_parameters = self.FIS.consequent_parameters
+        nr_rules = len(consequent_parameters)
+        nr_variables = len(labels)
+
+        # Standardize the parameters if data was not normalized
+        if self.FIS.minmax_norm_flag == False:
+            standard_deviations = np.std(self.FIS.x_train, axis=0)
+            std_y = np.std(self.FIS.y_train)
+            parameters = np.zeros((nr_variables, nr_rules))
+            for rule in range(0, nr_rules):
+                consequent = consequent_parameters[rule]
+                n = np.zeros(nr_variables)
+                for var in range(0, nr_variables):
+                    std = standard_deviations[var]
+                    parameter = consequent[var]
+                    norm = (std / std_y) * parameter
+                    n[var] = norm
+                parameters[:, rule] = n
+
+        # Used the raw values if data was normalized        
+        elif self.FIS.minmax_norm_flag == True:
+            parameters = np.zeros((nr_variables, nr_rules))
+            for rule in range(0, nr_rules):
+                consequent = consequent_parameters[rule]
+                n = np.zeros(nr_variables)
+                for var in range(0, nr_variables):
+                    n[var] = consequent[var]
+                parameters[:, rule] = n
+
+        # Color the bars in the plot based on the relationship to the target variable
+        cc = ['colors'] * len(parameters[:, rule_number])
+        for n, val in enumerate(parameters[:, rule_number]):
+            if val < 0:
+                cc[n] = 'firebrick'
+            elif val >= 0:
+                cc[n] = 'navy'
+
+        # Create the information for the legend
+        legend_elements = [Patch(facecolor='firebrick', label="Negatively related to target variable"),
+                           Patch(facecolor='navy', label="Positively related to target variable")]
+
+        # Create the plot
+        ax.barh(labels, np.abs(parameters[:, rule_number]), align='center', color=cc)
+        ax.grid(color='grey', linestyle='dotted', linewidth=1.5)
+        ax.invert_yaxis()
+        if self.FIS.minmax_norm_flag == False:
+            fig_title = 'Standardized consequent parameters for rule ' + str(rule_number + 1)
+        elif self.FIS.minmax_norm_flag == True:
+            fig_title = 'Consequent parameters for rule ' + str(rule_number + 1)
+        if set_title == True: ax.set_title(fig_title);
+        if set_legend == True: ax.legend(handles=legend_elements)
+        # fig.tight_layout()
+
+        # Save the plot if requested, otherwise just show the plot to the user
+        if ax != None:
+            return ax
+        elif output_file != "":
+            fig = ax.get_figure()
+            fig.savefig(output_file)
+        else:
+            plt.show()
+
+    def _denormalize_antecedent_set(self, data, normalization_values):
+        """
+        Takes a normalized antecedent set, and returns the denormalized parameters
+        defining that set. This method only works when during modeling the 
+        data was normalized using the min-max method.
+    
+        Args:
+            xdata: The input data (as numpy array with each row a different data instance and variables in the same order as in the original training data set) for which the normalized values should be calculated. 
+    
+        Returns:
+            Normalized values.
+        """
+
+        (_, min_value, max_value) = normalization_values
+
+        x = data[-1]
+
+        denormalized_mu = (x[0] * (np.array(max_value) - np.array(min_value))) + np.array(min_value)
+        denormalized_sigma = (x[1] * (np.array(max_value) - np.array(min_value)))
+
+        denormalized_set = tuple([data[0], [denormalized_mu, denormalized_sigma]])
+
+        return denormalized_set
+
+    def plot_denormalized_mf(self, variable_name, output_file='', highlight_element=None, highlight_mf=None, ax=None,
+                             xscale='linear'):
+        normalization_values = self.FIS.normalization_values
+        antecedent_sets = self.FIS.antecedent_parameters
+
+        if normalization_values is None:
+            raise Exception(
+                'ERROR: The input data for the pyFUME model was not normalized during training. Denormaliztaion is therefore not possible.')
+
+        # Check if variables were removed (during feature selection)
+        to_keep = []
+        for i in range(0, len(normalization_values)):
+            if normalization_values[i][0] in self.FIS.selected_variable_names:
+                to_keep.append(i)
+
+        # Keep only the values for variables that were selected
+        normalization_values = [normalization_values[i] for i in to_keep]
+
+        # Denormalize the antecedent set parameters
+        denormed_antecedent_sets = []
+
+        x = 0
+        cnt = 0
+        for i in range(0, len(antecedent_sets)):
+            norm_vals = normalization_values[x]
+            denormed_set = self._denormalize_antecedent_set(antecedent_sets[i], norm_vals)
+            denormed_antecedent_sets.append(denormed_set)
+            cnt += 1
+
+            if cnt == self.nr_clus:
+                x += 1
+                cnt = 0
+
+        UoD = []
+        _, mi, ma = zip(*self.FIS.normalization_values)
+        for i in range(0, len(mi)):
+            # UoD.append(tuple((mi[i]-0.05*ma[i],ma[i]+0.05*ma[i])))
+            UoD.append(tuple((mi[i], ma[i])))
+
+        simpbuilder = SugenoFISBuilder(
+            denormed_antecedent_sets,
+            np.tile(1, (self.nr_clus, len(self.FIS.selected_variable_names) + 1)),
+            self.FIS.selected_variable_names,
+            extreme_values=UoD,
+            save_simpful_code='trial.py',
+            fuzzy_sets_to_drop=self.FIS._antecedent_estimator._info_for_simplification,
+            verbose=False)
+        dummymodel = simpbuilder.simpfulmodel
+
+        # Plot the requested variable using Simpful
+        dummymodel.plot_variable(var_name=variable_name, outputfile=output_file, TGT=highlight_element,
+                                 highlight=highlight_mf, ax=ax, xscale=xscale)
+
+
+if __name__ == '__main__':
+    from numpy.random import seed
+
+    seed(4)
+
+    FIS = pyFUME(datapath='Concrete_data.csv', nr_clus=3, method='Takagi-Sugeno',
+                 merge_threshold=.8, operators=None)
+    print("The calculated error is:", FIS.calculate_error())
+
+    FIS.get_model().produce_figure("bla.pdf")
```

### Comparing `pyFUME-0.3.1/pyfume/simpfulfier.py` & `pyfume-0.3.4/pyfume/simpfulfier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,275 +1,276 @@
-import copy
-
-import simpful
-
-
-class SimpfulConverter(object):
-    """    This object converts a description of a Fuzzy System into a readable
-        Simpful project file.
-
-        Args:
-            input_variables_names: The names of the input variables of the fuzzy model.
-            consequents_matrix: The parameters of the consequent function.
-            fuzzy_sets: list containing a sub-list for each fuzzy set in the model. The sub-list should contain the shape of the fuzzy set (e.g. 'gauss') and the parameters of the function (e.g. mu, sigma). For example: ('gauss', 5, 1).
-            model_order: The order of the fuzzy model ('zero' or 'first') (default = 'first').
-            fuzzy_sets_to_drop: Fuzzy sets that should be disabled in the Simpful code, for example when flagged by GRABS for simplification (default = None).
-            extreme_values: The values that should be used for the universe of discourse for the vaiables in the fuzzy model (default = None).
-            operators: A list of strings, specifying fuzzy operators to be used instead of defaults (default = None). For more information see Simpful's documentation.
-            verbose: Boolean (True/False) that indicates whether extra information will be printed in the user's console (default = True).
-
-    """
-
-    def __init__(self,
-                 input_variables_names,
-                 consequents_matrix,
-                 fuzzy_sets,
-                 model_order='first',
-                 fuzzy_sets_to_drop=None,
-                 setnes_dropped_antecedents=None,
-                 extreme_values=None,
-                 operators=None,
-                 verbose=False,
-                 categorical_indices=None):
-        super().__init__()
-        self._input_variables = input_variables_names
-        self._consequents_matrix = consequents_matrix
-        self._clusters = len(self._consequents_matrix)
-        self._fuzzy_sets = fuzzy_sets
-        self._model_order = model_order
-        self._fuzzy_sets_to_drop = fuzzy_sets_to_drop
-        self._setnes_dropped_antecedents = setnes_dropped_antecedents
-        self._extreme_values = extreme_values
-        self.verbose = verbose
-        if self._fuzzy_sets_to_drop is None:
-            self._fuzzy_sets_to_drop = {}
-        self._categorical_indices = categorical_indices if categorical_indices is not None else []
-
-        if self._setnes_dropped_antecedents is None:
-            self._setnes_dropped_antecedents = {}
-
-        if self._model_order == 'first':
-            if self._categorical_indices is not None:
-                # TEMPORARILY IGNORE
-                # assert (len(self._input_variables) + 1 == len(self._consequents_matrix[0]) + len(self._categorical_indices))
-                pass
-            else:
-                assert (len(self._input_variables) + 1 == len(self._consequents_matrix[0]))
-
-        if self.verbose: print(" * Detected %d rules / clusters" % self._clusters)
-
-        self._source_code = []
-        self._source_code.append('# WARNING: this source code was automatically generated by pyFUME.')
-        self._source_code.append("from simpful import *")
-        if operators is None:
-            self._source_code.append("\nFS = FuzzySystem(show_banner=False)")
-        else:
-            # experimental, please test ASAP
-            self._source_code.append("\nFS = FuzzySystem(operators=" + str(operators) + ")")
-
-    def save_code(self, path):
-        """
-            Saves the Simpful code.
-            
-            Args:
-                path: Path to the folder where the Simpful code should be saved.
-        """
-        code = self.generate_code()
-        with open(path, "w") as fo:
-            fo.write(code)
-        if self.verbose is True:
-            print(" * Code saved to file %s" % path)
-
-    def generate_object(self):
-        """
-            Generates the executable object containing the fuzzy model.
-        """
-        code = self.generate_code()
-        if self.verbose:
-            exec(code, globals())
-        elif self.verbose is False:
-            import os
-            import contextlib
-            with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
-                exec(code, globals())
-
-        from copy import deepcopy
-        self._fuzzyreasoner = deepcopy(FS)
-
-    def generate_code(self):
-        """
-            Generates the Simpful code.
-        """
-        # rules
-        rule_texts = self.create_rules()
-        for i in range(1, self._clusters + 1):
-            self._source_code.append('RULE%d = "%s"' % (i, rule_texts[i - 1]))
-        self._source_code.append(
-            "FS.add_rules([%s])" % (", ".join(["RULE%d" % i for i in range(1, self._clusters + 1)])))
-
-        self._source_code.append("")
-
-        # output functions
-
-        if self._model_order == 'first':
-            B = self._create_consequents()
-            for i in range(self._clusters):
-                self._source_code.append("FS.set_output_function('%s', '%s')" % ("fun%d" % (i + 1), B[i]))
-        elif self._model_order == 'zero':
-            for i in range(self._clusters):
-                self._source_code.append(
-                    "FS.set_crisp_output_value('%s', %s)" % ("fun%d" % (i + 1), self._consequents_matrix[i]))
-        else:
-            raise Exception("Model order not supported," + self._model_order)
-        self._source_code.append("")
-
-        # fuzzy sets and membership functions
-        result = self._create_fuzzy_sets()
-        self._source_code.append(result)
-
-        self._source_code.append("# end of automatically generated code #")
-
-        return "\n".join(self._source_code)
-
-    def _create_fuzzy_sets(self):
-
-        j = 0
-        chunk = ""
-
-        for num_var, var in enumerate(self._input_variables):
-
-            subchunk = []
-            for cluster in range(self._clusters):
-
-                if (num_var, cluster) in self._fuzzy_sets_to_drop:
-                    chunk += "# "
-
-                try:
-                    if cluster in self._setnes_dropped_antecedents[num_var]:
-                        print(" * Dropping cluster%d from variable %s due to Setnes' method." % (cluster, var))
-                        chunk += "# "
-                except KeyError:
-                    pass
-
-                # if self.verbose: print (" * Creating fuzzy set for variable %s, cluster%d" % (var, cluster+1))
-
-                chunk += 'FS_%d = FuzzySet(' % (j + 1)
-                term = 'cluster%d' % (cluster + 1)
-
-                fstype, params = self._fuzzy_sets[j]
-                if fstype == 'gauss':
-                    chunk += "function=Gaussian_MF(%f, %f), term='%s')" % (params[0], params[1], term)
-
-                elif fstype == 'gauss2':
-                    chunk += "function=DoubleGaussian_MF(%f, %f, %f, %f), term='%s')" % (
-                        params[0], params[1], params[2], params[3], term)
-
-                elif fstype == 'sigmoid':
-                    chunk += "function=Sigmoid_MF(%f, %f), term='%s')" % (params[0], params[1], term)
-
-                elif fstype == 'invgauss':
-                    chunk += "function=InvGaussian_MF(%f, %f), term='%s')" % (params[0], params[1], term)
-
-                elif fstype == 'singleton':
-                    chunk += f"function=Singletons_MF({params}), term='{term}')"
-
-                else:
-                    raise Exception("Fuzzy set type not supported," + fstype)
-
-                # first check GRABS
-                if (num_var, cluster) not in self._fuzzy_sets_to_drop:
-                    # also check Setnes
-                    res_setnets = self._setnes_dropped_antecedents.get(num_var, [])
-                    if cluster not in res_setnets:
-                        # finally can append
-                        subchunk.append("FS_%d" % (j + 1))
-                # print ( self._fuzzy_sets[j] )
-                j += 1
-                chunk += "\n"
-                # print(chunk)
-            if self._extreme_values is None:
-                chunk += "MF_%s = LinguisticVariable([%s], concept='%s')\n" % (var, ", ".join(subchunk), var)
-            else:
-                chunk += "MF_%s = LinguisticVariable([%s], concept='%s' , universe_of_discourse=%s)\n" % (
-                    var, ", ".join(subchunk), var, self._extreme_values[num_var])
-            chunk += "FS.add_linguistic_variable('%s', MF_%s)\n\n" % (var, var)
-
-        return chunk
-
-    def _create_consequents(self):
-        variable_count = [  # number of columns in the consequent matrix, for each variable
-            len(self._fuzzy_sets[self._clusters * i][1]) - 1
-            if i in self._categorical_indices else 1
-            for i in range(len(self._input_variables))
-        ]
-        result = []
-        for row in self._consequents_matrix:
-            function = f'{row[-1]}'
-            j = 0
-            for i, v in enumerate(self._input_variables):
-                if i in self._categorical_indices:
-                    for k in range(variable_count[i]):
-                        function += f'+{{IF {v} IS {k} THEN {row[j]}}}'
-                        j += 1
-                else:
-                    function += f'+{row[j]}*{v}'
-                    j += 1
-            result.append(function)
-        return result
-
-    def _create_antecedents(self):
-        """ Creates the 'text' for the antecedents of rules. All rules are created here,
-            one for each cluster. This is where antecedents dropped with Setnes' method
-            should be canceled. """
-
-        result = []
-
-        for i in range(self._clusters):
-
-            pieces = []
-            for j, var in enumerate(self._input_variables):
-
-                # SETNES
-                try:
-                    if i in self._setnes_dropped_antecedents[j]:
-                        # if (j,i) in self._setnes_dropped_antecedents:
-                        print(" * Dropping cluster%d from variable %s in antecedent due to Setnes' method." % (i, var))
-                        continue  # experimental
-                except KeyError:
-                    pass
-
-                value = "cluster%d" % (i + 1)
-
-                # GRABS
-                if (j, i) in self._fuzzy_sets_to_drop.keys():
-                    value = "cluster%d" % (self._fuzzy_sets_to_drop[(j, i)] + 1)
-                pieces.append("(%s IS %s)" % (var, value))
-
-            chunk = (" AND ".join(pieces))
-            result.append(chunk)
-
-        return result
-
-    def create_rules(self):
-        A = self._create_antecedents()
-        # B = self._create_consequents()
-        B = ["fun%d" % (i + 1) for i in range(self._clusters)]
-        result = ["IF %s THEN (OUTPUT IS %s)" % (a, b) for a, b in zip(A, B)]
-        return result
-
-
-if __name__ == '__main__':
-    SC = SimpfulConverter(
-        input_variables_names=["pippo", "pluto"],
-        consequents_matrix=[[1, 2, 3],
-                            [2, 3, 5]],
-        fuzzy_sets=[
-            ["gauss", [0, 1]],
-            ["sigmoid", [1, 2]],
-            ["gauss2", [0, 1, 2, 3]],
-            ["invgauss", [0, 1]]
-        ]
-    )
-
-    SC.save_code("TEST.py")
-    SC.generate_object()
-    print(FS._mfs['pippo'])
+import copy
+
+import simpful
+
+
+class SimpfulConverter(object):
+    """    This object converts a description of a Fuzzy System into a readable
+        Simpful project file.
+
+        Args:
+            input_variables_names: The names of the input variables of the fuzzy model.
+            consequents_matrix: The parameters of the consequent function.
+            fuzzy_sets: list containing a sub-list for each fuzzy set in the model. The sub-list should contain the shape of the fuzzy set (e.g. 'gauss') and the parameters of the function (e.g. mu, sigma). For example: ('gauss', 5, 1).
+            model_order: The order of the fuzzy model ('zero' or 'first') (default = 'first').
+            fuzzy_sets_to_drop: Fuzzy sets that should be disabled in the Simpful code, for example when flagged by GRABS for simplification (default = None).
+            extreme_values: The values that should be used for the universe of discourse for the vaiables in the fuzzy model (default = None).
+            operators: A list of strings, specifying fuzzy operators to be used instead of defaults (default = None). For more information see Simpful's documentation.
+            verbose: Boolean (True/False) that indicates whether extra information will be printed in the user's console (default = True).
+
+    """
+
+    def __init__(self,
+                 input_variables_names,
+                 consequents_matrix,
+                 fuzzy_sets,
+                 model_order='first',
+                 fuzzy_sets_to_drop=None,
+                 setnes_dropped_antecedents=None,
+                 extreme_values=None,
+                 operators=None,
+                 verbose=False,
+                 categorical_indices=None,
+                 decimals = 6):
+        super().__init__()
+        self._input_variables = input_variables_names
+        self._consequents_matrix = consequents_matrix.round(decimals=decimals, out=None)
+        self._clusters = len(self._consequents_matrix)
+        self._fuzzy_sets = fuzzy_sets
+        self._model_order = model_order
+        self._fuzzy_sets_to_drop = fuzzy_sets_to_drop
+        self._setnes_dropped_antecedents = setnes_dropped_antecedents
+        self._extreme_values = extreme_values
+        self.verbose = verbose
+        if self._fuzzy_sets_to_drop is None:
+            self._fuzzy_sets_to_drop = {}
+        self._categorical_indices = categorical_indices if categorical_indices is not None else []
+
+        if self._setnes_dropped_antecedents is None:
+            self._setnes_dropped_antecedents = {}
+
+        if self._model_order == 'first':
+            if self._categorical_indices is not None:
+                # TEMPORARILY IGNORE
+                # assert (len(self._input_variables) + 1 == len(self._consequents_matrix[0]) + len(self._categorical_indices))
+                pass
+            else:
+                assert (len(self._input_variables) + 1 == len(self._consequents_matrix[0]))
+
+        if self.verbose: print(" * Detected %d rules / clusters" % self._clusters)
+
+        self._source_code = []
+        self._source_code.append('# WARNING: this source code was automatically generated by pyFUME.')
+        self._source_code.append("from simpful import *")
+        if operators is None:
+            self._source_code.append("\nFS = FuzzySystem(show_banner=False)")
+        else:
+            # experimental, please test ASAP
+            self._source_code.append("\nFS = FuzzySystem(operators=" + str(operators) + ")")
+
+    def save_code(self, path):
+        """
+            Saves the Simpful code.
+            
+            Args:
+                path: Path to the folder where the Simpful code should be saved.
+        """
+        code = self.generate_code()
+        with open(path, "w") as fo:
+            fo.write(code)
+        if self.verbose is True:
+            print(" * Code saved to file %s" % path)
+
+    def generate_object(self):
+        """
+            Generates the executable object containing the fuzzy model.
+        """
+        code = self.generate_code()
+        if self.verbose:
+            exec(code, globals())
+        elif self.verbose is False:
+            import os
+            import contextlib
+            with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
+                exec(code, globals())
+
+        from copy import deepcopy
+        self._fuzzyreasoner = deepcopy(FS)
+
+    def generate_code(self):
+        """
+            Generates the Simpful code.
+        """
+        # rules
+        rule_texts = self.create_rules()
+        for i in range(1, self._clusters + 1):
+            self._source_code.append('RULE%d = "%s"' % (i, rule_texts[i - 1]))
+        self._source_code.append(
+            "FS.add_rules([%s])" % (", ".join(["RULE%d" % i for i in range(1, self._clusters + 1)])))
+
+        self._source_code.append("")
+
+        # output functions
+
+        if self._model_order == 'first':
+            B = self._create_consequents()
+            for i in range(self._clusters):
+                self._source_code.append("FS.set_output_function('%s', '%s')" % ("fun%d" % (i + 1), B[i]))
+        elif self._model_order == 'zero':
+            for i in range(self._clusters):
+                self._source_code.append(
+                    "FS.set_crisp_output_value('%s', %s)" % ("fun%d" % (i + 1), self._consequents_matrix[i]))
+        else:
+            raise Exception("Model order not supported," + self._model_order)
+        self._source_code.append("")
+
+        # fuzzy sets and membership functions
+        result = self._create_fuzzy_sets()
+        self._source_code.append(result)
+
+        self._source_code.append("# end of automatically generated code #")
+
+        return "\n".join(self._source_code)
+
+    def _create_fuzzy_sets(self):
+
+        j = 0
+        chunk = ""
+
+        for num_var, var in enumerate(self._input_variables):
+
+            subchunk = []
+            for cluster in range(self._clusters):
+
+                if (num_var, cluster) in self._fuzzy_sets_to_drop:
+                    chunk += "# "
+
+                try:
+                    if cluster in self._setnes_dropped_antecedents[num_var]:
+                        print(" * Dropping cluster%d from variable %s due to Setnes' method." % (cluster, var))
+                        chunk += "# "
+                except KeyError:
+                    pass
+
+                # if self.verbose: print (" * Creating fuzzy set for variable %s, cluster%d" % (var, cluster+1))
+
+                chunk += 'FS_%d = FuzzySet(' % (j + 1)
+                term = 'cluster%d' % (cluster + 1)
+
+                fstype, params = self._fuzzy_sets[j]
+                if fstype == 'gauss':
+                    chunk += "function=Gaussian_MF(%f, %f), term='%s')" % (params[0], params[1], term)
+
+                elif fstype == 'gauss2':
+                    chunk += "function=DoubleGaussian_MF(%f, %f, %f, %f), term='%s')" % (
+                        params[0], params[1], params[2], params[3], term)
+
+                elif fstype == 'sigmoid':
+                    chunk += "function=Sigmoid_MF(%f, %f), term='%s')" % (params[0], params[1], term)
+
+                elif fstype == 'invgauss':
+                    chunk += "function=InvGaussian_MF(%f, %f), term='%s')" % (params[0], params[1], term)
+
+                elif fstype == 'singleton':
+                    chunk += f"function=Singletons_MF({params}), term='{term}')"
+
+                else:
+                    raise Exception("Fuzzy set type not supported," + fstype)
+
+                # first check GRABS
+                if (num_var, cluster) not in self._fuzzy_sets_to_drop:
+                    # also check Setnes
+                    res_setnets = self._setnes_dropped_antecedents.get(num_var, [])
+                    if cluster not in res_setnets:
+                        # finally can append
+                        subchunk.append("FS_%d" % (j + 1))
+                # print ( self._fuzzy_sets[j] )
+                j += 1
+                chunk += "\n"
+                # print(chunk)
+            if self._extreme_values is None:
+                chunk += "MF_%s = LinguisticVariable([%s], concept='%s')\n" % (var, ", ".join(subchunk), var)
+            else:
+                chunk += "MF_%s = LinguisticVariable([%s], concept='%s' , universe_of_discourse=%s)\n" % (
+                    var, ", ".join(subchunk), var, self._extreme_values[num_var])
+            chunk += "FS.add_linguistic_variable('%s', MF_%s)\n\n" % (var, var)
+
+        return chunk
+
+    def _create_consequents(self):
+        variable_count = [  # number of columns in the consequent matrix, for each variable
+            len(self._fuzzy_sets[self._clusters * i][1]) - 1
+            if i in self._categorical_indices else 1
+            for i in range(len(self._input_variables))
+        ]
+        result = []
+        for row in self._consequents_matrix:
+            function = f'{row[-1]}'
+            j = 0
+            for i, v in enumerate(self._input_variables):
+                if i in self._categorical_indices:
+                    for k in range(variable_count[i]):
+                        function += f'+{{IF {v} IS {k} THEN {row[j]}}}'
+                        j += 1
+                else:
+                    function += f'+{row[j]}*{v}'
+                    j += 1
+            result.append(function)
+        return result
+
+    def _create_antecedents(self):
+        """ Creates the 'text' for the antecedents of rules. All rules are created here,
+            one for each cluster. This is where antecedents dropped with Setnes' method
+            should be canceled. """
+
+        result = []
+
+        for i in range(self._clusters):
+
+            pieces = []
+            for j, var in enumerate(self._input_variables):
+
+                # SETNES
+                try:
+                    if i in self._setnes_dropped_antecedents[j]:
+                        # if (j,i) in self._setnes_dropped_antecedents:
+                        print(" * Dropping cluster%d from variable %s in antecedent due to Setnes' method." % (i, var))
+                        continue  # experimental
+                except KeyError:
+                    pass
+
+                value = "cluster%d" % (i + 1)
+
+                # GRABS
+                if (j, i) in self._fuzzy_sets_to_drop.keys():
+                    value = "cluster%d" % (self._fuzzy_sets_to_drop[(j, i)] + 1)
+                pieces.append("(%s IS %s)" % (var, value))
+
+            chunk = (" AND ".join(pieces))
+            result.append(chunk)
+
+        return result
+
+    def create_rules(self):
+        A = self._create_antecedents()
+        # B = self._create_consequents()
+        B = ["fun%d" % (i + 1) for i in range(self._clusters)]
+        result = ["IF %s THEN (OUTPUT IS %s)" % (a, b) for a, b in zip(A, B)]
+        return result
+
+
+if __name__ == '__main__':
+    SC = SimpfulConverter(
+        input_variables_names=["pippo", "pluto"],
+        consequents_matrix=[[1, 2, 3],
+                            [2, 3, 5]],
+        fuzzy_sets=[
+            ["gauss", [0, 1]],
+            ["sigmoid", [1, 2]],
+            ["gauss2", [0, 1, 2, 3]],
+            ["invgauss", [0, 1]]
+        ]
+    )
+
+    SC.save_code("TEST.py")
+    SC.generate_object()
+    print(FS._mfs['pippo'])
```

