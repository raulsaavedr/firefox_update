# firefox_update

This script help you to install an update your firefox on debian GNU linux.
If you have problems updating your firefox on debian this is your script.
Features:
1) Automatically detects the system core (32bits or 64bits)
2) Works for install and for update 
3) Automatic detection of firefox versions

# How to use

For use the script execute in a bash shell <code>./check_firefox</code> or <code>source check_firefox</code> 

# Automatic updates

To automatically check and install the new Firefox version, the script could be added as a weekly Cron job.

<code>touch /etc/cron.weekly/check_firefox</code>

<code>chmod 755 /etc/cron.weekly/check_firefox</code>

# Firefox language version

You may change the Firefox language version from default US for example to French:

<code>sed -i "s/en-US/fr/g" /etc/cron.weekly/check_firefox</code>

All Firefox language versions are listed here: https://ftp.mozilla.org/pub/firefox/releases/latest/README.txt
