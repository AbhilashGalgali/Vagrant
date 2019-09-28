# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.

Vagrant.configure("2") do |config|
#configuring ubuntu 
  config.vm.define "ubuntu" do |ubuntu|
  ubuntu.vm.box = "ubuntu/trusty64"
  ubuntu.vm.hostname = "ubuntu-abhilash"
  ubuntu.vm.network "public_network", bridge: "enO: Wi-Fi (Airport)", type: "dhcp"
  ubuntu.vm.network "forwarded_port", guest:80, host: 8087
 end
#configuring centos
  config.vm.define "centos" do |centos|
  centos.vm.box = "centos/7"
  centos.vm.hostname = "centos-abhilash"
  centos.vm.network "public_network", bridge: "enO: Wi-Fi (Airport)", type: "dhcp"
  centos.vm.network "forwarded_port", guest:80, host: 8081
 end
end
