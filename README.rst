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

StumpWM
-------

I blame Lisp mysticism for getting the better for me.  This PKGBUILD
assumes you've installed the dependencies via Quicklisp already.

- ``stumpwm-git``
