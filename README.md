# zimbra_lockoutd
This is a monitoring daemon for Zimbra. It has been tested with Zimbra NE 8.6 on Ubuntu 14.04

It monitors the server logs, and will send an alert email if a user account goes into lockout mode.

To get it to start on boot, I added the contents of the file ADD_TO_crontab to the end of the server's /etc/crontab 
