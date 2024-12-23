## Select base (select and where)

#### select all user in a table
`employees is a table name`
```sql
SELECT * FROM employees; 
```

#### just select id in a table

```sql
SELECT id FROM employees; 
```
![alt text](image.png)

#### select a user in a table (select and where)
`To use 'select' and 'where' to select a user in a table`
```sql
SELECT * FROM employees WHERE name = 'Bob';
```
![alt text](image-1.png)

`To use 'select', 'where' and 'between' to select a user in a table`
```sql
SELECT * FROM employees WHERE salary BETWEEN 1000 AND 0000;
```
![alt text](image-2.png)

#### select and where (or, and, not, NULL)

`To use 'select', 'where' and 'or' to select a user in a table`
```sql
SELECT * FROM employees WHERE salary BETWEEN 1000 AND 0000 OR salary BETWEEN 1000 AND 0000;
```

`To use 'select', 'where' and 'and' to select a user in a table`
```sql  
SELECT * FROM employees WHERE salary BETWEEN 1000 AND 0000 AND salary BETWEEN 1000 AND 0000;
```

`To use 'select', 'where' and 'not' to select a user in a table`
```sql
SELECT * FROM employees WHERE salary BETWEEN 1000 AND 0000 AND salary BETWEEN 1000 AND 0000;
```

#### how to select a value of NULL in a table
`To use 'select', 'where' to select a value of NULL in a table`
```sql
SELECT * FROM employees WHERE salary IS NULL;
```
![alt text](image-3.png)

#### how to use 'in' to select a value in a table
`To use 'select', 'where' and 'in' to select a value in a table`
```sql
SELECT * FROM employees WHERE id IN (1, 2);
```
![alt text](image-4.png)

#### how to use 'like' to select a value in a table
`To use 'select', 'where' and 'like' to select a value in a table`
```sql
SELECT * FROM employees WHERE name LIKE '%Bob%';
```
`note: like is fuzzy matching, % is a wildcard character`
![alt text](image-5.png)

