# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. 

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"

  config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

   config.vm.provision "shell", path: "script.sh"

end
