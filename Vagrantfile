# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "centos-71-virtualbox.box"
  config.vm.provider "virtualbox" do |v|
    v.name = "centos71"
    v.linked_clone = true
    v.memory = "1024"
    v.cpus = 2
  end
end

