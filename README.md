# backups
> Repository for personal backup purposes

The goal is to backup the data I have in various cloud providers to (another) cloud provider for redundancy and protection against disasters / account lockouts / bans etc.

Providers:
1. Dropbox (source)
2. Google Drive (source)
3. Rsync.net (Destination)
4. Backblaze B2 (Destination)

Tools:
1. Rclone - To sync from sources to Rsync.net
2. Restic - To backup from Rsync.net to B2
3. Github Actions - Control the flow, cron runner to ssh into Rsync.net

In this way, data does not flow through my personal computer with its' limited bandwidth.
