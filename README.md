# cron_cpanel_backup
Perform a full cPanel backup, then move it to the /backup location for cPanel servers.

Change the 'USER' variable to be the username of the cPanel account that is to be backed up.  From there, schedule the script via  Root CRON job so that there are effective permissions to make sure all processes are completed correctly.
