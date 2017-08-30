# Vagrant
This project tested on mac os and VirtualBox

**install a Ubuntu 16.04 Vagrant image with Apache.**

1- Creat a folder and name it. (ex: VagrantTest)\n
2- Download **script.sh** in VagrantTest folder > this script will install **Apache2**
3- Open **Terminal** and enter to this folder by typing: (*cd PathToFolder/VagrantTest*)
4- Then in **Terminal** run *vagrant init ubuntu/xenial64* > vagrantfile will created in VagrantTest folder
5- Open vagrantfile and:
- uncomment this line (config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1")
- add this line ( config.vm.provision "shell", path: "script.sh")
6- Go bact to the **Terminal** and run *vagrant up* > This will creat the virtual device in VirtualBox

**Test the project:**
open the browser> type the *host_ip:host*

- you can access to your **Ubuntu 16.04** by running *vagrant ssh*
