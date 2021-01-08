# Oracle MDA Utility

This VBO allows connectivity from Blue Prism to an Oracle RBMS. It provides the following functionality:

- Configure - Setting a flag to report connectivity exceptions
- Set Connection - Defines the parameters in order to connect to the Oracle host.
- Transaction Support - Begin - Commit/Rollback
- Execute - Executes a valid SQL Script.
- Get Number - Returns a numeric scalar value.
- Get Text - Returns a string value.
- Get Collection - Returns a set of data as a Blue Prism collection.
- Get CSV File - Returns comma separate variable (CSV) file based on the supplied SQL Select query.
- Get CSV - Returns a comma separated variable string based on the supplied SQL Select query.
- Get User Name - Returns the current user name from the environment.
- Get Machine Name - Returns the current machine name from the environment.
- Delete Rows - Where - Deletes a set of rows from the supplied table based on the where clause being satisfied.
- Drop Table - Removes a table from the schema. 
- Truncate Table - Removes all rows from the supplied table name.

# Update Notes Jan 2021

An issue was reported with the asset in relation to failing to close connections if this asset was used in a loop. This should now be fixed but it is now necessary to provide 2 versions of the asset. The bprelease file format changed at Blue Prism version 6.6. Therefore I have provided 2 versions of the asset, one which is for 6.5 and earlier and one for 6.6 and later. For the record, this version was created using Blue Prism V6.9 and the pre 6.5 version was created using the StudioDisplayFix tool, available on github.

The file OracleMDA_6_displayfix.bprelease is for Blue Prism V6.5 and earlier.
The file OracleMDA_6_Post6.5.bprelease is for Blue Prism V6.6 and later.

Please advise any issues using the community forums.
