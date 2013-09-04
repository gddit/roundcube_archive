Extended archiving plugin for Roundcube
=======================================

Possible deprecation
--------------------

It seems, that roundcube is extending their included archive plugin with
the functionality of this plugin (probably) in the next release.

I will wait and see, if that extension meets my needs. If that is so, 
this plugin will be deprecated.

Introduction
------------

This plugin extends roundcube with a complete archiving solution, that
archives mails under an archiving folder by month, year or sender.

Based on the original archive plugin by Andre Rodier, Thomas Bruederli
Button and skin-settings taken from the Archivefolder plugin by Andre
Rodier, Thomas Bruederli and Roland 'rosali' Liebl

Supports account-specific configuration for the accounts-plugin by Roland
'rosali' Liebl

Supports both classic and larry skins.

Install
-------

To install, put this into a folder named "de_dieploegers_archive" under the
plugin directory and add "de_dieploegers_archive" to the array
"$rcmail_config['plugins']" in main.inc.php

Usage
-----

To use the plugin, first go to settings, section "Archive" and set up your
archiving folder and the archiving type.

The following types are available

 * By Year - Will use a structure like "Archive/2010",
 "Archive/2011" and "Archive/2012"
 * By Month - Will use a structure like "Archive/2010/2010-01",
 "Archive/2010/2010-02" and "Archive/2012/2012-11"
 * By Sender - Will use a structure like "Archive/sender@domain.com". If your
  IMAP server uses "." as the hierarchy delimiter, Roundcube will use "_" in
  email-addresses like "sender@domain_com".
