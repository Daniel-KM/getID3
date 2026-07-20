Fork of getID3
==============

The aim of this fork is to maintain a stable, namespaced and PSR-4 compliant
version of the library getID3 via periodic merges of the master branch (1.9)
into the v2.0 branch, whose status is dev/beta since May 2019.

To use it, just use a standard require command, without need to change minimum
stability:

```bash
$ composer require "sempia/getid3"
```

The namespace of the library is kept (`JamesHeinrich\GetID3\`), so you don't
need to change anything in the code. This package replaces `james-heinrich/getid3`
at the same version numbers, so it is a drop-in substitute for the upstream 2.0
betas. It is not compatible with the 1.9 api (global classes getID3 and getid3_lib).

The version numbering follows the upstream 2.0 branch: 2.0.x, where each
release integrates the fixes merged from the upstream 1.9 branch.

**Below is the official readme**


getID3
======

A PHP library to extract and write useful information to/from popular multimedia file formats.  
If you want to donate, there is a link on <https://www.getid3.org> for PayPal donations.

[![Latest Stable Version](https://poser.pugx.org/james-heinrich/getID3/version.svg)](https://packagist.org/packages/james-heinrich/getid3)
[![Build Status](https://github.com/JamesHeinrich/getID3/actions/workflows/continuous-integration.yml/badge.svg?branch=2.0)](https://github.com/JamesHeinrich/getID3/actions?query=branch%3A2.0)


Installation
============
Using [composer](https://packagist.org/packages/james-heinrich/getid3):
```bash
$ composer require "james-heinrich/getid3:^2.0-dev"
```

__How can I check that getID3() works on my server/files?:__  
  _Unzip getID3() to a directory, then access `/demos/demo.browse.php`_


Usage
=====
See /demos/demo.basic.php for a very basic use of getID3() with no fancy output, just scanning one file.  
For an example of a complete directory-browsing, file-scanning implementation of getID3(), please run /demos/demo.browse.php  

See /demos/demo.mysql.php for a sample recursive scanning code that scans every file in a given directory, and all sub-directories, stores the results in a database and allows various analysis / maintenance operations.  

See /demos/demo.write.php for how to write tags.


Documentation
-------------
* [What does getID3() do?](docs/Features.md)
* [What does the returned data structure look like?](docs/Structure.md)
* [Requirements](docs/Requirements.md)
* [Upgrading](docs/Upgrading.md)
* [License](LICENSE.md)
* [References](docs/References.md)
* [Known Bugs/Issues in other programs](docs/External-Issues.md)
* [Known Bugs/Issues in getID3() that cannot be fixed](docs/Known-Issues.md)
* [Known Bugs/Issues in getID3() that may be fixed eventually](docs/Outstanding-Issues.md)
* [Future Plans](docs/TODO.md)
