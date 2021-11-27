# Check which packages are installed, Ubuntu
apt list --installed 

# List upgradable packages
apt list --upgradable

```
apt actually works on a database of available packages. If the database is not updated, the system won’t know if there are any newer packages available. This is why updating the repository should be the first thing to do in in any Linux system after a fresh install.
Updating the package database requires superuser privileges so you’ll need to use sudo.
```

sudo apt update

# See the content of a package
apt show <package_name>

# List all the packages available for your system:
apt list --all-versions

# List info about an installed packe
apt list --installed <package_name>
- example, 
apt list --installed openssl

# install a packge
sudo apt install <package_name>

# remove a package
sudo apt remove <package_name>

# Links 
https://itsfoss.com/apt-command-guide/

# examples

In this example, the openssl package was updated from 1.1.1f-1ubuntu2.8 to 1.1.1f-1ubuntu2.9
```
blevine@ubuntu20vm:~$ apt list --installed openssl
Listing... Done
openssl/focal-security,now 1.1.1f-1ubuntu2.8 amd64 [installed,upgradable to: 1.1.1f-1ubuntu2.9]
N: There is 1 additional version. Please use the '-a' switch to see it
```

```
blevine@ubuntu20vm:~$ sudo apt install openssl
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages will be upgraded:
  openssl
1 upgraded, 0 newly installed, 0 to remove and 41 not upgraded.
Need to get 622 kB of archives.
After this operation, 0 B of additional disk space will be used.
Get:1 http://us.archive.ubuntu.com/ubuntu focal-updates/main amd64 openssl amd64 1.1.1f-1ubuntu2.9 [622 kB]
Fetched 622 kB in 1s (733 kB/s) 
(Reading database ... 71512 files and directories currently installed.)
Preparing to unpack .../openssl_1.1.1f-1ubuntu2.9_amd64.deb ...
Unpacking openssl (1.1.1f-1ubuntu2.9) over (1.1.1f-1ubuntu2.8) ...
Setting up openssl (1.1.1f-1ubuntu2.9) ...
Processing triggers for man-db (2.9.1-1) ...
```

```
blevine@ubuntu20vm:~$  apt list --installed openssl
Listing... Done
openssl/focal-updates,now 1.1.1f-1ubuntu2.9 amd64 [installed,automatic]
N: There are 2 additional versions. Please use the '-a' switch to see them.
```
---
# Sending output to Syslog... might want to do this just to have a record of things you do, to save information between sessions, etc. 
use logger command. example,


$ echo "hello world" | logger
Nov 26 17:23:52 ubuntu20vm blevine: hello world

$ logger -t mylogz "It's jean!"
Nov 26 17:24:56 ubuntu20vm mylogz: It's jean!

use -s tag to echo output to stdout and to the syslog

$ logger -t mylogz -s "What the heck d'ya'mean?"
<13>Nov 26 17:26:27 mylogz: What the heck d'ya'mean?

Run a command and copy output to the console and to syslog,
cat .bashrc | logger -s

Nov 26 17:29:19 ubuntu20vm blevine: # ~/.bashrc: executed by bash(1) for non-login shells.
Nov 26 17:29:19 ubuntu20vm blevine: # see /usr/share/doc/bash/examples/startup-files (in the package bash-doc)
Nov 26 17:29:19 ubuntu20vm blevine: # for examples


#Links
https://www.urbanautomaton.com/blog/2014/09/09/redirecting-bash-script-output-to-syslog/
https://ubuntu.com/tutorials/viewing-and-monitoring-log-files#2-log-files-locations

