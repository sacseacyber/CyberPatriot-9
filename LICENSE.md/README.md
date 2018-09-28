# CyberPatriot
Checklists for AFA CyberPatriot (Open Division)

Ctrl + Alt + T to open the terminal.
//Anything in Bold is command lines needed to be typed into the terminal.
//Anything in Italic is lines needed to be added/modified in txt files. 
Type in sudo passwd root to change the password for root.
You need to type in the password of the user you are on first in order to set up a new root password.
Type in su, hit enter and type in the password you just set.
Now you are in root mode in the terminal.
Type in passwd (username) for all the administrators to change their password to something complicated.
Type in the following lines (Read the readme first for critical services - if it is listed than don’t purge it):
Apt-get purge john -y
Apt-get purge hydra -y
Apt-get purge telnet -y
Apt-get purge vsftpd -y
Set your terminal aside
Open System setting from the top right corner and goto update settings.
Check every checkbox in all the tabs and turn on automatic updates checking.
Go back to your terminal
Type in apt-get update (hit enter and wait for 10 years)
Type in apt-get upgrade (hit enter and set it aside)

Set the terminal aside and open up forensics question(s).
Answer forensics questions. (use google if don’t know how to find answers)
Open the readme and add/delete users as well as set users to administrator or standard.
While one terminal is taking 10 years to update/upgrade the system, open another terminal
Type in su and hit enter, type in the password for root to goto root mode.
Type in gedit /etc/lightdm/lightdm.conf and hit enter.
At the bottom of the txt file popped up, add line: allow-guest=false
Hit Ctrl+s to save the file and close it.
Type in gedit /etc/ssh/sshd_config and hit enter
Goto where it says Permitrootlogin, change the yes to no.
Hit Ctrl+s to save the file and close it.
Type in ufw enable in the terminal.
Look for .mp3/.mp4/.jpg files in the computer system.
Delete them all.
Sit back and relax.
After 10 years the upgrade/update are done, go home and sleep.
Theoretically, if you do all the above step by step, you will get 100 out of 100 in the first round. I don’t remember the difficulty of the second round but the above should be good for 80-90 points. However, remember to do the above step by step because ubuntu will act weirdly if you do those out of order.
