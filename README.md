Server Manager
=============

###Objective
The objective of this server management system is to allow easy end user control of servers.
User control should include the ability to add, remove, restart, modify, and perform software-specific actions.

####Server Modules
Each server type should have a "module." These modules should be of a standard type (json, yaml, txt) and flat
file. These modules will contain the information that the server manager needs in order to generate a server
and will be used as a reference when writing the management system. This information should consist of proper restarting
/starting/stopping procedures, special commands and functions that can be issued though the interface, 

####Adding
Server adding should be nearly entirely automated. Default fields such as path, port, and source version should 
be autofilled with appropriate values. The user should mainly be prompted for the name, privacy, and mods.

###Guideline
