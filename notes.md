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
## Nikto
## WPscan
After discovering there was a webserver running on the target machine, this meant we could use wpscan. After running the scan, we were able to find *office.paper* which could be added to the etc/hosts file. 

URL: http:office.paper 
Looking around the webpage



Chat app:
After doing further enumeration against the site, we came across a link that gave us access to a chat app. Once creating an account, we came across a bot that had very basic terminal commands such as listing files, showing their contents, etc. We used directory traversal techniques in order to break out of the chat app directory. This meant we could find the directory of the chat app which revealed the version and login credentials. These login credentials were used to SSH into the box.
# Initial Access
## SSH into the box
After gaining access to the box, straight away we could grab the *user.txt* file whihc is the user flag. 

# Privilege escalation
## Using linpeas to find priv esc vulnerabilites















