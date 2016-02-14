# diesel-tools
Game Master tools for the forum game Era of Diesel.

docs/eod-data-model.txt
-----------------------

This file contains a conceptual data model for the game Era of Diesel.
The types of data that GM tools would have to deal with are represented
as relations. A data types is associated with another type by including
the primary key attribute(s) of the associated type as a foreign key.

docs/eod-ext-data-model.txt
---------------------------

This file describes a general text file syntax for table-structured data.
The syntax is designed to be conveniently readable and writable for both
humans and machines.

This file also contains a model for the data files that GM tools for Era
of Diesel might use. Each data file contains a number of tables and
matrices, some of which may be optional.

Each table contains a number of records (rows), which contain named fields
(columns). Table records may have implicit fields, which may be derived
from the name of the data file, records in preceding tables or the command
line arguments of the GM tool.

Matrices are special tables that are used to compactly represent
many-to-many relationships. Each matrix associates specific values with
specific combinations of a row key and a column key.

docs/eod-ext-data-example.txt
-----------------------------

This file contains examples of the tables and matrices that may be used
in data files for Era of Diesel. Some of the tables will probably have
a much greater number of records in practical data files (e.g. the Trait,
Technology and Province tables, the ProvinceLink and Occupancy matrices).

