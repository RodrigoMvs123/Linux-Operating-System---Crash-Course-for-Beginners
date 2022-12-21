# Linux-Operating-System---Crash-Course-for-Beginners

https://www.youtube.com/watch?v=ROjZy1WbCIA

Free and Open source
Unix-like Operating System Kernel 
Directly talk to the hardware 
Manage the resources and processes
Linux is not Unix

Course Distribution 
Ubuntu - Debian Based Distro 
Desktop 
Server
Core 

Install Ubuntu 
https://ubuntu.com/download

Direct 
Virtual Machine 
Cloud 

Virtual Box
Type-2 hypervisor 
Can be installed on Windows, macOS, Linux.
Try before you commit 
Newer Hardware that supports virtualization 

https://www.virtualbox.org/wiki/Downloads


Desktop Environment 

Terminal 
Open emulator 
To run a command as administrator ( user “root” ), use “ sudo <command>”.
Josh@utbuntu20:~$ 

Working with Directories 
Josh@utbuntu20:~$ man man
Josh@utbuntu20:~$ man pwd
Josh@utbuntu20:~$ pwd
/home/josh 
Josh@utbuntu20:~$ man cd
No manual entry for cd 
Josh@utbuntu20:~$ cd /home
Josh@utbuntu20:/home$ cd josh/
Josh@utbuntu20:~$ cd /home
Josh@utbuntu20:/home$ cd
Josh@utbuntu20:~$ man ls
Josh@utbuntu20:~$ cd Documents/ ansible-examples/ 
Josh@utbuntu20:~Documents/ ansible-examples$ 
Josh@utbuntu20:~Documents/ ansible-examples$ ls // README.md / .README.md
Josh@utbuntu20:~Documents/ ansible-examples$ ls 
Josh@utbuntu20:~Documents/ ansible-examples$ ls -a 
Josh@utbuntu20:~Documents/ ansible-examples$ clear
Josh@utbuntu20:~Documents/ ansible-examples$ ls 
Josh@utbuntu20:~Documents/ ansible-examples$ ls -l
Josh@utbuntu20:~Documents/ ansible-examples$ ls -la
Josh@utbuntu20:~Documents/ ansible-examples$ ls -lah 
Josh@utbuntu20:~Documents/ ansible-examples$ clear
Josh@utbuntu20:~Documents/ ansible-examples$ cd
Josh@utbuntu20:~$ clear
Josh@utbuntu20:~$ man mkdir 
Josh@utbuntu20:~$ cd Documents/
Josh@utbuntu20:~/Documents$ ls
ansible-exemples 
Josh@utbuntu20:~/Documents$ mkdir Test 
Josh@utbuntu20:~/Documents$ mkdir Test
mkdir: cannot create directory ‘Test’: Files exists 
Josh@utbuntu20:~/Documents$ ls
ansible-examples  Test 
Josh@utbuntu20:~/Documents$ cd Test/
Josh@utbuntu20:~/Documents/Test$ 
Josh@utbuntu20:~/Documents$ mkdir Test2 
Josh@utbuntu20:~/Documents/Test$ ls
Test2
Josh@utbuntu20:~/Documents/Test$ cd
Josh@utbuntu20:~$ cd Documents/  
Josh@utbuntu20:~/Documents$ ls
ansible-examples Test  
Josh@utbuntu20:~/Documents$  mkdir -p Linux/Ubuntu/josh
Josh@utbuntu20:~/Documents$  ls
ansible-exemples Linux Test 
Josh@utbuntu20:~/Documents$  cd Linux/
Josh@utbuntu20:~/Documents/Linux$ ls
Ubuntu 
Josh@utbuntu20:~/Documents/Linux$ cd Ubuntu/
Josh@utbuntu20:~/Documents/Linux/Ubuntu$ ls
Josh
Josh@utbuntu20:~/Documents/Linux/Ubuntu$ clear
Josh@utbuntu20:~/Documents/Linux/Ubuntu$ cd
Josh@utbuntu20:~$ cd Documents/ 
Josh@utbuntu20:~Documents$ ls
ansible-examples Linux Test 
Josh@utbuntu20:~Documents$ man rmdir 
Josh@utbuntu20:~Documents$ cd Test/
Josh@utbuntu20:~Documents/Test$ ls
Test2
Josh@utbuntu20:~Documents/Test$ rmdir Test2 
Josh@utbuntu20:~Documents/Test$ ls 
Josh@utbuntu20:~Documents/Test$ cd
Josh@utbuntu20:~$ cd Documents/ 
Josh@utbuntu20:~/Documents$ ls
ansible-example Linux Test 
Josh@utbuntu20:~/Documents$ rmdir  Linux/
rmdir:failed to remove ‘Linux/’: Directory not empty
Josh@utbuntu20:~/Documents$ rmdir -p Linux/Ubuntu/Josh/
Josh@utbuntu20:~/Documents$ ls 
ansible-exemples Test 
Josh@utbuntu20:~/Documents$ 

