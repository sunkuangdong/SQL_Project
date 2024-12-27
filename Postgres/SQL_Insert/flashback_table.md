## Flashback

`flashback is a feature that allows you to restore a table to its previous state.`

#### flashback a table
```sql
CREATE TABLE employees_backup AS SELECT * FROM employees;
DROP TABLE employees;
SELECT * FROM employees_backup;
SHOW recyclebin;
FLASHBACK TABLE employees TO BEFORE DROP;
```

`If we use drop table xxx purge, we can't flashback the table.`
