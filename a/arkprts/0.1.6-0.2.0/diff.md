# Comparing `tmp/arkprts-0.1.6.tar.gz` & `tmp/arkprts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.6.tar", last modified: Sat Jun  3 19:20:34 2023, max compression
+gzip compressed data, was "arkprts-0.2.0.tar", last modified: Tue Jul  4 21:46:15 2023, max compression
```

## Comparing `arkprts-0.1.6.tar` & `arkprts-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.646733 arkprts-0.1.6/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3019 2023-06-03 19:20:34.642736 arkprts-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2687 2023-06-03 19:10:54.000000 arkprts-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.556785 arkprts-0.1.6/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.6/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1925 2023-06-02 18:37:27.000000 arkprts-0.1.6/arkprts/__main__.py
--rw-rw-rw-   0        0        0    13911 2023-06-03 18:46:42.000000 arkprts-0.1.6/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.6/arkprts/errors.py
--rw-rw-rw-   0        0        0     7295 2023-06-03 19:11:28.000000 arkprts-0.1.6/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.634742 arkprts-0.1.6/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.6/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-06-03 18:45:01.000000 arkprts-0.1.6/arkprts/models/base.py
--rw-rw-rw-   0        0        0    11643 2023-06-03 18:59:38.000000 arkprts-0.1.6/arkprts/models/data.py
--rw-rw-rw-   0        0        0     7056 2023-06-03 19:00:31.000000 arkprts-0.1.6/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.6/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.611754 arkprts-0.1.6/arkprts.egg-info/
--rw-rw-rw-   0        0        0     3019 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 19:20:34.646733 arkprts-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-06-03 19:19:53.000000 arkprts-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.640737 arkprts-0.1.6/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.6/tests/test_config.py
--rw-rw-rw-   0        0        0      360 2023-05-26 14:03:38.000000 arkprts-0.1.6/tests/test_gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.843008 arkprts-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 21:46:04.000000 arkprts-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-04 21:46:15.843008 arkprts-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-04 21:46:04.000000 arkprts-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.839007 arkprts-0.2.0/arkprts/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.839007 arkprts-0.2.0/arkprts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.839007 arkprts-0.2.0/arkprts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-04 21:46:04.000000 arkprts-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:46:15.843008 arkprts-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-04 21:46:04.000000 arkprts-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.843008 arkprts-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-04 21:46:04.000000 arkprts-0.2.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 21:46:04.000000 arkprts-0.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 21:46:04.000000 arkprts-0.2.0/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.6/LICENSE` & `arkprts-0.2.0/LICENSE`

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

### Comparing `arkprts-0.1.6/arkprts/errors.py` & `arkprts-0.2.0/arkprts/errors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,84 @@
-"""Arkprts errors."""
-import typing
-
-
-class BaseArkprtsError(Exception):
-    """Base class for all Arkprts errors."""
-
-    message: str = "Arkprts error."
-
-    def __init__(self, message: typing.Optional[str] = None) -> None:
-        super().__init__(message or self.message)
-
-
-class NotLoggedInError(BaseArkprtsError):
-    """Raised when a user is not logged in."""
-
-    message = "Not logged in."
-
-
-class ArkPrtsError(BaseArkprtsError):
-    """Raised when result code is not 0."""
-
-    data: typing.Mapping[str, typing.Any]
-
-    def __init__(self, data: typing.Mapping[str, typing.Any]) -> None:
-        self.data = data
-        super().__init__(f"[{data['result']}] {data}")
-
-
-class InvalidStatusError(BaseArkprtsError):
-    """Raised when a response has an invalid status code."""
-
-    status: int
-    data: typing.Mapping[str, typing.Any]
-
-    def __init__(self, status: int, data: typing.Mapping[str, typing.Any]) -> None:
-        self.status = status
-        self.data = data
-
-        super().__init__(f"[{status}] {data}")
-
-
-class InvalidContentTypeError(BaseArkprtsError):
-    """Raised when a response has an invalid content type."""
-
-    message = "Invalid content type."
-    content: str
-
-    def __init__(self, content: str) -> None:
-        self.content = content
-        super().__init__()
+"""Arkprts errors."""
+import json
+import typing
+
+
+class BaseArkprtsError(Exception):
+    """Base class for all Arkprts errors."""
+
+    message: str = "Arkprts error."
+
+    def __init__(self, message: typing.Optional[str] = None) -> None:
+        super().__init__(message or self.message)
+
+
+class NotLoggedInError(BaseArkprtsError):
+    """Raised when a user is not logged in."""
+
+    message = "Not logged in."
+
+
+class ArkPrtsError(BaseArkprtsError):
+    """Raised when result code is not 0."""
+
+    data: typing.Mapping[str, typing.Any]
+
+    def __init__(self, data: typing.Mapping[str, typing.Any]) -> None:
+        self.data = data
+        super().__init__(f"[{data['result']}] {self.message} {data}")
+
+
+class GameServerError(BaseArkprtsError):
+    """Game server error."""
+
+    status_code: int
+    error: str
+    code: int
+    msg: str
+    info: typing.Mapping[str, typing.Any]
+
+    def __init__(self, data: typing.Mapping[str, typing.Any]) -> None:
+        self.status_code = data.get("statusCode", 400)
+        self.error = data["error"]
+        self.code = data.get("code", 0)
+        self.msg = data.get("msg", "")
+        self.info = json.loads(data.get("info", "{}"))
+
+        super().__init__(str(data))
+
+
+class GeetestError(ArkPrtsError):
+    """Raised when login is flagged by geetest."""
+
+    message: str = "Geetest verification is required."
+    challenge: str
+    gt: str
+
+    def __init__(self, data: typing.Mapping[str, typing.Any]) -> None:
+        self.challenge = data["captcha"]["challenge"]
+        self.gt = data["captcha"]["gt"]
+        super().__init__(data)
+
+
+class InvalidStatusError(BaseArkprtsError):
+    """Raised when a response has an invalid status code."""
+
+    status: int
+    data: typing.Mapping[str, typing.Any]
+
+    def __init__(self, status: int, data: typing.Mapping[str, typing.Any]) -> None:
+        self.status = status
+        self.data = data
+
+        super().__init__(f"[{status}] {data}")
+
+
+class InvalidContentTypeError(BaseArkprtsError):
+    """Raised when a response has an invalid content type."""
+
+    message = "Invalid content type."
+    content: str
+
+    def __init__(self, content: str) -> None:
+        self.content = content
+        super().__init__()
```

### Comparing `arkprts-0.1.6/arkprts/models/data.py` & `arkprts-0.2.0/arkprts/models/data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,323 +1,321 @@
-"""Arknights API data models.
-
-Any field description prefixed with IDK means it's just a guess.
-"""
-import datetime
-import typing
-
-import pydantic
-
-from . import base
-
-
-class Avatar(base.BaseModel):
-    """User display avatar."""
-
-    type: typing.Literal["ASSISTANT", "ICON", "DEFAULT"] = "DEFAULT"
-    """Avatar type."""
-    id: typing.Optional[str] = None
-    """Avatar ID. For example a skin ID."""
-
-
-class Status(base.BaseModel):
-    """General user data."""
-
-    nickname: str = pydantic.Field(alias="nickName")
-    """Player nickname."""
-    nick_number: str = pydantic.Field(alias="nickNumber")
-    """Player nickname number after #."""
-    level: int
-    """Player level."""
-    exp: int
-    """Player experience."""
-    social_point: int = pydantic.Field(alias="socialPoint")
-    """Credit shop credits."""
-    gacha_ticket: int = pydantic.Field(alias="gachaTicket")
-    """Amount of single headhunting permits."""
-    ten_gacha_ticket: int = pydantic.Field(alias="tenGachaTicket")
-    """Amount of 10-headhunting permits."""
-    instant_finish_ticket: int = pydantic.Field(alias="instantFinishTicket")
-    """Amount of expedited completion permits."""
-    hgg_shard: int = pydantic.Field(alias="hggShard")
-    """Amount of yellow distinction certificates."""
-    lgg_shard: int = pydantic.Field(alias="lggShard")
-    """Amount of green commendation certificates.."""
-    recruit_license: int = pydantic.Field(alias="recruitLicense")
-    """Amount of recruitment permit."""
-    progress: int = pydantic.Field(repr=False)
-    """IDK."""
-    buy_ap_remain_times: int = pydantic.Field(alias="buyApRemainTimes", repr=False)
-    """IDK. Ap refers to sanity."""
-    ap_limit_up_flag: bool = pydantic.Field(alias="apLimitUpFlag", repr=False)
-    """IDK. Ap refers to sanity."""
-    uid: str
-    """User ID."""
-    flags: typing.Mapping[str, bool] = pydantic.Field(repr=False)
-    """Completed stories."""
-    ap: int
-    """Current sanity. Actually not a true value."""
-    max_ap: int = pydantic.Field(alias="maxAp")
-    """Max sanity."""
-    pay_diamond: int = pydantic.Field(alias="payDiamond")
-    """Bough originium prime."""
-    free_diamond: int = pydantic.Field(alias="freeDiamond")
-    """Earned originium prime."""
-    diamond_shard: int = pydantic.Field(alias="diamondShard")
-    """Amount of orundum."""
-    gold: int
-    """Amount of LMD."""
-    practice_ticket: int = pydantic.Field(alias="practiceTicket")
-    """Amount of training permits."""
-    last_refresh_ts: datetime.datetime = pydantic.Field(alias="lastRefreshTs")
-    """IDK. When sanity was last incremented."""
-    last_ap_add_time: datetime.datetime = pydantic.Field(alias="lastApAddTime")
-    """IDK."""
-    main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
-    """Current main story stage ID. None if completed."""
-    register_ts: datetime.datetime = pydantic.Field(alias="registerTs")
-    """Account creation time."""
-    server_name: str = pydantic.Field(alias="serverName")
-    """Server name. Should always be Terra."""
-    avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
-    """IDK. Always 0."""
-    resume: str
-    """Player display bio."""
-    friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
-    """How many friend slots are open."""
-    secretary: str
-    """ID of the secretary operator."""
-    secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
-    """ID of the secretary operator's skin."""
-    global_voice_lan: typing.Optional[str] = pydantic.Field(None, alias="globalVoiceLan")
-    """Default voice-over language."""
-    avatar: Avatar
-    """Selected avatar."""
-
-    @property
-    def basic_item_inventory(self) -> typing.Mapping[str, int]:
-        """Basic item inventory. These are not shown in the inventory object."""
-        return {
-            "SOCIAL_PT": self.social_point,
-            "AP_GAMEPLAY": self.ap,
-            "4001": self.gold,
-            "4002": self.pay_diamond + self.free_diamond,
-            "4003": self.diamond_shard,
-            "4004": self.hgg_shard,
-            "4005": self.lgg_shard,
-            "5001": self.exp,
-            "6001": self.practice_ticket,
-            "7001": self.recruit_license,
-            "7002": self.instant_finish_ticket,
-            "7003": self.gacha_ticket,
-            "7004": self.ten_gacha_ticket,
-        }
-
-
-class SquadSlot(base.BaseModel):
-    """Squad slot."""
-
-    char_inst_id: int = pydantic.Field(alias="charInstId")
-    """Operator index."""
-    skill_index: int = pydantic.Field(alias="skillIndex")
-    """Index of chosen skill."""
-    current_equip: typing.Optional[str] = None
-    """Currently equipped module ID."""
-
-    @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
-    def _fix_amiya(cls, values: typing.Any) -> typing.Any:
-        """Flatten Amiya to only keep her guard form."""
-        if values and values.get("tmpl"):
-            current = values["tmpl"][values["currentTmpl"]]
-            values.update(current)
-
-        return values
-
-
-class Squads(base.BaseModel):
-    """Operator squad data."""
-
-    squad_id: str = pydantic.Field(alias="squadId")
-    """Squad ID."""
-    name: str
-    """Squad name."""
-    slots: typing.Sequence[typing.Optional[SquadSlot]]
-    """Equipped operators."""
-
-
-class Skill(base.BaseModel):
-    """Operator skill data."""
-
-    skill_id: str = pydantic.Field(alias="skillId")
-    """Skill ID."""
-    unlock: bool
-    """Whether the skill is unlocked."""
-    state: bool = pydantic.Field(repr=False)
-    """IDK. Always false."""
-    specialize_level: int = pydantic.Field(alias="specializeLevel")
-    """Skill mastery level."""
-    complete_upgrade_time: typing.Optional[datetime.datetime] = pydantic.Field(alias="completeUpgradeTime")
-    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
-
-    @property
-    def static(self) -> base.DDict:
-        """Static data for this skill."""
-        return self.client.gamedata.skill_table[self.skill_id]
-
-
-class Equip(base.BaseModel):
-    """Operator module data."""
-
-    hide: bool
-    """Whether the module is hidden."""
-    locked: bool
-    """Whether the module is locked."""
-    level: int
-    """Module level."""
-
-
-class Character(base.BaseModel):
-    """Operator data."""
-
-    inst_id: int = pydantic.Field(alias="instId")
-    """Index of the operator."""
-    char_id: str = pydantic.Field(alias="charId")
-    """Operator ID."""
-    favor_point: int = pydantic.Field(alias="favorPoint")
-    """Operator trust points."""
-    potential_rank: int = pydantic.Field(alias="potentialRank")
-    """Operator potential. Starts at 0."""
-    main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
-    """Operator skill level."""
-    skin: str
-    """Operator skin ID."""
-    level: int
-    """Operator level."""
-    exp: int
-    """Operator experience."""
-    evolve_phase: int = pydantic.Field(alias="evolvePhase")
-    """Elite phase."""
-    default_skill_index: int = pydantic.Field(alias="defaultSkillIndex")
-    """Index of the default skill."""
-    skills: typing.Sequence[Skill]
-    """Operator skills."""
-    voice_lan: str = pydantic.Field(alias="voiceLan")
-    """Operator voice-over language."""
-    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
-    """Currently equipped module."""
-    equip: typing.Mapping[str, Equip]
-    """Operator modules."""
-    star_mark: bool = pydantic.Field(False, alias="starMark")
-    """Whether the operator is marked as favorite."""
-
-    @property
-    def static(self) -> base.DDict:
-        """Static data for this operator."""
-        return self.client.gamedata.character_table[self.char_id]
-
-    @property
-    def trust(self) -> int:
-        """Trust calculated from favor_point."""
-        return self.client.gamedata.calculate_trust_level(self.favor_point)
-
-    @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
-    def _fix_amiya(cls, values: typing.Any) -> typing.Any:
-        """Flatten Amiya to only keep her guard form."""
-        if values and values.get("tmpl"):
-            current = values["tmpl"][values["currentTmpl"]]
-            values.update(current)
-            values["skin"] = current["skinId"]  # why even?
-
-        return values
-
-
-class CharGroup(base.BaseModel):
-    """Additional operator data."""
-
-    favor_point: int = pydantic.Field(alias="favorPoint")
-    """Operator trust points."""
-
-    @property
-    def trust(self) -> int:
-        """Trust calculated from favor_point."""
-        return self.client.gamedata.calculate_trust_level(self.favor_point)
-
-
-class Troops(base.BaseModel):
-    """Operator data."""
-
-    cur_char_inst_id: int = pydantic.Field(alias="curCharInstId")
-    """Amount of owned operators."""
-    cur_squad_count: int = pydantic.Field(alias="curSquadCount")
-    """Amount of squads. Should be always 4."""
-    squads: typing.Mapping[int, Squads]
-    """Squad data."""
-    chars: typing.Mapping[int, Character]
-    """Operator data."""
-    char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
-    """Additional operator data."""
-    char_mission: typing.Mapping[str, typing.Mapping[str, int]] = pydantic.Field(alias="charMission", repr=False)
-    """IDK. Special operation missions."""
-    addon: base.DDict = pydantic.Field(default_factory=base.DDict, repr=False)
-    """IDK."""
-
-
-class Skins(base.BaseModel):
-    """Operator skin data."""
-
-    character_skins: typing.Mapping[str, bool] = pydantic.Field(alias="characterSkins")
-    """Owned skins."""
-    skin_ts: typing.Mapping[str, datetime.datetime] = pydantic.Field(alias="skinTs")
-    """When the skins were obtained."""
-
-
-class AssistChar(base.BaseModel):
-    """Assist operator data."""
-
-    char_inst_id: int = pydantic.Field(alias="charInstId")
-    """Index of the operator."""
-    skill_index: int = pydantic.Field(alias="skillIndex")
-    """Index of the selected skill."""
-    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
-    """Currently equipped module."""
-
-
-class Social(base.BaseModel):
-    """Social data."""
-
-    assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
-    """Support operators."""
-    yesterday_reward: base.DDict = pydantic.Field(alias="yesterdayReward")
-    """IDK. Clue exchange data."""
-    y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs", repr=False)
-    """IDK."""
-    medal_board: base.DDict = pydantic.Field(default_factory=base.DDict, alias="medalBoard")
-    """Medal board."""
-
-
-class ConsumableExpire(base.BaseModel):
-    """Consumable expiration data."""
-
-    ts: typing.Optional[datetime.datetime]
-    """When the consumable expires."""
-    count: int
-    """Amount of consumables."""
-
-
-class User(base.BaseModel):
-    """User sync data. Not fully modeled."""
-
-    status: Status
-    """General user data."""
-    troop: Troops
-    """Operator data."""
-    skin: Skins
-    """Operator skin data."""
-    social: Social
-    """Data related to friends."""
-    consumable: typing.Mapping[str, typing.Mapping[int, ConsumableExpire]] = {}
-    """Consumable data."""
-    inventory: typing.Mapping[str, int]
-    """Inventory data. Item ID to amount.
-
-    To access the static data for an item, use `client.gamedata.get_item(item_id)`.
-    """
+"""Arknights API data models.
+
+Any field description prefixed with IDK means it's just a guess.
+"""
+import typing
+
+import pydantic
+
+from . import base
+
+
+class Avatar(base.BaseModel):
+    """User display avatar."""
+
+    type: typing.Literal["ASSISTANT", "ICON", "DEFAULT"] = "DEFAULT"
+    """Avatar type."""
+    id: typing.Optional[str] = None
+    """Avatar ID. For example a skin ID."""
+
+
+class Status(base.BaseModel):
+    """General user data."""
+
+    nickname: str = pydantic.Field(alias="nickName")
+    """Player nickname."""
+    nick_number: str = pydantic.Field(alias="nickNumber")
+    """Player nickname number after #."""
+    level: int
+    """Player level."""
+    exp: int
+    """Player experience."""
+    social_point: int = pydantic.Field(alias="socialPoint")
+    """Credit shop credits."""
+    gacha_ticket: int = pydantic.Field(alias="gachaTicket")
+    """Amount of single headhunting permits."""
+    ten_gacha_ticket: int = pydantic.Field(alias="tenGachaTicket")
+    """Amount of 10-headhunting permits."""
+    instant_finish_ticket: int = pydantic.Field(alias="instantFinishTicket")
+    """Amount of expedited completion permits."""
+    hgg_shard: int = pydantic.Field(alias="hggShard")
+    """Amount of yellow distinction certificates."""
+    lgg_shard: int = pydantic.Field(alias="lggShard")
+    """Amount of green commendation certificates.."""
+    recruit_license: int = pydantic.Field(alias="recruitLicense")
+    """Amount of recruitment permit."""
+    progress: int = pydantic.Field(repr=False)
+    """IDK."""
+    buy_ap_remain_times: int = pydantic.Field(alias="buyApRemainTimes", repr=False)
+    """IDK. Ap refers to sanity."""
+    ap_limit_up_flag: bool = pydantic.Field(alias="apLimitUpFlag", repr=False)
+    """IDK. Ap refers to sanity."""
+    uid: str
+    """User ID."""
+    flags: typing.Mapping[str, bool] = pydantic.Field(repr=False)
+    """Completed stories."""
+    ap: int
+    """Current sanity. Actually not a true value."""
+    max_ap: int = pydantic.Field(alias="maxAp")
+    """Max sanity."""
+    pay_diamond: int = pydantic.Field(alias="payDiamond")
+    """Bough originium prime."""
+    free_diamond: int = pydantic.Field(alias="freeDiamond")
+    """Earned originium prime."""
+    diamond_shard: int = pydantic.Field(alias="diamondShard")
+    """Amount of orundum."""
+    gold: int
+    """Amount of LMD."""
+    practice_ticket: int = pydantic.Field(alias="practiceTicket")
+    """Amount of training permits."""
+    last_refresh_ts: base.ArknightsTimestamp = pydantic.Field(alias="lastRefreshTs")
+    """IDK. When sanity was last incremented."""
+    last_ap_add_time: base.ArknightsTimestamp = pydantic.Field(alias="lastApAddTime")
+    """IDK."""
+    last_online_ts: base.ArknightsTimestamp = pydantic.Field(alias="lastOnlineTs")
+    """IDK. When the player was last online."""
+    main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
+    """Current main story stage ID. None if completed."""
+    register_ts: base.ArknightsTimestamp = pydantic.Field(alias="registerTs")
+    """Account creation time."""
+    server_name: str = pydantic.Field(alias="serverName")
+    """Server name. Should always be Terra."""
+    avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
+    """IDK. Always 0."""
+    resume: str
+    """Player display bio."""
+    friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
+    """How many friend slots are open."""
+    secretary: str
+    """ID of the secretary operator."""
+    secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
+    """ID of the secretary operator's skin."""
+    global_voice_lan: typing.Optional[str] = pydantic.Field(None, alias="globalVoiceLan")
+    """Default voice-over language."""
+    avatar: Avatar
+    """Selected avatar."""
+
+    # fmt: off
+    # optional:
+    monthly_subscription_start_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(None, alias="monthlySubscriptionStartTime")
+    """When the monthly subscription started."""
+    monthly_subscription_end_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(None, alias="monthlySubscriptionEndTime")
+    """When the monthly subscription is ending."""
+    tip_monthly_card_expire: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(None, alias="tipMonthlyCardExpire")
+    """IDK."""
+    # fmt: on
+
+    @property
+    def basic_item_inventory(self) -> typing.Mapping[str, int]:
+        """Basic item inventory. These are not shown in the inventory object."""
+        return {
+            "SOCIAL_PT": self.social_point,
+            "AP_GAMEPLAY": self.ap,
+            "4001": self.gold,
+            "4002": self.pay_diamond + self.free_diamond,
+            "4003": self.diamond_shard,
+            "4004": self.hgg_shard,
+            "4005": self.lgg_shard,
+            "5001": self.exp,
+            "6001": self.practice_ticket,
+            "7001": self.recruit_license,
+            "7002": self.instant_finish_ticket,
+            "7003": self.gacha_ticket,
+            "7004": self.ten_gacha_ticket,
+        }
+
+
+class SquadSlot(base.BaseModel):
+    """Squad slot."""
+
+    char_inst_id: int = pydantic.Field(alias="charInstId")
+    """Operator index."""
+    skill_index: int = pydantic.Field(alias="skillIndex")
+    """Index of chosen skill."""
+    current_equip: typing.Optional[str] = None
+    """Currently equipped module ID."""
+    tmpl: typing.Mapping[str, base.DDict] = pydantic.Field(default_factory=base.DDict, repr=False)
+    """Alternative operator class data. Only for Amiya."""
+
+
+class Squads(base.BaseModel):
+    """Operator squad data."""
+
+    squad_id: str = pydantic.Field(alias="squadId")
+    """Squad ID."""
+    name: str
+    """Squad name."""
+    slots: typing.Sequence[typing.Optional[SquadSlot]]
+    """Equipped operators."""
+
+
+class Skill(base.BaseModel):
+    """Operator skill data."""
+
+    skill_id: str = pydantic.Field(alias="skillId")
+    """Skill ID."""
+    unlock: bool
+    """Whether the skill is unlocked."""
+    state: bool = pydantic.Field(repr=False)
+    """IDK. Always false."""
+    specialize_level: int = pydantic.Field(alias="specializeLevel")
+    """Skill mastery level."""
+    complete_upgrade_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(alias="completeUpgradeTime")
+    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
+
+    @property
+    def static(self) -> base.DDict:
+        """Static data for this skill."""
+        return self.client.gamedata.skill_table[self.skill_id]
+
+
+class Equip(base.BaseModel):
+    """Operator module data."""
+
+    hide: bool
+    """Whether the module is hidden."""
+    locked: bool
+    """Whether the module is locked."""
+    level: int
+    """Module level."""
+
+
+class Character(base.BaseModel):
+    """Operator data."""
+
+    inst_id: int = pydantic.Field(alias="instId")
+    """Index of the operator."""
+    char_id: str = pydantic.Field(alias="charId")
+    """Operator ID."""
+    favor_point: int = pydantic.Field(alias="favorPoint")
+    """Operator trust points."""
+    potential_rank: int = pydantic.Field(alias="potentialRank")
+    """Operator potential. Starts at 0."""
+    main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
+    """Operator skill level."""
+    skin: str
+    """Operator skin ID."""
+    level: int
+    """Operator level."""
+    exp: int
+    """Operator experience."""
+    evolve_phase: int = pydantic.Field(alias="evolvePhase")
+    """Elite phase."""
+    default_skill_index: int = pydantic.Field(alias="defaultSkillIndex")
+    """Index of the default skill."""
+    skills: typing.Sequence[Skill]
+    """Operator skills."""
+    voice_lan: str = pydantic.Field(alias="voiceLan")
+    """Operator voice-over language."""
+    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
+    """Currently equipped module."""
+    equip: typing.Mapping[str, Equip]
+    """Operator modules."""
+    star_mark: bool = pydantic.Field(False, alias="starMark")
+    """Whether the operator is marked as favorite."""
+    tmpl: typing.Mapping[str, base.DDict] = pydantic.Field(default_factory=base.DDict, repr=False)
+    """Alternative operator class data. Only for Amiya."""
+
+    @property
+    def static(self) -> base.DDict:
+        """Static data for this operator."""
+        return self.client.gamedata.character_table[self.char_id]
+
+    @property
+    def trust(self) -> int:
+        """Trust calculated from favor_point."""
+        return self.client.gamedata.calculate_trust_level(self.favor_point)
+
+
+class CharGroup(base.BaseModel):
+    """Additional operator data."""
+
+    favor_point: int = pydantic.Field(alias="favorPoint")
+    """Operator trust points."""
+
+    @property
+    def trust(self) -> int:
+        """Trust calculated from favor_point."""
+        return self.client.gamedata.calculate_trust_level(self.favor_point)
+
+
+class Troops(base.BaseModel):
+    """Operator data."""
+
+    cur_char_inst_id: int = pydantic.Field(alias="curCharInstId")
+    """Amount of owned operators."""
+    cur_squad_count: int = pydantic.Field(alias="curSquadCount")
+    """Amount of squads. Should be always 4."""
+    squads: typing.Mapping[int, Squads]
+    """Squad data."""
+    chars: typing.Mapping[int, Character]
+    """Operator data."""
+    char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
+    """Additional operator data."""
+    char_mission: typing.Mapping[str, typing.Mapping[str, int]] = pydantic.Field(alias="charMission", repr=False)
+    """IDK. Special operation missions."""
+    addon: base.DDict = pydantic.Field(default_factory=base.DDict, repr=False)
+    """IDK."""
+
+
+class Skins(base.BaseModel):
+    """Operator skin data."""
+
+    character_skins: typing.Mapping[str, bool] = pydantic.Field(alias="characterSkins")
+    """Owned skins."""
+    skin_ts: typing.Mapping[str, base.ArknightsTimestamp] = pydantic.Field(alias="skinTs")
+    """When the skins were obtained."""
+
+
+class AssistChar(base.BaseModel):
+    """Assist operator data."""
+
+    char_inst_id: int = pydantic.Field(alias="charInstId")
+    """Index of the operator."""
+    skill_index: int = pydantic.Field(alias="skillIndex")
+    """Index of the selected skill."""
+    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
+    """Currently equipped module."""
+    tmpl: typing.Mapping[str, base.DDict] = pydantic.Field(default_factory=base.DDict, repr=False)
+    """Alternative operator class data. Only for Amiya."""
+
+
+class Social(base.BaseModel):
+    """Social data."""
+
+    assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
+    """Support operators."""
+    yesterday_reward: base.DDict = pydantic.Field(alias="yesterdayReward")
+    """IDK. Clue exchange data."""
+    y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs", repr=False)
+    """IDK."""
+    medal_board: base.DDict = pydantic.Field(default_factory=base.DDict, alias="medalBoard")
+    """Medal board."""
+
+
+class ConsumableExpire(base.BaseModel):
+    """Consumable expiration data."""
+
+    ts: typing.Optional[base.ArknightsTimestamp]
+    """When the consumable expires."""
+    count: int
+    """Amount of consumables."""
+
+
+class User(base.BaseModel, extra="allow"):
+    """User sync data. Not fully modeled."""
+
+    status: Status
+    """General user data."""
+    troop: Troops
+    """Operator data."""
+    skin: Skins
+    """Operator skin data."""
+    social: Social
+    """Data related to friends."""
+    consumable: typing.Mapping[str, typing.Mapping[int, ConsumableExpire]] = {}
+    """Consumable data."""
+    inventory: typing.Mapping[str, int]
+    """Inventory data. Item ID to amount.
+
+    To access the static data for an item, use `client.gamedata.get_item(item_id)`.
+    """
```

### Comparing `arkprts-0.1.6/arkprts/models/social.py` & `arkprts-0.2.0/arkprts/models/social.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,201 +1,193 @@
-"""Arknights API social models.
-
-Any field description prefixed with IDK means it's just a guess.
-"""
-import datetime
-import typing
-
-import pydantic
-
-from . import base
-
-
-class Avatar(base.BaseModel):
-    """User display avatar."""
-
-    type: typing.Literal["ASSISTANT", "ICON", "DEFAULT"] = "DEFAULT"
-    """Avatar type."""
-    id: typing.Optional[str] = None
-    """Avatar ID. For example a skin ID."""
-
-
-class Skill(base.BaseModel):
-    """Skill of a character."""
-
-    skill_id: str = pydantic.Field(alias="skillId")
-    """Skill ID."""
-    unlock: bool
-    """Whether the skill is unlocked."""
-    state: bool = pydantic.Field(repr=False)
-    """IDK. Always false."""
-    specialize_level: int = pydantic.Field(alias="specializeLevel")
-    """Skill mastery level."""
-    complete_upgrade_time: typing.Optional[datetime.datetime] = pydantic.Field(alias="completeUpgradeTime")
-    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
-
-    @property
-    def static(self) -> base.DDict:
-        """Static data for this skill."""
-        return self.client.gamedata.skill_table[self.skill_id]
-
-
-class UniEquip(base.BaseModel):
-    """Equipped modules."""
-
-    hide: bool
-    """IDK. Whether the module is publicly hidden."""
-    locked: bool
-    """Whether module access is locked."""
-    level: int
-    """Module level."""
-
-
-class AssistChar(base.BaseModel):
-    """Publicly visible operator info."""
-
-    char_id: str = pydantic.Field(alias="charId")
-    """Character ID."""
-    skin_id: str = pydantic.Field(alias="skinId")
-    """Equipped skin ID."""
-    skills: typing.Sequence[Skill]
-    """Operator skills."""
-    main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
-    """Level of the equipped skill."""
-    skill_index: int = pydantic.Field(alias="skillIndex")
-    """Index of the equipped skill."""
-    evolve_phase: int = pydantic.Field(alias="evolvePhase")
-    """Elite phase."""
-    favor_point: int = pydantic.Field(alias="favorPoint")
-    """Operator trust points."""
-    potential_rank: int = pydantic.Field(alias="potentialRank")
-    """Operator potential. Starts at 0."""
-    level: int
-    """Operator level."""
-    crisis_record: base.DDict = pydantic.Field(alias="crisisRecord", repr=False)
-    """IDK. selectedCrisis is used for contingency contracts elsewhere."""
-    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
-    """ID of the currently equipped module."""
-    equip: typing.Mapping[str, UniEquip]
-    """Equipped modules. Module ID to module info."""
-
-    @property
-    def static(self) -> base.DDict:
-        """Static data for this operator."""
-        return self.client.gamedata.character_table[self.char_id]
-
-    @property
-    def trust(self) -> int:
-        """Trust calculated from favor_point."""
-        return self.client.gamedata.calculate_trust_level(self.favor_point)
-
-    @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
-    def _fix_amiya(cls, values: typing.Any) -> typing.Any:
-        """Flatten Amiya to only keep her guard form."""
-        if values and values.get("tmpl"):
-            current = values["tmpl"][values["currentTmpl"]]
-            values.update(current)
-
-        return values
-
-
-class PlacedMedal(base.BaseModel):
-    """A single medal on a board."""
-
-    id: str
-    """Medal ID."""
-    pos: typing.Tuple[int, int]
-    """Medal position on the board."""
-
-    @property
-    def static(self) -> base.DDict:
-        """Static data for this medal."""
-        return self.client.gamedata.medal_table.medal_list[self.id]
-
-
-class MedalBoardCustom(base.BaseModel):
-    """Custom medal board layout."""
-
-    layout: typing.Sequence[PlacedMedal]
-    """Medals on the board."""
-
-
-class MedalBoardTemplate(base.BaseModel):
-    """Template medal board layout."""
-
-    group_id: str = pydantic.Field(alias="groupId")
-    """Medal board template ID."""
-    medal_list: typing.Sequence[str] = pydantic.Field(alias="medalList")
-    """Medal IDs on the board."""
-
-    @property
-    def static(self) -> base.DDict:
-        """Static data for this medal board."""
-        groups = self.client.gamedata.medal_table.medal_type_data.activity_medal.group_data
-        return next(i for i in groups if i.group_id == self.group_id)
-
-
-class MedalBoard(base.BaseModel):
-    """Medal board info."""
-
-    type: typing.Literal["CUSTOM", "TEMPLATE", "EMPTY"]
-    """Medal board layout type."""
-    custom: typing.Optional[MedalBoardCustom]
-    """Custom medal board layout."""
-    template: typing.Optional[MedalBoardTemplate]
-    """Template medal board layout."""
-
-
-class PartialPlayer(base.BaseModel):
-    """Partial player info from search."""
-
-    nickname: str = pydantic.Field(alias="nickName")
-    """Player nickname."""
-    nick_number: str = pydantic.Field(alias="nickNumber")
-    """Player nickname number after #."""
-    uid: str
-    """Player UID."""
-    friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
-    """How many friend slots are open."""
-    server_name: str = pydantic.Field(alias="serverName")
-    """Server name. Should always be Terra."""
-    level: int
-    """Player level."""
-    avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
-    """IDK. Always 0."""
-    avatar: typing.Optional[Avatar] = None
-    """Selected avatar."""
-    assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
-    """Assist operator list."""
-    last_online_time: datetime.datetime = pydantic.Field(alias="lastOnlineTime")
-    """Last online time."""
-    medal_board: MedalBoard = pydantic.Field(alias="medalBoard")
-    """Medal board."""
-
-
-class Player(PartialPlayer):
-    """Player info."""
-
-    register_ts: datetime.datetime = pydantic.Field(alias="registerTs")
-    """Account creation time."""
-    main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
-    """Current main story stage ID. None if completed."""
-    char_cnt: int = pydantic.Field(alias="charCnt")
-    """Number of operators owned."""
-    furn_cnt: int = pydantic.Field(alias="furnCnt")
-    """Number of furniture owned."""
-    secretary: str
-    """ID of the secretary operator."""
-    secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
-    """ID of the secretary operator's skin."""
-    resume: str
-    """Player display bio."""
-    team_v2: typing.Mapping[str, int] = pydantic.Field(alias="teamV2")
-    """Amount of characters owned in each faction."""
-    board: typing.Sequence[str]
-    """Factions with full trust. Shows up blue in-game."""
-    info_share: typing.Optional[datetime.datetime] = pydantic.Field(alias="infoShare")
-    """IDK."""
-    recent_visited: bool = pydantic.Field(alias="recentVisited")
-    """IDK."""
-    info_share_visited: typing.Optional[int] = pydantic.Field(None, alias="infoShareVisited")
-    """IDK."""
+"""Arknights API social models.
+
+Any field description prefixed with IDK means it's just a guess.
+"""
+import typing
+
+import pydantic
+
+from . import base
+
+
+class Avatar(base.BaseModel):
+    """User display avatar."""
+
+    type: typing.Literal["ASSISTANT", "ICON", "DEFAULT"] = "DEFAULT"
+    """Avatar type."""
+    id: typing.Optional[str] = None
+    """Avatar ID. For example a skin ID."""
+
+
+class Skill(base.BaseModel):
+    """Skill of a character."""
+
+    skill_id: str = pydantic.Field(alias="skillId")
+    """Skill ID."""
+    unlock: bool
+    """Whether the skill is unlocked."""
+    state: bool = pydantic.Field(repr=False)
+    """IDK. Always false."""
+    specialize_level: int = pydantic.Field(alias="specializeLevel")
+    """Skill mastery level."""
+    complete_upgrade_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(alias="completeUpgradeTime")
+    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
+
+    @property
+    def static(self) -> base.DDict:
+        """Static data for this skill."""
+        return self.client.gamedata.skill_table[self.skill_id]
+
+
+class UniEquip(base.BaseModel):
+    """Equipped modules."""
+
+    hide: bool
+    """IDK. Whether the module is publicly hidden."""
+    locked: bool
+    """Whether module access is locked."""
+    level: int
+    """Module level."""
+
+
+class AssistChar(base.BaseModel):
+    """Publicly visible operator info."""
+
+    char_id: str = pydantic.Field(alias="charId")
+    """Character ID."""
+    skin_id: str = pydantic.Field(alias="skinId")
+    """Equipped skin ID."""
+    skills: typing.Sequence[Skill]
+    """Operator skills."""
+    main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
+    """Level of the equipped skill."""
+    skill_index: int = pydantic.Field(alias="skillIndex")
+    """Index of the equipped skill."""
+    evolve_phase: int = pydantic.Field(alias="evolvePhase")
+    """Elite phase."""
+    favor_point: int = pydantic.Field(alias="favorPoint")
+    """Operator trust points."""
+    potential_rank: int = pydantic.Field(alias="potentialRank")
+    """Operator potential. Starts at 0."""
+    level: int
+    """Operator level."""
+    crisis_record: typing.Mapping[str, int] = pydantic.Field(alias="crisisRecord")
+    """Maximum risk this operator was used as a support in. -1 if never used."""
+    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
+    """ID of the currently equipped module."""
+    equip: typing.Mapping[str, UniEquip]
+    """Equipped modules. Module ID to module info."""
+    tmpl: typing.Mapping[str, base.DDict] = pydantic.Field(default_factory=base.DDict, repr=False)
+    """Alternative operator class data. Only for Amiya."""
+
+    @property
+    def static(self) -> base.DDict:
+        """Static data for this operator."""
+        return self.client.gamedata.character_table[self.char_id]
+
+    @property
+    def trust(self) -> int:
+        """Trust calculated from favor_point."""
+        return self.client.gamedata.calculate_trust_level(self.favor_point)
+
+
+class PlacedMedal(base.BaseModel):
+    """A single medal on a board."""
+
+    id: str
+    """Medal ID."""
+    pos: typing.Tuple[int, int]
+    """Medal position on the board."""
+
+    @property
+    def static(self) -> base.DDict:
+        """Static data for this medal."""
+        return self.client.gamedata.medal_table.medal_list[self.id]
+
+
+class MedalBoardCustom(base.BaseModel):
+    """Custom medal board layout."""
+
+    layout: typing.Sequence[PlacedMedal]
+    """Medals on the board."""
+
+
+class MedalBoardTemplate(base.BaseModel):
+    """Template medal board layout."""
+
+    group_id: str = pydantic.Field(alias="groupId")
+    """Medal board template ID."""
+    medal_list: typing.Sequence[str] = pydantic.Field(alias="medalList")
+    """Medal IDs on the board."""
+
+    @property
+    def static(self) -> base.DDict:
+        """Static data for this medal board."""
+        groups = self.client.gamedata.medal_table.medal_type_data.activity_medal.group_data
+        return next(i for i in groups if i.group_id == self.group_id)
+
+
+class MedalBoard(base.BaseModel):
+    """Medal board info."""
+
+    type: typing.Literal["CUSTOM", "TEMPLATE", "EMPTY"]
+    """Medal board layout type."""
+    custom: typing.Optional[MedalBoardCustom]
+    """Custom medal board layout."""
+    template: typing.Optional[MedalBoardTemplate]
+    """Template medal board layout."""
+
+
+class PartialPlayer(base.BaseModel):
+    """Partial player info from search."""
+
+    nickname: str = pydantic.Field(alias="nickName")
+    """Player nickname."""
+    nick_number: str = pydantic.Field(alias="nickNumber")
+    """Player nickname number after #."""
+    uid: str
+    """Player UID."""
+    friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
+    """How many friend slots are open."""
+    server_name: str = pydantic.Field(alias="serverName")
+    """Server name. Should always be Terra."""
+    level: int
+    """Player level."""
+    avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
+    """IDK. Always 0."""
+    avatar: typing.Optional[Avatar] = None
+    """Selected avatar."""
+    assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
+    """Assist operator list."""
+    last_online_time: base.ArknightsTimestamp = pydantic.Field(alias="lastOnlineTime")
+    """Last online time."""
+    medal_board: MedalBoard = pydantic.Field(alias="medalBoard")
+    """Medal board."""
+
+
+class Player(PartialPlayer):
+    """Player info."""
+
+    register_ts: base.ArknightsTimestamp = pydantic.Field(alias="registerTs")
+    """Account creation time."""
+    main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
+    """Current main story stage ID. None if completed."""
+    char_cnt: int = pydantic.Field(alias="charCnt")
+    """Number of operators owned."""
+    furn_cnt: int = pydantic.Field(alias="furnCnt")
+    """Number of furniture owned."""
+    secretary: str
+    """ID of the secretary operator."""
+    secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
+    """ID of the secretary operator's skin."""
+    resume: str
+    """Player display bio."""
+    team_v2: typing.Mapping[str, int] = pydantic.Field(alias="teamV2")
+    """Amount of characters owned in each faction."""
+    board: typing.Sequence[str]
+    """Factions with full trust. Shows up blue in-game."""
+    info_share: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(alias="infoShare")
+    """IDK."""
+    recent_visited: bool = pydantic.Field(alias="recentVisited")
+    """IDK."""
+    info_share_visited: typing.Optional[int] = pydantic.Field(None, alias="infoShareVisited")
+    """IDK."""
```

### Comparing `arkprts-0.1.6/pyproject.toml` & `arkprts-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [project]
+name = "arkprts"
 requires-python = ">=3.9"
