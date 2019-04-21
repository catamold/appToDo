---
title: Mapping
parent: NHibernate
grand_parent: Final Assignment
has_children: false
---

## NuGet

NuGet is distributed as a Visual Studio extension. It supports multiple programming languages, including _.NET Framework_ packages and Native packages written in C++.
The application need some Frameworks to work installed from NuGet:
* MySQL.Data _by Oracle_ **v6.10.8**
* MySQL.Data.Entity _by Oracle_ **v6.10.8**
* NHibernate _by NHibernate community, Hibernate community_

## NHibernate Class

The class will represent the object. We have to create properties in the class that will match the fields in the database. 
> **public virtual int property { get; set; }** sets a class property that matches a field in the database. Note the property is defined with a virtual keyword. This makes it possible for the fields to be overridden.

## NHibernate Mapping

NHibernate uses XML files for mapping database fields to objects properties. The XML file should always end with _*.hbm.xml_ extension. In Solution Explorer of _MyClass.hbm.xml_ the Build Action has to be set as Embedded Resource.
> **hibernate-mapping xmlns="urn:nhibernate-mapping-2.2" assembly="CustomerRecords" namespace="CustomerRecords"** is the root element of the mapping file. The element has xmlns, assembly and namespace attributes. The assembly and namespace attributes should match your project assembly and namespace values. _Assembly_ name and _namespace_ name can be found in application's Properties.
>
> **class name="Customers"** defines the class element.
>
> **id name="customer_id"** defines primary key. In our case its customer_id
>
> **property name="field_name"** matches the fields in the table that you wish to manipulate using NHibernate.

## NHibernate Connection String MySQL

> **x.ConnectionString** our connection string will connect to the local machine because we set the server property to a dot. _(e.g. "Database=test_db;Data Source=localhost;Port=3306;User Id=admin;Password=123")_
>
> **x.Driver<MySqlDataDriver>();** we will work with MySqlDataDriver
>
> **x.Dialect<MySQL55Dialect>();** we will use the dialect for MySQL Server. This will make available the features in MySQL Server.

## Executing Hibernate Query Language (HQL)**

Hibernate Query Langauge (HQL) is very similar to SQL.
* **FROM…** indicates this is a SELECT query in SQL language
* **WHERE…** works the same as in SQL

In case of mapping
> **class name**="MyClass" **table**="MY_TABLE"

The query should be
> **session.CreateQuery**("FROM MyClass")

## Transactions

_CreateQuery()_ with the select clause picks which objects and properties to return in the query result set.

_Save()_ takes a new object without an identifier and attaches it to the session. The object will be **INSERT**'ed.

_Update()_ takes an existing object that has an identifier but is not in the session and attaches it to the session. The object will be **UPDATE**'d.

_SaveOrUpdate()_ looks at the identifier and decides what is necessary in the above. The object will be **INSERT**'ed or **UPDATE**'d if already exists. The object will be **UPDATE**'d.

_Delete()_ will remove an object's state from the database. The object will be **DELETE**'d.

_Commit()_ will flush the session and commit the transaction.

_Flush()_ will force the SQL **INSERT**.

_Close()_ represents the end of a session.