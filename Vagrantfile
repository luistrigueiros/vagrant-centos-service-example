# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "generic/centos7"
  config.vm.network :private_network, ip: "192.168.2.2"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  #config.ssh.insert_key = false

  config.vm.synced_folder '.', '/vagrant'
end
