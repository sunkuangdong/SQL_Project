## Just insert base

## insert a value to a table

```
INSERT INTO employees (name, salary) VALUES ('Bob', 1000);
```

## Add

#### add a column of bonus to a table
```sql
ALTER TABLE employees ADD COLUMN bonus NUMERIC DEFAULT 0;
```
![alt text](image.png)

## add and select 
`salary + nouns AS annual_salary`
```sql
SELECT salary + nouns AS annual_salary FROM employees;
```
![alt text](image-1.png)

## Update

#### update a column of bonus to a table
```sql
UPDATE employees SET bonus = 2000 WHERE name = 'Bob';
```

#### update key 
`update the key of a table`
```sql
ALTER TABLE employees RENAME COLUMN name TO first_name;
```

## Insert

#### insert a value to a table
```sql
INSERT INTO employees(name, position, salary, nouns, annual_salary, create_date) VALUES ('Alan', 'Manger', 300000, 20000, 320000, NOW());
```

## Delete

#### delete a value from a table
```sql
DELETE FROM employees WHERE name = 'Alan';
```

#### delete all values from a table
```sql
DELETE FROM employees;
```
#### truncate a table
```sql
TRUNCATE TABLE employees;
```
`truncate is faster than delete because it doesn't log the deleted rows. You can't rollback and flashback a truncate.`
