# CPT264 Assignment 1

---------------
Basic
---------------

The basic script retrieves basic information about the system and the current user.

Example:	./basic freemem

freemem | diskfree | quota | groups | history
	
	freemem  - Displays the amount of free memory available on the system
	diskfree - Displays the amount of disk space free on each partition on the system
	quota    - Displays the disk quota(s) for the current user
	groups	- Displays the groups that the current user is a member of
	history	- Displays a history of commands that have been entered into the current shell


----------------
Advanced
----------------

The advanced script retrieves system information or performs a backup.

Example:	./advanced -b \*.php php-files-folder

-p | -o | -b wildcard destination

	-p 							- Prints the number of CPUS available in the system
	-o 							- Outputs the maximum number of open files allowed per user
	-b wildcard destination - Searches for all files that match the wildcard 
											and copies them to the destination


---------------
Userman
---------------

The userman script retrieves information about the user from the /etc/passwd file.

Example:	./userman groupid ryan

userid user | groupid user | comment user | home user | shell user

	userid user 	- Displays the user ID (a number) for the user specified
	groupid user 	- Displays the default group ID for the user specified
	comment user 	- Displays the comment field (GECOS) for the user specified
	home user 		- Displays the home directory of the user specified
	shell user 		- Displays the default login shell for the user specified


--------------
Sysman
--------------

The sysman script provides an interface to easily access functions from the basic, advanced,
and userman scripts. It takes no arguments.

Example:	./sysman

Users will be prompted with a menu, at which they may enter numbers corresponding to the menu item
to navigate the system.


------------------
Known issues
------------------

'./basic quota' does not correctly display quota.


-----------------
Other notes
-----------------

This was the first time I've had much experience with Unix at all, let alone scripting.
I enjoy programming so found this quite enjoyable, and I've learnt a lot from this assignment
already. The getopts section of the advanced script proved to be one of the more difficult aspects
but otherwise I feel like it went well.
