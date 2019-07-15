# cron_cpanel_backup
Perform a full cPanel backup, then move it to the /backup location for cPanel servers.

Change the 'USER' variable to be the username of the cPanel account that is to be backed up.  From there, schedule the script via  Root CRON job so that there are effective permissions to make sure all processes are completed correctly.

Installation:

1. Download the cpanel_cron script:
    
    wget -O ./cpanel_cron https://raw.githubusercontent.com/Hummdis/cron_cpanel_backup/master/cpanel_cron
    
2. Edit the file and change the username to the username that you want the actual backup job to run for.
3. Make the file executable:
    
    chmod +x ./cpanel_cron
    
4. Edit the Root crontab file to make this script run at the times desired.
    
    crontab -e
    
The reason you want to run it as Root is to ensure that the script has all of the needed access to avoid failures.