Working with Files 
Josh@utbuntu20:~/Documents$ ls
ansible-examples Linux Test
Josh@utbuntu20:~/Documents$ rmdir Linux/ 
rmdir:failed to remove ‘Linux/’: Directory not empty
Josh@utbuntu20:~/Documents$ rmdir -p Linux/Ubuntu/Josh/
Josh@utbuntu20:~/Documents$ ls
ansible-examples Test
Josh@utbuntu20:~/$ man file
Josh@utbuntu20:~/$ cd Documents
ansible–examples Test
Josh@utbuntu20:~/Documents$ cd ansible-examples/
Josh@utbuntu20:~/Documents/ansible-examples$ ls
jboss-standalone mongodb windows…
Josh@utbuntu20:~/Documents/ansible-examples$ cd lamp-haproxy/
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ ls
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ file README.md
README.md :ASCII Text 
Josh@utbuntu20:~/Documents/ansible-exemples/lamp_haproxy$ file rolling_update.yml
rolling_update.yml: ASCII text 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ cd..
Josh@utbuntu20:~/Documents/ansible-examples$ cd mongodb/
group_vars/ images/ playbooks/ roles/ 
Josh@utbuntu20:~/Documents/ansible-examples$ cd mongodb/images
Josh@utbuntu20:~/Documents/ansible-examples/mongodb/images$ ls 
check.png  nosql_primer.png  replica_set.png scale.png sharding.png site.png 
Josh@utbuntu20:~/Documents/ansible-examples/mongodb/images$ file check.png
check.png PNG image data, 1346x1010, 8-bit/color RGBA, non-interlaced 
Josh@utbuntu20:~/Documents/ansible-examples/mongodb/images$ cd
Josh@utbuntu20:~$ clear 

man touch 
Josh@utbuntu20:~$ cd Document 
Josh@utbuntu20:~/Documents$ touch file1.txt 
Josh@utbuntu20:~/Documents$ ls
ansible-examples filed1. txt Test 
Josh@utbuntu20:~/Documents$ touch file2.txt file3.txt 
Josh@utbuntu20:~/Documents$ ls
ansible-example file1.txt file2.txt file3.txt Test 
Josh@utbuntu20:~/Documents$ man rm
Josh@utbuntu20:~/Documents$ rm file1.txt 
Josh@utbuntu20:~/Documents$ ls 
ansible-examples file2.txt file3.txt Test 
Josh@utbuntu20:~/Documents$ rm -i file2.txt file3.txt 
rm: remove regular empty file ‘file2.txt’ ? yes 
rm: remove regular empty file ‘file3.txt’ ? yes 
Josh@utbuntu20:~/Documents$ ls
ansible-example Test 
Josh@utbuntu20:~/Documents$ rm Test/ 
rm: cannot remove ‘Test’ : Is a directory
Josh@utbuntu20:~/Documents$ rm -rf T Test/
Josh@utbuntu20:~/Documents$ ls
ansible-examples 
Josh@utbuntu20:~/Documents$ mkdir test 
Josh@utbuntu20:~/Documents$ ls
ansible-example Test 
Josh@utbuntu20:~/Documents$ cd test 
Josh@utbuntu20:~/Documents/test$ ls 
Josh@utbuntu20:~/Documents/test$ touch file1.txt 
Josh@utbuntu20:~/Documents/test$ ls
file1.txt 
Josh@utbuntu20:~/Documents/test$ man cp
Josh@utbuntu20:~/Documents/test$  cp file1.txt file1cp.txt 
Josh@utbuntu20:~/Documents/test$ ls
file1cp.txt file1.txt 
Josh@utbuntu20:~/Documents/test$ cp file1.txt /home/ Josh/ Documents/ 
Josh@utbuntu20:~/Documents/test$ ls
file1cp.txt file1.txt 
Josh@utbuntu20:~/Documents/test$ ls/ home/ Josh/ Documents/
ansible-examples file1.txt test 
Josh@utbuntu20:~/Documents/test$ cd ..
Josh@utbuntu20:~/Documents$ cp -r test testcp 
Josh@utbuntu20:~/Documents$ ls
ansible-examples file1.txt test testcp
Josh@utbuntu20:~/Documents$ ls testcp/ 
file1cp.txt file1.txt 
Josh@utbuntu20:~/Documents$ man mv 
Josh@utbuntu20:~/Documents$ ls
ansible-examples file1.txt test testcp 
Josh@utbuntu20:~/Documents$ mv file1.txt file2.txt 
Josh@utbuntu20:~/Documents$ ls
ansible-examples file2.txt test testcp 
Josh@utbuntu20:~/Documents$ mv file2.txt test/ file3.txt
Josh@utbuntu20:~/Documents$ ls
ansible-examples test testcp
Josh@utbuntu20:~/Documents$ ls test/ 
file1cp.txt file1.txt file3.txt 
Josh@utbuntu20:~/Documents$ ls
ansible-examples test testcp 
Josh@utbuntu20:~/Documents$ mv testcp testpc 
Josh@utbuntu20:~/Documents$ ls 
ansible-examples test testpc 
Josh@utbuntu20:~/Documents$ 

