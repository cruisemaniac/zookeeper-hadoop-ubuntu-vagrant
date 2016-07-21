# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.provider "virtualbox" do |vm|
      vm.memory = 512
      vm.cpus = 1
  end

  if Vagrant.has_plugin?("vagrant-cachier")
    config.cache.scope = :box
  end

  config.vm.define "zk001" do |config|
    config.vm.network "private_network", ip: "192.168.1.12", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "zk001"
  end

  config.vm.define "zk002" do |config|
    config.vm.network "private_network", ip: "192.168.1.13", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "zk002"
  end

  config.vm.define "zk003" do |config|
    config.vm.network "private_network", ip: "192.168.1.14", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "zk003"
  end

  config.vm.define "nn001" do |config|
    config.vm.network "private_network", ip: "192.168.1.15", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "nn001"
  end

  config.vm.define "nn002" do |config|
    config.vm.network "private_network", ip: "192.168.1.16", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "nn002"
  end

  config.vm.define "dn001" do |config|
    config.vm.network "private_network", ip: "192.168.1.17", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "dn001"
  end

  config.vm.define "dn002" do |config|
    config.vm.network "private_network", ip: "192.168.1.18", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "dn002"
  end

  config.vm.define "dn003" do |config|
    config.vm.network "private_network", ip: "192.168.1.19", # eth2
    virtualbox__intnet: true
    config.vm.host_name = "dn003"

  end
end
