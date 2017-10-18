=======
ego kit
=======

---------------------------------------------
Funtoo Linux Kit Module
---------------------------------------------

:Author: Daniel Robbins <drobbins@funtoo.org>
:Version: ##VERSION##
:Manual section: 1
:Manual group: Funtoo Linux Core System

SYNOPSIS
========

``ego kit status``

``ego kit list``

USAGE
=====

Use the ``ego kit`` command to display information about currently-enabled kits as well as available kits.

STATUS INFORMATION
==================

Use ``ego kit status`` to display status information on meta-repo and all kits. A table will be printed to the
console displaying the location of meta-repo, the last time it was updated using ``ego sync``, all kits, the current
branch selected for each kit, the default branch for the kit (if different than the current branch,) and the stability
level of each branch.

It's important to note that the stability level indicates the *true* stability of the branch; for example, Funtoo Linux
developers may create a ``3.0-prime`` branch but immediately after its creation, it will be considered to have a
``dev`` (not ``prime``) stability level. Only when the necessary fixes and patches have been applied will Funtoo Linux
developers bump the branch to ``prime`` stability. So in this regard, the name of the branch indicates its eventual,
intended stability level, while the stability level itself indicates the *actual* stability level of the branch.

LIST ALL KITS
=============

``ego kit list`` will display information similar to ``ego kit status``, but will also show not-currently-enabled kits
and their stability level. See ``BRANCH STABILITY LEVELS``, below.

BRANCH STABILITY LEVELS
=======================

The following branch stability levels are currently defined:

PRIME
  Production-level, enterprise-quality and fully supported with backports, or a current Gentoo branch that is our
  default branch.

NEAR-PRIME
  Nearing production quality, requiring additional testing and user validation before marked as ``prime``

BETA
  Beta release -- not yet guaranteed to be particularly stable, yet appropriate for adventurous users to test only.

ALPHA
  Alpha release -- only for adventurous users, who should expect some breakage.

DEV
  Developer release -- in active development; not indended for non-developers.

CURRENT
  Current means that the branch tracks Gentoo, and is *not* our default branch. Some of our branches track Gentoo but
  are our default branch, in which case the branch will be marked as ``prime``.