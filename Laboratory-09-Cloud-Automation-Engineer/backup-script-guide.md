# Backup Script Guide

### 1. Backup Script

The following Bash script creates a compressed backup of the application data directory.

#!/bin/bash

# Automated Backup Script for CloudNova Technologies
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

mkdir -p "$BACKUP_DIR"

tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"

### 2. File Permissions

The command "chmod +x backup.sh" gives the script executable permission. This allows the user to run the script directly using "./backup.sh", provided the other execution requirements are satisfied.

### 3. Cron Job Configuration

The Cron expression used is:

0 2 * * * /root/backup.sh

Explanation of the Five Time Fields

Field| Value| Explanation
Minute| "0"| Runs at minute zero.
Hour| "2"| Runs at 2 AM.
Day of Month| "*"| Runs every day of the month.
Month| "*"| Runs every month.
Day of Week| "*"| Runs every day of the week.

The command schedules the backup script to run every day at 2:00 AM, according to the system's local time.

### 4. Verification

I tested the script by executing "./backup.sh" and checking the contents of the "backups" directory with "ls -l backups/". I also verified the scheduled task using "crontab -l".

### 5. Screenshots

- "screenshots/script-execution.png" — Evidence of the script execution and generated backup file.
- "screenshots/cron-schedule.png" — Evidence of the installed Cron schedule.
