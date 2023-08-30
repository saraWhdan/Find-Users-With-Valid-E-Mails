# Find-Users-With-Valid-E-Mails
## Problem Link:
[Find Users With Valid E-Mails](https://leetcode.com/problems/find-users-with-valid-e-mails/description/?envType=study-plan-v2&envId=top-sql-50)
## solution:
```sql
SELECT *
FROM Users
WHERE mail LIKE '[A-Za-z]%@leetcode.com'
  AND mail NOT LIKE '%[^a-z0-9._-]%@leetcode.com'