Working with File Content

Josh@utbuntu20:~/Documents$ man head
Josh@utbuntu20:~/Documents$ ls 
ansible-examples test test.pc 
Josh@utbuntu20:~/Documents$ cd ansible-examples/ 
Josh@utbuntu20:~/Documents/ansible-examples$ ls
jboss-standalone mongodb tomcat standalone…
Josh@utbuntu20:~/Documents/ansible-examples$ head README.md
Ansible Examples 
This repository contains examples and best practices for building Ansible Playbooks
Josh@utbuntu20:~/Documents/ansible-examples$ head -5 README.md 
Josh@utbuntu20:~/Documents/ansible-examples$ man tail
Josh@utbuntu20:~/Documents/ansible-examples$ tail README.md 
Ansible Examples 
This repository contains examples and best practices for building Ansible Playbooks
Josh@utbuntu20:~/Documents/ansible-examples$ cd lamp_haproxy/
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ ls
aws hosts provision.yml roles site.yml  
group_vars LICENSE.md README.md rolling_update.yml 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ head site.yml 
— 
## This playbook deploys the whole application stack in this site.
# Apply common configuration to all hosts 
-hosts: all
roles: 
common 
# configure and deploy database servers  
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ tail site.yml 


# Configure and deploy the Nagios monitoring node(s).
-hosts: monitoring
roles: 
base-apache
nagios 
tags: 
monitoring 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ clear

Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ man cat
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ man cat.yml 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ cd
Josh@utbuntu20:~$ cd Documents/ 
Josh@utbuntu20:~/Documents$ ls 
ansible-examples test testpc 
Josh@utbuntu20:~/Documents$ man echo
Josh@utbuntu20:~/Documents$ echo The >test1.txt 
Josh@utbuntu20:~/Documents$ ls 
ansible-examples test testpc test1.txt 
Josh@utbuntu20:~/Documents$ cat test1.txt 
The 
Josh@utbuntu20:~/Documents$ echo big >test2.txt 
Josh@utbuntu20:~/Documents$ echo apple >test3.txt 
Josh@utbuntu20:~/Documents$ cat test 
test/ testpc/
Josh@utbuntu20:~/Documents$ cat test1.txt 
The 
Josh@utbuntu20:~/Documents$ cat test2.txt
big 
Josh@utbuntu20:~/Documents$ cat test3.txt 
apple
Josh@utbuntu20:~/Documents$ cat test1.txt teste2.txt test3.txt 
The
big 
apple
Josh@utbuntu20:~/Documents$ cat test1.txt teste2.txt test3.txt > all.txt
Josh@utbuntu20:~/Documents$ ls
all.txt ansible-examples test testpc test1.txt teste2.txt test3.txt 
Josh@utbuntu20:~/Documents$ cat all.text 
The 
big 
apple
Josh@utbuntu20:~/Documents$ clear

Josh@utbuntu20:~/Documents$ cat > file1.txt 
I am having a good day. 
I hope you are too! Josh@utbuntu20:~/Documents$
Josh@utbuntu20:~/Documents$ cat file1.txt 
I am having a good day.

I hope you are too! Josh@utbuntu20:~/Documents$ 
Josh@utbuntu20:~/Documents$ ls
all.txt ansible-examples file1.txt test testpc test1.txt test2.txt test3.txt 
Josh@utbuntu20:~/Documents$ cat file1.txt 
I am having a good day. 
I hope you are too! Josh@utbuntu20:~/Documents$
Josh@utbuntu20:~/Documents$ cat file1.txt > file2.txt 
Josh@utbuntu20:~/Documents$ ls 
all.txt ansible-examples file1.txt test testpc test1.txt test2.txt test3.txt 
Josh@utbuntu20:~/Documents$ cat file2.txt 
I am having a good day. 
I hope you are too! Josh@utbuntu20:~/Documents$
Josh@utbuntu20:~/Documents$ clear 

