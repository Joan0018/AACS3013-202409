## Normalisation

### 1NF
- Identify repeating Group
- One table with 2 primary keys
- Special case happens if we have date in the table then 3 primary keys in 1NF

### 2NF (‼️MUST have an associative entity‼️) 
- One table with one primary key
- One table with one primary key
- One table with a composite key (associative entity) (PK and FK together) – Special case happens if there is any date in the associative entity we need to assign as the primary key.

### 3NF
- Further separate the table from 2NF
- Check for any table that contains an ID which is not the primary key, which means you need to move it to another table.
- Remember to assign the FK to the existing table (from where you remove the column)
