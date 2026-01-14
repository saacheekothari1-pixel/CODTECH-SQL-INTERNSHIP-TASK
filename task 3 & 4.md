TASK 3 – DATABASE MIGRATION
-- Migration Steps (Written Explanation)

-- Step 1: Export MySQL Database
mysqldump -u root -p old_db > backup.sql

-- Step 2: Create PostgreSQL Database
createdb new_db

-- Step 3: Import Data
psql -U postgres new_db < backup.sql

------------------------------------------------------------------------------------------------------------------------------

TASK 4 – BACKUP & RESTORE
-- Backup
mysqldump -u root -p database_name > backup.sql

-- Restore
mysql -u root -p database_name < backup.sql
