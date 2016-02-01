# zimbra_lockoutd
This is a monitoring daemon for Zimbra. It has been tested with Zimbra NE 8.6 on Ubuntu 14.04

It monitors the server logs, and will send an alert email if a user account goes into lockout mode.

To get it to start on boot, I added the following line to the server's /etc/crontab 

# start email lockout report on boot
@reboot root /root/bin/lockout_report