+version = "0.2.0"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
@@ -42,51 +44,60 @@
 # SLF: Private member access
 # TCH: Not using TYPE_CHECKING (ugly)
 # TD: TODO comment conventions
 # ANN10: Missing type annotation for self/cls (useless)
 # ANN401: Use of typing.Any (complicates)
 # B008: Do not perform function calls in argument defaults (pydantic)
 # B027: Empty method in ABC (optional rewrite)
+# B028: No stacklevel in warnings
 # B905: zip without strict= (ugly)
 # C408: Unnecessary dict call (ugly)
 # D105: Missing docstring in magic method (useless)
+# E501: Line too long (black already manages this)
 # N805: First argument is not self (pydantic)
 # PGH003: Specific rules when ignoring type issues
 # PLR0913: Too many arguments
 # PLR2004: constant value in comparison (asserts)
 # PLW2901: Redefining for-loop variable
 # RET504: Unnecessary variable before return (ugly)
-# TRY003: Long exception message
 # S101: Use of assert (type-checking)
 # S110: Try, Except, Pass (annoying)
+# S3xx: Use of random or md5
+# S607: Using git instead of an entire path
+# TRY003: Long exception message
+# UP013: Functional TypedDict
 ignore = [
   "A",
   "ARG",
   "EM",
   "ERA",
   "FBT",
   "SLF",
   "TCH",
   "TD",
   "ANN10",
   "ANN401",
   "B008",
   "B027",
+  "B028",
   "B905",
   "C408",
   "D105",
+  "E501",
   "N805",
   "PGH003",
   "PLR0913",
   "PLR2004",
   "PLW2901",
   "RET504",
   "S101",
+  "S3",
+  "S607",
   "TRY003",
-  "S110",
+  "UP013",
 ]
 # auto-fixing too intrusive
 # F401: Unused import
 # F841: Unused variable
 # B007: Unused loop variable
 unfixable = ["F401", "F841", "B007"]
```