Josh@utbuntu20:~/Documents$ man more 
Josh@utbuntu20:~/Documents$ cd ansible-examples/lamp_haproxy/
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ ls
aws group_vars hosts LICENSE.md provision.yml README.md roles rolling_update.yml site.yml
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ more provision.yml
…
space button 
space button 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$  man less
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ less provision.yml
…
space button 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_haproxy$ 

Linux File Structure 
Josh@utbuntu20:~$ cd /
Josh@utbuntu20:~/ ls -l
lrwxrwxrw 1 root root 7 feb 2:14:56 bin -> usr/bin 
…
Josh@utbuntu20:~/$ 


System Information 

Josh@utbuntu20:~/$ man uptime 
Josh@utbuntu20:~/$ uptime
15:03:44 up 2:50, 1 user, load average 0.04, 0.05, 0.02
Josh@utbuntu20:~/$  man free 
Josh@utbuntu20:~/$ free
            total         used      free         shared    buff/cache  available 
mem:   8142740  960800  5952728  9920      1229212     6919404
            total         used      free           shared    buff/cache  available 
Swap:  1533028   0            1533028   
Josh@utbuntu20:~/$ man ps
Josh@utbuntu20:~/$ ps -A
Josh@utbuntu20:~/$ man df
Josh@utbuntu20:~/$ df
Josh@utbuntu20:~/$ df -h
Josh@utbuntu20:~/$ man fdisk 
Josh@utbuntu20:~/$ fdisk -l 
Josh@utbuntu20:~/$ sudo fdisk -l 
[sudo] password for Josh: …
Josh@utbuntu20:~/$ man lsblk
Josh@utbuntu20:~/$ lsblk
Josh@utbuntu20:~/$ man top 
Josh@utbuntu20:~/$ top 
Josh@utbuntu20:~/$ man htop 
No manual entry for htop
Josh@utbuntu20:~/$ htop
Command ‘htop’ not found, but can be installed with sudo apt install htop
Josh@utbuntu20:~/$ sudo apt in install htop 
Josh@utbuntu20:~/$ htop

Networking 

Josh@utbuntu20:~/$ man ifconfig
No manual entry for ifconfig
Josh@utbuntu20:~/$ ifconfig 
Command ‘ifconfig’ not found, but can be installed with:
sudo apt install net-tools 
Josh@utbuntu20:~/$ sudo apt install net-tools
[sudo] password for Josh: …
Josh@utbuntu20:~/$ man ifconfig 
Josh@utbuntu20:~/$ ifconfig 
Josh@utbuntu20:~/$ man ip 
Josh@utbuntu20:~/$ ip
Josh@utbuntu20:~/$ ip a 

Package Manager

Josh@utbuntu20:~/$ man sudo 
Josh@utbuntu20:~/$ man apt 
Josh@utbuntu20:~/$ sudo apt update 
[sudo] password for Josh: …
Josh@utbuntu20:~/$ sudo apt upgrade
Do you want to continue ? [Y/n]
Josh@utbuntu20:~/$ sudo apt search gimp
Josh@utbuntu20:~/$ sudo apt zip
Josh@utbuntu20:~/$ sudo apt install zip 
Josh@utbuntu20:~/$ sudo apt install unzip
Josh@utbuntu20:~/$ sudo apt remove gimp 
Josh@utbuntu20:~/$ sudo apt remove unzip
Do you want to continue ? [Y/n] Y
Josh@utbuntu20:~/$ sudo apt install unzip

Text Editors 

Josh@utbuntu20:~/$ man nano 
Josh@utbuntu20:~/$ cd Documents/ansible-examples/
Josh@utbuntu20:~/$ cd Documents/ansible-examples/lamp_simple/
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ ls 
group-vars hosts LICENSE.md README.md roles site.yml 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ cat hosts 
[webservers] 
web3 
[dbservers]
web2 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ nano 
group-vars hosts LICENSE.md README.md roles site.yml 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ nano hosts

[webservers] 
web3 
[dbservers]
web2 

Ubuntu
20.04 LTS 

Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ cat hosts 

[webservers] 
web3 
[dbservers]
web2 

Ubuntu
20.04 LTS 

Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ sudo apt install vim
[sudo] password for Josh: …
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ vim README.md 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ cat README.md
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ vim README.md
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ vim README.md 
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ cat README.md
Josh@utbuntu20:~/Documents/ansible-examples/lamp_simple$ 










