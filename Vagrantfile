# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "debian/jessie64"
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.synced_folder "src", "/home/vagrant/src", nfs: true
end

