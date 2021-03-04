# Read: 14a - DB Normalization

# Database Normalization
- limit tables to one purpose
- this helps with:
  - duplicate data
  - to not have to modify table later
  - make queries easier
### duplicate data
- wastes memory, lowers performance
- more cumbersome to maintain
- difficult to add changes
### Modification Anomolies
- insert issues, whats minimum data for an insert?
- Having to alter duplicated data in all its locations
- Deleteing items removes useful data since it is tied to other elements
### Search and Sort
- If needed data can live in multiple locations search queries are inherently less effecient
- sort by becomes an issue
### Normalize
- "First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key"

