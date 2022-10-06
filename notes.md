# Paper Hack the Box notes
This will contain all my notes during this hack the box exercise.

Prerequisites:
- I have connected to the hack the box vpn service
- The *Paper* machine is up and running.
- Have my note taking workflow ready



# Initial Recon
## NMAP:
**First Scan**
The first NMAP scan, we were able to find 3 ports were open (22,80 and 443). This meant we could look at the webpage being hosted.







nikto
wpscan
After discovering there was a webserver running on the target machine, this meant we could use wpscan. After running the scan, we were able to find *office.paper* which could be added to the etc/hosts file. 

URL: http:office.paper 



Chat app:
After doping further enumeration against the site, we came across a