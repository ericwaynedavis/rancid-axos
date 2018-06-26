Rancid login script for Calix AXOS based systems

Calix AXOS scripts for Rancid. 

Changes:
-------
version 1.0 - Initial release. Modified existing clogin and ios.pm scripts to work with AXOS using Rancid verison 3.7.

Includes:
--------
axoslogin - basic login script, confirmed to work with stock AXOS configuration. 
axos.pm - the Rancid Perl wrapper module to parse the configuration.
rancid.types.conf - added 'axos' device type configuration

Installation:
------------
1) Copy axoslogin to your '~/rancid/bin/' directory.
2) Copy axos.pm to your '~/rancid/lib/rancid/' directory.
3) Append rancid.types.conf to your existing rancid.types.conf file.
4) Add a new device to your 'router.db', with the vendor of 'axos'.
5) Add an entry to your .clogin file with the following elements:
	add method <host> ssh
	add user <host> <username>
	add password <host> <password>


Bugs:
----
None observed, but I'm sure they're there.
