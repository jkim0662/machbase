# Jump-start Lab for DB developers

Machbase provides SDK for developing various applications. Machbase supports CLI, ODBC, JDBC, Python and RESTful API libraries. In this page, you will find brief definitions of each application.

If you need more detailed information, please refer to[SDK Guide chapter](http://doc.machbase.com/cli-and-odbc).

**List of Contents**

* [CLI and ODBC](http://doc.machbase.com/jump-start-lab-for-db-developers$CLI and ODBC)
* [JDBC](http://doc.machbase.com/jump-start-lab-for-db-developers$JDBC)
* [Python module](http://doc.machbase.com/jump-start-lab-for-db-developers$Python module)
* [RESTful API](http://doc.machbase.com/jump-start-lab-for-db-developers$RESTful API)

Sample files are located under $MACHBASE\_HOME/sample  directory as shown below.

\[mach@localhost ~\] cd $MACHBASE\_HOME/sample

| Directory name | Description |
| :--- | :--- |
| cli | sample code with CLI library. |
| jdbc | sample code with JDBC library. |
| python | sample code with python library. |
| rest | sample code with RESTful API. |

### CLI and ODBC

CLI is one of software development standards inISO/IEC 9075-3:2003. It defines how CLI passes SQL to database and also its functions and specifications how the results are received and analyzed. The well-known standard interface is ODBC \(Open Database Connectivity\) and it allows client programs how to be connected with the database, regardless of database types.

Machbase provides samples with using CLI library. These samples help you connect to Machbase server, insert data directly, insert data with prepared statement, insert data with high speed input protocol , get column information, insert data with multi thread from reading text file and  retrieve data from Machbase.

For more detailed information, please see the[CLI and ODBC page.](http://doc.machbase.com/cli-and-odbc)

### JDBC

Java Database Connectivity \(JDBC\) is an application programming interface \(API\) for the programming language Java, that defines how a client may access a database. It is the the set of API that provides consistent interface for various relational databases and it is a series of the object-oriented programs. In other words, Machbase has the advantage of adapting it immediately without modifying the code if JDBC driver is provided, no matter which database that you use.

Machbase provides samples with using JDBC driver. These samples help you connect to Machbase server, insert data directly, insert data with prepared statement, insert data with high speed input protocol from reading text file and retrieve data from Machbase.

For more detailed information, please see the[JDBC page.](http://doc.machbase.com/jdbc)

### Python module

Python module is an application programming interface for the programming language Python, its classes are provided to use CLI method in order to communicate with the Machbase server.

Machbase provides samples with using python modules. These samples help you connect to Machbase server, insert data directly, insert data with high speed input protocol from reading text file and retrieve data from Machbase.

For more detailed information, please see the[Python module page](http://doc.machbase.com/python-module).

### RESTful API

Representational State Transfer \(REST\) is a Software Architecturestyle consisting of guidelines and best practices for creating scalable web services. Machbase is not standard REST API, rather RESTful API that processes CRUD by using POST and GET methods. It uses POST method for inserting data and GET method for rest of operations to do the other work.

For more detailed information, please see the[RESTful API page](http://doc.machbase.com/restful-api).

