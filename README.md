# INTRO
A set of OSINT commands all in one script. Saves results to files for further processing as necessary.
Includes passive scanning using Nmap. Essential to run these through TL-OSINT in VirtualBox.
See https://www.tracelabs.org/initiatives/osint-vm and how to install TL-OSINT.
You can also use these scripts in Kali Linux. Any other Linux version will not have the necessary dependencies.
Written by Nathan Jones nathan.jones@arcadeusops.com 

# INSTALLATION
git clone https://github.com/ArcadeusOPS/OSINT.git
cd OSINT
sudo chmod 777 *.sh
sudo ./install.sh
rm install.sh

NOTE: Make sure that torrc is configured to SOCKS_PORT localhost:9050

# Scripts
install.sh installs a few extras.
up.sh updates the base, installed TL-OSINT OS.
osint.sh runs the scripts and saves output to local storage. Follow the instruction in the osint.sh file comments.

# SSH
Use port 1965 or higher if you want to be extra security minded. Use UFW firewall.

# SECURITY
You can install Lynis, ufw, apparmor, artillery, fail2ban - for added security.
Run Lynis and follow the recommendations.

# USAGE
./osint.sh userIP uport udir uname umail wlan - as single command line argument but can use website instead of IP address e.g. google.com for 8.8.8.8.
See install.sh for notes.

# TO DO
Collate all output to a single XML or HTML file and email to designated user.

# Bugs
Send issues to info@arcadeusops.com stating nature of issue. A screenshot will help too. Thanks.
