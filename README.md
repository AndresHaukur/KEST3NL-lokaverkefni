# KEST3NL-lokaverkefni
Lokaverkefni í áfanganum KEST3NL í Tækniskólanum

# Things to do

- [x] Install and configure the server1, client1 and client2 with hostnames and domain as ddp.is.
The FQDN will be (server1.ddp.is) for server1, client1.ddp.is for client1 and client2.ddp.is for
client2.
- [ ] configure the server1 with static IP Address, from the IP Address block 192.168.100.0/24.
The server must be configured with the last usable IP Address.
- [ ] Install and configure DHCP on server1, so both clients get an IPv4 Addresses, Gateway,
DNS IP address and domain name automatically from HDCP.
- [ ] Install and configure DNS server on server1, so Hostnames are resolved to IP Addresses.
- [ ] Create the users accounts using a script, see the Users file.
- [ ] Install and configure MySQL on server1 and create Human Resource database. The
database stores information about employees, employees are identified by their Kinnitala,
firtsname, lastname, email, phone number, hire date and salary. Employees work in
departments each department has one manager, departments are identified by department
ID, department name. Each department is in different location. Locations are identified by
their location ID, city, address and zip code. One or more employees’ woks on different jobs,
and the jobs are identified by job ID, job title, min salary and max salary.
- [ ] Due to data loss the company policy requires taking backups weekly, as system engineer
you are required to schedule backups of home directories to run weekly at midnight each
Friday. (use cron)
- [ ] Install and configure NTP on the server and both clients, server1 must be master and clients
must synchronize the time from the server.
- [ ] install and configure syslog server on server1, server1 should get logs from both clients for
proactive management and monitoring. (user rsyslog)
- [ ] Install and configure Postfix on server1, so users can send and receive emails using
Roundcube open source software.
- [ ] Install and configure shared printers for each group, only users that belong the group should
print only, accept IT and Management groups should print and manage the printers. (Use
CUPS)
- [ ] For security reasons, install and configure SSH on the server and clients, SSH login should
use RSA keys instead of the password authentication.
- [ ] All unused ports should be closed, use NMAP for testing.

# Report

1. on server1 
``` 
sudo hostnamectl set-hostname server1.ddp.is 
```
on client1 
``` 
sudo hostnamectl set-hostname client1.ddp.is 
```
on client2 
``` 
sudo hostnamectl set-hostname client2.ddp.is 
```
These commands are used to set the hostnames for the appropriate devices

