Using ansible templates, update the ntp server details with following in remote hosts.
server 0.asia.pool.ntp.org
server 1.asia.pool.ntp.org
server 2.asia.pool.ntp.org
server 3.asia.pool.ntp.org



In this assignment first of all NTP package is installed in the remote server 'CentOS' with the name 'Chrony'. it is started and enabled. Soon after NTP configuration are deployed from the templates directory where 'ntp.conf.j2' is present as a configuration file. and soon after the chronyd service is restarted.


'ntp.conf.j2' file contain the configuration for ntpd .
