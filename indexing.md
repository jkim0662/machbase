# RED-BLACK Index

It is a memory index for real-time data retrieval and can be created only on volatile tables. It can be created on all columns of a volatile table and can only be created on a single column.  
The volatile table provides a red-black tree optimized for real-time search, and indexes can be installed for all data types. However, one index can be created for one column, and no composite index is provided.

Example;

```
mach> CREATE VOLATILE TABLE v_table (id INTEGER primary key, name VARCHAR(10));

Created successfully.
```

```
mach>CREATE INDEX idx_vrb on v_table (name) INDEX_TYPE REDBLACK;

Created successfuly.
```



