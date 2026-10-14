# Laboratory 09: Cloud Automation Engineer

## Mission Overview

This laboratory focuses on automating server maintenance using Bash scripting and cron jobs. A backup script is created to compress application data into timestamped archives, while cron is configured to schedule the backup process every day at 2:00 AM.

## Objectives

- Understand Bash scripts, variables, and cron jobs.
- Create sample application data for backup testing.
- Develop a Bash script that creates compressed backup archives.
- Configure file permissions using `chmod +x`.
- Schedule automated backups using cron.
- Verify backup files and the installed cron schedule.
- Document the implementation and reflect on cloud automation.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir -p app-data` | Creates the application data directory. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a sample data file. |
| `nano backup.sh` | Creates or edits the Bash script. |
| `./backup.sh` | Executes the backup script. |
| `chmod +x backup.sh` | Grants execute permission. |
| `ls -l backups/` | Lists the generated backup files. |
| `tar -tzf backups/backup_*.tar.gz` | Lists archive contents. |
| `crontab -l` | Displays scheduled cron jobs. |
| `env EDITOR=nano crontab -e` | Opens the cron table for editing. |


## Skills Learned

- Writing and executing Bash scripts.
- Using variables and timestamps in automation.
- Compressing files with the `tar` command.
- Managing execution permissions in Linux.
- Scheduling recurring tasks using cron.
- Verifying backup archives.
- Documenting and organizing cloud computing projects.

