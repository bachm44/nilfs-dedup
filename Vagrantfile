# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "reproduction-nilfs-dedup"

  config.vm.provider "virtualbox" do |vb|
    vb.customize ['modifyvm', :id, '--paravirtprovider', 'kvm']
  end

  config.vm.synced_folder "../../tests", "/tests"
end
