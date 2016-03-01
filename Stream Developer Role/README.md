# Strean Developer Role

##Description
This rule package creates a new role for developers (role_dev). With this role
the user is granted rights to create apps, tags and data connections.
The rules will also based on group membership grant users access to read, update,
delete and publish in streams where the custom property \@DevGroup contain a group
that the developer is member of.
In the QMC the developer will have access to
* Apps
* Content libraries
* Streams
* Tags  

##Rules
|Rule|Description|
|DevCreate|Grants create rights to role role_dev that need to be assigned to developers|
|DevRUDP|Grants developers in a group that a stream or data connection has marked with \@DevGroup to read, update, delete and publish if a stream|
|DevSection|The sections in the QMC that developers in the role role_dev can access|

##Custom Properties
|Custom Property|Description|
|\@DevGroup|Custom property on streams and data connections that points out which group a developer need to belong to to be able to work with content of a stream or a data connection|
