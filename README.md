# zip_crack
zip_crack is a file password recovery tool and Linux shadow file cracker. 
It uses the dictionary search or Brute force method for cracking passwords.
## Supported Files
*	RAR Files
*	Legacy ZIP Files
*	PDF Files
*	Linux Shadow Files (zydra can find all the user’s password in the linux shadow file one after the other)
## Prerequisites
To run the app, minimal requirements are:
*	Python 3.3 or higher
*	debian-based linux distro, preferably Kali linux 2
*	**qpdf** and **unrar** packages<br /> Installing these packages on kali is as easy as running the following commands on terminal:
<br />```$ apt-get update```
<br />```$  apt-get upgrade -y```
<br />```$ termux-setup-storage```https://github.com/Noobhacker0077/zip_crk.git
<br />```$ git clone https://github.com/Noobhacker0077/zip_crk.git
*	some python modules in this program need to be installed manually, like:
zipfile, rarfile, crypt, pyfiglet, py-term(for term module) and so on.
you can use pip3 for install them
example: <br />```$ pip3 install py-term```
<br />**notice**: rar,zip and pdf files must have an extension, shadow files does not need an extension.
*   Install figlet font "epic" if it does not exists on your system:
<br/> ```sudo wget http://www.figlet.org/fonts/epic.flf -O /usr/share/figlet/epic.flf```
## Disclaimer
This tool is only for testing and academic purposes Do not use it for illegal purposes!
## Features
*	Cracking files password using two methods:  **1.** dictionary method **2.** brute force method
*	In the brute force method, you can specify the min length and max length of the passwords.
*	 In the brute force method, you can specify the type of characters that may be used in the password.
*	There is a percent progress bar showing how much of the process has been performed.
*	Error handling.
*	One of the most important features of Zydra is the multiprocessing feature that speeds up the program. For example if you have 8 CPU cores, zip_crk will use all of them for processing at the same time.
## Installation
## Examples
**1- Dictionary search to find the password for a zip file**
<br />In this example I use rockyou.txt dictionary
<br /><br />```$ python3 zc.py –f file.zip –d rockyou.txt```
 
**2- Brute force search to find the password for the users in the shadow file**
<br />Minimum length of password is 4 and maximum length is 4 and we try to find passwords that are composed of numbers and symbols letters.
<br /><br />```$ python3 zc.py –f shadow –b digits,symbols –m 4 –x 4```<br /><br />
 		

