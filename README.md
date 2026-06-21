# MariaDB Backup Automation Project

## Project Overview
This project demonstrates automated database backup using MariaDB, Bash scripting, and Cron jobs on Linux.

## Technologies Used
- Linux
- MariaDB
- Bash Scripting
- Cron Job

## Project Tasks Performed
- Created MariaDB database (serverdb)
- Created employee table
- Inserted sample data into the table
- Performed database backup using mysqldump
- Created Bash script for backup automation
- Generated timestamp-based backup files
- Configured Cron job for scheduled daily backups

## Commands Used

### Create Database
```sql
CREATE DATABASE serverdb;
```

### Create Table
```sql
CREATE TABLE employee (
    id INT PRIMARY KEY,
    name VARCHAR(50)
);
```

### Verify Data
```sql
SELECT * FROM employee;
```

### Manual Backup
```bash
mysqldump -u root -p serverdb > ~/db_backup/serverdb_backup.sql
```

## Backup Automation
A Bash script was created to automate database backups and generate timestamp-based backup files.

## Cron Job Configuration
```bash
0 1 * * * /root/mariadb-backup-project/backup.sh
```

This Cron job runs daily at 1:00 AM and automatically creates a database backup.

## Skills Demonstrated
- Linux Administration
- MariaDB Administration
- Bash Scripting
- Database Backup and Recovery
- Cron Job Scheduling

## Screenshots
Project screenshots are available in the screenshots folder.
