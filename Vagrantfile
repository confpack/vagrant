# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "debian/jessie64"
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.synced_folder "src", "/home/vagrant/src", nfs: true

  config.vm.network :private_network, ip: "192.168.33.46"
  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--nictype1", "virtio"]
  end
  
  config.ssh.forward_agent = true
end

