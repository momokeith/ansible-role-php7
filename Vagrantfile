# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # Ubuntu 14.04
  config.vm.define "ubuntu1404", primary: true do |node|
    node.vm.box = "ubuntu/trusty64"
    node.vm.provision "ansible" do |ansible|
      ansible.playbook = "test.yml"
      ansible.sudo = true
    end
  end
end