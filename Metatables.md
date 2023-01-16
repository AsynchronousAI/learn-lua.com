Introduction
------------

Metatables in Roblox Lua scripting allow developers to store metadata about data and alter the behavior of data. The primary functions for giving and finding a table's metatable are setmetatable and getmetatable.

Setting a metatable
-------------------

To set a metatable for a table, use the setmetatable function, which takes two arguments: the table and the metatable. The following example shows how to set a metatable for a table called myTable:

    myMetatable = {}
    myTable = {}
    setmetatable(myTable, myMetatable)


Getting a metatable
-------------------

To access the metatable of a table, use the getmetatable function, which takes one argument: the table. The following example shows how to get the metatable of the myTable table:

    myMetatable = getmetatable(myTable)


Metamethods
-----------

In addition to setmetatable and getmetatable, there are other metamethods available for use in metatables. These metamethods can be used to customize the behavior of tables when certain actions are performed on them. Some of the most common metamethods are:

*   index : Determines what should be returned when a key is accessed on a table that does not exist.
*   newindex : Determines what should be done with the value when a key is set on a table that does not exist.
*   add : Determines what should be returned when the addition operator (+) is used on two tables.
*   sub : Determines what should be returned when the subtraction operator (-) is used on two tables.
*   mul : Determines what should be returned when the multiplication operator (*) is used on two tables.
*   div : Determines what should be returned when the division operator (/) is used on two tables.
*   mod : Determines what should be returned when the modulo operator (%) is used on two tables.
*   unm : Determines what should be returned when the unary minus operator (-) is used on a table.
*   concat : Determines what should be returned when the concatenation operator (..) is used on two tables.
*   len : Determines what should be returned when a the length of the table (using #table) is called
