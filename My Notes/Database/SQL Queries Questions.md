
---
### There is a table Person. Gender is column male or female. WAQ to make male as female and female as male.

```sql
UPDATE Person
SET Gender = CASE 
                WHEN Gender = 'Male' THEN 'Female'
                WHEN Gender = 'Female' THEN 'Male'
                ELSE Gender
             END;
```

---
