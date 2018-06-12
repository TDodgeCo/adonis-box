# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "tdodge1986/adonis-box"
  config.vm.box_version = "0.0.3"
  config.vm.provider "virtualbox" do |v|
    v.customize [ "modifyvm", :id, "--uartmode1", "disconnected" ]
  end

  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.hostname = "adonis-box"
  config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]
end
