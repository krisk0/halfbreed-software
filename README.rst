Half-breed -- near-native compilation of open-source software for your device
==========

Now that I can compile and run on my desktop Linux programs meant to run on my smaller computer (such as Android phone), how do I compile from source common programs such as busybox, 7-zip, python?

The repository answers the question, by giving exact recipes to build some must-have software. As of today (22 July 2016), only 7zip and busybox recipe is here.

Hopefully the recipes can be easily modified to build code for a different CPU, or code for `musl <https://github.com/krisk0/alien-libc/tree/master/musl>`_ or `uclibc <https://github.com/krisk0/alien-libc/tree/master/uclibc>`_ rather than bionic.

Prerequisites
^^^^^^^^^^^^^
  a) Ability to compile code for your device. For Intel Atom tablet, you use my built from source `bionic toolchain <https://github.com/krisk0/pc-linux-android/>`_ or some other development software.
  
  b) Root access to a Gentoo Linux computer or at least to something Unix-like with Portage package manager.
  
  c) Ability to download ``.zip`` and ``.tar.gz`` from `github <https://github.com>`_ and other sites, or downloaded files planted onto your ``/distfiles``.

Directory structure
^^^^^^^^^^^^^^^^^^^
The repository is organized in the following manner. ``common`` subdirectory contains generally useful files; other directories contain recipes to build a specific software under specific conditions. For instance, ``p7zip`` folder contains working script and detailed instrucion on how to build 7-zip command-line executable for 64-bit Intel/Android on a 64-bit Intel/Linux.
