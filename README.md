# 🛡️ MySQL Auto Backup Script (Linux)

This script automates the process of backing up a MySQL database and securely transferring the backup to a remote Linux machine over SSH.

## 📂 Files

- `Assign4_backup.sh`: Main backup script
- `Screenshots/`: Folder containing proof of functionality (CLI outputs, transfer success, etc.)

## 🔧 What the Script Does

1. **Creates a backup** of a specified MySQL database using `mysqldump`.
2. **Stores** the backup file locally with a filename that includes the current date.
3. **Transfers** the backup securely to a second virtual machine using `scp`.
4. (Optional) **Deletes the local copy** after transfer to conserve space.

## 🖥️ How to Use

1. Update the script with your:
   - MySQL credentials (`USER`, `PASSWORD`, `DATABASE`)
   - Backup directory
   - Remote machine IP and target directory

2. Make the script executable:
   ```bash
   chmod +x Assign4_backup.sh
