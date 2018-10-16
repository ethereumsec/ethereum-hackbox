# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/bionic64"
    
  # Provision
  config.vm.provision :shell, :path => "base.sh"

  # Shared folder
  config.vm.synced_folder "vagrant/", "/home/vagrant", create: true
end