# -*- mode: ruby -*-
# vi: set ft-ruby "
Vagrant.configure(2) do |config|
  config.vm.define "node1" do |node1|
    node1.vm.box = "bento/ubuntu-16.04"
    node1.vm.hostname = 'node1'
    node1.vm.network :private_network, ip: "192.168.33.11"
  end
  config.vm.define "node2" do |node2|
    node2.vm.box = "bento/ubuntu-16.04"
    node2.vm.hostname = 'node2'
    node2.vm.network :private_network, ip: "192.168.33.12"
  end
  config.vm.define "master", primary: true do |master|
    master.vm.hostname = 'master'
    master.vm.box = "bento/ubuntu-16.04"
    master.vm.network :private_network, ip: "192.168.33.10"
  end
end