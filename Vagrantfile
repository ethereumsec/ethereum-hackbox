# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  # Ubuntu 18 preloaded with Python stuff we'll need
  config.vm.box = "gingeleski/ubuntu18_python"
  config.vm.box_version = "1.0"

  # (1) I prefer this password-based authN for local stuff
  # (2) This seems to get around the "Authentication failure. Retrying..." hang-up
  config.ssh.username = "vagrant"
  config.ssh.password = "vagrant"
    
  # Provision
  config.vm.provision "shell", path: "base.sh"
  config.vm.provision "shell", path: "solidity.sh"
  config.vm.provision "shell", path: "tools.sh"

  # Shared folder
  ##config.vm.synced_folder "vagrant/", "/home/vagrant", create: true
end