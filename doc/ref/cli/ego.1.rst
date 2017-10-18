=========
ego
=========

---------------------------------------------
Funtoo Linux System Management Meta-Command
---------------------------------------------

:Author: Daniel Robbins <drobbins@funtoo.org>
:Version: ##VERSION##
:Manual section: 1
:Manual group: Funtoo Linux Core System

SYNOPSIS
--------

The *ego* command is a meta-command that consists of several modules that provide functionality. Currently, the
following modules are supported:

sync
  Ego sync module. See ego-sync(8).

profile
  Ego profile module (shortcut: *epro*) See ego-profile(8).

query
  Ego query module. See ego-query(1).

doc
  Ego Wiki Documentation module. (shortcut: *edoc*) See ego-doc(1).

You can invoke the relevant module by using the calling convention ``ego module [arg1...]``. For example, to view the
Funtoo Linux Installation Guide, type ``ego doc Install | less``. Alternatively, you can use the module shortcut if
one exists, such as ``edoc install | less``.

LICENSE
--------

.. include:: ../../../COPYRIGHT.txt