---
title: Attachment
parent: Iteration 3
has_children: false
---

## Read / Write BLOBs from / to SQL Server using C#
**Obtaining BLOB Values from a Database**
Binary large objects (BLOBs) contain gigabytes of data. When accessing the data in the BLOB field, use the _GetBytes_ or _GetChars_ typed accessors of the DataReader, which fill an array with data.

_GetBytes_ and _GetChars_ will return a long value, which represents the number of bytes or characters returned. If you pass a null array to _GetByte_ or _GetChars_, the long value returned will be the total number of bytes or characters in the BLOB.

**Writing BLOB Values to a Database**
You can write a binary large object (BLOB) to a database as either binary or character data, depending on the type of field at your data source. To write a BLOB value to your database, issue the appropriate **INSERT** or **UPDATE** statement and pass the BLOB value as an input parameter.

If the BLOB is stored in binary format, such as a SQL Server image field, you can pass an array of type byte as a binary parameter.

Data can be exported into XML files for each users in a general format, so that it can be used for other applications. This will ensure users that they will not lose their data. Also they can import other XML files from other applications to the application.

![Diagram](../../images/final-assignment/SQL.png)
