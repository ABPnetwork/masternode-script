![Example-Logo](https://abpnetwork.io/img/abp-logo.png)
# ABP Network Masternode Setup Guide (Ubuntu 16.04)
This guide will assist you in setting up a ABP Network Masternode on a Linux Server running Ubuntu 16.04. (Use at your own risk)

If you require further assistance contact us @ [Discord](https://discord.gg/MDyb4K3)
***
## Requirements
1) **1,000 ABP Network coins.**
2) **A VPS (Vultr) running Linux Ubuntu 16.04.**
3) **A Windows or MAC OS X local wallet.**
4) **An SSH client**
***
## Contents
* **Section A**: Creating the VPS within [Vultr](https://www.vultr.com/?ref=7296974).
* **Section B**: How to Install an SSH Client and Connect to an SSH Server on Windows
* **Section C**: Connecting to the VPS and installing the MN script via CMDER.
* **Section D**: Preparing the local wallet.
* **Section E**: Connecting & starting the masternode.
***

## Section A: Creating the VPS within [Vultr](https://www.vultr.com/?ref=7296974) 
***Step 1***
Register at [Vultr](https://www.vultr.com/?ref=7296974)
***

***Step 2***
After you have added funds to your account go [here](https://my.vultr.com/deploy/) to create your Server
***

***Step 3*** 
Choose a server location (preferably somewhere close to you)
![vultr-server-location](https://coinlabs.cc/content/images/2018/05/vultr-server-location.png)
***

***Step 4***
Choose a server type: Ubuntu 16.04
![vultr-server-type](https://coinlabs.cc/content/images/2018/05/vultr-server-type.png)
***

***Step 5***
Choose a server size: $5/mo will be fine 
![vultr-server-size](https://coinlabs.cc/content/images/2018/05/vultr-server-size.png)
***

***Step 6*** 
Set a Server Hostname & Label (name it whatever you want)
![vultr-server-hostname-label](https://coinlabs.cc/content/images/2018/05/vultr-server-hostname-label.png)
***

***Step 7***
Click "Deploy now"
![vultr-deploy-now](https://coinlabs.cc/content/images/2018/05/vultr-deploy-now.png)
***


## Section B: How to Install an SSH Client and Connect to an SSH Server on Windows 

## Contents
**A**: Downloading and installing Cmder terminal.
**B**: Connecting to the VPS.
***

## A. Downloading and Installing Cmder Terminal. 

***Step 1***
Download Cmder terminal [here](https://github.com/cmderdev/cmder/releases/download/v1.3.6/cmder.zip)
***

***Step 2***
Select the ***Download Now*** button Then follow the installation instructions. 

![cmder-installation](https://coinlabs.cc/content/images/2018/05/cmder-installation.png)
***

***Step 3***
After running Cmder.exe, a prompt should pop up asking you to either Extract All or Run. Press Extract all first.

![extract-all-example](https://coinlabs.cc/content/images/2018/05/extract-all-example.png)
***

***Step 4***
After pressing extract-all, you will be prompted to press extract. Go ahead!
***

***Step 5***
Once you have done extracting, you will to run Cmder.exe again, and press Unblock and Continue to get it to run.

![unblock-and-continue-example](https://coinlabs.cc/content/images/2018/05/unblock-and-continue-example.png)
***

***Step 6***
The Cmder terminal should be open after, and look similar to this.

![example-cmder](https://coinlabs.cc/content/images/2018/05/example-cmder.png)
***

***Warning!***
You will need to keep the Cmder application in its new folder, once everything is done above. Please delete the first Cmder folder, and keep the one generated. Always open Cmder from that folder to avoid any errors when starting the application up.

## B. Connecting to the VPS.

***Step 1***
Copy your VPS IP (you can find this by going to the server tab within Vultr and clicking on your server. 

![vultr-copy-address](https://coinlabs.cc/content/images/2018/05/vultr-copy-address.png)
***

***Step 2***
Open the Cmder terminal and type the following `ssh root@YOURVPSIPADDRESS`

![example-connect-to-vps](https://coinlabs.cc/content/images/2018/05/example-connect-to-vps.png)
***

***Step 3*** 
Once you press enter, it will prompt a security alert (type yes).  

![example-prompt](https://coinlabs.cc/content/images/2018/05/example-prompt.png)
***


***Step 4***
Then you will be asked to enter your password, so navigate back to Vultr and click on your server and copy your root's password. 

![example-vultr-password](https://coinlabs.cc/content/images/2018/05/example-vultr-password.png)
***

***Step 5***
Once you have copied the password, paste it into Cmder terminal and press enter.

![example-enter-password](https://coinlabs.cc/content/images/2018/05/example-enter-password.png)
***


## Section C: Installing the MN script via Terminal.

**Step 1***

Paste the code below into the terminal then press enter (it will just go to a new line)

`wget -q https://github.com/ABPnetwork/ABP/releases/`
***

***Step 8***
* Paste the code below into the putty terminal then press enter

`bash ABP Network_install.sh`

![Example-Bash](https://i.imgur.com/Ktythm3.png)

***

***Step 9***
* Sit back and wait for the install (this will take 10-20 mins)
***

***Step 10***
* When prompted to enter your private key - press enter

![Example-installing](https://i.imgur.com/Ps5UPU8.png)
***
