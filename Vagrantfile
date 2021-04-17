# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
 config.vm.define :clienteUbuntu do |clienteUbuntu|
 clienteUbuntu.vm.box = "bento/ubuntu-20.04"
 config.vm.provision :shell, path: "bootstrap.sh"
 clienteUbuntu.vm.network :private_network, ip: "192.168.100.2"
 clienteUbuntu.vm.hostname = "clienteUbuntu"
 end
 config.vm.define :servidorUbuntu do |servidorUbuntu|
 servidorUbuntu.vm.box = "bento/ubuntu-20.04"
 config.vm.provision :shell, path: "bootstrap.sh"
 servidorUbuntu.vm.network :private_network, ip: "192.168.100.3"
 servidorUbuntu.vm.hostname = "servidorUbuntu"
 end
end
