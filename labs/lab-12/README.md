Lab 12: Backup and Recovery
Objective

To ensure that you can back up and restore Nginx configuration and website data in case of accidental deletion, corruption, or server migration.

Task 12.1: Backup Nginx Configuration

Create a backup directory:

mkdir -p ~/nginx-backups/config


Copy the Nginx configuration files:

sudo cp -r /etc/nginx/* ~/nginx-backups/config/


Compress the backup:

tar -czvf nginx-config-backup.tar.gz ~/nginx-backups/config

Task 12.2: Backup Website Files

Backup all website data:

mkdir -p ~/nginx-backups/websites
sudo cp -r /var/www/* ~/nginx-backups/websites/


Compress:

tar -czvf nginx-websites-backup.tar.gz ~/nginx-backups/websites

Task 12.3: Automate Backups with Cron

Open cron editor:

crontab -e


Add a daily backup job at midnight:

0 0 * * * tar -czf ~/nginx-backups/nginx-config-$(date +\%F).tar.gz /etc/nginx && tar -czf ~/nginx-backups/nginx-websites-$(date +\%F).tar.gz /var/www

Task 12.4: Test Recovery

Simulate data loss (careful—only if you have backups):

sudo rm -rf /etc/nginx
sudo rm -rf /var/www


Restore from backup:

sudo tar -xzvf ~/nginx-backups/nginx-config-backup.tar.gz -C /
sudo tar -xzvf ~/nginx-backups/nginx-websites-backup.tar.gz -C /


Restart Nginx:

sudo systemctl restart nginx
