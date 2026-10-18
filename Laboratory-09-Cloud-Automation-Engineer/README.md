# Mission Overview

This laboratory activity focuses on automating cloud operations using Bash scripting and Cron. I created a test application directory, developed a script to compress and back up the data, and configured a scheduled task to automate the backup process.

### Objectives

- Understand the basic syntax of Bash scripting.
- Create and execute a backup script.
- Use Linux file permissions to make a script executable.
- Configure a Cron job to schedule an automatic task.
- Document the process using Markdown.

### Commands Executed

mkdir app-data
echo "This is critical client data." > app-data/data.txt
ls app-data
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e

### Skills Learned

Through this activity, I learned how to write a Bash script, create compressed backups, change file permissions, and schedule automatic tasks using Cron. I also practiced documenting technical procedures and organizing screenshots in my GitHub portfolio.

