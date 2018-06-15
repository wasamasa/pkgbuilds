PKGBUILDs
=========

Virtual Fonts
-------------

I'm not a fan of nearly every GUI package requiring at least one font
to be installed system-wide, so I created a number of virtual font
packages to satisy the respective dependencies.

- ``ttf-font-virtual``
- ``ttf-dejavu-virtual``
- ``ttf-cantarell-virtual``

GTK3
----

Patched version for better interoperability with `Orbment
<https://github.com/Cloudef/orbment>`_.  Enable with ``GTK_CSD=0``.

- ``gtk3-optional-csd``

IUP
---

An interesting GUI toolkit.  Due to problems with the build process, I
packaged the pre-compiled dynamic libraries.  Doesn't work properly on
Arch (debug dialogs are broken, padding and margin are zero), but well
enough for getting an idea how the application will look like.

- ``iup-bin``
- ``libcd-bin``
- ``libim-bin``

KiWi
----

Widgets for SDL2.  Packaged because nobody else did.

- ``kiwi-git``

libui
-----

A GUI toolkit in the spirit of IUP, but built on top of a more recent
GTK3.  This has been created because the AUR PKGBUILD is out of date
due to upstream switching to CMake.

StumpWM
-------

I blame Lisp mysticism for getting the better for me.  This PKGBUILD
assumes you've installed the dependencies via Quicklisp already.

- ``stumpwm-git``

timelimit
---------

Not packaged yet.  I realized later that ``timeout`` is a thing
already, so there's probably no need for anyone to install this one.

cloc
----

For some reason there's only a SVN version of this package on the AUR.

Kawa
----

Alternative version of the existing git package that makes use of the
JLine3 library.

the_silver_searcher
-------------------

The new stable release broke search in compressed files and upstream
doesn't respond to MRs, so I added patches to the official PKGBUILD.

Ancient and obscure programming language implementations
--------------------------------------------------------

I'm always looking out for candidates to implement `MAL
<https://github.com/kanaka/mal>`_ in.

- ``aikido``
- ``awe``
- ``cim``
- ``cm3-bin``
- ``cm3-doc``
- ``jff-algol``
- ``red-snapshot``
- ``redtamarin-sdk-bin``
