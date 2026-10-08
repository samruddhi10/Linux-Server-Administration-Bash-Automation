# Linux-Server-Administration-Bash-Automation
Linux Server Administration &amp; Bash Automation

                    INTERNET
                       │
                ┌──────┴──────┐
                │             │
              SSH :22       HTTP :80
                │             │
                └──────┬──────┘
                       ↓
              ┌─────────────────┐
              │    AWS EC2      │
              │ Ubuntu Server   │
              └────────┬────────┘
                       │
       ┌───────────────┼────────────────┐
       ↓               ↓                ↓
   Linux Admin       Nginx         Bash Automation
       │               │                │
       │               ↓          ┌─────┴─────┐
       │           Web Application │           │
       │                           ↓           ↓
       │                      Health Check   Backup
       │                           │           │
       ↓                           ↓           ↓
   systemd                     Cron Jobs    Logs
       │
       ↓
   Services
