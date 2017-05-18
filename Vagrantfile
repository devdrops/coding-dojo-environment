# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.synced_folder "./dojo", "/dojo", create: true

  config.vm.provision "shell", path: "./provision/intro", run: "always"
  config.vm.provision "shell", path: "./provision/setup"
  config.vm.provision "shell", path: "./provision/tools"

  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
  end
end

