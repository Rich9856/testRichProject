# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "centos/7"

  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.hostname = "Focal64"
  
  #NO_PROXY = "localhost,127.0.0.1"

   config.vm.provision "shell", inline: 
  
  config.vm.define "Ubuntu" do |machine|
    config.vm.provider "virtualbox" do |vb|
      vb.memory = 2048
      vb.cpus = 4
    end
  end

  config.vm.synced_folder "C:/Users/Rich/Documents/Vagrant_Ubuntu/vagrant_Sync", "/home/vagrant/vagrant-sync"

  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
