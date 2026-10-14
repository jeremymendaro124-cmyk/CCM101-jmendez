# Backup Script Guide

## 1. Purpose

The `backup.sh` script automates the process of creating compressed backups of the `app-data` directory. It generates a timestamped `.tar.gz` archive inside the `backups` directory so that multiple backup files can be stored separately.

## 2. Full Backup Script

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball (.tar.gz)
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. File Permissions

Command:

```bash
chmod +x backup.sh
```

The `chmod +x` command adds execute permission to the script, allowing it to be run directly using `./backup.sh`.

## 4. Cron Job Configuration

Cron expression:

```cron
0 2 * * * /root/backup.sh
```

This expression schedules the backup script to run every day at 2:00 AM, using the server's configured timezone.

### Breakdown of the Five Time Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Runs at minute zero. |
| Hour | `2` | Runs at 2 AM. |
| Day of Month | `*` | Runs every day of the month. |
| Month | `*` | Runs every month. |
| Day of Week | `*` | Runs every day of the week. |

The final part, `/root/backup.sh`, specifies the absolute path to the script that cron will execute.

