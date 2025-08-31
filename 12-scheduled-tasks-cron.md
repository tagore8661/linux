
# 12. Linux Scheduled Tasks (Cron)

Cron is used to schedule tasks to run automatically at specified times.

## 1. List Cron Jobs
Show current user's cron jobs:
```bash
crontab -l
```

## 2. Edit Cron Jobs
Edit current user's cron jobs:
```bash
crontab -e
```

## 3. Cron Syntax
Format:
```
* * * * * command-to-run
| | | | |
| | | | +----- Day of week (0 - 7)
| | | +------- Month (1 - 12)
| | +--------- Day of month (1 - 31)
| +----------- Hour (0 - 23)
+------------- Minute (0 - 59)
```

## 4. Example Cron Jobs
Run backup every day at 2 AM:
```bash
0 2 * * * /home/user/backup.sh
```
Run script every 5 minutes:
```bash
*/5 * * * * /home/user/script.sh
```

## 5. System-Wide Cron Jobs
- `/etc/crontab` for system jobs
- `/etc/cron.d/` for custom jobs
- `/etc/cron.daily/`, `/etc/cron.hourly/` for periodic jobs

## 6. Remove Cron Jobs
Remove all jobs for current user:
```bash
crontab -r
```

## 7. View Cron Logs
Check cron execution logs:
```bash
sudo tail -f /var/log/cron
```

---

This file covers all major aspects of Linux scheduled tasks and cron jobs. For more, see `man crontab` and `man 5 crontab`.
