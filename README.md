Server Manager
=============

###Objective
The objective of this server management system is to allow easy end user control of servers.
User control should include the ability to add, remove, restart, modify, and perform software-specific actions.

####Server Modules
Each server type should have a "module." These modules should be of a standard type that allows for easy parsing 
into a python class on startup. These modules will contain the information that the server manager needs in order 
to check, start, stop, and manage a server. They should also point to any necessary dependencies.

Priorities
    - Status (player numbers, uptime, map)
    - Start and Stop
    - Restart
    - Reconfigure
    - Creation
    - Deletion

Game Type Priorities
    - Minecraft
    - NS2
    - Tremulous or UV

###Permissions
The manager should be able to know who requested a restart. Using this information, it should be able to check
if the user has appropriate permissions to restart a server of this type. Ideally, in the future, server admins
should be able to modify who can manage what server and to what extent.

###Logging
All actions on the manager should be logged, even automatic system actions. This will be done through <MySQL, 
flat file, flat sql, PostgreSQL>.

###Guidelines
This server management system will be written in python where at all possible. The modules linked into this manager
will be written in <json, yaml, xml>. A web front end will be served through django whenever possible. PHPBB3
will be our backend for user management and permission checking. MySQL calls will be made through python whenever
possible. All python code written should follow PEP 8 guidelines. No tabs are allowed and any modules should 
follow similar formatting when at all possible.
