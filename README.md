ddclient-pace_4111n
===================

Script to get WAN ip address from ATT Pace 4111n router for use with ddclient.

Clone repository and copy script to `/etc/ddclient/get_wan_ip` (or wherever.)

Edit script and config as necessary (IP address.)

Test script - no need to run as root and you should see your WAN ip address.

ddclient example setup using freedns.afraid.org:
```
daemon=60s
timeout=10
ssl=yes
use=cmd, cmd=/etc/ddclient/get_wan_ip
protocol=freedns
server=freedns.afraid.org
login=<your_login>
password=<your_password>
<your_ddns_hostname>
```
